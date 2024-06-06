---
title: Créer des espaces de travail
description: Un espace de travail est un ensemble de types d’enregistrement utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans la planification Adobe Workfront. Les types d’enregistrement sont organisés par section dans un espace de travail.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 6%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Créer des espaces de travail

{{planning-important-intro}}

Dans Adobe Workfront Planning, les espaces de travail sont des emplacements centralisés pour que les équipes planifient le travail.

Un espace de travail est un ensemble de types d’enregistrement utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans la planification Adobe Workfront.

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
   Ou
   <p>Actuel : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Vous recevez les autorisations Gérer pour les espaces de travail que vous créez. </p>  
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

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considérations relatives aux espaces de travail

* Vous pouvez créer des espaces de travail pour des entités organisationnelles spécifiques au sein de votre organisation, afin de correspondre au fonctionnement unique de chaque unité.
* Les types d’enregistrement contenus dans un espace de travail doivent correspondre au cycle de vie du travail d’une entité organisationnelle.
* Lorsque vous créez un espace de travail, vous seul êtes autorisé à y accéder et à le gérer. Vous devez le partager avec d’autres utilisateurs afin qu’ils puissent collaborer avec vous dans le même espace. Pour plus d’informations, voir [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md). Les administrateurs système peuvent gérer tous les espaces de travail, même ceux qu’ils n’ont pas créés.
* Vous pouvez disposer des éléments suivants :

   * Jusqu’à 50 sections dans un seul espace de travail.
   * Jusqu’à 1 000 types d’enregistrement de toutes les sections dans un espace de travail. Tous les types d’enregistrement sont propres à chaque espace de travail. <!--this might change-->
   * Jusqu’à 1 000 espaces de travail dans l’instance Workfront de votre entreprise.


## Créer un espace de travail

Vous pouvez créer un espace de travail et y ajouter des types d’enregistrement afin d’organiser vos objets dans la planification Workfront. Pour plus d’informations sur la modification d’un espace de travail, voir [Modification des espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

<!--replace the snippet with the new snippet with the landing page The Workfront Planning landing page opens. 
    ![](assets/planning-landing-page-admin.png)
    1. (Optional) Click the **My workspaces** tab to view workspaces you created
    Or
    Click the **Other workspaces** tab to view workspaces shared with you. 
    -->

1. (Conditionnel) Si votre environnement ne contient aucun espace de travail, cliquez sur **Créer un espace de travail**

   Ou, dans un espace de travail existant, cliquez sur la flèche vers le bas située à droite du nom de l’espace de travail, puis cliquez sur **Créer un espace de travail**.

   ![](assets/workspace-drop-down-right-menu.png)


1. (facultatif et conditionnel) Cliquez sur **Aperçu** dans l’un des modèles d’espace de travail prédéfinis suivants :

   * Gestion marketing
   * Gestion des ventes
   * Gestion des produits

   Il existe une indication des types d’enregistrements opérationnels, des taxonomies et du nombre de champs associés à chaque modèle.

   ![](assets/previewing-a-workspace-template.png)

   Pour plus d’informations sur les modèles d’espace de travail de la planification Workfront, voir [Liste des modèles d&#39;espace de travail](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Cliquez sur **Utiliser un modèle** pour commencer à créer l’espace de travail à partir du modèle sélectionné

   Ou

   Cliquez sur **Créer un espace de travail** pour créer entièrement un espace de travail.

   L’un des types d’espaces de travail suivants est créé :

   * Un espace de travail vide nommé **Espace de travail sans titre** où vous pouvez commencer à ajouter manuellement des types d’enregistrement lorsque vous créez un espace de travail à partir de zéro.
   * Espace de travail nommé d’après le modèle que vous avez sélectionné et rempli avec des exemples de types d’enregistrement. Vous pouvez personnaliser davantage les types d’enregistrement et l’espace de travail.

1. Cliquez à l’intérieur du nom de l’espace de travail dans l’en-tête du nouvel espace de travail pour le renommer, puis appuyez sur Entrée.

1. (Facultatif et conditionnel) Si vous avez créé l’espace de travail à partir d’un modèle, cliquez dans le nom de la fonction **Types d’enregistrement opérationnels** ou **Taxonomies** sections

   Ou

   Passez la souris sur le nom d’une section, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Renommer** pour renommer la section .

   >[!TIP]
   >
   >Vous pouvez renommer n’importe quelle section à partir de n’importe quel espace de travail, même si vous n’avez pas créé la section.

   Pour plus d’informations sur la modification des espaces de travail, y compris la modification des sections de l’espace de travail, voir [Modification des espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Facultatif) Cliquez sur **Ajouter un type d’enregistrement** pour ajouter des types d’enregistrement à l’espace de travail dans n’importe quelle section.

   Pour plus d’informations, voir [Création de types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   Pour plus d’informations sur la modification et la suppression des types d’enregistrement dans un espace de travail, voir [Modification des espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).


