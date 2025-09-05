---
title: Gestion du Workspace GenStudio dans Adobe Workfront Planning
description: L’espace de travail GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits et que votre instance de Workfront est intégrée à l’instance de GenStudio de votre société. Vous pouvez afficher l’espace de travail GenStudio à partir de Planning et mettre à jour les informations dans les deux systèmes.
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4745b93e02c9de087afbee752e0303280e52d688
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 3%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# Gestion de l’espace de travail GenStudio dans Adobe Workfront Planning

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

L’espace de travail Adobe GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits et que votre instance de Workfront est intégrée à l’instance de GenStudio de votre société.

Vous pouvez afficher l’espace de travail GenStudio à partir de Planning et mettre à jour les informations dans les deux systèmes.

Pour plus d’informations sur l’utilisation et la gestion de l’espace de travail GenStudio à partir de GenStudio Performance Marketing, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home).

Pour obtenir des informations générales sur l’intégration de GenStudio à Workfront Planning, voir [Prise en main de l’intégration d’Adobe Workfront Planning et d’Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

>[!IMPORTANT]
>
>Les étapes décrites dans cet article illustrent comment mettre à jour l’espace de travail GenStudio à partir de Workfront Planning lorsque vous disposez des autorisations de gestion pour celui-ci.
>> Toutes les fonctionnalités ne sont pas disponibles lorsque vous disposez des autorisations de niveau Contribution pour l’espace de travail GenStudio.
>
>Si votre société dispose de plusieurs instances de Workfront, tous les utilisateurs disposent des autorisations de niveau Contribution sur l’espace de travail GenStudio dans Workfront Planning.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout package Workfront</p>
<p>N’importe quel package Planning</p>

</td> </tr>
   <tr> 
<td> 
   <p> Produits supplémentaires</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Rôles utilisateur Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Tout rôle d’utilisateur GenStudio pour accéder aux campagnes, aux produits et aux rôles</li>
   <li>GenStudio System Manager pour accéder aux activations et aux événements</li></ul>
   Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> Rôles utilisateur et autorisations </a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  
   <p>Dans Workfront Planning : </p>
   <ul>
   <li><p>Gérez les autorisations de l’espace de travail GenStudio pour modifier l’architecture de l’espace de travail, les types d’enregistrements et les champs</p></li>
   <li><p>Autorisations de contribution à l’espace de travail GenStudio pour ajouter, mettre à jour ou supprimer des enregistrements dans l’espace d’enregistrement GenStudio</p> </li> 
   </ul>
   <p>Dans Adobe GenStudio for Performance Marketing : <p>
   <ul>
   <li><p> Toutes les autorisations dans Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Création d’autorisations dans Adobe GenStudio for Performance Marketing pour créer des éléments</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur l’accès à Adobe Workfront Planning, consultez [Présentation de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Pour plus d’informations sur Adobe GenStudio for Performance Marketing, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home).

+++   

<!--Old/ original table:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Adobe Workfront Workflow package</p>
<p>Any Adobe Workfront Planning package</p>  

   </td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio package</p></td> 
   <td> 
<p>??? DOES GEN STUDIO HAVE A PACKAGE THAT SUPPORTS THIS???</p>  

   </td> </tr>
 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio license</p></td> 
   <td><p> ??? DOES GEN STUDIO REQUIRE A SPECIFIC LICENSE THAT SUPPORTS THIS???</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
   <p>Configuration for GenStudio: ???WHAT IS THE ACCESS LEVEL NEED FOR GENS???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions*</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Contribute or higher permissions to a workspace and record type  </p> </li> 
   <li><p>System Administrators have permissions to all workspaces, including the ones they did not create</p></li>
   </ul>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Considérations relatives à la gestion d’un espace de travail GenStudio dans Workfront Planning

* Votre entreprise doit acheter Adobe GenStudio for Performance Marketing avant de pouvoir afficher un espace de travail GenStudio dans Workfront Planning.

* Les utilisateurs de Workfront doivent avoir accès à GenStudio pour pouvoir voir l’espace de travail GenStudio dans Workfront Planning.

* En fonction du nombre d’instances Workfront dont dispose votre organisation, vous disposez automatiquement des autorisations suivantes sur l’espace de travail GenStudio dans Planning :

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>Une instance de Workfront</p></td> 
      <td> 
   <p>Il existe un espace de travail GenStudio dans Workfront Planning</p>
   <p>Tous les utilisateurs ayant accès à GenStudio et à Workfront Planning disposent des autorisations de niveau Gérer sur l’espace de travail GenStudio</p> 
   </td> </tr>
      <tr> 
   <td> 
      <p> Instances multiples de Workfront</p> </td> 
      <td> 
      <p>Il existe un espace de travail GenStudio dans chaque instance de Workfront Planning</p>
   <p>Tous les utilisateurs ayant accès à GenStudio et à Workfront Planning disposent d’autorisations de niveau Contribution dans l’espace de travail GenStudio de chaque instance</p> </td> 
   </tr>

  </tbody> 
   </table>

* La mise à jour de la configuration de l’espace de travail, des types d’enregistrements, des vues et des champs pour un espace de travail GenStudio est identique à la mise à jour d’un espace de travail Workfront Planning avec ses éléments.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Gestion de l’espace de travail GenStudio à partir de Workfront Planning

>[!NOTE]
>
>Avant de gérer l’espace de travail GenStudio, consultez l’article [Prise en main de l’intégration de Workfront Planning and GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) pour plus d’informations.
>

1. Connectez-vous à Workfront en tant qu’utilisateur ayant également accès à GenStudio.
1. Cliquez sur l&#39;icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Planification]**.

   La page principale Planification de Workfront s’ouvre.

1. Cliquez sur **Autres espaces de travail** et recherchez un espace de travail qui comporte une indication créée par le **Système** et la balise **GenStudio** sur sa carte.

   ![Carte d’espace de travail GenStudio avec balise ](assets/genstudio-card-with-tag-highlighted.png)

1. Cliquez sur la carte **Espace de travail GenStudio** pour ouvrir l’espace de travail GenStudio dans Workfront Planning.
1. Par défaut, les types d’enregistrements GenStudio suivants sont créés et visibles à partir de Workfront Planning :

   * Campagnes
   * Produits
   * Personas
   * Activations
   * Canaux
   * Régions

   La carte de type d’enregistrement GenStudio indique qu’ils ont été créés à l’origine dans GenStudio.

   <!--check screen shot-->

   ![Carte de type enregistrement GenStudio avec balise](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’espace de travail, puis cliquez sur l’une des options suivantes :

   * **Modifier**

     Pour plus d’informations, voir [Modifier les espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. Cliquez sur **Partager** dans le coin supérieur droit pour partager l’espace de travail avec d’autres personnes.

   Pour plus d’informations, voir [Partager des espaces de travail](/help/quicksilver/planning/access/share-workspaces.md)

1. Cliquez sur l’une des cartes de type d’enregistrement pour afficher les enregistrements de ce type.

   Pour gérer le type d’enregistrement, les vues et les champs, reportez-vous à la section [Gérer les types d’enregistrement GenStudio à partir de Workfront Planning](#manage-genstudio-record-types-from-workfront-planning) dans cet article.


## Gérez les types d’enregistrements, les vues et les enregistrements de l’espace de travail GenStudio dans Workfront Planning

>[!NOTE]
>
>Avant de gérer l’espace de travail GenStudio, consultez l’article [Prise en main de l’intégration de Workfront Planning and GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) pour plus d’informations.
>

1. Accédez à l’espace de travail GenStudio dans Workfront Planning et ouvrez une page de type d’enregistrement, comme décrit dans la section [Gérer l’espace de travail GenStudio à partir de Workfront Planning](#manage-the-genstudio-workspace-from-workfront-planning) de cet article.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur l’une des options suivantes :

   * **Modifier**

     Pour plus d’informations, voir [Modifier les types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md).
   * **Gestion des automatisations**

     Pour plus d’informations, voir [Configuration des automatisations d’Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).
   * **Gérer les formulaires de demande**

     Vous pouvez créer plusieurs formulaires de demande. Les formulaires de demande seront disponibles dans la zone des Demandes de Workfront et vous pouvez également les partager publiquement ou avec un lien.

     Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

1. Pour gérer la vue et le type d’enregistrement, procédez comme suit :

   * Cliquez sur **Partager** dans le coin supérieur droit de la page du type d’enregistrement, puis cliquez sur l’une des options suivantes :
      * **Partager le type d’enregistrement**
Pour plus d’informations, voir [Partager les types d’enregistrements](/help/quicksilver/planning/access/share-record-types.md).
      * **Partager la vue actuelle**
Pour plus d’informations, voir [Partager des vues](/help/quicksilver/planning/access/share-views.md).
      * **Copiez le lien d’affichage**
Un lien vers la vue est copié dans le presse-papiers.
      * **Exporter la vue courante**
Pour plus d’informations, voir [Exporter des enregistrements en mode Tableau](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

1. Pour gérer les vues de type enregistrement, procédez comme suit :

   * Cliquez sur **+ Affichage** pour créer une vue pour le type d’enregistrement GenStudio.

     Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   * Cliquez sur l’icône **Plein écran** ![Ouvrir l’affichage complet en plein écran](assets/open-full-screen-icon.png) pour ouvrir n’importe quel affichage en mode plein écran.

   * Gérer les éléments d’une vue depuis n’importe quelle vue.

     Par exemple, vous pouvez modifier le filtre, les regroupements, le tri, les paramètres d’une vue, le cas échéant.

     Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

1. Pour ajouter des enregistrements, effectuez l’une des opérations suivantes :

   * Cliquez sur **Nouvel enregistrement** depuis n’importe quel affichage pour créer entièrement des enregistrements

   * Importer des enregistrements à l&#39;aide d&#39;un fichier Excel ou CSV en mode Tableau

   * Cliquez n’importe où dans les vues chronologique ou Calendrier pour ajouter des enregistrements.

     Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

     Les enregistrements sont visibles depuis Workfront et GenStudio.

1. Pour modifier des enregistrements, effectuez l’une des opérations suivantes :

   * Modifier les enregistrements intégrés à partir de la vue Tableau

   * Cliquez sur un enregistrement dans n’importe quel affichage pour ouvrir sa page de détails.

     Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

     Les modifications que vous apportez à partir de l’espace de travail GenStudio dans Planning sont immédiatement visibles à partir de GenStudio.

1. Sélectionnez un enregistrement en mode Tableau, puis cliquez sur **Supprimer**.

   Pour plus d’informations, voir [Supprimer des enregistrements](/help/quicksilver/planning/records/delete-records.md).

   Les enregistrements supprimés sont immédiatement supprimés de GenStudio.

   >[!TIP]
   >
   >Les enregistrements supprimés peuvent être récupérés à partir de la vue Tableau bin Récemment supprimé dans Workfront Planning. Les enregistrements supprimés de GenStudio peuvent également être récupérés à partir de la classe Récemment supprimés dans Workfront Planning.

   Pour plus d’informations, voir [ Restaurer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md)

1. Cliquez sur l’icône + dans le coin supérieur droit de la vue du tableau pour créer les éléments suivants :

   * Champs d’enregistrement

     Pour plus d’informations, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md)

   * Connexions d’enregistrement

     Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md)

     Les champs créés à partir de l’espace de travail GenStudio sont visibles dans les zones suivantes :

      * Vues Workfront Planning
      * Détails de l’enregistrement Workfront Planning
      * Détails de l’enregistrement GenStudio

     >[!TIP]
     >
     >Les champs créés dans Workfront Planning ne sont pas visibles dans la vue Liste de GenStudio.

1. Pointez sur un champ en mode Tableau, puis cliquez sur le menu déroulant pour effectuer l’une des opérations suivantes :

   * Trier en fonction de ce critère
   * Masquer
   * Modifier ses paramètres
     <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

     <!--GenStudio-native fields are note removed from GenStudio. -->

     >[!NOTE]
     >
     >Vous pouvez modifier la configuration d’un champ et ajouter d’autres champs uniquement lorsque vous disposez des autorisations de niveau Gérer dans GenStudio.

