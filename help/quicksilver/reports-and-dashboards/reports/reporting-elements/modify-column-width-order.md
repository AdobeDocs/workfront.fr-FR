---
product-area: reporting
navigation-topic: reporting-elements
title: Modifier la largeur et l’ordre des colonnes
description: Consultez cet article pour en savoir plus sur les directives relatives à la largeur des colonnes et sur la manière de modifier la largeur et l’ordre des colonnes dans Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 95%

---

# Modifier la largeur et l’ordre des colonnes

<!-- Audited: 11/2024 -->

Vous trouverez ci-dessous des directives sur le fonctionnement des largeurs de colonnes dans Adobe Workfront :

* Workfront définit par défaut la largeur des colonnes dans les listes et les rapports.
* Workfront ajuste automatiquement la largeur des colonnes en fonction des informations `valueformat` contenues dans toutes les listes et tous les rapports, sauf indication contraire dans le mode texte de la colonne.

  >[!NOTE]
  >
  >Workfront n’ajuste pas la largeur des colonnes en fonction des informations `valueformat` contenues dans les listes disponibles dans les zones Configuration et Rapports.

  La valeur `valueformat` définit le type d’informations qui s’affiche dans la colonne. Par exemple, les colonnes qui affichent un nombre sont plus étroites que celles qui affichent le champ Description.

* Vous pouvez personnaliser la largeur des colonnes dans vos listes et rapports Workfront pour répondre à vos besoins, en fonction du type d’informations que vous souhaitez afficher dans les colonnes.

  Vous pouvez modifier la largeur des colonnes temporairement, lors de l’affichage d’une liste ou d’un rapport, ou de manière permanente, en ajustant la largeur de la colonne dans le générateur d’affichage. Pour plus d’informations sur la modification temporaire de la largeur des colonnes, voir [Remarques concernant la modification temporaire de la largeur et de l’ordre des colonnes](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) de cet article.

* La largeur des colonnes qui apparaissent dans les vues intégrées est préalablement définie par Workfront et codée en dur. Pour modifier ces largeurs, vous devez manuellement mettre à jour la largeur de ces colonnes à l’aide du mode texte dans le générateur d’affichage.

  Pour plus d’informations sur la modification de la colonne en mode texte, voir [Vue : modifier de manière permanente la largeur d’une colonne](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Contributeur ou version ultérieure</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Requête ou supérieure</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier la vue d’un rapport.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier une vue dans un rapport.</p> <p>Gérer les autorisations d’une vue pour la modifier</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier la largeur et l’ordre des colonnes

Vous pouvez modifier la largeur et l’ordre des colonnes dans vos rapports de la manière suivante :

* [Modifier temporairement la largeur et l’ordre des colonnes](#modify-width-and-order-of-columns-temporarily)
* [Modifier la largeur et l’ordre des colonnes de façon permanente](#modify-width-and-order-of-columns-permanently)

### Modifier temporairement la largeur et l’ordre des colonnes {#modify-width-and-order-of-columns-temporarily}

Vous pouvez faire glisser les bordures des colonnes pour les redimensionner et faire glisser et déposer les colonnes pour les réorganiser temporairement dans la plupart des listes du site Workfront. Cela comprend les rapports, les vues, les rapports sur les tableaux de bord et la vue Gantt.

Pour plus d’informations sur les listes Workfront, consultez l’article [Prise en main des listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Points à prendre en compte lors de la modification temporaire de la largeur et de l’ordre des colonnes](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Redimensionner temporairement les colonnes](#resize-columns-temporarily)
* [Réorganiser temporairement des colonnes](#reorder-columns-temporarily)

#### Points à prendre en compte lors de la modification temporaire de la largeur et de l’ordre des colonnes {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Vous pouvez modifier temporairement la largeur et l’ordre des colonnes d’une liste sans en modifier la vue.

Tenez compte des éléments suivants lorsque vous redimensionnez et ordonnez temporairement des colonnes :

* Lors du redimensionnement des colonnes, les nouvelles tailles de colonnes sont stockées dans la mémoire locale de votre navigateur et sont enregistrées par défaut. L’utilisation d’un autre navigateur ou l’effacement de votre cache ou de vos données de navigation a pour effet de ramener la taille des colonnes à la valeur par défaut. L’actualisation de votre page conserve les modifications apportées à la largeur des colonnes.

>[!NOTE]
> 
>La largeur des colonnes est limitée par la taille de la fenêtre du navigateur. Si la page est actualisée, la largeur des colonnes sera réduite jusqu’à ce que toutes les colonnes puissent tenir dans la fenêtre sans défilement horizontal. Pour forcer la conservation d’une colonne plus large que le navigateur ne le permet, vous devez définir la largeur de la colonne en mode texte comme décrit dans la section [Modifier la largeur et l’ordre des colonnes de façon permanente](#modify-width-and-order-of-columns-permanently) et éviter d’ajuster manuellement la largeur des colonnes en faisant glisser leurs bordures.
>

* Une fois que vous avez réorganisé les colonnes, l’ordre que vous avez choisi n’est conservé que jusqu’à ce que vous quittiez la liste ou actualisiez la page du navigateur. Après avoir quitté la liste ou actualisé la page du navigateur, les colonnes reprennent leur ordre par défaut.
* Pour garantir des performances optimales, les colonnes que vous réorganisez ne doivent pas contenir plus de 100 éléments dans la liste.
* Quand vous ajustez la taille des colonnes, vos modifications ne sont valides que pour la vue que vous utilisez actuellement et ne sont visibles que par vous. Quand vous partagez une vue avec un autre utilisateur ou une autre utilisatrice, cela ne signifie pas que les tailles de colonnes que vous avez définies sont également partagées.
* Après avoir ajusté la taille d’une colonne en déplaçant sa bordure vers la droite, la largeur de la colonne voisine est maintenue, sauf dans les emplacements suivants :

   * Zone de configuration
   * Zone de rapports
   * Listes et rapports de document

  >[!NOTE]
  >
  >Il est impossible de déplacer la bordure gauche d’une colonne au-delà de la bordure gauche de la colonne voisine dans une liste.

* Si vous exportez une liste vers un fichier, l’ordre temporaire des colonnes n’est pas transféré dans le fichier exporté. Le fichier exporté affiche l’ordre des colonnes de la liste originale, avant que les colonnes n’aient été réorganisées.

Pour plus d’informations sur l’export de données à partir de listes et de rapports, consultez l’article [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Redimensionner temporairement des colonnes {#resize-columns-temporarily}

1. Accédez à la liste que vous souhaitez modifier.
1. Faites glisser la bordure d’un en-tête de colonne jusqu’à ce que la colonne atteigne la taille souhaitée.\
   ![Redimensionner la colonne](assets/column-resize-350x124.png)

#### Réorganiser temporairement des colonnes {#reorder-columns-temporarily}

1. Accédez à la liste que vous souhaitez modifier.
1. Cliquez sur l’en-tête de colonne à déplacer et faites-le glisser jusqu’à l’emplacement souhaité.

>[!TIP]
>
>Cette fonction se révèle particulièrement utile pour afficher simultanément le graphique de Gantt et la vue Liste. Lors de l’affichage du graphique de Gantt, les colonnes peuvent être masquées. Pour afficher une colonne lorsque le graphique de Gantt est visible, il vous suffit de faire glisser la colonne que vous souhaitez visualiser afin qu’elle apparaisse sur le côté gauche de la page.

### Modifier la largeur et l’ordre des colonnes de façon permanente {#modify-width-and-order-of-columns-permanently}

Pour réorganiser les colonnes de façon permanente, consultez la section [Créer ou personnaliser une vue standard](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) dans l’article [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

La seule manière de modifier définitivement la largeur d’une colonne est en utilisant le mode texte.

Pour plus d’informations sur l’utilisation du mode texte et la modification permanente de la largeur d’une colonne, consultez l’article [Vue d’ensemble des utilisations courantes du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
