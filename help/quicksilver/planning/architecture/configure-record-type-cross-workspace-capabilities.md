---
title: Configuration des fonctionnalités de plusieurs espaces de travail pour le type d’enregistrement
description: Vous pouvez activer l’ajout d’un type d’enregistrement à un autre espace de travail ou la connexion à partir d’un autre espace de travail.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 7%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Configurer les fonctionnalités de l’espace de travail croisé pour les types d’enregistrements

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Vous pouvez configurer des types d’enregistrements pour qu’ils fonctionnent sur plusieurs espaces de travail.

Vous trouverez ci-dessous des fonctionnalités inter-espaces de travail de types d’enregistrements :

* Vous pouvez désigner un type d’enregistrement comme centralisé. Les utilisateurs peuvent ajouter des types d’enregistrements centralisés à d’autres espaces de travail qu’ils peuvent gérer.
* Vous pouvez désigner un type d’enregistrement comme pouvant être connecté. Les utilisateurs peuvent se connecter à ce type d’enregistrement à partir d’autres espaces de travail.

Vous devez d’abord définir les fonctionnalités inter-espaces de travail d’un type d’enregistrement avant que les responsables d’espace de travail puissent le connecter à partir de ou l’ajouter à d’autres espaces de travail.

Vous définissez les fonctionnalités inter-espaces de travail d’un type d’enregistrement lorsque vous créez ou modifiez un type d’enregistrement.

Pour plus d’informations, consultez l’un des articles suivants :

* [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md)
* [Modifier des types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md)

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
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Tout package Workfront</p></li>
<p>Et</p>
<li><p>Tout package Planning permettant de créer des types d'enregistrements connectables</p></li>
<li><p>Package Planning Plus pour créer des types d'enregistrements centralisés</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre gestionnaire de compte Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Configuration des types d’enregistrements centralisés

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

En tant que gestionnaire d’espace de travail, vous pouvez configurer un type d’enregistrement comme étant un type d’enregistrement centralisé. Un type d’enregistrement centralisé peut être ajouté à d’autres espaces de travail.

Un gestionnaire d’espace de travail peut ajouter un type d’enregistrement centralisé à un espace de travail qu’il gère. Les champs d’origine du type d’enregistrement sont également ajoutés.

Les utilisateurs peuvent ajouter des enregistrements à un type d&#39;enregistrement centralisé à partir de n&#39;importe quel espace de travail disposant d&#39;autorisations Contribute et où le type d&#39;enregistrement centralisé est ajouté, y compris son espace de travail d&#39;origine. Ils peuvent afficher les enregistrements de l’espace de travail pour lequel ils disposent uniquement des autorisations d’affichage.

Pour plus d’informations, voir [Présentation des types d’enregistrements de l’espace de travail](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

Pour configurer un type d’enregistrement comme centralisé :

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez configurer les types d’enregistrements comme centralisés.

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte du type d’enregistrement
   * Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement.
1. Cliquez sur **Modifier**.

   ![Autres options de menu de la carte de type d’enregistrement](assets/more-menu-options-from-record-type-card.png)

   >[!TIP]
   >
   >Si un type d’enregistrement a déjà été désigné comme type d’enregistrement centralisé et qu’il a été ajouté à d’autres espaces de travail, l’option Modifier est grisée.

1. Dans la zone **Modifier le type d’enregistrement**, cliquez sur l’onglet **Paramètres avancés**.
1. Activez le paramètre **Autoriser l’ajout de ce type d’enregistrement à d’autres espaces de travail**.

   ![Modifier les paramètres avancés du type d’enregistrement avec Ajouter aux autres espaces de travail active](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Après avoir ajouté un type d’enregistrement centralisé à un autre espace de travail, ce paramètre ne peut plus être désactivé.

1. Dans le champ **Sélectionner les personnes autorisées à ajouter ce type d’enregistrement aux espaces de travail qu’elles gèrent**, ajoutez les entités que vous souhaitez autoriser à ajouter ce type d’enregistrement aux espaces de travail qu’elles gèrent.

   Votre nom est automatiquement ajouté au champ.

   Vous pouvez ajouter des utilisateurs individuels, ou des groupes, des équipes, des fonctions ou des sociétés dont vous souhaitez autoriser les utilisateurs à ajouter ce type d’enregistrement aux espaces de travail qu’ils gèrent.

   Vous devez désigner au moins une entité (utilisateur, équipe, groupe, rôle ou entreprise) pour pouvoir activer ce paramètre.

   Vous pouvez modifier ce champ après avoir enregistré le type d’enregistrement.

1. (Facultatif) Supprimez votre nom du champ **Sélectionner qui peut ajouter ce type d’enregistrement aux espaces de travail qu’il gère**.

1. Cliquer sur **Enregistrer**.

   Les événements suivants se produisent :

   * Le type d’enregistrement et ses champs peuvent désormais être ajoutés à un autre espace de travail par les personnes que vous avez désignées.

   >[!NOTE]
   >
   >Vous ne pouvez modifier l’aspect et les paramètres du type d’enregistrement, ainsi que ses champs d’origine, qu’à partir de son espace de travail d’origine.

   * La carte Type d’enregistrement affiche une icône centralisée ![icône de type d’enregistrement centralisé](assets/global-icon.png) pour indiquer que le type d’enregistrement peut être ajouté à d’autres espaces de travail.
   * Un champ **Workspace** généré par le système est ajouté à la vue Tableau du type d&#39;enregistrement et des détails de ses enregistrements.

     Le champ Workspace affiche l’espace de travail à partir duquel chaque enregistrement est créé.

     Ce champ est en lecture seule et ne peut pas être supprimé.
1. (Facultatif) Accédez à un autre espace de travail et créez un type d’enregistrement à l’aide d’un type d’enregistrement existant. Sélectionnez le type d’enregistrement que vous avez activé dans les étapes ci-dessus.

   Pour plus d’informations, voir [Ajouter des types d’enregistrements existants depuis un autre espace de travail](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Configuration des types d’enregistrements connectables

<!--this is a UI term; don't change the title of this section-->

Vous pouvez configurer un type d’enregistrement auquel se connecter à partir d’autres espaces de travail lorsque vous créez ou modifiez le type d’enregistrement.

Pour configurer un type d’enregistrement auquel se connecter à partir d’autres espaces de travail lorsque vous modifiez le type d’enregistrement :

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les types d’enregistrements.

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte du type d’enregistrement, puis cliquez sur **Modifier**
   * Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Modifier**.

   ![Autres options de menu de la carte de type d’enregistrement](assets/more-menu-options-from-record-type-card.png)

1. Dans la zone **Modifier le type d’enregistrement**, cliquez sur l’onglet **Paramètres avancés**.
1. Activez le paramètre **Autoriser la connexion à ce type d’enregistrement dans d’autres espaces de travail**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Modifier l’onglet Paramètres avancés de type d’enregistrement avec la connexion depuis d’autres espaces de travail activée](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Lorsqu’il est activé, le type d’enregistrement est accessible et peut être connecté à à partir d’autres espaces de travail.

1. Choisissez parmi les espaces de travail accessibles pour le type d’enregistrement. Choisissez l’une des options suivantes :

   * **À l’échelle du système** : les utilisateurs peuvent se connecter à ce type d’enregistrement à partir de tous les espaces de travail pour lesquels ils disposent des autorisations Gérer.
   * **Espaces de travail spécifiques** : ajoutez les noms des espaces de travail auxquels les responsables d’espace de travail peuvent se connecter à ce type d’enregistrement.
1. Cliquer sur **Enregistrer**.

   Les événements suivants se produisent :

   * Le type d’enregistrement et ses champs sont désormais disponibles pour la connexion à partir des espaces de travail que vous avez désignés.
   * La carte de type d’enregistrement affiche une icône de connexion entre espaces de travail ![icône de connexion entre espaces de travail](assets/connect-from-other-workspaces-icon.png) pour indiquer que le type d’enregistrement peut être connecté à partir de n’importe quel espace de travail que vous avez désigné dans votre configuration.

   Le type d’enregistrement peut être connecté à partir des espaces de travail désignés.
1. (Facultatif) Accédez à un autre espace de travail et ajoutez une connexion au type d’enregistrement que vous avez activé pour la connectabilité entre les espaces de travail dans les étapes ci-dessus.

   Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).









