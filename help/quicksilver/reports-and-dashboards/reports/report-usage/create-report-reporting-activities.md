---
product-area: reporting
keywords: change,propriétaire,partagé,rapport,partager,run,utilisateur,accès,droits,entrée,dernier,affichage,date,création de rapports,activités
navigation-topic: report-usage
title: Créer un rapport sur les activités de reporting
description: Lorsque vous créez un rapport sur les rapports, vous pouvez identifier des informations spécifiques sur les rapports, notamment si des rapports sont attribués à des utilisateurs désactivés, si des rapports sont configurés pour s’exécuter avec les droits d’accès d’un utilisateur désactivé, si des utilisateurs accèdent à un rapport que vous prévoyez de supprimer, etc.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 2%

---

# Créer un rapport sur les activités de reporting

Lorsque vous créez un rapport sur les rapports, vous pouvez identifier des informations spécifiques sur les rapports, notamment si des rapports sont attribués à des utilisateurs désactivés, si des rapports sont configurés pour s’exécuter avec les droits d’accès d’un utilisateur désactivé, si des utilisateurs accèdent à un rapport que vous prévoyez de supprimer, etc.

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
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créer un rapport sur les rapports existants {#create-the-report-about-existing-reports}

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Rapports**, puis **Nouveau rapport**.
1. Dans le **Nouveau rapport** menu déroulant, sélectionnez **Rapport** pour créer un rapport sur les rapports existants.

1. Dans le **Colonnes (affichage)** ajoutez les colonnes de votre choix dans votre rapport.\
   Certains des champs suivants peuvent s’avérer utiles :

   | Champ | Description |
   |---|---|
   | **Exécuter en tant qu’utilisateur : Nom** | Il s’agit de l’utilisateur spécifié dans la variable **Exécutez ce rapport avec les droits d’accès de :** sur le rapport. Si cet utilisateur est désactivé, aucun rapport ne s’affiche pour les utilisateurs avec lesquels le rapport est partagé. |
   | **Partagé avec** | Il s’agit de toutes les entités avec lesquelles le rapport est partagé. |
   | **Entré par** | C&#39;est le propriétaire du rapport. |
   | **Dernière date d&#39;affichage** | Il s’agit de la date et de l’heure de la dernière consultation du rapport par un utilisateur. |

   {style=&quot;table-layout:auto&quot;}

1. (Facultatif) Pour limiter votre liste de rapports à des utilisateurs désactivés spécifiques :

   1. Sélectionnez la **Filtres** , puis cliquez sur **Ajouter une règle de filtre**.

   1. Ajouter le filtre **Exécuter comme ID utilisateur** > **Égal**.

   1. Saisissez le nom de l’utilisateur désactivé à ajouter au filtre, puis cliquez sur le nom qui s’affiche dans la liste.
   1. Répétez l’étape C jusqu’à ce que vous ayez sélectionné tous les utilisateurs désactivés à inclure dans le rapport.

1. (Facultatif) Pour limiter votre liste de rapports aux rapports planifiés :

   1. Sélectionnez la **Filtres** , puis cliquez sur **Ajouter une règle de filtre**.

   1. Ajouter le filtre **Identifiant de rapport planifié** > **N’est pas vierge**.

1. Cliquez sur **Enregistrer + Fermer**, puis saisissez le nom du rapport, puis cliquez sur **Enregistrer le rapport**.

   Les informations de votre rapport s’affichent.

1. (Facultatif) Exportez ce rapport dans Excel et enregistrez-le sur votre ordinateur.\
   Pour plus d’informations sur l’export d’un rapport, voir [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Mise à jour d’informations sur un rapport

Une fois votre rapport créé, vous pouvez le mettre à jour selon vos besoins.

1. Accédez au rapport que vous souhaitez mettre à jour.
1. Selon l’action que vous souhaitez effectuer, effectuez l’une des opérations suivantes :

   * Mettez à jour le **Exécutez ce rapport avec les droits d’accès de :** à un utilisateur principal : Pour plus d’informations, voir [Exécution et diffusion d’un rapport avec les droits d’accès d’un autre utilisateur](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Créez une copie du rapport : Pour plus d’informations, voir [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Supprimer un rapport : pour plus d’informations, voir la section [Créer une copie exacte d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) section de l’article [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Partager un rapport : pour plus d’informations, voir [Partage d’un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Conditionnel) Si vous copiez les rapports d’origine, utilisez les informations du rapport que vous avez créé dans [Créer un rapport sur les rapports existants](#create-the-report-about-existing-reports) pour partager les nouvelles copies avec les mêmes entités que les rapports d’origine.
