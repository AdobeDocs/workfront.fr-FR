---
product-area: reporting
keywords: change,propriétaire,partagé,rapport,partager,run,utilisateur,accès,droits,entrée,dernier,affichage,date,création de rapports,activités
navigation-topic: report-usage
title: Créer un rapport sur les activités de création de rapports
description: Lorsque vous créez un rapport sur les rapports, vous pouvez identifier des informations spécifiques sur les rapports, notamment si des rapports sont attribués à des utilisateurs désactivés, si des rapports sont configurés pour s’exécuter avec les droits d’accès d’un utilisateur désactivé, si des utilisateurs accèdent à un rapport que vous prévoyez de supprimer, etc.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 18%

---

# Créer un rapport sur les activités de création de rapports

Lorsque vous créez un rapport sur les rapports, vous pouvez identifier des informations spécifiques sur les rapports, notamment si des rapports sont attribués à des utilisateurs désactivés, si des rapports sont configurés pour s’exécuter avec les droits d’accès d’un utilisateur désactivé, si des utilisateurs accèdent à un rapport que vous prévoyez de supprimer, etc.

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
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer un rapport sur les rapports existants {#create-the-report-about-existing-reports}

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Rapports**, puis sur **Nouveau rapport**.
1. Dans la liste déroulante **Nouveau rapport** , sélectionnez **Rapport** pour créer un rapport sur les rapports existants.

1. Dans l&#39;onglet **Colonnes (vues)** , ajoutez les colonnes de votre choix dans votre rapport.\
   Certains des champs suivants peuvent s’avérer utiles :

   | champ | Description |
   |---|---|
   | **Exécuter En Tant Qu’Utilisateur : Nom** | Il s’agit de l’utilisateur spécifié dans le champ **Exécuter ce rapport avec les droits d’accès de :** du rapport. Si cet utilisateur est désactivé, aucun rapport ne s’affiche pour les utilisateurs avec lesquels le rapport est partagé. |
   | **Partagé Avec** | Il s’agit de toutes les entités avec lesquelles le rapport est partagé. |
   | **Entré Par** | C&#39;est le propriétaire du rapport. |
   | **Date de dernière consultation** | Il s’agit de la date et de l’heure de la dernière consultation du rapport par un utilisateur. |

   {style="table-layout:auto"}

1. (Facultatif) Pour limiter votre liste de rapports à des utilisateurs désactivés spécifiques :

   1. Sélectionnez l’onglet **Filtres**, puis cliquez sur **Ajouter une règle de filtre**.

   1. Ajoutez le filtre **Exécuter en tant qu’ID utilisateur** > **Égal**.

   1. Saisissez le nom de l’utilisateur désactivé à ajouter au filtre, puis cliquez sur le nom qui s’affiche dans la liste.
   1. Répétez l’étape C jusqu’à ce que vous ayez sélectionné tous les utilisateurs désactivés à inclure dans le rapport.

1. (Facultatif) Pour limiter votre liste de rapports aux rapports planifiés :

   1. Sélectionnez l’onglet **Filtres**, puis cliquez sur **Ajouter une règle de filtre**.

   1. Ajoutez le filtre **ID de rapport planifié** > **N’est pas vierge**.

1. Cliquez sur **Enregistrer + Fermer**, puis saisissez le nom du rapport et cliquez sur **Enregistrer le rapport**.

   Les informations de votre rapport s’affichent.

1. (Facultatif) Exportez ce rapport dans Excel et enregistrez-le sur votre ordinateur.\
   Pour plus d&#39;informations sur l&#39;export d&#39;un rapport, voir [Export de données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Mise à jour d’informations sur un rapport

Une fois votre rapport créé, vous pouvez le mettre à jour selon vos besoins.

1. Accédez au rapport que vous souhaitez mettre à jour.
1. Selon l’action que vous souhaitez effectuer, effectuez l’une des opérations suivantes :

   * Mettez à jour le champ **Exécuter ce rapport avec les droits d’accès de :** vers un utilisateur actif : pour plus d’informations, voir [Exécution et diffusion d’un rapport avec les droits d’accès d’un autre utilisateur](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Créer une copie du rapport : pour plus d’informations, voir [Création d’une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Supprimer un rapport : pour plus d’informations, voir la section [Créer une copie exacte d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) de l’article [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Partager un rapport : pour plus d’informations, voir [Partager un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Conditionnel) Si vous copiez les rapports d’origine, utilisez les informations du rapport que vous avez créé dans [Créer le rapport sur les rapports existants](#create-the-report-about-existing-reports) pour partager les nouvelles copies avec les mêmes entités que les rapports d’origine.
