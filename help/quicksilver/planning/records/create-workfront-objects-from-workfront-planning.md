---
title: Créer des objets Workfront à partir de Workfront Planning en les connectant à des enregistrements
description: Vous pouvez créer des types d'objets Workfront en les connectant à partir d'autres enregistrements dans Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 57592455c61f0ddd14f6d2bcc033b58a8cdc7028
workflow-type: tm+mt
source-wordcount: '1267'
ht-degree: 5%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Créer des objets Workfront à partir de Workfront Planning en les connectant à des enregistrements

<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez créer des objets Adobe Workfront à partir de Workfront Planning des manières suivantes :

* Connexion d&#39;objets Workfront à partir d&#39;enregistrements Planning

  Cet article décrit comment créer des objets Workfront à partir de Workfront Planning en les connectant à partir d&#39;enregistrements Planning.
* Lorsque vous utilisez des automatisations à partir d’une page d’enregistrement.

  Pour plus d’informations sur la création d’objets Workfront à l’aide d’automatisations, voir [Création d’objets à l’aide des automatisations d’enregistrements Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

>[!IMPORTANT]
>
>Vous pouvez créer les objets Workfront suivants à partir de Workfront Planning lorsque vous les connectez à des enregistrements Planning :
>
>* Projets
>* Portefeuilles
>* Programmes
>
>Vous pouvez connecter les objets Workfront suivants aux enregistrements Planning, mais vous ne pouvez pas les créer dans le processus de connexion :
>
>* Groupes
>* Entreprises
>

Tenez compte des points suivants lors de la connexion et de la création d’objets Workfront à des enregistrements Workfront Planning :

* Vous pouvez connecter des projets, portfolios, programmes, groupes et sociétés Workfront à partir d’un champ de connexion provenant des zones suivantes de Workfront Planning :

   * Vue Tableau d’un type d’enregistrement
   * Page de détails ou zone de prévisualisation d’un enregistrement
   * Onglet Connexions d’un enregistrement

* Vous pouvez créer des projets à partir des zones suivantes de Workfront Planning :

   * Vue Tableau d’un type d’enregistrement
   * La zone Détails d’un enregistrement dans le champ de connexion
   * Page d’enregistrement connecté d’un enregistrement

* Vous pouvez créer des portfolios et des programmes à partir des zones suivantes de Workfront Planning :

   * Vue Tableau d’un type d’enregistrement
   * La zone Détails d’un enregistrement dans le champ de connexion

Pour plus d&#39;informations sur la connexion des enregistrements Planning aux objets Workfront, voir [Connexion des enregistrements](/help/quicksilver/planning/records/connect-records.md).

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
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront et tout package Planning</p> <p>Tout workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td>

<tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p> 
   <p>Modifiez l’accès avec l’accès à Créer des objets dans Workfront pour les types d’objets que vous souhaitez créer (projets, portfolios, programmes). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Autorisations de niveau Contribution ou supérieur à l’espace de travail et au type d’enregistrement dans lesquels vous souhaitez ajouter des enregistrements. </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
   <p>Gérez les autorisations sur les objets Workfront (portfolios) pour ajouter des objets enfants (projets).</p>
   </td> 
  </tr>   
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
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
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  -->


## Conditions préalables à la création d&#39;objets Workfront lors de leur connexion avec des enregistrements de Workfront Planning

Vous devez disposer des éléments suivants avant de pouvoir ajouter de nouveaux projets ou portfolios en les connectant à partir d’enregistrements existants :

* Types d’enregistrements liés aux projets, portfolios ou programmes Workfront. Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
* Enregistrements pour les types d’enregistrements connectés aux objets Workfront. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* L’accès et les autorisations appropriés dans Workfront Planning et Workfront, comme décrit dans la section [Exigences d’accès](#access-requirements) de cet article.

## Créer des projets en les connectant à des enregistrements de Workfront Planning

Vous pouvez créer des projets en les connectant à des enregistrements dans Workfront Planning dans les domaines suivants de Workfront Planning :

* Vue tabulaire d’un type d’enregistrement ou zone Détails d’un enregistrement dans le champ de connexion
* Page Enregistrement connecté d’un enregistrement dans la zone Détails d’un enregistrement

### Créer des projets à partir de la zone Détails d&#39;un enregistrement ou de la vue Tableau d&#39;un type d&#39;enregistrement

Pour créer des projets au fur et à mesure que vous les connectez à partir d’autres enregistrements :

1. Accédez à la page de détails d’un enregistrement ou à la table du type d’enregistrement et commencez à connecter les enregistrements Workfront Planning aux projets Workfront, comme décrit dans l’article [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

1. (Conditionnel) Cliquez sur **Ajouter un projet**
Ou
Commencez à saisir le nom d’un projet, puis cliquez sur **Ajouter un projet** si vous ne le trouvez pas. Le bouton Ajouter est suivi du nom du projet que vous avez saisi.

   ![Ajouter un projet lors de sa connexion à partir d’un champ de connexion](assets/add-project-when-connecting-it-from-connection-field.png)

   La boîte **Créer un projet** s’ouvre.

1. (Facultatif) Mettez à jour le **nom du projet**. Par défaut, le projet est nommé en fonction de ce que vous avez ajouté comme élément de recherche lors de sa connexion à partir de l’enregistrement .
1. (Facultatif) Sélectionnez un **modèle de projet**. Si vous ne sélectionnez pas de modèle, Workfront crée un projet vierge sans tâche.
1. Cliquez sur **Créer**.
1. (Conditionnel) Si vous avez choisi de créer un projet à partir d’un modèle, suivez les étapes de l’article [Créer un projet à l’aide d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) pour terminer l’ajout du projet.

   Le nouveau projet est créé et ajouté au champ connecté de l&#39;enregistrement sélectionné.

1. (Facultatif) Cliquez sur le nom du nouveau projet dans Workfront Planning pour ouvrir la page du projet dans Workfront et apporter des mises à jour supplémentaires au projet.

### Créer des projets à partir de la page Enregistrements connectés d’un enregistrement

1. Connectez le type d&#39;objet Project à un type d&#39;enregistrement Workfront Planning en mode Tableau.

   Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Cliquez sur le nom d’un enregistrement dans n’importe quel affichage. La zone d’aperçu Détails s’ouvre.

1. Ajoutez une **Page Enregistrements connectés** pour les projets.

   Pour plus d’informations, consultez la section « Ajouter une page Enregistrements connectés à un enregistrement » de l’article [Gérer la mise en page de la page d’enregistrement](/help/quicksilver/planning/records/manage-the-record-page.md).

   La page Enregistrements connectés s’affiche en mode Tableau. Les projets connectés s’affichent dans le tableau.

   ![Vue Tableau Projets dans la page Enregistrements connectés](assets/projects-connected-records-page-table.png)

1. Cliquez sur **Nouvelle ligne** dans le tableau Projets pour ajouter un projet.

   Vous pouvez uniquement ajouter un projet vierge dans cette zone. Vous ne pouvez pas ajouter un projet à l’aide d’un modèle.
1. (Facultatif) Cliquez sur le nom du projet dans la vue Tableau pour ouvrir le projet dans Workfront et ajouter plus d’informations.

## Créer des portfolios en les connectant à des enregistrements de Workfront Planning

Vous pouvez créer des portfolios à partir de la vue Tableau d’un type d’enregistrement ou de la page Détails d’un enregistrement.

Pour créer des portefeuilles au fur et à mesure que vous les connectez à partir d&#39;enregistrements Planning :

1. Accédez à la page de détails d’un enregistrement ou à la table du type d’enregistrement et commencez à connecter les enregistrements Workfront Planning aux portfolios Workfront, comme décrit dans l’article [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

1. (Conditionnel) Cliquez sur **Ajouter un portfolio**

   Ou

   Commencez à saisir le nom d’un portfolio, puis cliquez sur **Ajouter un portfolio** si vous ne le trouvez pas. Le bouton Ajouter est suivi du nom du portfolio que vous avez saisi.

   ![Ajouter un portfolio lors de sa connexion à partir d’un champ de connexion](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Le portfolio est créé et ajouté au champ de connexion de l’enregistrement que vous avez sélectionné.

1. (Facultatif) Cliquez sur le nom du nouveau portefeuille dans Workfront Planning pour ouvrir la page du portefeuille dans Workfront et effectuer des mises à jour supplémentaires sur le portefeuille.

## Créer des programmes en les connectant à des enregistrements de Workfront Planning

Vous pouvez créer des programmes à partir de la vue Tableau d’un type d’enregistrement ou de la page Détails d’un enregistrement.

Pour créer des programmes au fur et à mesure que vous les connectez à partir des enregistrements Planning :

1. Accédez à la page de détails d’un enregistrement ou à la table du type d’enregistrement et commencez à connecter les enregistrements Workfront Planning aux portfolios Workfront, comme décrit dans l’article [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

1. Cliquez sur **Ajouter un programme**

   Ou

   Commencez à saisir le nom d’un programme, puis cliquez sur **Ajouter un programme** si vous ne le trouvez pas. Le bouton Ajouter est suivi du nom du programme que vous avez saisi.

   ![Ajouter le programme Workfront lors de sa connexion à partir du champ de connexion](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   La boîte de dialogue **Créer un programme** s’ouvre.

1. Mettez à jour le **nom du programme**. Champ obligatoire.
1. Choisissez un **Portfolio** dans la liste déroulante ou commencez à saisir le nom d&#39;un portfolio, puis sélectionnez-le lorsqu&#39;il s&#39;affiche dans la liste. Champ obligatoire.
1. Cliquez sur **Créer**.

   Le programme est créé et ajouté dans le champ de connexion de l&#39;enregistrement que vous avez sélectionné.

1. (Facultatif) Cliquez sur le nom du nouveau programme dans Workfront Planning pour ouvrir la page du programme dans Workfront et y apporter des mises à jour supplémentaires.

