---
title: Partager des enregistrements
description: Vous pouvez partager des enregistrements avec d’autres personnes afin d’accroître la collaboration.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 74%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Partager des enregistrements

{{planning-important-intro}}

Pour collaborer avec d’autres personnes, vous pouvez partager des enregistrements.

Vous pouvez partager un enregistrement Adobe Workfront Planning de différentes manières :

* Copiez le lien de la page d’enregistrement depuis votre navigateur lorsque la page est ouverte.

* Copiez un lien vers la page de l’enregistrement lors de l’affichage des enregistrements dans la vue de table du type d’enregistrement.

* Vous pouvez partager tous les enregistrements d’un espace de travail avec d’autres personnes en partageant l’espace de travail. Pour plus d’informations, voir [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md).

Cet article décrit comment copier un lien vers une page d’enregistrement à partir de la vue Tableau d’un type d’enregistrement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès pour Workfront Planning.

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
   <td><p> Contributeur, Léger ou Standard </p>
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
   <td>  <p>Autorisations d’affichage ou autorisations supérieures pour un espace de travail afin de partager un enregistrement à l’aide d’un lien </p>
   <p>Gérer les autorisations d’un espace de travail pour partager les enregistrements de l’espace de travail auquel appartient l’enregistrement </p>
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


<!--OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share the workspace the record belongs to </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
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

   Pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![](assets/more-menu.png), puis cliquez sur **Copier le lien**.

   ![](assets/contextual-menu-for-record-row.png)

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
