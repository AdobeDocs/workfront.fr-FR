---
title: Création d’objets Workfront à partir de Workfront Planning
description: Vous pouvez créer des types d'objets Workfront en les connectant à partir d'autres enregistrements dans Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '1088'
ht-degree: 10%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Créer des objets Workfront à partir de Workfront Planning en les connectant à des enregistrements

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">Les informations mises en évidence sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles pour tous. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez créer des objets Adobe Workfront à partir de Workfront Planning des manières suivantes :

* Connexion d&#39;objets Workfront à partir d&#39;enregistrements Planning

  Cet article décrit comment créer des objets Workfront à partir de Workfront Planning en les connectant à partir d&#39;enregistrements Planning.
* Lorsque vous utilisez des automatisations à partir d’une page d’enregistrement.

  Pour plus d’informations sur la création d’objets Workfront à l’aide d’automatisations, voir [Création d’objets à l’aide des automatisations d’enregistrements Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Vous pouvez créer les types d&#39;objets Workfront suivants à partir de Workfront Planning lorsque vous connectez un enregistrement Workfront Planning aux types d&#39;objets Workfront suivants :

* Projets
* Portefeuilles
* Programmes

>[!IMPORTANT]
>
>* Vous ne pouvez créer que des projets, portfolios et programmes dans Workfront lors de leur connexion à partir d’un enregistrement.
>
>* Vous ne pouvez pas créer de groupes ou de sociétés lors de leur connexion à partir d&#39;un enregistrement dans Workfront Planning.
>

Vous pouvez connecter des projets, des portfolios et des programmes à partir d’un champ de connexion dans les zones suivantes de Workfront Planning :

* Vue Tableau d’un type d’enregistrement
* Page de détails ou zone de prévisualisation d’un enregistrement
* Onglet Connexions d’un enregistrement

Pour plus d&#39;informations sur la connexion des enregistrements Planning aux objets Workfront, voir [Connexion des enregistrements](/help/quicksilver/planning/records/connect-records.md).

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
   <td> Standard
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p> 
   <p>Modifiez l’accès dans Workfront pour les types d’objets que vous souhaitez créer (projets, programmes et portfolios) lorsque vous connectez les enregistrements à ceux-ci. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Gérez les autorisations relatives à l’espace de travail <span class="preview">et au type d’enregistrement</span> où vous souhaitez ajouter des enregistrements. </p>  
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

## Conditions préalables à la création d&#39;objets Workfront lors de leur connexion avec des enregistrements de Workfront Planning

Vous devez disposer des éléments suivants avant de pouvoir ajouter de nouveaux projets ou portfolios en les connectant à partir d’enregistrements existants :

* Types d’enregistrements liés aux projets, portfolios ou programmes Workfront. Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
* Enregistrements. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* L’accès et les autorisations appropriés dans Workfront Planning et Workfront, comme décrit dans la section [Exigences d’accès](#access-requirements) de cet article.

## Créer des projets en les connectant à des enregistrements de Workfront Planning

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

## Créer des portfolios en les connectant à des enregistrements de Workfront Planning

Pour créer des portefeuilles au fur et à mesure que vous les connectez à partir d&#39;enregistrements Planning :

1. Accédez à la page de détails d’un enregistrement ou à la table du type d’enregistrement et commencez à connecter les enregistrements Workfront Planning aux portfolios Workfront, comme décrit dans l’article [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

1. (Conditionnel) Cliquez sur **Ajouter un portfolio**

   Ou

   Commencez à saisir le nom d’un portfolio, puis cliquez sur **Ajouter un portfolio** si vous ne le trouvez pas. Le bouton Ajouter est suivi du nom du portfolio que vous avez saisi.

   ![Ajouter un portfolio lors de sa connexion à partir d’un champ de connexion](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Le portfolio est créé et ajouté au champ de connexion de l’enregistrement que vous avez sélectionné.

1. (Facultatif) Cliquez sur le nom du nouveau portefeuille dans Workfront Planning pour ouvrir la page du portefeuille dans Workfront et effectuer des mises à jour supplémentaires sur le portefeuille.

## Créer des programmes en les connectant à des enregistrements de Workfront Planning

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

