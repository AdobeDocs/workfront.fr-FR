---
title: Gestion du Workspace GenStudio dans Adobe Workfront Planning
description: L’espace de travail GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits et que votre instance de Workfront est intégrée à l’instance de GenStudio de votre société. Vous pouvez afficher l’espace de travail GenStudio à partir de Planning et mettre à jour les informations dans les deux systèmes.
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 9%

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

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

L’espace de travail Adobe GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits et que votre instance de Workfront est intégrée à l’instance de GenStudio de votre société.

Vous pouvez afficher l’espace de travail GenStudio à partir de Planning et mettre à jour les informations dans les deux systèmes.

Pour plus d’informations sur l’utilisation et la gestion de l’espace de travail GenStudio à partir de GenStudio Performance Marketing, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home).

Pour obtenir des informations générales sur l’intégration de GenStudio à Workfront Planning, voir [Prise en main de l’intégration d’Adobe Workfront Planning et d’Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

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
<p>Tout package de workflow Adobe Workfront</p>
<p>Tout package Adobe Workfront Planning</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Package Adobe GenStudio</p></td> 
   <td> 
<p>??? GEN STUDIO A-T-IL UN PACKAGE QUI PREND EN CHARGE CELA ???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe GenStudio</p></td> 
   <td><p> ??? GEN STUDIO NÉCESSITE-T-IL UNE LICENCE SPÉCIFIQUE PRENANT EN CHARGE CETTE FONCTIONNALITÉ ???</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> Produits supplémentaires</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
   <p>Configuration pour GenStudio : ???QUEL EST LE NIVEAU D’ACCÈS NÉCESSAIRE POUR LES GENS ???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet*</p></td> 
   <td>  
   <p>Dans Workfront Planning : </p>
   <ul>
   <li><p>Autorisations de niveau Contribution ou supérieur à un espace de travail et à un type d’enregistrement  </p> </li> 
   <li><p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p></li>
   </ul>
   <p>Dans Adobe GenStudio for Performance Marketing : <p>
   <ul>
   <li><p> Toutes les autorisations dans Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Création d’autorisations dans Adobe GenStudio for Performance Marketing pour créer des éléments</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Pour plus d’informations sur Adobe GenStudio for Performance Marketing, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home).

+++   

## Considérations relatives à la gestion d’un espace de travail GenStudio dans Workfront Planning

* Votre entreprise doit acheter Adobe GenStudio for Performance Marketing avant de pouvoir afficher un espace de travail GenStudio dans Workfront Planning.

* Les utilisateurs de Workfront doivent avoir accès à GenStudio pour pouvoir voir l’espace de travail GenStudio dans Workfront Planning.

* Vous pouvez mettre à jour les informations suivantes d’un espace de travail GenStudio à partir de Workfront Planning :

   * Modifier les paramètres de l’espace de travail <!--check to see if this is correct? is this editable or read only from Planning??-->
   * Modifiez les types d’enregistrements et leurs champs <!--check on this-->
   * Partager, modifier et ajouter des vues
   * Ajouter de nouveaux types d’enregistrements
   * Modifier, ajouter ou supprimer des enregistrements

* La mise à jour de la configuration de l’espace de travail, des types d’enregistrements, des vues et des champs pour un espace de travail GenStudio est identique à la mise à jour d’un espace de travail Workfront Planning avec ses éléments.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Gestion des types d’enregistrements GenStudio à partir de Workfront Planning

>[!NOTE]
>
>Avant de gérer l’espace de travail GenStudio, consultez l’article [Prise en main de l’intégration de Workfront Planning and GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

1. Connectez-vous à Workfront en tant qu’utilisateur ayant également accès à GenStudio.
1. Cliquez sur l&#39;icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Planification]**.

   La page principale Planification de Workfront s’ouvre.

1. Cliquez sur **Autres espaces de travail** et recherchez un espace de travail qui comporte une indication créée par le **Système** et la balise **GenStudio** sur sa carte.

   ![Carte d’espace de travail GenStudio avec balise ](assets/genstudio-card-with-tag-highlighted.png)

1. Cliquez sur la carte **Espace de travail GenStudio** pour ouvrir l’espace de travail GenStudio dans Workfront Planning.
1. Par défaut, les types d’enregistrements GenStudio suivants sont créés et visibles à partir de Workfront Planning :

   * Campagnes
   * Produits
   * Activations
   * Canaux
   * Régions

   La carte de type d’enregistrement GenStudio indique qu’ils ont été créés à l’origine dans GenStudio.

   <!--check screen shot-->

   ![Carte de type enregistrement GenStudio avec balise](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Cliquez sur l’une des cartes de type d’enregistrement pour afficher les enregistrements de ce type.

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **Partager** dans le coin supérieur droit de la page du type d’enregistrement, puis cliquez sur l’une des options suivantes :
      * **Copiez le lien d’affichage** pour partager un lien vers le type d’enregistrement.
      * **Exporter la vue actuelle** pour l&#39;exporter au format CSV ou Excel.
Vous pouvez uniquement exporter la vue Tableau. <!--check on this later; is this true or are there more options in the Share button-->

   * Cliquez sur **+ Affichage** pour créer une vue pour le type d’enregistrement GenStudio.

     Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   * Cliquez sur l’icône **Plein écran** ![Ouvrir l’affichage complet en plein écran](assets/open-full-screen-icon.png) pour ouvrir n’importe quel affichage en mode plein écran.

   * Gérer les éléments d’une vue depuis n’importe quelle vue.

     Par exemple, vous pouvez modifier le filtre, les regroupements, le tri, les paramètres d’une vue, le cas échéant.

     Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   * Ajoutez des enregistrements dans le tableau ou la vue chronologique.

     Vous pouvez uniquement créer des enregistrements à partir de zéro ou en important un fichier CSV ou Excel.

     Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

     Les enregistrements sont visibles depuis Workfront et GenStudio.

   * Modifiez des enregistrements intégrés à partir de la vue Tableau ou cliquez sur un enregistrement pour ouvrir sa page de détails.

     Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

   * Supprimer les enregistrements en mode Tableau.

     Pour plus d’informations, voir [Supprimer des enregistrements](/help/quicksilver/planning/records/delete-records.md).

     Les enregistrements supprimés peuvent être récupérés à partir de la corbeille de la vue Tableau dans Workfront Planning, s’ils sont supprimés de Workfront.

     Pour plus d’informations, voir [ Restaurer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md)

   * Pointez sur un champ en mode Tableau pour trier ou masquer le champ.

     >[!NOTE]
     >
     >Vous pouvez modifier la configuration d’un champ et ajouter d’autres champs uniquement lorsque vous disposez des autorisations de niveau Gérer dans GenStudio. <!--check to see if this is true??-->
