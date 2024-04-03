Préconisations pour les utilisateurs de Sucombe
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Dans cette partie, on rassemble des préconisations qui ont été formulées dans les autres parties en marge de l'analyse d'un aspect des données de Sucombe.

.. collapse:: Décomposition en prestations élémentaires
    :class: custom-summary
    :open:

    Une prestation doit concerner un champ limité en termes d'étendue géographique, temporelle et de nature. 
    Il faut distinguer autant de prestations qu'il y a d'actions que l'on peut réaliser indépendamment. 

    Comme le champ *Lieu* permet de distinguer en fonction des tunnels, il faut séparer les prestations par tunnel.

    Comme le champ *Type* permet par exemple de distinguer des types, préventif et curatif par exemples, il faut faire des prestations spécifiques pour les actions de chaque type.

    Par exemple, Préventif **CAC,PMV,SAV du secteur X** mériterait peut-être d'être décomposé par catégorie d'équipements et par axe.

.. collapse:: Description de la prestation
    :class: custom-summary
    :open:

    La *Description de la prestation* est un champ dont la saisie par le TDM est *libre* à la différence des champs pour lesquels il faut choisir une valeur dans une liste. 

    Les informations saisies dans la description de la prestation doivent servir à compléter les informations qui sont 
    déjà saisies par ailleurs dans les champs *Lieu*, *Ligne d'équipements*, *Marché*, Numéro d'OT* et *Type*. 

    Il n'est pas utile de saisir une information déjà contenue dans un autre champ, mais on peut fournir des précisions intéressantes.
    En particulier, quand le marché n'est pas connu de Sucombe, mentionner le fournisseur dans la description est utile. 
    Il faut aussi donner des informations sur la nature de la prestation quand le prix du BPU est générique ou qu'il n'y a pas de prix enregistré dans Sucombe.
    Quand le lieu est général tel que *SIRIUS*, *PCTT*, *Tous tunnels*, la description peut donner une précision de localisation.
    Quand la prestation concerne des équipements particuliers et non pas toute la ligne d'équipements, la description peut préciser le périmètre.




