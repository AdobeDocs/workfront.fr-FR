---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Exporter une liste de feuilles de temps
description: En tant que personne responsable du personnel ou de l’approbation des feuilles de temps, vous devrez peut-être télécharger une liste des feuilles de temps pour consulter rapidement des informations sur les feuilles de temps des personnes dont vous êtes responsable. Pour ce faire, vous pouvez exporter une liste de feuilles de temps.
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 63%
---
# Exporter une liste de feuilles de temps

<!--Audited: 8/2024-->

En tant que personne responsable du personnel ou de l’approbation des feuilles de temps, vous devrez peut-être télécharger une liste des feuilles de temps pour consulter rapidement des informations sur les feuilles de temps des personnes dont vous êtes responsable. Pour ce faire, vous pouvez exporter une liste de feuilles de temps.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td> <p>Léger ou supérieur </p>
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td>Configuration du niveau d’accès</td> 
   <td> <p>Afficher ou un accès supérieur aux tâches et aux événements</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Autorisations Affichage ou supérieures pour les tâches et problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exporter une liste de feuilles de temps

{{step1-to-timesheets}}

Toutes les feuilles de temps que vous êtes autorisé à consulter s&#39;affichent par défaut.

![Liste des feuilles de temps](assets/list-of-all-timesheets.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez,

     Ou

     Sélectionnez **Mes feuilles de temps** pour afficher uniquement vos feuilles de temps.

     Cette action applique les filtres **Mes approbations de feuille de temps** ou **Ma feuille de temps** à la liste des feuilles de temps.

   * Cliquez sur l’icône **Filtre** ![Icône Filtre](assets/filter-nwepng.png) pour appliquer un filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste des feuilles de temps ou dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé ces filtres des contrôles de liste dans la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, consultez la section [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Facultatif) Cliquez sur les icônes **Affichage** ![Icône Affichage](assets/view-icon.png) ou **Regroupement** ![Icône Regroupement](assets/grouping.png) pour appliquer une vue ou un regroupement ou en créer un nouveau.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, voir les articles suivants :

   * [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Sélectionnez les feuilles de temps à exporter, puis cliquez sur l’icône **Exporter** ![Exporter](assets/export-38x15.png).

   ![Cliquez sur l’icône Exporter](assets/export-timesheets.png)

1. Sélectionnez le type de fichier vers lequel vous souhaitez exporter la liste des feuilles de temps à partir des options suivantes :

   * PDF - Paysage
   * PDF - Portrait
   * Autres formats de PDF
   * Excel
   * Excel (xlsx)
   * Délimité par des tabulations

   Une liste de feuilles de temps est téléchargée sur votre ordinateur au format sélectionné et contient les informations suivantes :

   * Période
   * Nom du propriétaire
   * Total des heures
   * Quantité d’heures supplémentaires
   * Noms des approbateurs et approbatrices
   * Statut
