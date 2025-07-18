---
title: Dépublication d’un formulaire de demande dans Adobe Workfront Planning
description: Vous pouvez dépublier un formulaire de demande s’il n’est plus nécessaire ou pertinent. En dépubliant, vous supprimez les autorisations d’accès au formulaire accordées à tous.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 21%

---

# Dépublication d’un formulaire de demande dans Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez dépublier un formulaire de demande s’il n’est plus nécessaire ou pertinent. En dépubliant, vous supprimez les autorisations d’accès au formulaire accordées à tous.

Vous pouvez également modifier les entités avec lesquelles vous partagez un formulaire de demande, si vous souhaitez qu’il reste disponible pour un plus petit groupe de personnes.

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
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>

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
   <li><p>Gérer les autorisations pour un espace de travail <span class="preview">et le type d’enregistrement</span> </p></li>
    <li><p>L’administration système peut gérer les espaces de travail qu’elle n’a pas créés. </p></li>
    </ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p>  
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

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Gérer les formulaires de demande**.

   Tous les formulaires de demande associés au type d’enregistrement s’affichent dans une vue tabulaire.
1. Pointez sur le nom d’un formulaire de demande, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite de son nom, puis cliquez sur **Partager**.
1. Mettez à jour les choix de partage en sélectionnant l’une des options suivantes :

   * Toute personne disposant d’un accès en affichage ou supérieur à l’espace de travail
   * Toute personne disposant d’un accès en contribution ou supérieur à l’espace de travail
   * Toute personne disposant du lien

   Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Facultatif) Cliquez sur **Copier le lien**, si vous avez modifié le partage du formulaire de demande et que vous souhaitez le partager avec le nouveau groupe de personnes avec un nouveau lien.

## Dépublication d’un formulaire de demande pour un type d’enregistrement

Lorsqu’un formulaire de demande devient non pertinent et que vous ne souhaitez plus que quiconque y accède, vous pouvez le dépublier.

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre en mode Tableau.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Gérer les formulaires de demande**.

   Tous les formulaires de demande associés au type d’enregistrement s’affichent dans une vue tabulaire.
1. Pointez sur le nom d’un formulaire de demande, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite de son nom, puis cliquez sur **Dépublier**

Ou

Cliquez sur le nom du formulaire de demande pour l’ouvrir, puis cliquez sur **Dépublier** dans le coin supérieur droit du formulaire de demande.

![Bouton Dépublier mis en surbrillance](assets/unpublish-button-highlighted.png)

Un message de confirmation s’affiche au bas de l’écran pour vous informer que la publication du formulaire a été annulée.

Le lien ou le bouton **Dépublier** devient **Publier**.

1. (Conditionnel) Cliquez sur **Enregistrer** si vous avez dépublié le formulaire après l’avoir ouvert.

   Les utilisateurs ne peuvent plus accéder au formulaire de demande à partir d’un lien ou de la file d’attente des demandes dans la zone des Demandes de Workfront.

   Tous les enregistrements précédemment ajoutés à l’aide du formulaire de demande restent sur la page du type d’enregistrement.

   Toutes les demandes précédemment ajoutées restent dans la zone des Demandes de Workfront, dans l’onglet Planification .
