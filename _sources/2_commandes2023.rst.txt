Commandes de l'année 2023
**************************
L'une des tables produites par Sucombe qui est très utilisée est le **répertoire D**. 
Dans cette partie on examine cette table et on tente d'interpréter ses données.

Les lignes du répertoire D correspondent aux bons de commande enregistrés. En 2023, il y a 1470 lignes.

Le commandé, le constaté et le facturé
=======================================
* Le champs *Montant LC ou marché TTC* correspond au montant du bon de commande (Total : 26 815 k€).
* Le champs *Montant constats TTC* correspond au montant constaté (Total : 21 683 k€).
* Le champs *Facturé TTC* correspond au montant facturé (Total : 17 968 k€).

Les écarts entre les montants sont importants, plus de 5 M€ entre les commandes et les constats. 

Le montant facturé, quand il est connu, est le plus souvent égal au montant constaté. 
Dans un petit nombre de cas, le montant facturé est supérieur et dans plus de 50 cas, il est inférieur. 
Dans l'attente de mieux comprendre l'utilité de ce champ, on ne l'a pas étudié plus en détail.

Le champ intitulé **Montant LC ou marché TTC** correspond sans doute à l'engagement, 
mais que se passe t il quand tout ou partie d'un commande est désengagée ?
La valeur dans le REP D est-elle mise à jour ?

Si tel n'est pas le cas, la sommes des valeurs sera supérieure au total des engagements.

Les écarts entre les  ** totaux commandés** et les  **totaux constatés** sont très différents selon les marchés, 
comme le montre la table ci-dessous :

.. csv-table::
   :header: Marché,Commandé,Constaté
   :widths: 30, 30,30
   :width: 60%
    
    RAU/TSE,154.1,148.7
    Trafic,34.4,22.9
    CLIM2,246.0,225.5
    Cont Reg,566.0,540.7
    Automates23,91.2,56.9
    FERASS,142.8,108.4
    MIRT-Lot2,238.0,201.4
    Ventilation2,567.4,529.3
    Propreté,1164.8,1125.7
    Onduleur,478.3,421.4
    AEV,710.7,649.1
    Bat,703.0,625.2
    MIRT-Lot-3,103.8,-0.0
    MEC3-Lot1,819.8,715.7
    MEC2,2438.1,2330.1
    MIIET,357.4,235.0
    Detection2,793.5,662.5
    Eclairage,925.1,793.3
    Pompage,947.1,811.2
    RAU/TSE23,222.6,85.3
    MIRT-Lot1,696.2,526.5
    MERASS,518.9,343.8
    Vidéo,1630.4,1452.3
    AMO Tunnel,634.3,451.1
    MIRT-LOT-1,812.4,386.9
    SignaDyn,3326.1,2615.7
    MIISST2,3472.3,2192.1
    Marchés nationaux,450.7,305.1
    Marchés DIRIF,328.8,228.8
    Commandes Simples,2273.7,1926.6

Evolution du montant commandé au cours de l'année
===================================================
Dans le répertoire D figure une date que l'on suppose être la date à laquelle le bon de commande a été saisi ou validé par 
le chef d'unité qui a la prérogative de valider les commandes. Cette date est parfois antérieure au 1er janvier 2023.

Le graphique suivant montre la progression du volume commandé cumulé, en pourcentage du total, pour chaque semaine, 
à partir de la fin de l'année 2022.

.. raw:: html
   :file: _static/wMont.html


