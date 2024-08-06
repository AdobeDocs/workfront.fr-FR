---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Exporter une liste de feuilles de temps
description: En tant que gestionnaire des personnes ou approbateur de feuilles de temps, vous devrez peut-être télécharger une liste de feuilles de temps pour afficher rapidement des informations sur les feuilles de temps des personnes dont vous êtes responsable. Pour ce faire, vous pouvez exporter une liste de feuilles de temps.
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 20%

---

# Exporter une liste de feuilles de temps

<!--Audited: 8/2024-->

En tant que gestionnaire des personnes ou approbateur de feuilles de temps, vous devrez peut-être télécharger une liste de feuilles de temps pour afficher rapidement des informations sur les feuilles de temps des personnes dont vous êtes responsable. Pour ce faire, vous pouvez exporter une liste de feuilles de temps.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Léger ou supérieur </p>
   <p>Actuel : révision ou supérieur </p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Affichage ou accès supérieur aux tâches et aux problèmes </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures de la feuille de temps</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old permissions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to Tasks and Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the timesheets</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan or license type you have, contact your Workfront administrator.-->

## Exporter une liste de feuilles de temps

{{step1-to-timesheets}}

La zone **Fiches horaires** s’ouvre.


![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Cliquez sur l’icône **search** ![](assets/search-icon.png) et saisissez un mot-clé et recherchez une feuille de temps spécifique. Par exemple, vous pouvez rechercher une période de temps définie ou le nom du propriétaire.

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez.

     Ou

     Sélectionnez **Mes feuilles de calcul** pour n’afficher que vos feuilles de calcul.

     Cela applique les filtres Mes approbations de feuille de temps ou Ma feuille de temps à la liste des feuilles de temps.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Cliquez sur l’icône Filtrer ![](assets/filter-nwepng.png) pour appliquer un autre filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste de feuille de temps ni dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé les filtres Mes approbations de feuille de temps et Mes feuilles de temps des commandes de liste de la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, voir les articles suivants :
   >
   >   
   >   
   >   * [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facultatif) Cliquez sur les icônes **View** ![](assets/view-icon.png) ou **Grouping** ![](assets/grouping.png) pour appliquer une autre vue ou un autre regroupement ou en créer un nouveau.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, consultez les articles suivants :

   * [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Sélectionnez les feuilles de temps à exporter, puis cliquez sur l&#39;icône **Export** ![](assets/export-38x15.png) .

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. Sélectionnez le type de fichier vers lequel vous souhaitez exporter la liste des feuilles de temps à partir des options suivantes :

   * PDF Ladscape
   * Portrait PDF
   * Autres tailles du PDF
   * Excel
   * Excel (xlsx)
   * Délimité par des tabulations

   Une liste de feuilles de temps est téléchargée sur votre ordinateur au format sélectionné et contient les informations suivantes :

   * Période
   * Nom du propriétaire
   * Total des heures
   * Montant des heures supplémentaires
   * Noms des approbateurs
   * Statut
