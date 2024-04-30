Traitements pour envoyer les données sur Google Cloud
*******************************************************

Cette page vise à documenter les traitements qui permettent d traiter les données avec les outils de Google Cloud.

Etape 1 : Extraction des tables Sucombe avec Windev
=======================================================
Nicolas Bernard dispose d'une licence WinDev et des droits de lecture sur la base de Sucombe.
Il a programmé dans Windev l'importation quotidienne de plusieurs tables.
A partir de ces tables, il effectue des liaisons pour enrichir la table "produit_prestation" 
dont les enregistrements correspondent au lignes qui constituent les prestations.  Pour chaque prestation 
et chaque prix utilisé, l'enregistrement indique la qualité, le prix unitaire et toute les données relatives à la 
prestation et à la commande qui peuvent être utilisées dans des analyses.

Etape 2 : Envoi de la table à une adresse gmail
==================================================
Le fichier (xlsx) produit est envoyé quotidiennement à une adresse gmail.
Un script (AppScript) enregistre le fichier dans une Google Sheet.

.. block-code:

function myFunction() {
 const projectId = 'feu2401';
 const request = {
    // TODO (developer) - Replace query with yours
    query: 'SELECT SUBSTR(BdC,10) AS BDC,  Nom,  Designation,  Lieu,  Prix_Total AS Montant,'+
  'PARSE_DATE("%d/%m/%Y", Date_BdC) AS date FROM   `feu2401.sucombe.der24`'+
  'WHERE   LENGTH(Prix_Total)>8 ORDER BY   date DESC LIMIT 100 ;',
    useLegacySql: false
  };
 let queryResults = BigQuery.Jobs.query(request, projectId);
 const jobId = queryResults.jobReference.jobId;

  let sleepTimeMs = 500;
  while (!queryResults.jobComplete) {
    Utilities.sleep(sleepTimeMs);
    sleepTimeMs *= 2;
    queryResults = BigQuery.Jobs.getQueryResults(projectId, jobId);
  }

  // Get all the rows of results.
  let rows = queryResults.rows;
  while (queryResults.pageToken) {
    queryResults = BigQuery.Jobs.getQueryResults(projectId, jobId, {
      pageToken: queryResults.pageToken
    });
    rows = rows.concat(queryResults.rows);
  }

  if (!rows) {
    console.log('No rows returned.');
    return;
  }
  const spreadsheet = SpreadsheetApp.getActive();
  const sheet = spreadsheet.getActiveSheet();

  // Append the headers.
  const headers = queryResults.schema.fields.map(function(field) {
    return field.name;
  });
  sheet.appendRow(headers);

  // Append the results.
  const data = new Array(rows.length);
  for (let i = 0; i < rows.length; i++) {
    const cols = rows[i].f;
    data[i] = new Array(cols.length);
    for (let j = 0; j < cols.length; j++) {
      data[i][j] = cols[j].v;
    }
  }
  sheet.getRange(2, 1, rows.length, headers.length).setValues(data);










