Préconisations pour les utilisateurs de Sucombe
**************************************************
Dans cette partie, on rassemble des préconisations qui ont été formulées dans les autres parties en marge de l'analyse d'un aspect des données de Sucombe.

.. collapse:: Rédaction du champ description d'un bon de commande
    :class: custom-summary
    :open:

    Sur un bon de commande apparaissent les champs **Libellé** et **Description**. 
    Le **Répertoire D** qui est utilisé pour le suivi budgétaire ne reprend que le champ **Description**. 
    Ce champ doit donc être renseigné avec assez de précision, pour caractériser la nature et le périmètre de la commande. 

    Deux bons de commande différents, pour une même année et un même marché, ne doivent pas avoir le même champ **Description**.
    Si une même action doit faire l'objet de plusieurs commandes successives, la description de chaque commande doit comporter un éléments permettant de la distinguer des précédentes. A défaut de mieux, on utilisera "phase 2" ...
    


.. collapse:: Décomposition en prestations élémentaires
    :class: custom-summary
    :open:

    Une prestation doit concerner un champ limité en termes de *Lieux*, de *Types* et de *Lignes d’équipements*. 
    Il faut distinguer les prestations qui concernent des *Lieux*, des *Types* ou de *Lignes d’équipements* différents. 

    Comme le champ *Lieu* permet de distinguer en fonction des tunnels, il faut séparer les prestations par tunnel.

    Comme le champ *Type* permet de distinguer des types, préventif et curatif par exemples, il faut faire des prestations spécifiques pour les actions de chaque type.

    Par exemple, Une prestation dont la *Description* est **Préventif CAC,PMV,SAV du secteur X** mériterait d'être décomposée par *Lignes d’équipements*.

.. collapse:: Description de la prestation
    :class: custom-summary
    :open:

    La *Description de la prestation* est un champ dont la saisie par le TDM est *libre* à la différence des champs pour lesquels il faut choisir une valeur dans une liste. 

    Les informations saisies dans la description de la prestation doivent servir à compléter les informations qui sont 
    déjà saisies par ailleurs dans les champs *Lieu*, *Ligne d'équipements*, *Marché*, Numéro d'OT* et *Type*. 

    Il n'est pas utile de saisir dans la *Description de la prestation* une information déjà contenue dans un autre champ, mais on peut fournir des précisions intéressantes.
    Il faut aussi donner des informations sur la nature de la prestation quand le prix du BPU est générique ou qu'il n'y a pas de prix enregistré dans Sucombe.
    Quand le **Lieu** est général tel que *SIRIUS*, *PCTT*, *Tous tunnels*, la description peut donner une précision de localisation.
    Quand la prestation concerne des équipements particuliers et non pas toute la **Ligne d'équipements**, la description peut préciser le périmètre.


.. collapse:: Description de la prestation pour une commande simple
    :class: custom-summary
    :open:

    Pour les **commandes simples** (CS), il n'y a pas de *Bordereau des Prix* et de *numéro de prix*, pour renseigner sur la nature de la prestation.     
    Il faut compenser cette absence en introduisant dans la **Description** les informations qu'un numéro de prix aurait pu apporter.
    
    Dans le cas où l'on fait une commande simple après la fin d'un marché, en utilisant le bordereau des prix du marché, on peut inscrire dans la description le nom du marché et le numéro de prix utilisé.
    




