---
product-area: reporting
navigation-topic: reporting-elements
title: Modification de la largeur et de l’ordre des colonnes
description: Consultez cet article pour en savoir plus sur les conseils relatifs à la largeur des colonnes et sur la manière de modifier la largeur et l’ordre des colonnes dans Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 0%

---

# Modification de la largeur et de l’ordre des colonnes

Vous trouverez ci-dessous des instructions relatives au fonctionnement des largeurs de colonne dans Adobe Workfront :

* Workfront définit par défaut la largeur des colonnes des listes et des rapports.
* Workfront ajuste automatiquement la largeur des colonnes en fonction de la variable `valueformat`des informations dans toutes les listes et tous les rapports, sauf indication contraire en mode texte de la colonne.

  >[!NOTE]
  >
  >Workfront n’ajuste pas la largeur des colonnes en fonction de la variable `valueformat` des informations dans les listes disponibles dans les zones Configuration et Rapports .

  La variable `valueformat` définit le type d’informations affichées dans la colonne. Par exemple, les colonnes qui affichent un nombre sont plus étroites que les colonnes qui affichent le champ Description.

* Vous pouvez personnaliser la largeur des colonnes de vos listes et rapports Workfront en fonction de vos besoins, selon le type d’informations que vous souhaitez afficher en colonnes.

  Vous pouvez modifier temporairement la largeur des colonnes lors de l’affichage d’une liste ou d’un rapport, ou de manière permanente, en ajustant la largeur de la colonne dans le créateur de vues. Pour plus d’informations sur la modification temporaire de la largeur des colonnes, voir la section [Remarques concernant la modification temporaire de la largeur et de l’ordre des colonnes](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) dans cet article.

* Les colonnes qui apparaissent dans les vues natives ont des largeurs précédemment définies par Workfront et codées en dur. Pour modifier ces largeurs, vous devez mettre à jour manuellement la largeur de ces colonnes à l’aide du mode texte dans le générateur d’affichage.

  Pour plus d’informations sur la modification de la colonne en mode texte, voir [Afficher : permet de modifier définitivement la largeur d’une colonne.](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Requête ou supérieure </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux Rapports, tableaux de bord et calendriers pour modifier la vue dans un rapport</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier une vue dans un rapport</p> <p>Gérer les autorisations pour une vue pour la modifier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Modification de la largeur et de l’ordre des colonnes

Vous pouvez modifier la largeur et l’ordre des colonnes dans vos rapports de la manière suivante :

* [Modifier temporairement la largeur et l’ordre des colonnes](#modify-width-and-order-of-columns-temporarily)
* [Modifier la largeur et l’ordre des colonnes de manière permanente](#modify-width-and-order-of-columns-permanently)

### Modifier temporairement la largeur et l’ordre des colonnes {#modify-width-and-order-of-columns-temporarily}

Vous pouvez faire glisser des bordures de colonne pour redimensionner les colonnes et faire glisser-déposer des colonnes afin de les réorganiser temporairement dans la plupart des listes sur le site Workfront. Cela inclut les rapports, les vues, les rapports sur les tableaux de bord et la vue Gantt.

Pour plus d’informations sur les listes Workfront, voir l’article [Prise en main des listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Remarques concernant la modification temporaire de la largeur et de l’ordre des colonnes](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Redimensionner temporairement les colonnes](#resize-columns-temporarily)
* [Réorganiser temporairement les colonnes](#reorder-columns-temporarily)

#### Remarques concernant la modification temporaire de la largeur et de l’ordre des colonnes {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Vous pouvez temporairement modifier la largeur et l’ordre des colonnes d’une liste sans modifier sa vue.

Tenez compte de ce qui suit lors du redimensionnement et de l’ordre temporaires des colonnes :

* Lors du redimensionnement des colonnes, les nouvelles tailles de colonne sont stockées dans l’espace de stockage local de votre navigateur et sont enregistrées par défaut. L’utilisation d’un autre navigateur, l’effacement du cache ou la navigation dans les données entraînent la restauration de la taille des colonnes par défaut. L’actualisation de la page permet de conserver les modifications apportées à la largeur des colonnes.

>[!NOTE]
> 
>La largeur des colonnes est limitée par la taille de la fenêtre du navigateur. Si la page est actualisée, la largeur des colonnes est réduite jusqu’à ce que toutes les colonnes puissent s’adapter à la fenêtre sans défilement horizontal. Pour forcer une colonne à rester plus large que la largeur souhaitée par le navigateur, vous devez définir la largeur de la colonne en mode texte, comme décrit dans la section [Modifier la largeur et l’ordre des colonnes de manière permanente](#modify-width-and-order-of-columns-permanently) et évitez d’ajuster manuellement les largeurs de colonne en faisant glisser leurs bordures.
>

* Lors de la réorganisation des colonnes, l’ordre de votre choix n’est conservé que lorsque vous quittez la liste ou que vous actualisez la page du navigateur. Après avoir quitté la liste ou actualisé la page du navigateur, les colonnes retournent à leur ordre par défaut.
* Pour des performances optimales, les colonnes que vous réorganisez ne doivent pas comporter plus de 100 éléments dans la liste.
* Lorsque vous redimensionnez des colonnes, vos modifications s’appliquent uniquement à la vue que vous utilisez actuellement et qui n’est visible que par vous. Le partage d’une vue avec un autre utilisateur ne partage pas les tailles de colonne que vous avez définies.
* Après avoir redimensionné une colonne en faisant glisser sa bordure vers la droite, la largeur de la colonne voisine est conservée, sauf dans les cas suivants :

   * Zone Configuration
   * La zone Rapports
   * Listes et rapports de document

  >[!NOTE]
  >
  >Vous ne pouvez pas déplacer la bordure gauche d’une colonne au-delà de la bordure gauche de la colonne voisine dans une liste.

* Si vous exportez une liste dans un fichier, l’ordre temporaire des colonnes ne sera pas transféré vers le fichier exporté. Le fichier exporté affiche l’ordre des colonnes de la liste d’origine, avant que les colonnes n’aient été réorganisées.

Pour plus d’informations sur l’exportation de données à partir de listes et de rapports, reportez-vous à l’article [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Redimensionner temporairement les colonnes {#resize-columns-temporarily}

1. Accédez à la liste que vous souhaitez modifier.
1. Faites glisser la bordure d’une colonne jusqu’à ce que la colonne atteigne la taille souhaitée.\
   ![](assets/column-resize-350x124.png)

#### Réorganiser temporairement les colonnes {#reorder-columns-temporarily}

1. Accédez à la liste que vous souhaitez modifier.
1. Cliquez sur une colonne que vous souhaitez déplacer pour la sélectionner.
1. Faites glisser la colonne à l’emplacement approprié.
1. Déposez la colonne à l’emplacement où vous souhaitez la déplacer.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Cela s’avère particulièrement utile lorsque vous affichez simultanément le diagramme de Gantt et le mode Liste. Lorsque vous affichez le diagramme de Gantt, les colonnes peuvent devenir masquées. Pour afficher une colonne pendant l&#39;affichage du diagramme de Gantt, faites glisser la colonne que vous souhaitez afficher afin de l&#39;afficher sur le côté gauche de la page.

### Modifier la largeur et l’ordre des colonnes de manière permanente {#modify-width-and-order-of-columns-permanently}

Pour réorganiser définitivement les colonnes, voir la section [Création ou personnalisation d’une vue standard](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) dans l’article [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Vous ne pouvez modifier la largeur d’une colonne de manière permanente qu’en mode texte.

Pour plus d’informations sur l’utilisation du mode texte et la modification permanente de la largeur d’une colonne, consultez l’article . [Présentation des utilisations courantes du mode Texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
