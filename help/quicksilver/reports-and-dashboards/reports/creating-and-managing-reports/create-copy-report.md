---
product-area: reporting;user-management
keywords: save,new,report,copy
navigation-topic: create-and-manage-reports
title: Créer une copie d’un rapport
description: Vous pouvez créer une copie de tout rapport auquel vous avez accès. Vous pouvez soit créer une copie exacte d’un rapport personnalisé, soit enregistrer une nouvelle version d’un rapport par défaut. Après avoir copié un rapport, vous devenez la personne propriétaire du rapport copié et il s’affiche dans la section Mes rapports.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 9396cd2ac073a57b7d99618cdf09e54ddcf95130
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 82%

---

# Créer une copie d’un rapport

<!-- Audited: 11/2024 -->

Vous pouvez créer une copie de tout rapport auquel vous avez accès. Vous pouvez soit créer une copie exacte d’un rapport personnalisé, soit enregistrer une nouvelle version d’un rapport par défaut. Après avoir copié un rapport, vous devenez la personne propriétaire du rapport copié et il s’affiche dans la section Mes rapports.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et regroupements</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet*</td> 
   <td><p>Autorisations d’affichage pour un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une copie exacte d’un rapport

Si vous souhaitez effectuer une copie d’un rapport personnalisé, procédez comme suit :

1. Cliquez sur l’icône de **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône de **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Rapports]**.

1. Cliquez sur **Tous les rapports**, puis ouvrez un rapport.

1. Cliquez sur **Actions de rapport**, puis **Copier**.

   >[!TIP]
   >
   >Si le rapport est un rapport par défaut, l’option Copier n’apparaît pas dans le menu Actions de rapport.\
   >Pour plus d’informations sur la création d’une copie d’un rapport par défaut, voir [Créer une version d’un rapport](#create-a-new-version-of-a-report).

   ![Copier le rapport](assets/unshimmed-report-actions-copy.png)

   Une copie du rapport d’origine est créée avec le nom par défaut _[Nom du rapport d’origine] (Copie)_. Par exemple, une copie du rapport &quot;Tâches terminées du quatrième trimestre&quot; sera nommée &quot;Tâches terminées du quatrième trimestre (copie)&quot;.

1. (Facultatif) Pour renommer le rapport, cliquez sur **Actions de rapport**, puis sur **Modifier**. Saisissez un nouveau nom dans la zone de texte dans le coin supérieur gauche, puis cliquez sur **Enregistrer + Fermer** lorsque vous avez terminé.

1. (Facultatif) Pour partager la nouvelle version du rapport avec d’autres personnes, cliquez sur **Actions de rapport**, puis **Partage**.

   >[!NOTE]
   >
   >Les informations de partage ne sont pas transférées vers le rapport copié depuis la version d’origine.\
   >Pour plus d’informations sur la manière de voir avec qui le rapport précédent a été partagé, voir [Créer un rapport sur les activités de création de rapports](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Facultatif) Si vous disposez des autorisations de gestion pour le rapport d’origine et que ce dernier n’est plus nécessaire, vous pouvez le supprimer afin de supprimer les rapports superflus dupliqués dans Workfront.

   Pour supprimer le rapport d’origine, procédez comme suit :

   1. Accédez au rapport.

   1. Cliquez sur **Actions de rapport**, puis **Supprimer**.

   1. Cliquez sur **Oui, supprimez-le** pour confirmer que vous souhaitez supprimer le rapport.

## Créer une version d’un rapport {#create-a-new-version-of-a-report}

Si vous souhaitez créer une copie d’un rapport par défaut, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**, puis sur **Tous les rapports**.
1. Cliquez sur le nom d’un rapport par défaut pour l’ouvrir.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.

   ![Modifier le rapport](assets/unshimmed-report-actions-default-report.png)

1. Apportez les modifications nécessaires dans les onglets suivants du rapport :

   * **Colonnes (Vue)** : pour plus d’informations sur la personnalisation des vues, consultez l’article [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Regroupements** : pour plus d’informations sur la personnalisation des regroupements, voir l’article [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filtres** : pour plus d’informations sur la personnalisation des filtres, voir l’article [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Graphique** : pour plus d’informations sur la personnalisation d’un graphique de rapport, voir l’article [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Dans le coin supérieur droit, cliquez sur **Paramètres du rapport**.
1. Dans le champ **Titre du rapport**, attribuez un nouveau nom au rapport.
1. Cliquez sur **Terminer**.
1. Cliquez sur **Enregistrer en tant que nouveau rapport**.

   ![](assets/unshimmed-save-as-new-report.png)

1. (Facultatif) Pour partager la nouvelle version du rapport avec d’autres personnes, cliquez sur **Actions de rapport**, puis **Partage**.
