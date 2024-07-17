---
product-area: reporting;user-management
keywords: save,new,report,copy
navigation-topic: create-and-manage-reports
title: Créer une copie d’un rapport
description: Vous pouvez créer une copie de tout rapport auquel vous avez accès. Vous pouvez soit créer une copie exacte d’un rapport personnalisé, soit enregistrer une nouvelle version d’un rapport par défaut. Après avoir copié un rapport, vous devenez le propriétaire du rapport copié et il s’affiche dans la section Mes rapports .
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 19%

---

# Créer une copie d’un rapport

Vous pouvez créer une copie de tout rapport auquel vous avez accès. Vous pouvez soit créer une copie exacte d’un rapport personnalisé, soit enregistrer une nouvelle version d’un rapport par défaut. Après avoir copié un rapport, vous devenez le propriétaire du rapport copié et il s’affiche dans la section Mes rapports .

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations pour un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer une copie exacte d’un rapport

Si vous souhaitez faire une copie d’un rapport dont vous êtes le propriétaire, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**, puis sur **Tous les rapports**.
1. Ouvrez un rapport.
1. Cliquez sur **Actions de rapport**, puis sur **Copier**.

   >[!TIP]
   >
   >Si le rapport est un rapport par défaut, l’option Copier n’apparaît pas dans le menu Actions de rapport .\
   >Pour plus d&#39;informations sur la création d&#39;une copie d&#39;un rapport par défaut, voir [Création d&#39;une version d&#39;un rapport](#create-a-new-version-of-a-report).

   ![Copier le rapport](assets/nwe-fulllistofreportactions-2022.png)

   Une copie du rapport d’origine est créée avec le nom par défaut *Copie de [Nom du rapport d’origine]*. Par exemple, le nom du rapport &quot;Tâches terminées du quatrième trimestre&quot; serait &quot;Copie des tâches terminées du quatrième trimestre&quot;.

1. (Facultatif) Pour renommer le rapport, commencez à saisir un nouveau nom.

   >[!TIP]
   >
   >Si vous désélectionnez le titre avant de saisir le nouveau nom, sélectionnez le titre du rapport, supprimez le nom, puis saisissez le nouveau nom.

1. (Facultatif) Pour partager la nouvelle version du rapport avec d’autres utilisateurs, cliquez sur **Actions de rapport**, puis sur **Partage**.

   >[!NOTE]
   >
   >Les informations de partage ne sont pas transférées vers le rapport copié depuis la version d’origine.\
   >Pour plus d’informations sur la façon de voir avec qui le rapport précédent a été partagé, voir [Création d’un rapport sur les activités de création de rapports](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Facultatif) Si vous disposez des autorisations Manage (Gérer) pour le rapport d’origine et que ce dernier n’est plus nécessaire, vous pouvez le supprimer afin de supprimer les rapports superflus dupliqués dans Workfront.

   Pour supprimer le rapport d’origine, procédez comme suit :

   1. Accédez au rapport.
   1. Cliquez sur **Actions de rapport**, puis **Supprimer**.

   1. Cliquez sur **Oui, Supprimer** pour confirmer la suppression du rapport.

## Créer une version d’un rapport {#create-a-new-version-of-a-report}

Si vous souhaitez créer une copie d’un rapport par défaut, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**, puis sur **Tous les rapports**.
1. Cliquez sur le nom d’un rapport par défaut pour l’ouvrir.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.

   ![Modifier le rapport](assets/nwe-reportactionsfordefaultreport-2022.png)

1. Apportez les modifications nécessaires dans les onglets suivants du rapport :

   * **Colonnes (vues)** : pour plus d’informations sur la personnalisation des vues, consultez l’article [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Groupings** : pour plus d’informations sur la personnalisation des regroupements, consultez l’article [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filtres** : pour plus d’informations sur la personnalisation des filtres, consultez l’article [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Graphique** : pour plus d’informations sur la personnalisation d’un graphique de rapport, reportez-vous à l’article [Ajout d’un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Dans le coin supérieur droit, cliquez sur **Paramètres de rapport**.
1. Dans le champ **Titre du rapport**, donnez un nouveau nom au rapport.
1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer comme nouveau rapport**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (Facultatif) Pour partager la nouvelle version du rapport avec d’autres utilisateurs, cliquez sur **Actions de rapport**, puis sur **Partage**.
