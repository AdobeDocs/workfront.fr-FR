---
title: Création D’Objets Workfront À L’Aide Des Automatisations D’Enregistrements De Planification D’Adobe Workfront
description: Vous pouvez configurer des automatisations dans Adobe Workfront Planning qui, une fois activées, créent des objets dans Workfront ou des enregistrements dans Workfront Planning. Les objets et enregistrements créés sont automatiquement connectés aux enregistrements Planning existants. Cet article décrit comment gérer les automatisations, notamment comment les modifier, les désactiver, les supprimer et les déclencher pour créer des objets et des enregistrements.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 0a7bb953e7e02e24857bfb7ff671538e184bda17
workflow-type: tm+mt
source-wordcount: '1479'
ht-degree: 8%

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

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Vous pouvez configurer des automatisations dans Adobe Workfront Planning qui, lorsqu&#39;elles sont activées, créent des objets dans Workfront ou des enregistrements dans Workfront Planning lorsqu&#39;ils sont déclenchés à partir d&#39;un enregistrement Planning. Les objets ou enregistrements créés sont automatiquement connectés aux enregistrements à partir desquels vous déclenchez l’automatisation.

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

* Pour les nouveaux objets Workfront, le nom du nouvel objet est identique au nom d’enregistrement à partir duquel vous l’avez créé.
* Pour les nouveaux enregistrements Planning, vous pouvez indiquer quel champ d&#39;enregistrement d&#39;origine doit être utilisé pour déterminer le nom du nouvel enregistrement.
* Les nouveaux objets ou enregistrements ne remplacent pas les objets ou enregistrements existants dans le même champ. Le déclenchement de la même automatisation plusieurs fois pour les mêmes enregistrements ajoute les nouveaux objets ou enregistrements dans le même champ connecté de l&#39;enregistrement d&#39;origine, en plus de ceux créés précédemment.
* L’automatisation ajoute des objets supplémentaires uniquement dans les champs de type de connexion Plusieurs à plusieurs ou Un à plusieurs. Dans tous les autres cas, l’automatisation crée l’objet, mais ne le connecte pas à l’enregistrement d’origine à partir duquel l’automatisation est déclenchée.

## Configuration d’une automatisation dans Workfront Planning

Vous devez configurer une automatisation pour un type d&#39;enregistrement dans Workfront Planning, avant de pouvoir l&#39;utiliser pour créer des objets.

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

   * **Déclencheur** : sélectionnez l’action qui déclenchera l’automatisation. Par exemple, sélectionnez **Clic sur un bouton**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Mettez à jour les champs suivants dans la section **Actions** : <!--submitted bugs for these fields - see if they need changing here-->
   * **Type d’objet** : sélectionnez l’objet que l’automatisation doit créer. Champ obligatoire.

     Vous pouvez créer les objets suivants à partir des enregistrements Workfront Planning :

      * Projet
      * Portfolio
      * Programme
      * Groupe
      * Enregistrement

     >[!TIP]
     >
     >Après avoir enregistré l’automatisation, vous ne pouvez plus modifier le type d’objet dans ce champ.

1. (Conditionnel) Selon le type d’objet que vous souhaitez créer, mettez à jour les champs suivants :


   * **Projet** :
      * **Champ connecté où l’objet est créé** : il s’agit du champ connecté où le nouveau projet s’affichera. Champ obligatoire.
      * **Modèle à partir duquel créer le projet** : sélectionnez un modèle de projet que Workfront utilisera pour créer le projet.
   * **Portfolio**:
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau portfolio. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau portefeuille** : sélectionnez un formulaire personnalisé à joindre au nouveau portefeuille. Vous devez créer un formulaire personnalisé de portfolio avant de pouvoir le sélectionner.
   * **Programme** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où s&#39;affichera le nouveau programme. Champ obligatoire.
      * **Portefeuille de programmes** : sélectionnez le portefeuille dans lequel le nouveau programme sera ajouté. Champ obligatoire.
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
1. (Facultatif et conditionnel) Si vous ne disposez pas d’un champ de connexion pour un type d’objet Workfront, cliquez sur l’icône **Créer un champ de connexion** ![Créer une icône de champ de connexion](assets/create-a-connection-field-icon.png) pour ajouter un champ.

   Le nouveau champ est automatiquement créé et nommé **Connected &lt; Workfront object name >**. Par exemple, lorsqu’un champ connecté à un portfolio est créé pour l’enregistrement, il est nommé « Portfolio connecté ».

1. Cliquez sur **Enregistrer** dans le coin supérieur droit de la page des détails d’automatisation.

   L’automatisation s’affiche dans la liste des automatisations et peut être utilisée dans les enregistrements.
1. (Facultatif) Pour modifier, désactiver ou supprimer une automatisation, procédez comme suit :

   1. Dans la liste des automatisations, pointez sur le nom d’une automatisation enregistrée, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png).

   1. Cliquez sur **Modifier** pour mettre à jour les informations sur les champs de l’automatisation et les configurer.
   1. Cliquez sur **Désactiver** pour supprimer l’automatisation de la vue Tableau et empêcher les utilisateurs de l’utiliser pour créer des enregistrements ou des objets. Pour le rendre à nouveau disponible, cliquez de nouveau sur le menu **Plus** ![Plus](assets/more-menu.png), puis cliquez sur **Activer**.
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


<!--****************************************FUTURE ARTICLE AFTER THE RELEASE TO PREVIEW ON FEBRUARY 20:*****************************************************  

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

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

* For new Workfront objects, the new object name is the same as the record name from which you create it. 
* For new Planning records, you can indicate what original record field should be used to determine the new record's name. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same record adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning before you can use it to create objects.

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

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. *************update this step with a list of all possible triggers; right now only Button click is available*********

1. Update the following fields in the **Actions** section: **********submitted bugs for these fields - see if they need changing here***********
   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Select one of the following actions: 

      * Create group
      * Create program
      * Create portfolio
      * Create project
      * Create record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the action selected in this field.

1. (Conditional) Depending on what action you selected, update the following fields:

   * **Create project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Project template**: Select a project template that Workfront will use to create the project.  
   * **Create portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Create program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create record**: 
      * **Record type**: Select the record type you want to create. 

      The **Settings** sub-section displays. Update the following fields in the **Settings** sub-section: 

      * **Field on the connected record type where the current record will show**: This is the connected field on the record type selected for the action where the current record will display. 
      
      For example, if you are creating an automation for campaigns to connect Product records from, this is the connected field on the Product record type where the campaigns will display, after the products are created using the automation. 
      
      This is a required field. 
      
      ******submitted a change in functionality and UI text for this - revise?? *******
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 

      >[!TIP]
      >
      >The field types from the original record type must match the field types from the newly created record type.

1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Conditional) If you selected to create a record and there are no connection fields between the original record type and the record type selected in the **Actions** area, click the question mark icon to the right of the **Field on the connected record type where the current record will show** field, then click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   The new field is automatically created for the record type you selected in the **Actions** area, and named **Connected Record**. 
   
   A connected field for the selected record type is also created on the original record type from where you are configuring the automation. 
1. (Optional and conditional) If you selected to create a Workfront object and don't have a connection field for the selected Workfront object type, click the question mark icon to the right of the **Connected field where the < Workfront object type name > is created** field, and click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.

## Manage existing automations

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. (Optional) To edit, disable, or delete an automation, do one of the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.

      >[!TIP]
      >
      >   You cannot change the action you originally selected for an automation. 
   

   1. Click **Disable** to remove the automation from the record's table view and prevent users from using it to create records or objects. 

   Records that have been created using a disabled automation remain connected to the record originally selected.
   
   To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. 
   
   Records that have been created using a deleted automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the automation you want to use to autoamtically create and connect records or objects. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   The following things occur: 

   * A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   * The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   * The record you are triggering the automation from is added to the connected field of the new record.

   >[!NOTE]
   >
   >We recommend checking that the objects or records were created and the connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

***********you might need to add something about notifications and emails?!*************

-->