---
product-area: reporting
keywords: modifier,personne propriétaire,partagé,rapport,partager,exécuter,utilisateur ou utilisatrice,accès,droits,enré,dernier,affiché,date,reporting,activités
navigation-topic: report-usage
title: Créer un rapport sur les activités de création de rapports
description: Lorsque vous créez un rapport sur les rapports, vous pouvez identifier des informations spécifiques sur les rapports, notamment si des rapports sont attribués à des personnes désactivées, si des rapports sont configurés pour s’exécuter avec les droits d’accès d’une personne désactivée, si des personnes accèdent à un rapport que vous prévoyez de supprimer, etc.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 97%

---

# Créer un rapport sur les activités de création de rapports

Lorsque vous créez un rapport sur les rapports, vous pouvez identifier des informations spécifiques sur les rapports, notamment si des rapports sont attribués à des personnes désactivées, si des rapports sont configurés pour s’exécuter avec les droits d’accès d’une personne désactivée, si des personnes accèdent à un rapport que vous prévoyez de supprimer, etc.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Standard</p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un rapport sur les rapports existants {#create-the-report-about-existing-reports}

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Rapports**, puis sur **Nouveau rapport**.
1. Dans le menu déroulant **Nouveau rapport**, sélectionnez **Rapport** pour créer un rapport sur les rapports existants.

1. Dans l’onglet **Colonnes (Vue)**, ajoutez les colonnes de votre choix dans votre rapport.\
   Certains des champs suivants peuvent s’avérer utiles :

   | champ | Description |
   |---|---|
   | **Exécuter en tant qu’utilisateur ou utilisatice : nom** | Il s’agit de la personne spécifiée dans le champ **Exécuter ce rapport avec les droits d’accès suivants :** sur le rapport. Si cette personne est désactivée, aucun rapport ne s’affiche pour les personnes avec lesquelles le rapport est partagé. |
   | **Partagé avec** | Il s’agit de toutes les entités avec lesquelles le rapport est partagé. |
   | **Saisi par** | Il s’agit de la personne propriétaire du rapport. |
   | **Date de dernière consultation** | Il s’agit de la date et de l’heure de la dernière consultation du rapport par une personne. |

   {style="table-layout:auto"}

1. (Facultatif) Pour limiter votre liste de rapports à des personnes désactivées spécifiques, procédez comme suit :

   1. Sélectionnez l’onglet **Filtres**, puis cliquez sur **Ajouter une règle de filtrage**.

   1. Ajouter le filtre **Exécuter en tant qu’ID d’utilisateur ou d’utilisatrice** > **Égal**.

   1. Saisissez le nom de la personne désactivée à ajouter au filtre, puis cliquez sur le nom qui s’affiche dans la liste.
   1. Répétez l’étape C jusqu’à ce que vous ayez sélectionné toutes les personnes désactivées à inclure dans le rapport.

1. (Facultatif) Pour limiter votre liste de rapports aux rapports planifiés, procédez comme suit :

   1. Sélectionnez l’onglet **Filtres**, puis cliquez sur **Ajouter une règle de filtrage**.

   1. Ajouter le filtre **ID du rapport planifié** > **Non vide**.

1. Cliquez sur **Enregistrer et fermer**, saisissez le nom du rapport, puis cliquez sur **Enregistrer le rapport**.

   Les informations de votre rapport s’affichent.

1. (Facultatif) Exportez ce rapport au format Excel et enregistrez-le sur votre ordinateur.\
   Pour plus d’informations sur l’export d’un rapport, voir [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Mettre à jour les informations sur un rapport

Une fois votre rapport créé, vous pouvez le mettre à jour selon vos besoins.

1. Accédez au rapport que vous souhaitez mettre à jour.
1. Selon l’action que vous souhaitez effectuer, effectuez l’une des opérations suivantes :

   * Mettez à jour le champ **Exécuter ce rapport avec les droits d’accès de :** à un utilisateur ou une utilisatrice actif : pour plus d’informations, voir [Exécuter et diffuser un rapport avec les droits d’accès d’un autre utilisateur ou utilisatrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Créez une copie du rapport : pour plus d’informations, voir [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Supprimez un rapport : pour plus d’informations, voir la section [Créer une copie exacte d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) de l’article [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Partagez un rapport : pour plus d’informations, voir [Partager un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Le cas échéant) Si vous copiez les rapports d’origine, utilisez les informations du rapport que vous avez créé dans [Créer le rapport sur les rapports existants](#create-the-report-about-existing-reports) pour partager les nouvelles copies avec les mêmes entités que les rapports originaux.
