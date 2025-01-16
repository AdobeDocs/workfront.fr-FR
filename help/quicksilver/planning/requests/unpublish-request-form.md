---
title: Dépublication d’un formulaire de demande dans Adobe Workfront Planning
description: Vous pouvez dépublier un formulaire de demande s’il n’est plus nécessaire ou pertinent. En dépubliant, vous supprimez les autorisations d’accès au formulaire accordées à tous.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 28%

---

# Dépublication d’un formulaire de demande dans Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez dépublier un formulaire de demande s’il n’est plus nécessaire ou pertinent. En dépubliant, vous supprimez les autorisations d’accès au formulaire accordées à tous.

Vous pouvez également modifier les entités avec lesquelles vous partagez un formulaire de demande, si vous souhaitez qu’il reste disponible pour un plus petit groupe de personnes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
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
   <td>
   <ul>
   <li><p>Gérer les autorisations d’un espace de travail</p></li>
    <li><p>L’administration système peut gérer les espaces de travail qu’elle n’a pas créés. </p></li>
    </ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modification du partage d’un formulaire de demande

Si vous partagez une demande de publiquement, avec tout le monde, y compris les utilisateurs et utilisatrices externes à votre organisation, vous pouvez envisager de restreindre cet accès à certains utilisateurs et utilisatrices qui affichent ou gèrent l’espace de travail auquel le formulaire est associé.

Pour modifier le partage d’un formulaire de demande :

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre en mode Tableau.

1. Cliquez sur le ![](assets/more-menu.png) de menu **Plus** à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Mettre à jour le formulaire de demande**.
1. Cliquez sur **Partager** dans le coin supérieur droit de l’écran, puis mettez à jour les choix de partage. Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Facultatif) Cliquez sur **Copier le lien**, si vous avez modifié le partage du formulaire de demande et que vous souhaitez le partager avec le nouveau groupe de personnes avec un nouveau lien.

## Dépublication d’un formulaire de demande pour un type d’enregistrement

Lorsqu’un formulaire de demande devient non pertinent et que vous ne souhaitez plus que quiconque y accède, vous pouvez le dépublier.

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre en mode Tableau.

1. Cliquez sur le ![](assets/more-menu.png) de menu **Plus** à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Mettre à jour le formulaire de demande**.
1. Cliquez sur **Dépublier** dans le coin supérieur droit.

   ![](assets/unpublish-button-highlighted.png)

   Un message de confirmation s’affiche au bas de l’écran pour vous informer que la publication du formulaire a été annulée.

   Le bouton **Dépublier** devient **Publish**.

1. Cliquer sur **Enregistrer**.

   Le formulaire n&#39;est plus accessible à partir d&#39;un lien <!--or from the request queue in the Requests area of Workfront-->.

   Tous les enregistrements précédemment ajoutés à l’aide du formulaire de demande restent sur la page du type d’enregistrement.

   Toutes les demandes précédemment ajoutées restent dans la zone des Demandes de Workfront, dans l’onglet Planification .
