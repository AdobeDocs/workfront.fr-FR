---
title: Modifier des espaces de travail
description: Vous pouvez modifier les informations d’un espace de travail existant, par exemple le renommer.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 3856e56036a9845387d7dc6498a6f20728c8234a
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 5%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Modifier des espaces de travail

{{planning-important-intro}}

Dans Adobe Workfront Planning, les espaces de travail sont des emplacements centralisés pour que les équipes planifient le travail.

Un espace de travail est un ensemble de types d’enregistrement utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans la planification Adobe Workfront.

Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

Toutes les modifications que vous apportez à un espace de travail sont visibles par tous ceux qui détiennent au moins les autorisations d’affichage sur l’espace de travail.

## Conditions d’accès

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
   <p> Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouveau : Standard</p>
   <p>Actuel : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Workfront</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations de l’espace de travail </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Vous devez ajouter la zone Planning à votre modèle de mise en page. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Modifier un espace de travail

{{step1-to-planning}}

Cela ouvre la zone Espaces de travail de la planification Workfront.

1. Cliquez dans le nom de l’espace de travail dans l’en-tête du nouvel espace de travail pour le renommer, puis appuyez sur **Entrée**.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png)à droite du nom de l’espace de travail dans l’en-tête, puis cliquez sur **Modifier**.

   ![](assets/edit-workspace-box.png)

   Mettez à jour les informations suivantes dans la variable **Modifier l’espace de travail** box :

   * Ajoutez un nom pour l’espace de travail. <!--did they add a label for this field?-->
   * **Description**: ajoutez des informations sur l’espace de travail.
   * Sélectionnez une icône à associer à l’espace de travail.

1. Cliquez sur **Enregistrer** pour fermer la boîte de dialogue Modifier l’espace de travail et appliquer vos modifications.

1. (Facultatif) Pour ajouter une section d’espace de travail, effectuez l’une des opérations suivantes :

   * Cliquez sur **Ajouter une section** au bas de l’espace de travail.
   * Passez la souris sur le nom d’une section, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Ajouter la section ci-dessus** ou **Ajouter la section ci-dessous**.

1. (Facultatif) Pour modifier l’emplacement d’une section, effectuez l’une des opérations suivantes :

   * Passez la souris sur le nom d’une section, puis cliquez sur le bouton **attraper** icon ![](assets/grab-icon.png), puis faites-le glisser et déposez-le à l’endroit approprié.
   * Passez la souris sur le nom d’une section, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Déplacer vers le haut** ou **Déplacer vers le bas**. La section monte ou descend dans l’espace de travail.

1. (Facultatif) Pour supprimer une section d’espace de travail, procédez comme suit :

   1. Passez la souris sur le nom d’une section, puis cliquez sur l’icône **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Supprimer**. <!--add screen shot when UI is final?-->
   1. Sélectionnez une nouvelle section pour y déplacer tous les types d’enregistrement, puis cliquez sur **Supprimer**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Tous les types d’enregistrement sont déplacés vers la section de sélection et la section est supprimée.

1. (Facultatif) Cliquez sur **Ajouter un type d’enregistrement** pour ajouter des types d’enregistrement à l’espace de travail.

   Pour plus d’informations, voir [Création de types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Facultatif) Passez la souris sur une carte de type enregistrement, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit, puis cliquez sur **Modifier** pour modifier l’aspect d’un type d’enregistrement.

   Pour plus d’informations, voir [Modification des types d’enregistrement](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facultatif) Passez la souris sur une carte de type enregistrement, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit, puis cliquez sur **Supprimer** pour supprimer un type d’enregistrement.

   Pour plus d’informations, voir [Suppression des types d’enregistrement](/help/quicksilver/planning/architecture/delete-record-types.md)).

1. (Facultatif) Appuyez sur une carte de type enregistrement et cliquez dessus pour la faire glisser et la déposer à un nouvel emplacement. Vous pouvez faire glisser et déposer des types d’enregistrement d’une section d’espace de travail vers une autre.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Facultatif) Cliquez sur **Partager** dans le coin supérieur droit de l’espace de travail pour partager l’espace de travail avec d’autres personnes.

   Pour plus d’informations, voir [Partage des espaces de travail](/help/quicksilver/planning/access/share-workspaces.md).