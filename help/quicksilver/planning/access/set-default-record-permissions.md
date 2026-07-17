---
title: Définir les autorisations par défaut pour les enregistrements
description: Vous pouvez définir des autorisations par défaut pour les enregistrements lorsque vous modifiez le type d’enregistrement ou les paramètres de l’espace de travail. Vous pouvez accorder des autorisations d’ouverture ou restreintes à tous les enregistrements qui seront ajoutés pour un type d’enregistrement.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 9ef64f5a39c94426b2158c6504b913c8cb749c8e
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 5%

---


# Définition des autorisations par défaut pour les enregistrements

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}


Vous pouvez définir des autorisations par défaut pour les enregistrements lorsque vous modifiez le type d’enregistrement ou les paramètres de l’espace de travail.

Vous pouvez accorder des autorisations d’ouverture ou restreintes à tous les enregistrements qui seront ajoutés pour un type d’enregistrement.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront ou workflow avec un package Planning</p> 
Ou
<p>Tout package de produit autonome Workfront Planning</p>

</tr>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Tous</p> 
   <p><b>NOTE</b></p>
   <p>Seules les personnes disposant d’une licence Standard peuvent se voir accorder des autorisations de gestion des enregistrements. Toutes les autres licences ne peuvent avoir que des autorisations d’affichage et l’option Gérer est grisée pour celles-ci.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  <p>Gestion des autorisations relatives à un espace de travail et à un type d’enregistrement</p>  
   <p><b>IMPORTANT</b></p>
   <p>Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager un enregistrement</p></td> 
  </tr>
</tbody> 
</table>

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à la définition des autorisations d’enregistrement par défaut

Tenez compte des points suivants lors de la configuration des autorisations d’enregistrement par défaut :

* Une seule règle d’autorisation par défaut peut être active par type d’enregistrement à la fois.
* La modification de la règle affecte uniquement les enregistrements créés après la modification. Les enregistrements existants conservent leurs autorisations actuelles.
* Les administrateurs système et les responsables d’espace de travail conservent toujours un accès de niveau Gérer à chaque enregistrement, quelle que soit la règle.
* Une fois un enregistrement créé, ses autorisations peuvent être modifiées indépendamment dans sa boîte de dialogue de partage sans affecter la règle par défaut.
* Pour les types d’enregistrements globaux, chaque espace de travail (principal et secondaire) peut configurer sa propre règle par défaut, et les nouveaux enregistrements adoptent la règle de l’espace de travail dans lequel ils sont créés.

## Configuration des autorisations d’enregistrement par défaut pour un espace de travail

1. Accédez à un espace de travail > menu **Plus** ![menu Plus](assets/more-menu.png) > **Paramètres** > **Types d’enregistrement**.

   ![Zone des paramètres des types d&#39;enregistrements &#x200B;](assets/workspace-record-types-settings-area.png)

1. (Facultatif) Cliquez dans la cellule d’un **Type d’enregistrement** pour modifier les noms des types d’enregistrement.

1. Dans la colonne **Valeur par défaut de la nouvelle autorisation d&#39;enregistrement**, cliquez sur la cellule du type d&#39;enregistrement dont vous souhaitez mettre à jour les autorisations.

1. Choisissez l’une des options suivantes :

   * **Ouvert** : tous les contributeurs et contributrices d’espace de travail peuvent gérer l’enregistrement nouvellement créé. Il s’agit du comportement par défaut actuel pour tous les types d’enregistrements existants et nouveaux.
   * **Restreint** : seul le créateur de l’enregistrement et toute personne que vous ajoutez explicitement peuvent modifier les enregistrements nouvellement créés. Tous les autres utilisateurs bénéficient d’un accès en lecture seule.

1. (Conditionnel) Si vous modifiez les autorisations par défaut de **Restreint** en **Ouvrir**, cliquez sur **Basculer** dans la zone **Basculer vers l’ouverture** pour confirmer votre choix.
1. (Conditionnel) Si vous avez sélectionné **Restreint**, ajoutez des éditeurs supplémentaires dans la colonne **Qui peut modifier les enregistrements**. Vous pouvez ajouter des utilisateurs, des groupes, des équipes, des rôles ou des sociétés.

   >[!NOTE]
   >
   >* Le créateur d’enregistrement est toujours inclus et ne peut pas être supprimé.
   >* Vous pouvez uniquement sélectionner des entités qui disposent déjà d’autorisations de niveau Contribuer ou Gérer pour le type d’enregistrement.

   Les modifications sont enregistrées automatiquement. Une fois enregistrée, la règle prend effet immédiatement et s’applique automatiquement à tous les enregistrements créés pour ce type d’enregistrement.

## Configuration des autorisations d’enregistrement par défaut pour un type d’enregistrement

1. Accédez à un type d’enregistrement > menu **Plus** ![menu Plus](assets/more-menu.png) > **Paramètres** > **Paramètres d’enregistrement**.

   ![Onglet Paramètres d’enregistrement dans la zone Paramètres de type d’enregistrement](assets/record-settings-tab-in-record-type-settings-area.png)

1. Dans le champ **Type d&#39;autorisation des enregistrements**, cliquez sur l&#39;une des options suivantes :

   * **Ouvert** : tous les contributeurs et contributrices d’espace de travail peuvent gérer l’enregistrement nouvellement créé. Il s’agit du comportement par défaut actuel pour tous les types d’enregistrements existants et nouveaux.
   * **Restreint** : seul le créateur de l’enregistrement et toute personne que vous ajoutez explicitement peuvent modifier les enregistrements nouvellement créés. Tous les autres utilisateurs bénéficient d’un accès en lecture seule.
1. (Conditionnel) Si vous modifiez les autorisations par défaut de **Restreint** en **Ouvrir**, cliquez sur **Basculer** dans la zone **Basculer vers l’ouverture** pour confirmer votre choix.
1. (Conditionnel) Si vous avez sélectionné **Restreint**, ajoutez des éditeurs supplémentaires dans le champ **Qui peut modifier les enregistrements**. Vous pouvez ajouter des utilisateurs, des groupes, des équipes, des rôles ou des sociétés.

   >[!NOTE]
   >
   >* Le créateur d’enregistrement est toujours inclus et ne peut pas être supprimé.
   >* Vous pouvez uniquement sélectionner des entités qui disposent déjà d’autorisations de niveau Contribuer ou Gérer pour le type d’enregistrement.

   Les modifications sont enregistrées automatiquement. Une fois enregistrée, la règle prend effet immédiatement et s’applique automatiquement à tous les enregistrements créés pour ce type d’enregistrement.