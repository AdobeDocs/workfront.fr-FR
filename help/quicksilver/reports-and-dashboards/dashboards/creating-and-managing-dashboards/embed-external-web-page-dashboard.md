---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Intégrer une page web externe dans un tableau de bord
description: Vous pouvez incorporer une page Web externe dans un tableau de bord pour permettre l’accès aux informations connexes provenant d’autres systèmes dans Adobe Workfront ou d’autres pages Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 9%

---

# Intégrer une page web externe dans un tableau de bord

<!--Audited: 01/2024-->

Vous pouvez incorporer une page Web externe dans un tableau de bord pour permettre l’accès aux informations connexes provenant d’autres systèmes ou d’Adobe Workfront.

Par exemple, si votre entreprise dispose d’un référentiel de documents Web, d’un wiki ou d’un autre système de gestion de contenu qui contient des informations de projet régulièrement consultées via une URL, vous pouvez afficher ces informations dans Workfront en créant une page externe sur un tableau de bord.

>[!IMPORTANT]
>
>* Pour des raisons de sécurité, certains sites web ne vous permettent pas d’incorporer des pages web en tant qu’iframe. Si la page Web que vous souhaitez incorporer dans un tableau de bord ne l’autorise pas, elle ne s’affiche pas dans le tableau de bord. Vous pouvez toutefois accéder à la page externe en cliquant sur le nom du tableau de bord.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Pour permettre l’incorporation d’un site web dont vous êtes propriétaire, demandez à votre administrateur web d’ajuster le paramètre **X-Frame-Options**. Pour plus d’informations, voir [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).
>
>
>* Les pages de tableau de bord ne sont plus prises en charge en tant que pages externes incorporées dans les tableaux de bord. Bien que les tableaux de bord existants ne soient pas automatiquement modifiés pour supprimer ces pages externes, toute modification apportée à un tableau de bord contenant une telle référence ne pourra pas être enregistrée tant que la référence n’aura pas été supprimée ou modifiée.
> Plus précisément, les sous-domaines Workfront.com suivants ne sont plus pris en charge :
>
>     * &#x200B; des tableaux de bord
>     * /dashboard/:ID &#x200B;
>     * /portfolio/:ID/content-dashboard__:dashboardID &#x200B;
>     * /program/:ID/content-dashboard__:dashboardID &#x200B;
>     * /project/:ID/content-dashboard__:dashboardID &#x200B;
>     * /task/:ID/content-dashboard__:dashboardID &#x200B;
>     * /template/:ID/content-dashboard__:dashboardID &#x200B;
>     * /templatetask/:ID/content-dashboard__:dashboardID &#x200B;
>     * /resourcemanagement/:ID/
>     * content-dashboard__:dashboardID &#x200B;
>     * /Team/:ID/content-dashboard__:dashboardID &#x200B;
>     * /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>     * /requests/:ID/content-dashboard__:dashboardID &#x200B;
>     * /group/:ID/content-dashboard__:dashboardID &#x200B;
>     * /billingrecord/:ID/content-dashboard__:dashboardID
>
>Autre solution : pensez à inclure un rapport de liste dans votre tableau de bord, comme expliqué dans la section [Ajouter un rapport à un tableau de bord](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Actuelle : formule </p>
   Ou
   <p>Nouvelle : standard </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

{{step1-to-dashboards}}

1. Pour modifier un tableau de bord existant, sélectionnez le tableau de bord dans lequel vous souhaitez incorporer la page du site web, puis cliquez sur **Actions du tableau de bord**, puis sur **Modifier**
Ou\
   Pour créer un tableau de bord, cliquez sur **Nouveau tableau de bord**.\
   Pour plus d’informations sur la création d’un tableau de bord, voir [Créer un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Cliquez sur **Ajouter une page externe** sous la zone **Sélectionner la mise en page/Ajouter des rapports/Ajouter des calendriers** .

   ![](assets/qs-add-external-page-350x239.png)

   La zone **Ajouter une page externe** s’affiche.

1. Indiquez les informations suivantes sur la page externe :

   * **Nom** : ajoutez un nom pour le tableau de bord.
   * **Description** : ajoutez plus d’informations sur le tableau de bord pour identifier les informations qu’il contient. La description s’affiche sur le tableau de bord pour toutes les personnes ayant accès à l’afficher, une fois que vous l’avez enregistré.
   * **URL** : collez l’URL que vous avez copiée précédemment dans ce champ.

     Vous pouvez spécifier les types d’URL suivants :

      * URL https (cryptée) vers une page web.\
        Seules les pages https (chiffrées) sont chargées avec l’URL.\
        ![](assets/add-external-page-dialog-qs-350x247.png)

      * URL de modèle contenant des informations de session pour un site web spécifique.\
        Par exemple : *https://localhost/?session={!$$SESSION}*
Vous devez être connecté au site web spécifié pour afficher la page externe.\
        Pour plus d’informations sur l’obtention d’un ID de session à partir de Workfront, voir [Principes de base des API](../../../wf-api/general/api-basics.md).\
        Pour des raisons de sécurité, votre administrateur Workfront peut configurer vos préférences système de manière à ne pas autoriser l’utilisation des informations de session dans vos pages externes. Dans ce cas, la page externe ne se charge pas sur le tableau de bord.\
        Pour plus d’informations sur les préférences de sécurité du système, voir [Configuration des préférences de sécurité du système](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
        ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

     >[!WARNING]
     >
     >L’utilisation de SessionID n’est pas sécurisée et n’est pas recommandée.
     >

   * **Hauteur** : saisissez un nombre supérieur à 0 pour définir l’espace occupé par la page externe sur le tableau de bord. La hauteur par défaut est de 500.

1. Cliquer sur **Enregistrer**.

   La page est automatiquement ajoutée au tableau de bord.

   Si vous créez des tableaux de bord supplémentaires, vous pouvez trouver cette page externe et l’ajouter à d’autres tableaux de bord. Vous trouverez toutes les pages externes existantes dans la liste des Rapports et calendriers disponibles lors de la création ou de la modification d’un tableau de bord.

   <!--
    *** This is linked to: Creating Dashboards, and Editing Dashboards.
   -->

## Mettre à jour une page externe dans un tableau de bord

Pour mettre à jour les informations d’une page externe utilisée dans un tableau de bord :

{{step1-to-dashboards}}

1. Cliquez sur le nom du tableau de bord que vous souhaitez mettre à jour pour l’ouvrir, puis cliquez sur **Actions sur le tableau de bord**, puis sur **Modifier**.

   La zone **Détails du tableau de bord** s’ouvre.

1. Dans la zone **Sélectionner la mise en page / Ajouter des rapports / Ajouter des calendriers** de la zone **Détails du tableau de bord**, recherchez la page externe à mettre à jour, survolez-la avec la souris et cliquez sur l’icône **Modifier**.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. Dans la zone **Modifier la page externe**, mettez à jour les champs que vous souhaitez modifier, puis cliquez sur **Enregistrer**.
1. (Facultatif) Cliquez sur l’icône **Supprimer** ![](assets/delete.png) pour supprimer la page externe du tableau de bord. Pour plus d’informations, voir [Suppression d’une page externe d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Cliquez sur **Enregistrer + Fermer**.

## Affichage des pages externes dans un rapport

Vous pouvez afficher toutes les pages externes de Workfront dans un rapport Page externe .

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport** > sélectionnez **Page externe**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Facultatif) Mettez à jour les onglets Affichage, Filtres ou Groupements du rapport.

   Pour plus d’informations, consultez [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Cliquez sur **Enregistrer+Fermer**.

   Vous pouvez afficher le nom et l’URL associés aux pages externes de votre système dans le nouveau rapport.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
