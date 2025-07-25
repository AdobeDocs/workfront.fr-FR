---
title: Configuration des fonctionnalités de plusieurs espaces de travail pour le type d’enregistrement
description: Vous pouvez activer l’ajout d’un type d’enregistrement à un autre espace de travail ou la connexion à partir d’un autre espace de travail.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 943c26efa6f6351abf885dbc5f3aa09c0b0fab05
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 11%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# Configurer les fonctionnalités de l’espace de travail croisé pour les types d’enregistrements

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Vous pouvez désigner un type d’enregistrement à ajouter à un autre espace de travail ou à connecter à partir d’un autre espace de travail, dans Adobe Workfront Planning.

Vous devez d&#39;abord définir les fonctionnalités inter-espaces de travail d&#39;un type d&#39;enregistrement avant que les responsables d&#39;espace de travail puissent le connecter ou l&#39;importer dans d&#39;autres espaces de travail.

Vous définissez les fonctionnalités inter-espaces de travail d’un type d’enregistrement lorsque vous créez ou modifiez un type d’enregistrement.

Pour plus d’informations, consultez l’un des articles suivants :

* [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md)
* [Modifier des types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
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
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuration de l’ajout d’un type d’enregistrement à d’autres espaces de travail

En tant que gestionnaire d’espace de travail, vous pouvez configurer un type d’enregistrement à ajouter à d’autres espaces de travail lorsque vous créez ou modifiez un type d’enregistrement.

Lorsque vous configurez l’ajout d’un type d’enregistrement à d’autres espaces de travail, un gestionnaire d’espace de travail peut importer le type d’enregistrement et toutes ses informations dans l’un des espaces de travail qu’il gère.

Pour configurer l’ajout d’un type d’enregistrement à un autre espace de travail lorsque vous modifiez le type d’enregistrement :

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les types d’enregistrements.

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte du type d’enregistrement
Ou
   * Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement.
1. Cliquez sur **Modifier**.

   ![Autres options de menu de la carte de type d’enregistrement](assets/more-menu-options-from-record-type-card.png)

1. Dans la zone **Modifier le type d’enregistrement**, sélectionnez l’onglet **Paramètres avancés**.
1. Activez le paramètre **Autoriser l’ajout de ce type d’enregistrement à d’autres espaces de travail**.

   ![Modifier les paramètres avancés du type d’enregistrement avec Ajouter aux autres espaces de travail active](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. Dans le champ **Sélectionner les personnes autorisées à ajouter ce type d’enregistrement aux espaces de travail qu’elles gèrent**, ajoutez les utilisateurs autorisés à ajouter ce type d’enregistrement aux espaces de travail qu’elles gèrent.

   Votre nom est automatiquement ajouté au champ.

   Vous pouvez ajouter des utilisateurs individuels, ou des groupes, des équipes, des fonctions ou des sociétés dont vous souhaitez autoriser les utilisateurs à ajouter ce type d’enregistrement aux espaces de travail qu’ils gèrent.

   Vous pouvez modifier ce champ après avoir enregistré le type d’enregistrement.
1. (Facultatif) Supprimez votre nom du champ **Sélectionner qui peut ajouter ce type d’enregistrement aux espaces de travail qu’il gère**.

1. Cliquer sur **Enregistrer**.

   Les événements suivants se produisent :

   * Le type d’enregistrement et ses champs peuvent désormais être ajoutés à un autre espace de travail par les personnes que vous avez désignées.

   >[!NOTE]
   >
   >Vous ne pouvez modifier le type d’enregistrement et ses champs qu’à partir de l’espace de travail d’origine.

   * La carte de type d’enregistrement affiche une icône globale ![icône de type d’enregistrement global](assets/global-icon.png) pour indiquer que le type d’enregistrement peut être ajouté à n’importe quel espace de travail dont vous avez désigné le responsable dans votre configuration.
   * Un champ **Workspace** généré par le système est ajouté au type d’enregistrement.

     Le champ Workspace affiche l’espace de travail à partir duquel chaque enregistrement a été créé.

     Ce champ est en lecture seule et ne peut pas être supprimé.

## Configuration de la connexion à un type d&#39;enregistrement à partir d&#39;autres espaces de travail

Vous pouvez configurer un type d’enregistrement auquel se connecter à partir d’autres espaces de travail lorsque vous créez ou modifiez le type d’enregistrement.

Pour configurer un type d’enregistrement auquel se connecter à partir d’autres espaces de travail lorsque vous modifiez le type d’enregistrement :

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les types d’enregistrements,

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte du type d’enregistrement, puis cliquez sur **Modifier**
Ou
   * Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Modifier**.

   ![Autres options de menu de la carte de type d’enregistrement](assets/more-menu-options-from-record-type-card.png)

1. Dans la zone **Modifier le type d’enregistrement**, sélectionnez l’onglet **Paramètres avancés**.
1. Activez le paramètre **Autoriser la connexion à ce type d’enregistrement dans d’autres espaces de travail**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Modifier l’onglet Paramètres avancés de type d’enregistrement avec la connexion depuis d’autres espaces de travail activée](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Lorsqu’il est activé, le type d’enregistrement est accessible et peut être connecté à partir d’autres espaces de travail.

1. Choisissez parmi les espaces de travail accessibles pour le type d’enregistrement. Choisissez l’une des options suivantes :

   * **À l’échelle du système** : les utilisateurs peuvent se connecter à ce type d’enregistrement à partir de tous les espaces de travail pour lesquels ils disposent des autorisations de gestion.
   * **Espaces de travail spécifiques** : ajoutez les noms des espaces de travail auxquels les responsables d’espace de travail peuvent se connecter à ce type d’enregistrement.
1. Cliquez sur **Modifier**.

   Les événements suivants se produisent :

   * Le type d’enregistrement et ses champs sont désormais disponibles pour se connecter à partir des espaces de travail que vous avez désignés.
   * La carte de type d’enregistrement affiche une icône de connexion entre espaces de travail ![icône de connexion entre espaces de travail](assets/connect-from-other-workspaces-icon.png) pour indiquer que le type d’enregistrement peut être connecté à partir de n’importe quel espace de travail que vous avez désigné dans votre configuration.

   Le type d’enregistrement peut être connecté à partir des espaces de travail désignés.









