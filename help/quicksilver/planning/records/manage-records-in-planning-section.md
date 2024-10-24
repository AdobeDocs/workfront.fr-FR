---
title: Gestion des enregistrements dans la section Planification des objets Adobe Workfront
description: Vous pouvez afficher les enregistrements de planification Workfront associés aux objets Adobe Workfront dans la section Planification d’un objet Workfront, dans le panneau de gauche.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: e82cf1b586ea3b08f419802bd1e88c6567b61b95
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 9%

---


<!--add also Group and Company when they are available-->

# Gestion des connexions d’enregistrement à partir d’objets Workfront

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, consultez la section [Activer ou désactiver les versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Vous pouvez afficher les enregistrements de planification Workfront et leurs enregistrements respectifs connectés aux objets Adobe Workfront dans les zones suivantes de Workfront :

* La section Planification d’un objet Workfront : affiche tous les types d’enregistrements connectés à un objet et leurs enregistrements connectés respectifs.
* <span class="preview">Un champ personnalisé Planification de la connexion : affiche un type d’enregistrement et ses enregistrements connectés respectifs. </span>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

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
<p>L’un des projets Workfront suivants est prévu :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p>
   </td>

<tr>
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td>
   <td>
<p>Tous</p>
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Affichage ou accès supérieur à Projets, programmes et Portfolios</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <p>Dans Workfront, affichez ou autorisations supérieures à un projet, un portfolio ou un programme</a> </p> 
   <p>Dans la planification Workfront, consultez les autorisations d’un espace de travail pour afficher tout enregistrement connecté ou Contribute ou les autorisations supérieures à un espace de travail pour connecter ou déconnecter des enregistrements</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail de planification Workfront, y compris ceux qu’ils n’ont pas créés.</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Pour afficher la zone Planification ou la section Planification d’un objet Workfront, tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page comprenant la zone Planification du menu principal et la zone Planification des projets, portefeuilles et programmes. </p> Pour plus d’informations, consultez la <a href="/help/quicksilver/planning/access/access-overview.md">présentation de l’accès à Adobe Planning</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gestion des enregistrements dans la section Planification

Vous pouvez utiliser la section Planification d’un objet Workfront pour afficher tous les types d’enregistrements et leurs enregistrements respectifs connectés à l’objet Workfront.
La section Planification est disponible pour les objets Workfront suivants :

* Projet
* Portfolio
* Programme
<!--* Group
* Company-->

### Points à prendre en compte concernant la section Planification des objets Workfront

Tenez compte de ce qui suit lorsque vous affichez des enregistrements de planification Workfront à partir de la section Planification d’un objet Workfront :

* Les types d’enregistrement de la planification Workfront doivent d’abord être connectés aux types d’objets Workfront.

  Pour plus d’informations, voir les articles suivants :

   * [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connect records](/help/quicksilver/planning/records/connect-records.md)
* Vous pouvez afficher la section Planification à partir d’un objet Workfront, même lorsqu’aucun enregistrement n’est associé à l’objet Workfront.

### Gestion des connexions d’enregistrement à partir de la section Planification

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur la carte d’un type d’enregistrement connecté à un projet, un portfolio ou un programme Workfront.
1. Accédez à un champ d’enregistrement connecté qui a une connexion avec un objet Workfront, soit en mode Tableau, soit à partir de la page de détails d’un enregistrement. Pour plus d’informations, consultez la section [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).
1. Cliquez sur le nom d’un objet Workfront dans le champ d’enregistrement connecté.
La page de l’objet s’ouvre dans Workfront.

   >[!NOTE]
   >
   >  Si vous connaissez un objet Workfront déjà connecté à un enregistrement Planning, vous pouvez accéder à la section Planning à partir de l’objet Workfront.

1. Cliquez sur **Planning** dans le panneau de gauche.

   >[!NOTE]
   >
   >   L’administrateur de Workfront ou de groupe doit ajouter la section Planification à votre modèle de mise en page avant qu’elle ne s’affiche pour un projet, un portfolio ou un programme Workfront.

   La section Planification affiche les informations suivantes :

   * Les enregistrements connectés s’affichent sur des cartes individuelles contenant les informations suivantes :
      * Nom de l’enregistrement
      * Miniature de l’enregistrement
      * Nom du champ d’enregistrement connecté tel qu’il s’affiche dans Workfront Planning.
   * Les enregistrements s’affichent sous leur espace de travail respectif et leur type d’enregistrement.

   ![](assets/planning-section-on-project.png)

1. (Facultatif) Cliquez sur **Afficher toutes les connexions** pour afficher tous les types d’enregistrements connectés, y compris ceux sans enregistrements connectés. Par défaut, les types d’enregistrements sans enregistrements connectés ne s’affichent pas.
1. Cliquez sur une carte d’enregistrement pour afficher plus d’informations sur l’enregistrement. La zone d’aperçu des enregistrements s’affiche.
1. (Facultatif) Commencez à modifier les champs dans la zone d’aperçu de l’enregistrement. Vos modifications sont enregistrées automatiquement.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de la zone d’aperçu pour ouvrir la page de détails de l’enregistrement. La page de détails de l’enregistrement s’ouvre dans Workfront Planning.
1. (Facultatif) Pointez sur une carte d’enregistrement, puis cliquez sur l’icône de déconnexion d’enregistrement **-**, puis cliquez sur **Déconnecter**.
Les événements suivants se produisent :
   * L’enregistrement n’est plus connecté à l’objet Workfront.
   * L’objet Workfront est également supprimé du champ connecté de l’enregistrement de Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont également supprimées.
1. Cliquez sur **Connect** pour connecter plus d’enregistrements pour les types d’enregistrements connectés. Pour plus d’informations, consultez [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).

   Les événements suivants se produisent :

   * Les enregistrements sont immédiatement connectés à l’objet Workfront et s’affichent dans la section Planification .
   * L’objet Workfront est ajouté au champ connecté de l’enregistrement Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont renseignées dans Workfront Planning.

<div class="preview">

## Gestion des enregistrements dans le type de champ Planning de connexion

Vous pouvez utiliser un champ personnalisé Planification de la connexion sur un objet Workfront pour afficher un type d’enregistrement et ses enregistrements respectifs connectés à l’objet Workfront.

Vous pouvez contrôler les types d’enregistrement Planning qui s’affichent pour l’objet Workfront lorsque vous créez des champs personnalisés de connexion Planning .

* Le champ Planification de la connexion affiche les enregistrements de planification une fois la connexion établie et lorsque le champ est joint aux formulaires pour les objets Workfront suivants :

   * Projet
   * Portfolio
   * Programme
   * Groupe
   * Entreprise

Pour plus d’informations, voir [Création d’un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Observations relatives au type de champ Planning de connexion

Tenez compte de ce qui suit lorsque vous affichez des enregistrements de planification Workfront à partir d’un champ de connexion Planning d’un objet Workfront :

* Vous ne pouvez associer qu&#39;un seul type d&#39;enregistrement à un champ de connexion Planning .
* Si vous disposez d’un accès correct, vous devez joindre un formulaire personnalisé avec un champ personnalisé de connexion Planning à un objet Workfront qui peut être connecté à Workfront Planning.
* Les types d’enregistrement de la planification Workfront doivent d’abord être connectés aux types d’objets Workfront. Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
* Vous pouvez connecter ou déconnecter des enregistrements du champ Planification de la connexion d’un objet Workfront uniquement pour les objets qui peuvent avoir des connexions Workfront Planning.
* Vous devez disposer des autorisations Contribute pour un espace de travail dans Workfront Planning pour pouvoir connecter ou déconnecter des enregistrements du champ Planification de la connexion d’un objet Workfront.
* Vous ne pouvez pas modifier un champ de planification de la connexion lors de la modification en masse d’objets Workfront.

### Gestion des connexions d’enregistrement à partir du type de champ Planification de la connexion

1. Accédez à l’un des types d’objets suivants qui a été connecté à un type d’enregistrement Workfront Planning :

   * Projet
   * Portfolio
   * Programme
   * Entreprise
   * Groupe

1. Cliquez sur **&lt; Objet > Détails** dans le panneau de gauche.
1. (Conditionnel) Ajoutez un formulaire personnalisé avec au moins un champ Planification de la connexion pour l’objet sélectionné, le cas échéant.

   >[!NOTE]
   >
   >L’administrateur de Workfront ou de groupe doit d’abord créer le formulaire et y ajouter un champ Planification de la connexion avant de pouvoir l’ajouter à un objet.


1. Cliquez dans le champ pour ajouter les enregistrements connectés, puis cliquez sur la flèche pointant vers le bas située à l&#39;intérieur du champ pour sélectionner des enregistrements dans la liste.

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Vous ne pouvez pas ajouter d’enregistrements aux champs de connexion Planification associés à des objets Workfront autres que l’objet sélectionné lors de la configuration du champ.
   >
   >Par exemple, vous ne pouvez pas ajouter d’enregistrements à un champ de connexion Planification créé pour une connexion par Portfolio à partir du formulaire personnalisé d’un projet.
   >
   >Il existe une indication que l’objet du champ et l’objet que vous avez sélectionné ne correspondent pas.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Cliquez en dehors de la liste pour la fermer.

   Les événements suivants se produisent :

   * Les enregistrements sont immédiatement connectés à l’objet Workfront et s’affichent dans le champ Connexion de planification , ainsi que dans la section Planification de l’objet Workfront.
   * L’objet Workfront est ajouté au champ connecté de l’enregistrement Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont renseignées dans Workfront Planning.
1. (Facultatif) Cliquez sur le nom d’un enregistrement dans le champ Planification de la connexion pour l’ouvrir dans Workfront Planning.
L’onglet Détails de l’enregistrement s’ouvre dans la planification Workfront.
Vous pouvez consulter les informations relatives à l’enregistrement ou accéder à la page du type d’enregistrement.

1. (Facultatif) Dans le formulaire personnalisé de Workfront, cliquez sur l’icône **Supprimer** ![](assets/remove-icon.png) sur un enregistrement pour le supprimer du champ Planification de la connexion et le déconnecter de l’objet Workfront.
L’objet Workfront est déconnecté de l’enregistrement de planification et toutes les informations de recherche de Workfront sont supprimées de l’enregistrement.

</div>