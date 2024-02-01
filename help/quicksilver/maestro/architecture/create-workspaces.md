---
title: Créer des espaces de travail
description: Un espace de travail est un ensemble de types d’enregistrements opérationnels et de taxonomies utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Créer des espaces de travail

{{maestro-important-intro}}

Dans Adobe Maestro, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail.

Un espace de travail est un ensemble de types d’enregistrements opérationnels et de taxonomies utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Maestro.

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
   <p> Produit</p> </td>
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
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouveau : Standard</p>
   <p>Actuel : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe pas de contrôle de niveau d’accès pour Maestro</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Vous recevez les autorisations Gérer pour les espaces de travail que vous créez. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Vous devez ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considérations relatives aux espaces de travail

* Vous pouvez créer des espaces de travail pour des entités organisationnelles spécifiques au sein de votre organisation, afin de correspondre au fonctionnement unique de chaque unité.
* Les types d’enregistrement et les taxonomies contenus dans un espace de travail doivent refléter le cycle de vie du travail d’une entité organisationnelle.
* Lorsque vous créez un espace de travail, vous seul êtes autorisé à y accéder et à le gérer. Vous devez le partager avec d’autres utilisateurs afin qu’ils puissent collaborer avec vous dans le même espace. Pour plus d’informations, voir [Partager un espace de travail](/help/quicksilver/maestro/access/share-workspaces.md).
* Votre entreprise peut contenir un maximum de 1 000 espaces de travail.
* Les espaces de travail contiennent des types d’enregistrement uniques à chaque espace de travail. <!--this might change-->

## Créer un espace de travail

{{step1-to-maestro}}

1. (Conditionnel) Si votre environnement ne contient aucun espace de travail, cliquez sur **Créer un espace de travail**

   Ou, dans un espace de travail existant, cliquez sur le pointeur vers le bas situé à droite du nom de l’espace de travail, puis cliquez sur **Créer un espace de travail**.

   ![](assets/workspace-drop-down-right-menu.png)

   Cela ouvre la zone Espaces de travail de Maestro.
1. (facultatif et conditionnel) Cliquez sur **Aperçu** dans l’un des modèles d’espace de travail prédéfinis suivants :

   * Gestion marketing
   * Gestion des ventes
   * Gestion des produits

   Il existe une indication des types d’enregistrements opérationnels, des taxonomies et du nombre de champs associés à chaque modèle.

   ![](assets/previewing-a-workspace-template.png)

   Pour plus d’informations sur les modèles d’espace de travail Maestro, voir [Liste des modèles d&#39;espace de travail](../architecture/workspace-templates.md).

1. Cliquez sur **Utiliser un modèle** pour commencer à créer l’espace de travail à partir du modèle sélectionné

   Ou

   Cliquez sur **Créer un espace de travail** pour créer entièrement un espace de travail.

   L’un des types d’espaces de travail suivants est créé :

   * Espace de travail vide dans lequel vous pouvez commencer à ajouter manuellement des types d’enregistrement.
   * Espace de travail rempli d’exemples de types d’enregistrement que vous pouvez personnaliser davantage.

1. Cliquez dans le nom de l’espace de travail dans l’en-tête du nouvel espace de travail pour le renommer, puis appuyez sur Entrée.

   Ou

   Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png)à droite du nom de l’espace de travail dans l’en-tête, puis cliquez sur **Renommer**.

1. (Facultatif) Cliquez sur **Ajouter un type d’enregistrement** pour ajouter des types d’enregistrement à l’espace de travail.

   Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

1. (Facultatif) Cliquez sur **Ajout d’une taxonomie** pour ajouter des taxonomies à l’espace de travail.

   Pour plus d’informations, voir [Création de taxonomies](../architecture/create-a-taxonomy.md).
