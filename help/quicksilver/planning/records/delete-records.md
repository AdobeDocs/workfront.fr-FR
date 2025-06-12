---
title: Supprimer enregistrements
description: Vous pouvez supprimer des enregistrements que vous ou une autre personne avez créés.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 36%

---


# Supprimer des enregistrements

<!--take Preview and Production references out at release-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez supprimer des enregistrements qui ne sont plus pertinents dans Adobe Workfront Planning. Vous pouvez récupérer les enregistrements supprimés pendant 30 jours après leur suppression. Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations de niveau Contribution ou supérieur à un espace de travail <span class="preview">et type d’enregistrement</span> </a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations sur la suppression des enregistrements

* Vous pouvez supprimer des enregistrements que vous ou une autre personne avez créés.
* Vous ne pouvez pas récupérer les enregistrements supprimés dans l’environnement de production. Vous pouvez récupérer les enregistrements supprimés dans l’environnement de Prévisualisation.
* Lorsque des enregistrements supprimés sont liés à d’autres enregistrements, ces enregistrements liés restent intacts, bien que les informations de l’enregistrement supprimé soient éliminées.
* Vous ne pouvez pas supprimer des enregistrements des vues Chronologie ou Calendrier.

## Supprimer des enregistrements

Vous pouvez supprimer un enregistrement à partir des zones suivantes :

* [À partir de la page de l’enregistrement](#delete-a-record-from-the-records-page)
* [À partir de la vue de tableau d’un type d’enregistrement](#delete-a-record-from-the-record-type-table-view)

### Supprimer un enregistrement à partir de la page de l’enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page du type d’enregistrement s’ouvre.
1. Utilisez l’une des méthodes suivantes :

   * À partir d’une vue en tableau, cliquez sur le nom d’un enregistrement.
   * En mode Tableau, passez la souris sur le nom d’un enregistrement, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Affichage**

     ![Menu contextuel pour la ligne d’enregistrement](assets/contextual-menu-for-record-row.png)
   * Dans une vue de chronologie, cliquez sur une barre d’un enregistrement.

   La page de l’enregistrement s’ouvre.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez de nouveau sur **Supprimer**, **Supprimer** pour confirmer.

   ![Plus d’options de menu à partir de la page des détails de l’enregistrement ](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
L’enregistrement est supprimé.
1. (Facultatif et conditionnel) Si vous supprimez l&#39;enregistrement dans l&#39;environnement Aperçu, accédez à la vue Tableau de la page d&#39;enregistrement, puis cliquez sur l&#39;icône **Annuler** ![Icône Annuler](assets/undo-icon.png) dans le coin supérieur droit de la vue, puis cliquez sur **Récemment supprimé** pour récupérer les enregistrements supprimés.

Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).

### Supprimer un enregistrement de la vue en tableau d’un type enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.
1. (Conditionnel) Dans le menu déroulant **Afficher** situé dans le coin supérieur gauche du tableau, sélectionnez une vue de tableau. Il s’agit de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue Chronologique lors de votre dernier accès.

   Les enregistrements associés au type d’enregistrement sélectionné s’affichent dans la vue Tableau.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez avec le bouton droit de la souris sur une ligne d’enregistrement, puis cliquez sur **Supprimer**.
   * Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez sur **Supprimer**.

     ![Menu contextuel pour la ligne d’enregistrement](assets/contextual-menu-for-record-row.png)

   * Cliquez sur l’icône **Ouvrir les détails** ![Icône Ouvrir les détails dans le champ nom de la table](assets/open-details-icon-in-table-name-field.png) pour ouvrir la zone contenant les informations détaillées de l’enregistrement, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’enregistrement, puis sur **Supprimer**.

   L’enregistrement est supprimé.

1. (Facultatif) Effectuez l’une des opérations suivantes pour annuler ou rétablir la suppression d’un enregistrement :

   * Cliquez sur l&#39;icône **Annuler** ![Icône Annuler](assets/undo-icon.png), puis **Récemment supprimé** pour récupérer les enregistrements supprimés. Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Utilisez les raccourcis clavier suivants pour annuler ou rétablir la suppression d’un enregistrement :

      * Ctrl + Z (⌘ + Z pour Mac) pour annuler la suppression d’un enregistrement
      * Ctrl+Maj+Z (⌘+Maj+Z pour Mac) pour rétablir la suppression de l’enregistrement.




