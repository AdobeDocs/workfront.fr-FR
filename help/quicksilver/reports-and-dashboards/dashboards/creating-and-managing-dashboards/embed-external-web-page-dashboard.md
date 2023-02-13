---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incorporation d’une page web externe dans un tableau de bord
description: Vous pouvez incorporer une page Web externe dans un tableau de bord pour permettre l’accès aux informations connexes provenant d’autres systèmes dans Adobe Workfront ou d’autres pages Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Incorporation d’une page web externe dans un tableau de bord

Vous pouvez incorporer une page Web externe dans un tableau de bord pour permettre l’accès aux informations connexes provenant d’autres systèmes dans Adobe Workfront ou d’autres pages Workfront.

Par exemple, si votre entreprise dispose d’un référentiel de documents Web, d’un wiki ou d’un autre système de gestion de contenu qui contient des informations de projet régulièrement consultées via une URL, vous pouvez afficher ces informations dans Workfront en créant une page externe sur un tableau de bord.

>[!IMPORTANT]
>
>Pour des raisons de sécurité, certains sites web ne vous permettent pas d’incorporer des pages web en tant qu’iframe. Si la page Web que vous souhaitez incorporer dans un tableau de bord ne l’autorise pas, elle ne s’affiche pas dans le tableau de bord. Vous pouvez toutefois accéder à la page externe en cliquant sur le nom du tableau de bord.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Pour permettre l’incorporation d’un site web dont vous êtes propriétaire, demandez à votre administrateur web d’ajuster la variable **X-Frame-Options** . Pour plus d’informations, voir [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Modification de l’accès aux rapports, aux tableaux de bord et aux calendriers</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gestion des autorisations pour le tableau de bord</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Vous devez créer un tableau de bord avant d’y incorporer une page externe.

Pour plus d’informations sur la création de tableaux de bord, voir [Création d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Incorporation d’une page externe dans un tableau de bord

>[!IMPORTANT]
>
>Vous pouvez supprimer une page externe d’un tableau de bord si elle n’est plus nécessaire. Cependant, vous ne pouvez pas supprimer une page externe une fois qu’elle a été créée dans Workfront. Vous ne pouvez supprimer une page externe qu’à l’aide de l’API. Pour plus d’informations, voir [Suppression d’une page externe d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Localisez l’URL de la page à afficher dans Workfront et copiez l’URL située dans la barre d’adresse.

   >[!NOTE]
   >
   >Si vous partagez des URL avec des objets Workfront, n’oubliez pas que certaines URL expirent au fil du temps. Par exemple, les URL de document expirent après leur ouverture. Il s’agit d’une mesure de sécurité. Ils sont, par conception, considérés comme des URL non statiques et ne doivent pas être partagés.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png), puis cliquez sur **Tableaux de bord**.

1. Pour modifier un tableau de bord existant, sélectionnez le tableau de bord dans lequel vous souhaitez incorporer la page du site web, puis cliquez sur **Actions du tableau de bord**, puis sélectionnez **Modifier** dans le menu.\
   Ou\
   Pour créer un tableau de bord, cliquez sur **Nouveau tableau de bord**.\
   Pour plus d’informations sur la création d’un tableau de bord, voir [Création d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Cliquez sur **Ajouter une page externe**.

   ![](assets/qs-add-external-page-350x239.png)

1. Spécifiez un **Nom** pour la page externe.
1. Spécifiez un **Description**.
1. Collez l’URL que vous avez copiée précédemment dans le **URL** champ .\
   Vous pouvez spécifier les types d’URL suivants :

   * URL https (cryptée) vers une page web.\
      Seules les pages https (chiffrées) sont chargées avec l’URL.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * URL de modèle contenant des informations de session pour un site web spécifique.\
      Par exemple : *https://localhost/?session={!$$SESSION}*
Vous devez être connecté au site web spécifié pour afficher la page externe.\
      Pour plus d’informations sur l’obtention d’un ID de session à partir de Workfront, voir [Principes de base des API](../../../wf-api/general/api-basics.md).\
      Pour des raisons de sécurité, votre administrateur Workfront peut configurer vos préférences système de manière à ne pas autoriser l’utilisation des informations de session dans vos pages externes. Dans ce cas, la page externe ne se charge pas sur le tableau de bord.\
      Pour plus d’informations sur les préférences de sécurité du système, voir [Configuration des préférences de sécurité système](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Cliquer sur **Enregistrer**.\
   La page est automatiquement ajoutée au tableau de bord. Si de futurs tableaux de bord sont créés, la page externe peut être ajoutée. La page externe se trouve dans les rapports disponibles.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Mettre à jour une page externe dans un tableau de bord

Pour mettre à jour les informations d’une page externe utilisée dans un tableau de bord :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png), puis cliquez sur **Tableaux de bord**.
1. Sélectionnez le tableau de bord à mettre à jour, puis cliquez sur **Modifier** ![](assets/edit-icon.png).

   ![Sélectionnez l’icône Modifier .](assets/nwe-editdashboard2021-350x188.png)

1. Dans la partie droite de l’écran, recherchez la page externe à mettre à jour, puis cliquez sur le bouton **Modifier** icône .\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. Dans le **Modifier la page externe** , mettez à jour les champs à modifier, puis cliquez sur **Enregistrer**.
1. (Facultatif) Cliquez sur le **Supprimer** icon ![](assets/delete.png) pour supprimer la page externe du tableau de bord. Pour plus d’informations, voir [Suppression d’une page externe d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Dans le coin inférieur gauche, cliquez sur **Enregistrer + Fermer**.

## Affichage des pages externes dans un rapport

Vous pouvez afficher toutes les pages externes de Workfront dans un rapport Page externe .

1. Accédez au **Menu Principal** icon ![](assets/main-menu-icon.png) > **Rapports**.
1. Cliquez sur **Nouveau rapport** > sélectionner **Page externe**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Facultatif) Mettez à jour les onglets Affichage, Filtres ou Groupes du rapport.

   Pour plus d’informations, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Vous pouvez afficher le nom et l’URL associés aux pages externes de votre système dans le nouveau rapport.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
