---
product-area: reporting;user-management
keywords: save,new,report,copy
navigation-topic: create-and-manage-reports
title: Créer une copie d’un rapport
description: Vous pouvez créer une copie de tout rapport auquel vous avez accès. Vous pouvez soit créer une copie exacte d’un rapport personnalisé, soit enregistrer une nouvelle version d’un rapport par défaut. Après avoir copié un rapport, vous devenez le propriétaire du rapport copié et il s’affiche dans la section Mes rapports .
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Créer une copie d’un rapport

Vous pouvez créer une copie de tout rapport auquel vous avez accès. Vous pouvez soit créer une copie exacte d’un rapport personnalisé, soit enregistrer une nouvelle version d’un rapport par défaut. Après avoir copié un rapport, vous devenez le propriétaire du rapport copié et il s’affiche dans la section Mes rapports .

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations pour un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créer une copie exacte d’un rapport

Si vous souhaitez faire une copie d’un rapport dont vous êtes le propriétaire, procédez comme suit :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**, puis **Tous les rapports**.
1. Ouvrez un rapport.
1. Cliquez sur **Actions de rapport**, puis **Copier**.

   >[!TIP]
   >
   >Si le rapport est un rapport par défaut, l’option Copier n’apparaît pas dans le menu Actions de rapport .\
   >Pour plus d’informations sur la création d’une copie d’un rapport par défaut, voir [Création d’une version d’un rapport](#create-a-new-version-of-a-report).

   ![Copier le rapport](assets/nwe-fulllistofreportactions-2022.png)

   Une copie du rapport d’origine est créée avec le nom par défaut de *Copie de [Nom du rapport d&#39;origine]*. Par exemple, le nom du rapport &quot;Tâches terminées du quatrième trimestre&quot; serait &quot;Copie des tâches terminées du quatrième trimestre&quot;.

1. (Facultatif) Pour renommer le rapport, commencez à saisir un nouveau nom.

   >[!TIP]
   >
   >Si vous désélectionnez le titre avant de saisir le nouveau nom, sélectionnez le titre du rapport, supprimez le nom, puis saisissez le nouveau nom.

1. (Facultatif) Pour partager la nouvelle version du rapport avec d’autres utilisateurs, cliquez sur **Actions de rapport**, puis **Partage**.

   >[!NOTE]
   >
   >Les informations de partage ne sont pas transférées vers le rapport copié à partir de la version d’origine.\
   >Pour plus d’informations sur la manière de voir avec qui le rapport précédent a été partagé, voir [Créer un rapport sur les activités de reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Facultatif) Si vous disposez des autorisations Manage (Gérer) pour le rapport d’origine et que ce dernier n’est plus nécessaire, vous pouvez le supprimer afin de supprimer les rapports superflus dupliqués dans Workfront.

   Pour supprimer le rapport d’origine, procédez comme suit :

   1. Accédez au rapport.
   1. Cliquez sur **Actions de rapport**, puis **Supprimer**.

   1. Cliquez sur **Oui, la supprimer** pour confirmer la suppression du rapport.

## Création d’une version d’un rapport {#create-a-new-version-of-a-report}

Si vous souhaitez créer une copie d’un rapport par défaut, procédez comme suit :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**, puis **Tous les rapports**.
1. Cliquez sur le nom d’un rapport par défaut pour l’ouvrir.
1. Cliquez sur **Actions de rapport**, puis **Modifier**.

   ![Modifier le rapport](assets/nwe-reportactionsfordefaultreport-2022.png)

1. Apportez les modifications nécessaires dans les onglets suivants du rapport :

   * **Colonnes (affichage)**: Pour plus d’informations sur la personnalisation des vues, reportez-vous à l’article [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Groupements**: Pour plus d’informations sur la personnalisation des regroupements, consultez l’article . [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filtres**: Pour plus d’informations sur la personnalisation des filtres, voir l’article [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Graphique**: Pour plus d’informations sur la personnalisation d’un graphique de rapport, reportez-vous à l’article [Ajout d’un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Dans le coin supérieur droit, cliquez sur **Paramètres des rapports**.
1. Dans le **Titre du rapport** , attribuez un nouveau nom au rapport.
1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer comme nouveau rapport**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (Facultatif) Pour partager la nouvelle version du rapport avec d’autres utilisateurs, cliquez sur **Actions de rapport**, puis **Partage**.
