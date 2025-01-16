---
title: Gestion des enregistrements dans la section Planification des objets Adobe Workfront
description: Vous pouvez afficher les enregistrements Workfront Planning connectés aux objets Adobe Workfront dans la section Planning d'un objet Workfront, dans le panneau de gauche.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 7%

---


<!--add also Group and Company when they are available-->

# Gérer les connexions d’enregistrement à partir d’objets Workfront

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

Vous pouvez afficher les enregistrements Workfront Planning et leurs enregistrements respectifs connectés aux objets Adobe Workfront dans les zones suivantes de Workfront :

* La section Planning d’un objet Workfront : affiche tous les types d’enregistrements connectés à un objet et leurs enregistrements correspondants connectés.
* Un champ personnalisé de connexion Planning : affiche un type d’enregistrement et ses enregistrements connectés respectifs.

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
<p>Tous</p>
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
   <td>
   <p>Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Accès en affichage ou supérieur aux projets, programmes et Portfolios</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <p>Dans Workfront, autorisations d’affichage ou supérieures pour un projet, un portfolio ou un programme</a> </p> 
   <p>Dans Workfront Planning, affichez les autorisations relatives à un espace de travail pour afficher tous les enregistrements connectés ou les autorisations Contribute ou supérieures relatives à un espace de travail pour connecter ou déconnecter des enregistrements</a> </p>  
   <p>Les administrateurs système disposent d’autorisations sur tous les espaces de travail Workfront Planning, y compris ceux qu’ils n’ont pas créés</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Pour afficher la zone Planning ou la section Planning d'un objet Workfront, tous les utilisateurs, y compris les administrateurs Workfront, doivent se voir attribuer un modèle de mise en page qui inclut la zone Planning dans le menu principal et la zone Planning pour les projets, portfolios et programmes. </p> Pour plus d'informations, voir Présentation de l'accès à la planification d'Adobe <a href="/help/quicksilver/planning/access/access-overview.md"></a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gestion des enregistrements dans la section Planification

Vous pouvez utiliser la section Planification d’un objet Workfront pour afficher tous les types d’enregistrements et leurs enregistrements respectifs connectés à l’objet Workfront.
La section Planning est disponible pour les objets Workfront suivants :

* Projet
* Portfolio
* Programme
<!--* Group
* Company-->

### Considérations relatives à la section Planification des objets Workfront

Tenez compte des points suivants lorsque vous affichez les enregistrements Workfront Planning à partir de la section Planning d’un objet Workfront :

* Les types d’enregistrements Workfront Planning doivent d’abord être connectés aux types d’objets Workfront.

  Pour plus d’informations, voir les articles suivants :

   * [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connect records](/help/quicksilver/planning/records/connect-records.md)
* Vous pouvez afficher la section Planning à partir d&#39;un objet Workfront, même si aucun enregistrement n&#39;est associé à l&#39;objet Workfront.

### Gérer les connexions aux enregistrements à partir de la section Planification

{{step1-to-planning}}

1. Cliquez sur la vignette d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la carte d’un type d’enregistrement connecté à un projet, un portfolio ou un programme Workfront.
1. Accédez à un champ d’enregistrement connecté ayant une connexion avec un objet Workfront, en mode Tableau ou à partir de la page de détails d’un enregistrement. Pour plus d’informations, consultez la section [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).
1. Cliquez sur le nom d’un objet Workfront dans le champ d’enregistrement connecté.
La page de l’objet s’ouvre dans Workfront.

   >[!NOTE]
   >
   >  Si vous connaissez un objet Workfront déjà connecté à un enregistrement Planning, vous pouvez accéder à la section Planning à partir de l&#39;objet Workfront.

1. Cliquez sur **Planification** dans le panneau de gauche.

   >[!NOTE]
   >
   >   Votre administrateur Workfront ou de groupe doit ajouter la section Planification à votre modèle de mise en page avant qu’elle ne s’affiche pour un projet, un portfolio ou un programme Workfront.

   La section Planification s’affiche avec les informations suivantes :

   * Les enregistrements connectés s’affichent sur des cartes individuelles contenant les informations suivantes :
      * Nom de l’enregistrement
      * La miniature de l’enregistrement
      * Nom du champ d’enregistrement connecté tel qu’il s’affiche dans Workfront Planning.
   * Les enregistrements s’affichent dans leur espace de travail et leur type d’enregistrement respectifs.

   ![](assets/planning-section-on-project.png)

1. (Facultatif) Cliquez sur **Afficher toutes les connexions** pour afficher tous les types d’enregistrements connectés, y compris ceux sans enregistrements connectés. Par défaut, les types d’enregistrements sans enregistrements connectés ne s’affichent pas.
1. Cliquez sur une carte d’enregistrement pour afficher plus d’informations sur l’enregistrement. La zone de prévisualisation des enregistrements s’affiche.
1. (Facultatif) Commencez à modifier les champs dans la zone d’aperçu de l’enregistrement. Vos modifications sont enregistrées automatiquement.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de la zone d’aperçu pour ouvrir la page des détails de l’enregistrement. La page de détails de l’enregistrement s’ouvre dans Workfront Planning.
1. (Facultatif) Pointez sur une carte d’enregistrement, puis cliquez sur l’icône Déconnecter l’enregistrement **-**, puis sur **Déconnecter**.
Les événements suivants se produisent :
   * L’enregistrement n’est plus connecté à l’objet Workfront.
   * L’objet Workfront est également supprimé du champ connecté de l’enregistrement dans Workfront Planning.
   * Les valeurs des champs de recherche Workfront liés à l&#39;enregistrement Planning sont également supprimées.
1. Cliquez sur **Connexion** pour connecter d’autres enregistrements pour les types d’enregistrements connectés. Pour plus d’informations, consultez [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).

   Les événements suivants se produisent :

   * Les enregistrements sont immédiatement associés à l&#39;objet Workfront et s&#39;affichent dans la section Planning.
   * L’objet Workfront est ajouté au champ connecté de l’enregistrement Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont renseignées dans Workfront Planning.

## Gérer les enregistrements dans le type de champ de connexion Planning

Vous pouvez utiliser un champ personnalisé de connexion Planning sur un objet Workfront pour afficher un type d’enregistrement et ses enregistrements respectifs connectés à l’objet Workfront.

Vous pouvez contrôler quels types d&#39;enregistrements Planning s&#39;affichent pour l&#39;objet Workfront lorsque vous créez des champs personnalisés de connexion Planning.

* Le champ de connexion Planning affiche les enregistrements Planning après l&#39;établissement d&#39;une connexion et lorsque le champ est joint à des formulaires pour les objets Workfront suivants :

   * Projet
   * Portfolio
   * Programme
   * Groupe
   * Entreprise

Pour plus d’informations, voir [Créer un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Considérations relatives au type de champ de connexion Planning

Tenez compte des points suivants lorsque vous affichez les enregistrements Workfront Planning à partir du champ de connexion Planning d’un objet Workfront :

* Vous ne pouvez associer qu&#39;un seul type d&#39;enregistrement à un champ de connexion Planning.
* Vous devez joindre un formulaire personnalisé avec un champ personnalisé de connexion Planning à un objet Workfront qui peut être connecté à partir de Workfront Planning, si vous disposez des droits d&#39;accès appropriés.
* Les types d’enregistrements Workfront Planning doivent d’abord être connectés aux types d’objets Workfront. Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
* Vous pouvez connecter ou déconnecter des enregistrements du champ de connexion Planning d&#39;un objet Workfront uniquement pour les objets qui peuvent avoir des connexions Workfront Planning.
* Vous devez disposer des autorisations Contribute pour un espace de travail dans Workfront Planning afin de pouvoir connecter ou déconnecter des enregistrements du champ de connexion Planning d&#39;un objet Workfront.
* Vous ne pouvez pas modifier un champ de connexion Planning lors de la modification en bloc d’objets Workfront.

### Gérer les connexions d&#39;enregistrement à partir du type de champ de connexion Planning

1. Accédez à l&#39;un des types d&#39;objets suivants qui a été connecté à un type d&#39;enregistrement Workfront Planning :

   * Projet
   * Portfolio
   * Programme
   * Entreprise
   * Groupe

1. Cliquez sur **&lt; Objet > Détails** dans le panneau de gauche.
1. (Conditionnel) Ajoutez un formulaire personnalisé avec au moins un champ de connexion Planning pour l&#39;objet que vous avez sélectionné, s&#39;il n&#39;en existe pas.

   >[!NOTE]
   >
   >Votre administrateur Workfront ou de groupe doit d&#39;abord créer le formulaire et y ajouter un champ de connexion Planning avant de pouvoir l&#39;ajouter à un objet.


1. Cliquez dans le champ pour ajouter des enregistrements connectés, puis cliquez sur la flèche pointant vers le bas à l’intérieur du champ pour sélectionner des enregistrements dans la liste.

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Vous ne pouvez pas ajouter d&#39;enregistrements aux champs de connexion Planning qui sont associés à des objets Workfront autres que l&#39;objet que vous avez sélectionné lors de la configuration du champ.
   >
   >Par exemple, vous ne pouvez pas ajouter d&#39;enregistrements à un champ de connexion Planning créé pour une connexion de Portfolio à partir du formulaire personnalisé d&#39;un projet.
   >
   >Cela indique que l’objet du champ et l’objet que vous avez sélectionné ne correspondent pas.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Cliquez en dehors de la liste pour la fermer.

   Les événements suivants se produisent :

   * Les enregistrements sont immédiatement associés à l&#39;objet Workfront et s&#39;affichent dans le champ de connexion Planning ainsi que dans la section Planning de l&#39;objet Workfront.
   * L’objet Workfront est ajouté au champ connecté de l’enregistrement Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont renseignées dans Workfront Planning.
1. (Facultatif) Cliquez sur le nom d&#39;un enregistrement dans le champ Connexion Planning pour l&#39;ouvrir dans Workfront Planning.
L’onglet Détails de l’enregistrement s’ouvre dans Workfront Planning.
Vous pouvez consulter les informations sur l’enregistrement ou accéder à la page du type d’enregistrement.

1. (Facultatif) Dans le formulaire personnalisé de Workfront, cliquez sur l’icône **Supprimer** ![](assets/remove-icon.png) sur un enregistrement pour le supprimer du champ de connexion Planning et le déconnecter de l’objet Workfront.
L&#39;objet Workfront est déconnecté de l&#39;enregistrement Planning et toutes les informations de recherche de Workfront sont supprimées de l&#39;enregistrement.