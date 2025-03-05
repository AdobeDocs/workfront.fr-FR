---
title: Création D’Objets Workfront À L’Aide Des Automatisations D’Enregistrements De Planification D’Adobe Workfront
description: Vous pouvez configurer des automatisations dans Adobe Workfront Planning qui, une fois activées, créent des objets dans Workfront ou des enregistrements dans Workfront Planning. Les objets et enregistrements créés sont automatiquement connectés aux enregistrements Planning existants. Cet article décrit comment gérer les automatisations, notamment comment les modifier, les désactiver, les supprimer et les déclencher pour créer des objets et des enregistrements.
hide: true
hidefromtoc: true
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '1802'
ht-degree: 8%

---

# Création d’objets à l’aide de l’automatisation des enregistrements Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Vous pouvez configurer des automatisations dans Adobe Workfront Planning qui, lorsqu&#39;elles sont activées, créent des objets dans Workfront ou des enregistrements dans Workfront Planning lorsqu&#39;ils sont déclenchés à partir d&#39;un enregistrement Planning. Les objets ou enregistrements créés sont automatiquement connectés aux enregistrements à partir desquels vous déclenchez l’automatisation.

Vous pouvez configurer et activer l’automatisation dans la page du type d’enregistrement dans Workfront Planning. L’objet connecté créé est placé dans le champ connecté du type d’enregistrement à partir duquel vous exécutez l’automatisation.

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
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
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
   <td> <p>Accordez des autorisations supérieures ou égales à l’espace de travail auquel vous souhaitez ajouter des enregistrements. </p>  
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

* Le nom de l&#39;objet ou de l&#39;enregistrement créé par une automatisation est identique au nom d&#39;enregistrement à partir duquel vous l&#39;avez créé.
* Les nouveaux objets ou enregistrements ne remplacent pas les objets ou enregistrements existants dans le même champ. Le déclenchement de la même automatisation plusieurs fois pour le même enregistrement ajoute les nouveaux objets ou enregistrements dans le même champ connecté de l&#39;enregistrement d&#39;origine, en plus de ceux créés précédemment.

<!--hide this for now; they are trying to remove this militation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

## Configuration d’une automatisation dans Workfront Planning

Vous devez configurer une automatisation pour un type d&#39;enregistrement dans Workfront Planning avant de pouvoir l&#39;utiliser pour créer des objets.

{{step1-to-planning}}

1. Cliquez sur une carte de type d’enregistrement, puis sur le nom d’un enregistrement.

   La page de type d’enregistrement s’ouvre.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Gérer les automatisations**.

   La liste des automatisations disponibles pour le type d’enregistrement sélectionné s’ouvre.

1. Cliquez sur **Nouvelle automatisation** dans le coin supérieur droit de l’écran. La boîte de dialogue **Nouvelle automatisation** s’ouvre.
1. Mettez à jour les champs suivants :

   * Remplacez **Automatisation sans titre** par le texte qui doit apparaître sur le bouton d’automatisation. Les utilisateurs cliqueront sur ce bouton lors de l&#39;utilisation de l&#39;automatisation pour créer un objet Workfront ou un enregistrement Planning.
   * **Description** : ajoutez une description pour identifier l’objectif de l’automatisation.
1. Cliquez sur **Enregistrer**.
La page d’informations sur l’automatisation s’ouvre.

1. Sur la page des détails de l&#39;automatisation, mettez à jour les champs suivants dans la section **Triggers** :

   * **Déclencheur** : sélectionnez l’action qui déclenchera l’automatisation. Par exemple, sélectionnez **Clic sur un bouton**. <!--update this step with a list of all possible triggers; right now only Button click is available-->

1. Mettez à jour les champs suivants dans la section **Actions** : <!--submitted bugs for these fields - see if they need changing here-->
   * **Actions** : sélectionnez l’action que Workfront doit effectuer lors du déclenchement de l’automatisation. Ce champ est obligatoire.
Sélectionnez l’une des actions suivantes :

      * Créer un groupe
      * Créer un programme
      * Créer un portfolio
      * Créer un projet
      * Créer un enregistrement

     >[!TIP]
     >
     >Après avoir enregistré l’automatisation, vous ne pouvez plus modifier l’action sélectionnée dans ce champ.

1. (Conditionnel) Selon l’action sélectionnée, mettez à jour les champs suivants :

   * **Créer un projet** :
      * **Champ connecté où l’objet est créé** : il s’agit du champ connecté où le nouveau projet s’affichera. Champ obligatoire.
      * **Modèle de projet** : sélectionnez un modèle de projet que Workfront utilisera pour créer le projet.
   * **Créer un portefeuille** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau portfolio. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau portefeuille** : sélectionnez un formulaire personnalisé à joindre au nouveau portefeuille. Vous devez créer un formulaire personnalisé de portfolio avant de pouvoir le sélectionner.
   * **Créer un programme** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau programme. Champ obligatoire.
      * **Portefeuille de programmes** : sélectionnez le portefeuille dans lequel le nouveau programme sera ajouté. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau programme** : sélectionnez un formulaire personnalisé à joindre au nouveau programme. Vous devez créer un formulaire personnalisé de programme avant de pouvoir le sélectionner.
   * **Créer un groupe** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau groupe. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau groupe** : sélectionnez un formulaire personnalisé à joindre au nouveau programme. Vous devez créer un formulaire personnalisé de programme avant de pouvoir le sélectionner.
   * **Créer un enregistrement** :
      * **Type d’enregistrement** : sélectionnez le type d’enregistrement à créer.

     La sous-section **Paramètres** s’affiche. Mettez à jour les champs suivants de la sous-section **Paramètres** :

      * **Champ sur le type d’enregistrement connecté où l’enregistrement actif s’affichera** : il s’agit du champ connecté sur le type d’enregistrement sélectionné pour l’action où l’enregistrement actif s’affichera.

     Par exemple, si vous créez une automatisation pour que les campagnes connectent les enregistrements de produit à partir de , il s’agit du champ connecté sur le type d’enregistrement de produit à partir duquel les campagnes s’afficheront, une fois les produits créés à l’aide de l’automatisation.

     Champ obligatoire.

     <!--submitted a change in functionality and UI text for this - revise??-->
      * **Mapper les champs**
         * **Transférer depuis** : sélectionnez les champs à partir du type d’enregistrement pour lequel l’automatisation est créée afin de les mapper aux champs du type d’enregistrement connecté.
         * **Transférer vers** : sélectionnez des champs du nouvel enregistrement qui seront renseignés avec les informations de l’enregistrement à partir duquel vous exécutez l’automatisation.

     >[!TIP]
     >
     >Les types de champ du type d’enregistrement d’origine doivent correspondre aux types de champ du type d’enregistrement nouvellement créé.

1. (Facultatif et conditionnel) Si vous avez choisi de créer un enregistrement, cliquez sur **Ajouter des champs** pour mapper des champs de recherche supplémentaires d’un enregistrement à un autre.
1. (Conditionnel) Si vous avez choisi de créer un enregistrement et qu&#39;il n&#39;existe pas de champs de connexion entre le type d&#39;enregistrement d&#39;origine et le type d&#39;enregistrement sélectionné dans la zone **Actions**, cliquez sur l&#39;icône de point d&#39;interrogation à droite du champ **Champ sur le type d&#39;enregistrement connecté où apparaîtra l&#39;enregistrement actif** puis cliquez sur l&#39;icône **Ajouter** ![icône Créer un champ de connexion](assets/create-a-connection-field-icon.png) pour ajouter un champ de connexion.

   Le nouveau champ est automatiquement créé pour le type d’enregistrement que vous avez sélectionné dans la zone **Actions** et nommé **Enregistrement connecté**.

   Un champ connecté pour le type d’enregistrement sélectionné est également créé sur le type d’enregistrement d’origine à partir duquel vous configurez l’automatisation.
1. (Facultatif et conditionnel) Si vous avez choisi de créer un objet Workfront et que vous ne disposez pas d’un champ de connexion pour le type d’objet Workfront sélectionné, cliquez sur l’icône de point d’interrogation à droite du champ **Connected field où le champ &lt; nom du type d’objet Workfront > est créé**, puis cliquez sur l’icône **Ajouter** ![icône Créer un champ de connexion](assets/create-a-connection-field-icon.png) pour ajouter un champ de connexion.

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   Le nouveau champ est automatiquement créé et nommé **Connected &lt; Workfront object name >**. Par exemple, lorsqu’un champ connecté à un portfolio est créé pour l’enregistrement, il est nommé « Portfolio connecté ».

1. Cliquez sur **Enregistrer** dans le coin supérieur droit de la page des détails d’automatisation.

   L’automatisation s’affiche dans la liste des automatisations et peut être utilisée dans les enregistrements.

## Gestion des automatisations existantes

{{step1-to-planning}}

1. Cliquez sur une carte de type d’enregistrement, puis sur le nom d’un enregistrement.

   La page de type d’enregistrement s’ouvre.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Gérer les automatisations**.

   La liste des automatisations disponibles pour le type d’enregistrement sélectionné s’ouvre.

1. (Facultatif) Pour modifier, désactiver ou supprimer une automatisation, effectuez l’une des opérations suivantes :

   1. Dans la liste des automatisations, pointez sur le nom d’une automatisation enregistrée, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png).

   1. Cliquez sur **Modifier** pour mettre à jour les informations sur les champs de l’automatisation et les configurer.

      >[!TIP]
      >
      >   Vous ne pouvez pas modifier l’action que vous avez initialement sélectionnée pour une automatisation.


   1. Cliquez sur **Désactiver** pour supprimer l’automatisation de la vue Tableau de l’enregistrement et empêcher les utilisateurs de l’utiliser pour créer des enregistrements ou des objets.

   Les enregistrements créés à l&#39;aide d&#39;une automatisation désactivée restent connectés à l&#39;enregistrement sélectionné à l&#39;origine.

   Pour le rendre à nouveau disponible, cliquez de nouveau sur le menu **Plus** ![Plus](assets/more-menu.png), puis cliquez sur **Activer**.
   1. Cliquez sur **Supprimer** pour supprimer l’automatisation. Impossible de récupérer une automatisation supprimée.

   Les enregistrements qui ont été créés à l&#39;aide d&#39;une automatisation supprimée restent connectés à l&#39;enregistrement sélectionné à l&#39;origine.

## Utiliser une automatisation de Workfront Planning pour créer un objet ou un enregistrement

1. Dans Workfront Planning, ouvrez la page Type d&#39;enregistrement qui contient l&#39;automatisation à utiliser pour créer et connecter automatiquement des enregistrements ou des objets.
1. Ouvrez la vue Tableau .
1. Sélectionnez un ou plusieurs enregistrements.

   Une barre bleue s’affiche au bas du tableau avec des boutons supplémentaires, y compris des boutons d’automatisation.
1. Cliquez sur le bouton d’automatisation près du coin inférieur droit de l’écran.

   ![Bouton Automatisation](assets/automation-custom-button.png)

   Les événements suivants se produisent :

   * Un message de confirmation s&#39;affiche en bas de l&#39;écran, si l&#39;automatisation a réussi à créer un objet ou un enregistrement.

   * Le nouvel objet s’affiche dans le champ connecté que vous avez indiqué dans la configuration du bouton d’automatisation. Vous devrez peut-être actualiser votre page avant d’afficher le nouvel objet.

   * L’enregistrement à partir duquel vous déclenchez l’automatisation est ajouté au champ connecté du nouvel enregistrement.

   >[!NOTE]
   >
   >Nous vous recommandons de vérifier que les objets ou enregistrements ont été créés et connectés comme prévu.

1. (Facultatif) Cliquez sur le nouvel objet dans le champ connecté. La page d’objet s’ouvre et vous pouvez apporter des modifications supplémentaires au nouvel objet.

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

