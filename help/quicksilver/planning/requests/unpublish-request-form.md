---
title: Annulation de la publication d’un formulaire de requête dans Adobe Workfront Planning
description: Vous pouvez annuler la publication d’un formulaire de requête s’il n’est plus nécessaire ou pertinent. En annulant la publication, vous supprimez les autorisations de tous les utilisateurs pour accéder au formulaire.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 28%

---


# Annulation de la publication d’un formulaire de requête dans Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez annuler la publication d’un formulaire de requête s’il n’est plus nécessaire ou pertinent. En annulant la publication, vous supprimez les autorisations de tous les utilisateurs pour accéder au formulaire.

Vous pouvez également modifier les entités avec lesquelles vous partagez un formulaire de demande, si vous souhaitez le mettre à disposition d’un plus petit groupe de personnes.

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
<p>L’un des projets Workfront suivants est prévu :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p>
   </td>

<tr>
   <td role="rowheader"><p>Package de planification Adobe Workfront*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p>
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

## Modifier le partage d’un formulaire de demande

Si vous partagez publiquement une demande pour , avec toutes les personnes, y compris les utilisateurs de l’extérieur de votre entreprise, vous pouvez envisager de restreindre cet accès à certains utilisateurs qui visualisent ou gèrent l’espace de travail auquel le formulaire est associé.

Pour modifier le partage d’un formulaire de demande :

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type enregistrement s’ouvre dans la vue de tableau.

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Mettre à jour le formulaire de demande**.
1. Cliquez sur **Partager** dans le coin supérieur droit de l’écran, puis mettez à jour les choix de partage. Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Facultatif) Cliquez sur **Copier le lien** si vous avez modifié le partage du formulaire de demande et que vous souhaitez le partager avec le nouveau groupe de personnes disposant d’un nouveau lien.

## Annuler la publication d’un formulaire de demande pour un type d’enregistrement

Lorsqu’un formulaire de demande n’est plus pertinent et que vous ne souhaitez plus que personne y accède, vous pouvez annuler sa publication.

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type enregistrement s’ouvre dans la vue de tableau.

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Mettre à jour le formulaire de demande**.
1. Cliquez sur **Annuler la publication** dans le coin supérieur droit.

   ![](assets/unpublish-button-highlighted.png)

   Une confirmation s’affiche en bas de l’écran pour vous informer que le formulaire a été dépublié.

   Le bouton **Annuler la publication** se transforme en **Publish**.

1. Cliquer sur **Enregistrer**.

   Le formulaire n&#39;est plus accessible à partir d&#39;un lien <!--or from the request queue in the Requests area of Workfront-->.

   Tout enregistrement précédemment ajouté à l’aide du formulaire de demande reste sur la page de type enregistrement.

   <span class="preview">Toutes les requêtes précédemment ajoutées restent dans la zone Demandes de Workfront, dans l’onglet Planification.</span>