---
title: Modifier les espaces de travail
description: Vous pouvez modifier les informations d’un espace de travail existant, par exemple le renommer.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 6d9583f8a0e1e0c3712c8a47d68c5d5d321679f9
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 45%

---


# Modifier des espaces de travail

{{planning-important-intro}}

Dans Adobe Workfront Planning, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail.

Un espace de travail est une collection de types d’enregistrements utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Adobe Workfront Planning.

Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

Toutes les modifications apportées à un espace de travail sont visibles par tous ceux qui disposent au moins des autorisations d&#39;affichage de l&#39;espace de travail.

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
   <td>  <p>Gérer les autorisations de l’espace de travail </p>   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD

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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to the workspace </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Planning area to your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Modifier un espace de travail

{{step1-to-planning}}

1. (Sous condition) Si vous êtes un administrateur Workfront, cliquez sur **Espaces de travail sur lesquels je travaille** pour accéder aux espaces de travail que vous avez créés, ou **Autres espaces de travail** pour accéder aux espaces de travail que d’autres personnes ont partagés avec vous.

<!--***********Replace the steps from the next below till the "Update the following information in the Edit workspace box:" (but keep this last step)*******-->

1. (Facultatif) Cliquez sur **Tout afficher** pour afficher des espaces de travail supplémentaires. Le lien **Tout afficher** s’affiche uniquement lorsque vous disposez de plus de deux lignes de cartes d’espace de travail.
1. (Facultatif) Cliquez sur K **Afficher moins** pour limiter le nombre d’espaces de travail affichés à l’écran.
1. Pour modifier un espace de travail, effectuez l’une des opérations suivantes :

   * Pointez sur la carte de l’espace de travail, puis cliquez sur le ![](assets/more-menu.png) de menu **Plus** dans le coin supérieur droit de la carte
Ou
   * Cliquez sur une carte d’espace de travail pour ouvrir l’espace de travail, puis cliquez sur l’![](assets/more-menu.png) du menu **Plus** à droite du nom de l’espace de travail.
1. Cliquez sur **Modifier**.

   La zone **Modifier l’espace de travail** s’affiche.

   ![](assets/edit-workspace-box.png)

1. Mettez à jour les informations suivantes dans la zone **Modifier l’espace de travail** :

   * Ajoutez un nom pour l’espace de travail. <!--did they add a label for this field?-->
   * **Description** : ajoutez des informations sur l’espace de travail.
   * Sélectionnez une icône à associer à l’espace de travail.

1. Cliquez sur **Enregistrer** pour fermer la zone Modifier l’espace de travail et appliquer vos modifications.

1. (Facultatif) Pour ajouter une nouvelle section d’espace de travail, effectuez l’une des opérations suivantes :

   * Cliquez sur **Ajouter une section** au bas de l’espace de travail.
   * Pointez sur le nom d’une section, puis cliquez sur le menu **Plus** ![](assets/more-menu.png), puis cliquez sur **Ajouter la section ci-dessus** ou **Ajouter la section ci-dessous**.

1. (Facultatif) Pour modifier l’emplacement d’une section, effectuez l’une des opérations suivantes :

   * Pointez sur le nom d’une section, puis cliquez sur l’icône **saisir** ![](assets/grab-icon.png), puis faites un glisser-déposer à l’endroit approprié.
   * Pointez sur le nom d’une section, puis cliquez sur le menu **Plus** ![](assets/more-menu.png), puis cliquez sur **Déplacer vers le haut** ou **Déplacer vers le bas**. La section se déplace vers le haut ou vers le bas dans l’espace de travail.

1. (Facultatif) Pour supprimer une section d’espace de travail, procédez comme suit :

   1. Pointez sur le nom d’une section, puis cliquez sur le menu **Plus** ![](assets/more-menu.png), puis cliquez sur **Supprimer**. <!--add screen shot when UI is final?-->
   1. Sélectionnez une nouvelle section pour y déplacer tous les types d’enregistrement, puis cliquez sur **Supprimer**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Tous les types d’enregistrement sont déplacés vers la section de sélection et la section est supprimée.

1. (Facultatif) Cliquez sur **Ajouter un type d’enregistrement** pour ajouter des types d’enregistrement à l’espace de travail.

   Pour plus d’informations, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Facultatif) Pointez sur une carte de type d’enregistrement, cliquez sur le ![](assets/more-menu.png) de menu **Plus** dans le coin supérieur droit, puis cliquez sur **Modifier** pour modifier l’aspect d’un type d’enregistrement.

   Pour plus d’informations, voir [Modifier les types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facultatif) Pointez sur une carte de type d’enregistrement, cliquez sur le ![](assets/more-menu.png) de menu **Plus** dans le coin supérieur droit, puis cliquez sur **Supprimer** pour supprimer un type d’enregistrement.

   Pour plus d’informations, voir [Supprimer des types d’enregistrements](/help/quicksilver/planning/architecture/delete-record-types.md).

1. (Facultatif) Appuyez sur un clic sur une carte de type enregistrement pour la faire glisser et la déposer à un nouvel endroit. Vous pouvez faire glisser et déposer des types d’enregistrements d’une section de l’espace de travail à une autre.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Facultatif) Cliquez sur **Partager** dans le coin supérieur droit de l’espace de travail pour partager l’espace de travail avec d’autres personnes.

   Pour plus d’informations, consultez la section [Partager des espaces de travail](/help/quicksilver/planning/access/share-workspaces.md).
