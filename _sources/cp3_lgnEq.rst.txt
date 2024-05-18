Ligne d'équipements
-----------------------
Le champ **Ligne d'équipements** prend des valeurs imposées par la configuration de l'application qui sont présentées dans une liste de choix.
Par nombres d'occurences décroissants les valeurs du  champ **Ligne d'équipements** sont :

* Distribution Electrique
* Video surveillance
* Batiment
* RAD
* Systeme informatique
* Detection
* Eclairage
* Signalisation Dynamique
* Pompage
* RAU
* Sécurité Tunnel
* Ventilation
* Climatisation
* Proprete
* Automates
* Communication de donnees
* Controle reglementaire
* Reseau Incendie
* Fermeture Physique
* Extincteurs
* Assainissement
* Evenementiel
* VH

Les nombres de prestations depuis 2020, par ligne et pour les principaux services, sont présentés dans le tableau ci-dessous.

.. csv-table:: Nombre de prestations saisies par Service et par ligne d'équipements
   :file: _static/lgnServ.csv
   :widths: 19,  9, 9, 9, 9, 9, 9, 9, 9, 9
   :header-rows: 1

Le configurateur de Sucombe a choisi d'ajouter des valeurs du champs **Ligne d'Equipements** qui ne sont pas
à proprement parler des lignes d'équipements comme :

   ``Controle règlementaire, Sécurité Tunnel, Propreté, Evenementiel`` .

Cela crée une ambiguité sur la valeur du champs *Ligne d'Equipements* qu'il faut choisir, par exemple, quand on fait le contrôle règlementaire d'un tableau électrique. 
L'utilisateur va parfois choisir la valeur du champ *Ligne d'équipements* en lien avec le marché spécifique concerné, mais cela n'est alors pas très utile puisque le marché est déjà renseigné dans Sucombe.

Il faudrait donc expliciter pour les utilisateurs les critères à utiliser pour sélectionner la valeur du champ *Ligne d'équipements*.

Certains choix de lignes d'équipements comme *Signalisation Dynamique* manquent de précision et pourraient être décomposés en *PMV, CAC, SAV ...*


