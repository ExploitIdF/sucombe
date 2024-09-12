Analyse des données de l'application Sucombe
============================================
Dernière mise à jour : avril 2024

.. toctree::
   :hidden:
   :maxdepth: 3

   champsPresta
   2_commandes
   4_preventive
   6_suivi
   preconisations

Source des données analysées
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
L'interface de l'application Sucombe, l'outil de gestions des commandes du STT/DETT, permet d'extraire des tables au format CSV, pour faire des analyses sur les données enregistrées dans Sucombe depuis 2017.
Dans le présent document, on se limitera aux données enregistrées depuis l'année 2020 car la manière d'utiliser Sucombe a évolué et l'objectif est d'examiner la situation actuelle.

Il est également possible d'accéder aux tables de la base de données sous-jacente de Sucombe, mais cela demande davantage d'effort et on essaiera autant que possible d'éviter d'y avoir recours.

Utilité des analyses envisagées
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
L'exploitation des données permet de fournir des analyses pertinentes pour la compréhension de l'activité du département DETT, en particulier sur la maintenance des équipements.
Elle éclaire aussi sur la manière dont l'application Sucombe est utilisée par les agents et permet de formuler des actions d'amélioration à ce niveau.

Table des prestations
^^^^^^^^^^^^^^^^^^^^^^
La première table analysée est celle des **prestations** car elle contient des informations assez riches sur l'ensemble des commandes.
Le tableau ci-dessous fournit les nombres de prestations saisies dans Sucombe sur la période 2020-23.

.. csv-table:: Nombre de prestations saisies par Service et par an depuis 2020
   :file: _static/servAn.csv
   :widths: 20,  20, 20, 20, 20
   :header-rows: 1

Les :doc:`champs de cette table <champsPresta>` sont les suivants :
``'Action', 'Libellé', 'Identifiant', 'Date création', 'Numméro OT','Ligne d'équipement', 'Type', 'Lieu','Date prév.', 
'Montant prestation HT', 'Montant Constaté HT', 'Marché', 'Agent', 'Service', 'État'``




