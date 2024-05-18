Libellé de la prestation
========================

Le libellé est un champ *libre* qui permet à l'utilisateur de décrire en quoi consiste la prestation. 
Il permet ainsi d'apporter des informations qui ne sont pas dans les champs ``Lieu, Ligne d'équipement, Marché, Type``.

En particulier, quand le marché et le produit (ligne du BPU) ne sont pas identifiés parce qu'il s'agit d'une commande simple, d'un marché DIRIF ou d'un marché national (Ministère, UGAP ...), il est utile de renseigner dans ce champ les produits, les quantités et le fournisseur.

Quand la prestation est liée à un **dégat au domaine publique** (DDP), à défaut de mieux pour enregistrer cette information, on pourrait intégrer le code DDP dans le champs Libellé.

Les utilisateurs recopient souvent dans le libellé les valeurs d'autres champs, ce qui n'est pas très utile. Il faut plutot utiliser ce champs pour ajouter des informations complémentaires qui résument la prestation.

Même s'il sagit d'un champ en texte libre, il faut autant que possible saisir des informations de manière systématique pour permettre des traitements automatisés des données. Si par exemple on a introduit le code DDP à l'intérieur du champ Libellé, le traitement automatique pourra tester la présence de ce code.


