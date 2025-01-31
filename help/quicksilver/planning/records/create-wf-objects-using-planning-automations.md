---
title: Création D’Objets Workfront À L’Aide Des Automatisations D’Enregistrements De Planification D’Adobe Workfront
description: Vous pouvez configurer des automatisations dans Adobe Workfront Planning qui, une fois activées, créent des objets dans Workfront ou des enregistrements dans Workfront Planning. Les objets et enregistrements créés sont automatiquement connectés aux enregistrements Planning existants.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 9%

---

# Création d’objets à l’aide de l’automatisation des enregistrements Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Vous pouvez configurer des automatisations dans Adobe Workfront Planning qui, une fois activées, créent des objets dans Workfront ou enregistrent Workfront Planning. Les objets ou enregistrements créés sont automatiquement liés aux enregistrements à partir desquels vous déclenchez l’automatisation.

Vous pouvez configurer et activer l’automatisation dans la page de l’enregistrement dans Workfront Planning. L’objet connecté créé est placé dans le champ connecté du type d’enregistrement à partir duquel vous exécutez l’automatisation.

Par exemple, vous pouvez créer une automatisation qui prend une campagne Workfront Planning et crée un projet dans Workfront pour suivre la progression de cette campagne. Le projet serait connecté à la campagne de planification Workfront dans le champ Projet connecté de la campagne.

Pour plus d’informations sur les enregistrements connectés, voir [Présentation des enregistrements connectés](/help/quicksilver/planning/records/connected-records-overview.md).

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
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td> Standard
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p> 
   <p>Modifiez l’accès dans Workfront pour les types d’objets que vous souhaitez créer (projets, portfolios, programmes). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Gérez les autorisations de l’espace de travail auquel vous souhaitez ajouter des enregistrements. </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
   <p>Gérez les autorisations sur les objets Workfront (portfolios) pour ajouter des objets enfants (projets).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Un modèle de mise en page comprenant la zone Planning du menu principal doit être affecté à tous les utilisateurs, y compris les administrateurs Workfront </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considérations relatives à la création d&#39;objets et d&#39;enregistrements à l&#39;aide d&#39;une automatisation

* Le nouvel objet ou nom d’enregistrement est identique au nom d’enregistrement à partir duquel vous l’avez créé. <!--take this out when they add the field mapping - no longer just the name of the original record-->
* Les nouveaux objets ne remplacent pas les objets existants dans le même champ.
* L’automatisation crée des objets supplémentaires uniquement dans les champs de type de connexion Plusieurs à plusieurs ou Un à plusieurs.

## Configuration d’une automatisation dans Workfront Planning

Vous devez configurer une automatisation pour un type d&#39;enregistrement dans Workfront Planning, avant de pouvoir l&#39;utiliser pour créer des objets.

{{step1-to-planning}}

1. Cliquez sur une carte de type d’enregistrement, puis sur le nom d’un enregistrement.

   La page de type d’enregistrement s’ouvre.
1. Cliquez sur le ![](assets/more-menu.png) de menu **Plus** à droite du nom du type d’enregistrement, puis cliquez sur **Gérer les automatisations**.

   La liste des automatisations disponibles s’ouvre.

1. Cliquez sur **Nouvelle automatisation** dans le coin supérieur droit de l’écran. La boîte de dialogue **Nouvelle automatisation** s’ouvre.
1. Mettez à jour les champs suivants :

   * Remplacez **Automatisation sans titre** par le texte qui doit apparaître sur le bouton d’automatisation. Les utilisateurs cliqueront sur ce bouton lors de l&#39;utilisation de l&#39;automatisation pour créer un objet Workfront ou un enregistrement Planning.
   * **Description** : ajoutez une description pour identifier l’objectif de l’automatisation.
1. Cliquez sur **Enregistrer**.
La page d’informations sur l’automatisation s’ouvre.

1. Sur la page des détails de l&#39;automatisation, mettez à jour les champs suivants dans la section **Triggers** :

   * **Déclencheur** : sélectionnez l’action qui déclenchera l’automatisation. Par exemple, sélectionnez **Clic sur un bouton**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Mettez à jour les champs suivants dans la section **Actions** : <!--submitted bugs for these fields - see if they need changing here-->
   * **Type d’objet** : sélectionnez l’objet que l’automatisation doit créer. Champ obligatoire.

     Vous pouvez créer les objets suivants à partir des enregistrements Workfront Planning :

      * Projet
      * Portfolio
      * Programme
      * Groupe
      * Enregistrement
1. (Conditionnel) Selon le type d’objet que vous souhaitez créer, mettez à jour les champs suivants :

   * **Projet** :
      * **Champ connecté où l’objet est créé** : il s’agit du champ connecté où le nouveau projet s’affichera. Champ obligatoire
      * **Modèle à partir duquel créer le projet** : sélectionnez un modèle de projet que Workfront utilisera pour créer le projet.
   * **Portfolio** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau portfolio. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau portefeuille** : sélectionnez un formulaire personnalisé à joindre au nouveau portefeuille. Vous devez créer un formulaire personnalisé de portfolio avant de pouvoir le sélectionner.
   * **Programme** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau programme. Champ obligatoire.
      * **Portefeuille de programmes** : sélectionnez le portefeuille dans lequel le nouveau programme sera ajouté. Champ obligatoire.
      * 
         * **Formulaire personnalisé à joindre au nouveau programme** : sélectionnez un formulaire personnalisé à joindre au nouveau programme. Vous devez créer un formulaire personnalisé de programme avant de pouvoir le sélectionner.
   * **Groupe** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau groupe. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau groupe** : sélectionnez un formulaire personnalisé à joindre au nouveau programme. Vous devez créer un formulaire personnalisé de programme avant de pouvoir le sélectionner.
   * **Enregistrement** :
      * **Type d’enregistrement connecté** : sélectionnez le type d’enregistrement à créer.
      * **Champ connecté où l&#39;enregistrement est créé** : il s&#39;agit du champ connecté où le nouvel enregistrement s&#39;affichera. Ce champ est obligatoire. <!--this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label-->
      * **Mapper les champs**
         * **Transférer depuis** : sélectionnez les champs à partir du type d’enregistrement pour lequel l’automatisation est créée afin de les mapper aux champs du type d’enregistrement connecté.
      * **Transférer vers** : sélectionnez des champs du nouvel enregistrement qui seront renseignés avec les informations de l’enregistrement à partir duquel vous exécutez l’automatisation.
1. (Facultatif et conditionnel) Si vous avez choisi de créer un enregistrement, cliquez sur **Ajouter des champs** pour mapper des champs de recherche supplémentaires d’un enregistrement à un autre.
1. (Facultatif et conditionnel) Si vous ne disposez pas d’un champ de connexion pour un type d’objet Workfront, cliquez sur l’icône **Créer un champ de connexion** ![](assets/create-a-connection-field-icon.png) pour ajouter un champ.
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de la page des détails d’automatisation.

   L’automatisation s’affiche dans la liste des automatisations et peut être utilisée dans les enregistrements.
1. (Facultatif) Pour modifier, désactiver ou supprimer une automatisation, procédez comme suit :

   1. Dans la liste des automatisations, passez la souris sur le nom d’une automatisation enregistrée, puis cliquez sur l’![](assets/more-menu.png) de menu **Plus**.

   1. Cliquez sur **Modifier** pour mettre à jour les informations sur les champs de l’automatisation et les configurer.
   1. Cliquez sur **Désactiver** pour supprimer l’automatisation de la vue Tableau et empêcher les utilisateurs de l’utiliser pour créer des enregistrements ou des objets. Pour le rendre à nouveau disponible, cliquez de nouveau sur le menu **Plus**, ![](assets/more-menu.png) cliquez sur **Activer**.
   1. Cliquez sur **Supprimer** pour supprimer l’automatisation. Impossible de récupérer une automatisation supprimée. Les enregistrements créés à l&#39;aide de l&#39;automatisation restent connectés à l&#39;enregistrement sélectionné à l&#39;origine.

## Utiliser une automatisation de Workfront Planning pour créer un objet ou un enregistrement

1. Dans Workfront Planning, ouvrez la page Type d&#39;enregistrement qui contient les enregistrements à utiliser pour créer des objets Workfront ou des enregistrements Planning.
1. Ouvrez la vue Tableau .
1. Sélectionnez un ou plusieurs enregistrements.

   Une barre bleue s’affiche au bas du tableau avec des boutons supplémentaires, y compris des boutons d’automatisation.
1. Cliquez sur le bouton d’automatisation près du coin inférieur droit de l’écran.

   ![Bouton Automatisation](assets/automation-custom-button.png)

   Un message de confirmation s&#39;affiche en bas de l&#39;écran, si l&#39;automatisation a réussi à créer un objet ou un enregistrement.

   Le nouvel objet s’affiche dans le champ connecté que vous avez indiqué dans la configuration du bouton d’automatisation. Vous devrez peut-être actualiser votre page avant d’afficher le nouvel objet.

   >[!NOTE]
   >
   >Nous vous recommandons de vérifier que l’objet a été créé et connecté comme prévu.

1. (Facultatif) Cliquez sur le nouvel objet dans le champ connecté. La page d’objet s’ouvre et vous pouvez apporter des modifications supplémentaires au nouvel objet.

<!--you might need to add something about notifications and emails?!-->
