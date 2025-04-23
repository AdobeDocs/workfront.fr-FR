---
title: Partager des enregistrements
description: Vous pouvez partager des enregistrements avec d’autres personnes afin d’accroître la collaboration.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 48%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Partager des enregistrements

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Pour collaborer avec d’autres personnes, vous pouvez partager des enregistrements.

Vous pouvez partager un enregistrement Adobe Workfront Planning de différentes manières :

* Copiez le lien de la page d’enregistrement depuis votre navigateur lorsque la page est ouverte.

* Copiez un lien vers la page de l’enregistrement lors de l’affichage des enregistrements dans la vue de table du type d’enregistrement.

* Vous pouvez partager tous les enregistrements d’un espace de travail avec d’autres utilisateurs en partageant l’espace de travail <span class="preview">et le type d’enregistrement</span>.

  Pour plus d’informations, voir les articles suivants :

   * [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [Partager un type d’enregistrement](/help/quicksilver/planning/access/share-record-types.md)

  </div>

Cet article décrit comment copier un lien vers une page d’enregistrement à partir de la vue Tableau d’un type d’enregistrement.

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
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Licence de contributeur ou d’une licence supérieure </p>
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
   <td>  <p>Autorisations d’affichage ou supérieures pour un espace de travail <span class="preview">et un type d’enregistrement</span> à partager   un enregistrement utilisant un lien </p>
   <p>Gérez les autorisations sur un espace de travail <span class="preview">et le type d’enregistrement</span> pour partager les enregistrements dans l’espace de travail </p>
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--replace the layout template info in the table with this at release: 

<div class="preview">
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   <li>Landing page</li>
   <li>Pins</li></ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   <p><b>NOTE</b></p>
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>

-->

## Partager des liens d’enregistrements à partir de la vue en tableau des types d’enregistrements

{{step1-to-planning}}

L’espace de travail auquel vous avez accédé en dernier s’ouvre.
1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.
1. (Le cas échéant) Dans le menu déroulant **Vue** situé dans le coin supérieur droit du tableau, sélectionnez la vue en tableau. Il doit s’agir de la vue par défaut, sauf si vous avez affiché le type d’enregistrement dans la vue chronologique la dernière fois que vous y avez accédé.

   Les enregistrements associés au type d’enregistrement sélectionné s’affichent dans la vue de tableau.
1. Effectuez un clic droit sur une ligne d’enregistrement

   Ou

   Pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Copier le lien**.

   ![Menu contextuel pour la ligne d’enregistrement](assets/contextual-menu-for-record-row.png)

   Le lien est copié dans le presse-papiers.

1. Collez le lien dans un e-mail ou une fenêtre de conversation à partager avec d’autres personnes. Le lien ouvre la page d’enregistrement.

   >[!TIP]
   >
   >Les champs de la page d’enregistrement sont les mêmes que ceux disponibles dans la vue Tableau de l’enregistrement.


   <!--add there when it will be available: if they have access to this record-->

## Partager tous les enregistrements dans un espace de travail en partageant l’espace de travail

Vous pouvez partager tous les enregistrements d&#39;un espace de travail lorsque vous partagez l&#39;espace de travail avec d&#39;autres personnes.

Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent le partager avec d’autres personnes.

Pour plus d’informations, consultez la section [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md).


<div class="preview">

## Partager tous les enregistrements d’un type d’enregistrement en partageant le type d’enregistrement

Dans l’environnement de production, les enregistrements héritent des autorisations de l’espace de travail .

Dans l’environnement Aperçu, les enregistrements héritent des autorisations du type d’enregistrement.

Par défaut, les types d’enregistrements héritent des autorisations de l’espace de travail .

Cependant, vous pouvez effectuer l’une des opérations suivantes :

* Désactivez les autorisations héritées de l’espace de travail sur un type d’enregistrement. Cela supprime les autorisations supérieures des enregistrements, mais conserve les autorisations d&#39;affichage de l&#39;espace de travail, du type d&#39;enregistrement et des enregistrements.
* Octroyez manuellement des autorisations aux utilisateurs pour un type d’enregistrement, même s’ils ne disposent d’aucune autorisation sur l’espace de travail. Ils disposent ainsi automatiquement des autorisations d’affichage pour l’espace de travail. Cela accorde des autorisations aux utilisateurs pour les enregistrements.

Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager ses types d’enregistrements et ses enregistrements avec d’autres utilisateurs.

Pour plus d’informations, voir [Partage de types d’enregistrements](/help/quicksilver/planning/access/share-record-types.md).

</div>
