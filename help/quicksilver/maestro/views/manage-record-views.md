---
title: Gestion des vues d’enregistrement
description: Vous pouvez afficher les enregistrements dans un tableau ou une chronologie lors de l’utilisation d’Adobe Manager.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---


# Gestion des vues d’enregistrement

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Après avoir sélectionné un type d’enregistrement dans Adobe Manager, vous pouvez afficher tous les enregistrements de ce type dans les vues suivantes :

* Tableau

  Pour plus d’informations, voir [Gestion de la vue de tableau](../views/manage-the-table-view.md).
* Journal

  Pour plus d’informations, voir [Gestion du mode Chronologie](../views/manage-the-timeline-view.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe de produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Tous</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Tous</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Niveau d’accès</td>
   <td> <p>Tous</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/grant-access.md">Accorder l’accès à Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant l’utilisation des vues Maestro

* Les vues dans Maestro sont spécifiques au type d’enregistrement. Vous ne pouvez pas appliquer la même vue à deux types d’enregistrements différents.
* Les vues que vous créez sont visibles pour tous ceux qui accèdent à la zone Maestro. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* La création de vues pour les types d’enregistrements opérationnels est identique à la création de vues pour les types d’enregistrements de taxonomie.
* Lorsque vous modifiez ou supprimez une vue, elle est modifiée et supprimée pour tous les utilisateurs qui peuvent accéder à la zone Maestro.
* Les éléments suivants sont propres à chaque vue dans Maestro :

   * Filtre
   * Regroupement
   * Trier

  <!-- some of these are not available in all of the views - edit above-->

  Par exemple, lors de la création d’un filtre dans une vue de tableau, les résultats du filtre ne sont visibles que dans la vue sélectionnée et non dans toutes les vues répertoriées dans le menu déroulant Affichage .

  >[!NOTE]
  >
  > Comme Maestro est actuellement en version bêta, certains éléments de vue peuvent ne pas être disponibles pour les deux vues.


Cet article décrit les informations suivantes sur les vues Maestro :

* [Création et modification d’une vue](#create-or-edit-record-views)
* [Suppression d’une vue](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
  <!--* [Share a view](#share-views) - not possible yet-->

## Similarités et différences entre les vues de tableau et de chronologie

Le tableau suivant montre les similitudes et les différences entre les vues du tableau et de la chronologie dans Maestro :

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Fonctionnalité | Vue Tableau | Mode Chronologie |
|-----------------------------------------------------------------------|------------|---------------|
| Afficher des enregistrements dans une liste ou une table | ✓ |              |
| Afficher tous les champs sous forme de colonnes dans le tableau, par défaut | ✓ |              |
| Masquer ou afficher des champs (ou des colonnes) | ✓ |               |
| Modifier les valeurs de champ de chaque enregistrement | ✓ |               |
| Ajouter des enregistrements en tant que nouvelles lignes dans la vue | ✓ |               |
| Ajouter des champs en tant que nouvelles colonnes dans la vue | ✓ |               |
| Copier des lignes d’une liste externe et les coller dans un tableau | ✓ |               |
| Afficher des enregistrements dans une chronologie |            | ✓ |
| Filtrage des enregistrements | ✓ | ✓ |
| Enregistrements de groupe |           | ✓ |
| Tri des enregistrements | ✓ |              |

<!--| Sort groupings                                                        | ✓          | ✓             |-->

<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

<!--| Color-code records                     |           | ✓              |-->
<!--| Color-code groupings                     |           | ✓              |-->

## Créer ou modifier des vues {#create-or-edit-views}

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->, puis cliquez sur **Maestro** ![](assets/maestro-icon.png).
L’espace de travail que vous avez consulté pour la dernière fois s’ouvre par défaut. Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md).
1. Cliquez sur une carte de type enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Création de types d’enregistrement](../architecture-and-fields/create-record-types.md).

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent en mode Tableau.

1. Cliquez sur le bouton **Affichage** , puis sélectionnez une **Vue Tableau** ![](assets/table-view-icon.png) ou cliquez sur **Créer une vue > Tableau** pour créer un tableau

   Ou

   Sélectionner un **Mode Chronologie** ![](assets/timeline-view-icon.png) afficher ou cliquer sur **Créer une vue > Chronologie** pour créer une vue chronologique.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Pour créer une vue de chronologie, le type d’enregistrement pour lequel vous créez la vue doit comporter au moins deux champs de date. Dans le cas contraire, l’option Chronologie est grisée.

1. (Facultatif) Mettez à jour le nom de la vue, puis cliquez sur **Créer** pour l’enregistrer.

   Par défaut, Maestro nomme la vue &quot;Tableau &lt; nombre >&quot; ou &quot;Chronologie &lt; nombre >&quot;. Le nombre est un incrément généré automatiquement.

1. (Facultatif) Pour renommer une vue après sa création, cliquez sur le menu déroulant Affichage , puis sur la variable **Plus** menu ![](assets/more-menu.png) > **Renommer** pour mettre à jour le nom de la vue. <!--ensure there is not another saving step here?!-->
1. (Facultatif) Pour gérer un affichage, reportez-vous aux articles suivants pour plus d’informations :

   * [Gestion de la vue de tableau](../views/manage-the-table-view.md)
   * [Gestion du mode Chronologie](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Suppression de vues

1. Dans la **Menu Principal** ![](assets/main-menu-workfront.png) dans le coin supérieur droit de l’écran, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> click **Maestro** ![](assets/maestro-icon.png).

   L’espace de travail que vous avez consulté pour la dernière fois s’ouvre par défaut. Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md).
1. Cliquez sur une carte de type enregistrement.

   Pour plus d’informations sur la création d’un type d’enregistrement, voir [Création de types d’enregistrement](../architecture-and-fields/create-record-types.md).

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent en mode Tableau.

1. Cliquez sur le menu déroulant d’affichage, survolez l’un des affichages de la liste avec la souris, puis cliquez sur l’icône **Plus** menu ![](assets/more-menu.png) > **Supprimer**.
1. Cliquez sur **Supprimer** pour confirmer. <!--ensure there is not another saving step here?!-->

   La vue est supprimée pour tous les utilisateurs qui peuvent accéder à la zone Maestro et elle ne peut pas être récupérée.

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->