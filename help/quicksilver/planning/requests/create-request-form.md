---
title: Création d’un formulaire de demande dans Adobe Workfront Planning
description: Après avoir sélectionné un type d’enregistrement dans la zone de planification Adobe Workfront, vous pouvez créer un formulaire de demande associé à ce type d’enregistrement et partager un lien avec celui-ci avec d’autres utilisateurs internes ou externes.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 20%

---

# Création d’un formulaire de demande dans Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Après avoir sélectionné un type d’enregistrement dans la zone de planification Adobe Workfront, vous pouvez créer un formulaire de demande et l’associer à ce type d’enregistrement. Vous pouvez ensuite partager un lien vers ce lien avec d’autres utilisateurs internes ou externes. <!--double-check on the external part of it-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Pour pouvoir accéder à Workfront Planning, vous devez disposer des éléments suivants :

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
   <td role="rowheader"><p>Forfait Adobe Workfront*</p></td>
   <td>
<p>L’un des projets Workfront suivants est prévu :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p>
   </td>

<tr>
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td>
   <td>
<p>N’importe quelle </p>   </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
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

* Pour plus d’informations sur les exigences d’accès à Workfront, consultez les [Conditions d’accès requises dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un formulaire de demande pour un type d’enregistrement

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page de type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type enregistrement s’ouvre dans la vue de tableau.

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Créer un formulaire de demande**.
1. Mettez à jour le nom du formulaire de requête. Par défaut, le nom du formulaire est **Formulaire de demande sans titre**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Facultatif) Ajoutez une **description** pour le formulaire de demande.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Cliquez sur **Créer**. Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre.

   Le formulaire de demande contient les informations suivantes, par défaut :

   * **Section par défaut** : il s’agit du saut de section par défaut appliqué par Workfront au formulaire de demande. La section Par défaut ne peut pas être renommée ni supprimée.
   * **Objet** : champ qui identifie la demande dans Workfront. Cette fonctionnalité n’est pas encore disponible.
   * Tous les champs associés au type d&#39;enregistrement.

   Les champs contenus dans le formulaire de demande seront visibles par tous ceux qui envoient une demande à ce type d’enregistrement.

1. (Facultatif) Supprimez le champ **Objet**, car celui-ci n’est pas visible dans la planification Workfront. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Pointez sur les champs du formulaire à supprimer. Ils sont ajoutés à l’onglet **Champs** sur le côté gauche du formulaire.
1. Cliquez sur un champ, puis utilisez les commandes situées à droite du formulaire pour définir les informations suivantes sur les champs :

   * **Libellé** : il s’agit du nom du champ tel qu’il apparaîtra sur le formulaire de demande. Cela ne modifie pas le nom du champ d’enregistrement.
   * **Instructions** : ajoutez des informations supplémentaires sur le champ.
   * **Créer un champ obligatoire** : lorsque cette option est sélectionnée, le champ doit avoir une valeur. Sinon, le formulaire ne peut pas être envoyé.
   * **Ajouter une logique** : définissez les conditions qui doivent être remplies pour que le champ s’affiche ou soit masqué.

1. Cliquez sur l’onglet Eléments de contenu situé à droite du formulaire, puis ajoutez l’un des éléments suivants :

   * Texte descriptif
   * Saut de section

   Pour plus d’informations sur la création d’un formulaire personnalisé, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).





