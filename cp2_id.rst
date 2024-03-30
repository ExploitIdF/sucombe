Identifiant de la prestation
------------------------------
L'identifiant est une chaine de caractères construite automatiquement, par exemple : 

* ``PRESTA/2021_PCTT Ouest_CS_27``
* ``PRESTA/2024_PCTT Est_Automates23_7``

Le schéma de construction du champ est :

``PRESTA/{année}_{Service}_{Marché}_{indice}``

On retrouve les champs Service et Marché dans la table des prestations.

Quand le marché n'est pas identifié on trouve soit **CS** soit **Hors Marchés**. 

.. warning::
   Quel est le critère qui détermine le choix entre ces deux valeurs ?


L'année est l'année de la *création* de la prestation qui peut être antérieure à l'année de réalisation ou l'année d'affectation budgétaire.

On a identifié quelques cas où deux prestations différentes ont le même identifiant. Il s'agit d'un **bug** de Sucombe.

* PRESTA/2024_PCTT Ouest_Detection3_2
* PRESTA/2024_PCTT Ouest_Detection3_3
* PRESTA/2024_PCTT Sud_MEC3-Lot1_6

Il serait utile de savoir les circonstances de la création par Sucombe de ces doublons pour comprendre l'origine de ce bug.

