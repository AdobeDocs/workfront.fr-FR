---
title: Modifier les types d’enregistrements
description: Vous pouvez modifier les types d’enregistrement après leur enregistrement. Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: c0a7603ed461d903f4d0b0f6788c17d58f20c328
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 34%

---


# Modifier des types d’enregistrements

{{planning-important-intro}}

Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Vous pouvez modifier l’apparence des types d’enregistrement que vous ou toute autre personne avez créés. Pour plus d’informations sur la création de types d’enregistrement Workfront Planning, voir [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

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
   <td><p> Standard </p>
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
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
   <p>Seuls les administrateurs système peuvent activer les types d’enregistrements pour se connecter à partir d’autres espaces de travail</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD:

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
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## Modifier des types d’enregistrements

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les types d’enregistrements,

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte du type d’enregistrement, puis cliquez sur **Modifier**
Ou
   * Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Modifier**.

   ![Autres options de menu de la carte de type d’enregistrement](assets/more-menu-options-from-record-type-card.png)

1. Dans la zone **Modifier le type d’enregistrement**, l’onglet **Apparence** s’ouvre par défaut.

   ![Onglet Apparence de la zone Modifier le type d’enregistrement ](assets/edit-record-type-box-appearance-tab.png)

   Mettez à jour les informations suivantes dans l’onglet **Apparence** :

   * Modifiez le nom du type d’enregistrement, si nécessaire. <!--did they add a field label for this?-->
   * **Description** : modifiez ou ajoutez une description pour le type d’enregistrement avec plus d’informations à son sujet.
   * Modifiez la couleur et la forme de l’icône associée au type d’enregistrement. Procédez comme suit :
      * Sélectionnez une couleur pour identifier le type d’enregistrement. Il s’agit de la couleur de l’icône du type d’enregistrement.
      * Sélectionnez une icône dans la liste ou commencez à saisir le nom d’une icône pour décrire ce qu’elle représente, puis sélectionnez-la lorsqu’elle s’affiche. Il s’agit de l’icône du type d’enregistrement. Une icône de fichier est sélectionnée par défaut.

1. (Conditionnel) Si vous êtes un administrateur système, cliquez sur l’onglet **Paramètres avancés** dans la zone **Modifier le type d’enregistrement**. <!--the info here is duplicated in the Create record types article-->

   ![Onglet Paramètres avancés de la zone Modifier le type d’enregistrement](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Conditionnel) Mettez à jour les informations suivantes dans l’onglet **Paramètres avancés** :

   * Activez le paramètre **Se connecter à partir d’un autre espace de travail**. Lorsqu’il est activé, le type d’enregistrement est accessible et peut être connecté à partir d’autres espaces de travail.
   * Choisissez parmi les espaces de travail accessibles pour le type d’enregistrement. Choisissez l’une des options suivantes :

      * **À l’échelle du système** : les utilisateurs peuvent se connecter à ce type d’enregistrement à partir de tous les espaces de travail pour lesquels ils disposent des autorisations de gestion.
      * **Espaces de travail spécifiques** : ajoutez les noms des espaces de travail auxquels les responsables d’espace de travail peuvent se connecter à ce type d’enregistrement.

1. Cliquer sur **Enregistrer**.

   La carte de type d’enregistrement de l’espace de travail affiche une icône de connectivité ![Icône Se connecter à partir d’autres espaces de travail](assets/connect-from-other-workspaces-icon.png) dans le coin supérieur droit pour indiquer que l’enregistrement est désormais accessible à partir d’autres espaces de travail.

1. (Facultatif) Cliquez sur la carte de type d’enregistrement de la zone de l’espace de travail pour ouvrir la page du type d’enregistrement, puis renommez le type d’enregistrement dans l’en-tête.

1. (Facultatif) Pour modifier un autre type d’enregistrement, sur la page Type d’enregistrement , développez la flèche pointant vers le bas à droite du nom d’un type d’enregistrement, recherchez un type d’enregistrement, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   ![Liste déroulante Type d’enregistrement sur la page Type d’enregistrement avec la zone de recherche](assets/record-type-drop-down-on-record-type-page-with-search-box.png)