---
title: Partage d’enregistrements à l’aide d’un lien
description: Vous pouvez partager des enregistrements avec d’autres personnes afin d’accroître la collaboration.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Ct6I5wnivCVr3V86Zj4F7stm2IVUJVH50yvTRyWFuUA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 721
ht-degree: 40%

---

<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Partager des enregistrements à l’aide d’un lien

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Pour collaborer avec d’autres personnes, vous pouvez partager des enregistrements.

Vous pouvez partager un enregistrement Adobe Workfront Planning de différentes manières :

* Copiez le lien de la page d’enregistrement depuis votre navigateur lorsque la page est ouverte.

* Copiez un lien vers la page de l’enregistrement lors de l’affichage des enregistrements dans la vue de table du type d’enregistrement.

* Dans l’environnement de production :

   * Vous pouvez partager tous les enregistrements d’un espace de travail avec d’autres utilisateurs en partageant l’espace de travail et le type d’enregistrement.

     Pour plus d’informations, voir les articles suivants :

      * [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md)

      * [Partager un type d’enregistrement](/help/quicksilver/planning/access/share-record-types.md)

<div class="preview">

* Dans l’environnement de Prévisualisation :

   * Vous pouvez partager des enregistrements individuels avec des personnes, des équipes, des rôles, des groupes ou des entreprises.

     Pour plus d’informations, voir [Partager des enregistrements](/help/quicksilver/planning/access/share-records.md).

</div>



<!--take out the sentence below when we release record-level sharing-->

Cet article décrit comment copier un lien vers une page d’enregistrement à partir de la vue Tableau d’un type d’enregistrement.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront et tout package Planning</p> <p>Tout workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Contributeur ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  <p>Autorisations d’affichage ou supérieures pour un espace de travail et un type d’enregistrement pour partager un enregistrement à l’aide d’un lien</p>
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  


<!--
Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Contributor or higher license </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>
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

Par défaut, les types d’enregistrements et les enregistrements héritent des mêmes autorisations de l’espace de travail .

Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent le partager avec d’autres personnes.

Pour plus d’informations, consultez la section [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md).

## Partager tous les enregistrements d’un type d’enregistrement en partageant le type d’enregistrement

Par défaut, les enregistrements héritent des autorisations du type d’enregistrement .

Par défaut, les types d’enregistrements héritent des autorisations de l’espace de travail .

Cependant, vous pouvez effectuer l’une des opérations suivantes :

* Désactivez les autorisations héritées de l’espace de travail sur un type d’enregistrement. Cela supprime les autorisations supérieures des enregistrements, mais conserve les autorisations d&#39;affichage de l&#39;espace de travail, du type d&#39;enregistrement et des enregistrements.
* Octroyez manuellement des autorisations aux utilisateurs pour un type d’enregistrement, même s’ils ne disposent d’aucune autorisation sur l’espace de travail. Ils disposent ainsi automatiquement des autorisations d’affichage pour l’espace de travail. Par défaut, cela accorde des autorisations d’affichage aux utilisateurs pour les enregistrements.

Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager ses types d’enregistrements et ses enregistrements avec d’autres utilisateurs.

Pour plus d’informations, voir [Partage de types d’enregistrements](/help/quicksilver/planning/access/share-record-types.md).

<div class="preview">

## Partage d’enregistrements individuels

Les utilisateurs héritent par défaut des autorisations d’enregistrement de l’espace de travail et du type d’enregistrement.

Pour n’accorder des autorisations de type enregistrement qu’à certains utilisateurs spécifiques Gérer les autorisations pour certains enregistrements uniquement, vous pouvez désactiver les autorisations héritées pour certains enregistrements et n’accorder à ces utilisateurs qu’un accès Gérer à ces enregistrements.

Vous pouvez ajuster en bloc les autorisations pour un enregistrement ou pour plusieurs enregistrements en même temps.

Pour plus d’informations, voir [Partager des enregistrements](/help/quicksilver/planning/access/share-records.md).

</div>

