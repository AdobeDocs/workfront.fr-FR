---
title: Gestion des enregistrements dans la section Planification des objets Adobe Workfront
description: Vous pouvez afficher les enregistrements de planification Workfront associés aux objets Adobe Workfront dans la section Planification d’un objet Workfront, dans le panneau de gauche.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 11%

---


<!--add also Group and Company when they are available-->

# Gérer des enregistrements dans la section Planning des objets Adobe Workfront

{{planning-important-intro}}

Vous pouvez afficher les enregistrements de planification Workfront associés aux objets Adobe Workfront dans la section Planification d’un objet Workfront, dans le panneau de gauche.

La section Planification est disponible pour les objets Workfront suivants :

* Projet
* Portfolio
* Programme
<!--* Group
* Company-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Pour pouvoir accéder à Workfront Planning, vous devez disposer des éléments suivants :

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
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, voir <a href="https://business.adobe.com/products/workfront/pricing.html">Prix et package Adobe Workfront</a>. </p>
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
   <p>Dans Workfront Planning, Contribute ou autorisations supérieures à un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail de planification Workfront, y compris ceux qu’ils n’ont pas créés.</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page comprenant la zone Planification du menu principal et la zone Planification des projets, portefeuilles et programmes. </p> Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Présentation des accès</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Points à prendre en compte concernant la section Planification des objets Workfront

* Les types d’enregistrement de la planification Workfront doivent être connectés aux types d’objets Workfront.

  Pour plus d’informations, voir les articles suivants :

   * [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connect records](/help/quicksilver/planning/records/connect-records.md)
* Vous pouvez afficher la section Planification dans un objet Workfront, même lorsqu’aucun enregistrement n’est associé à l’objet Workfront.
* Vous pouvez connecter des enregistrements de planification à des objets Workfront de Workfront, dans la section Planification lorsqu’au moins un enregistrement est connecté à l’objet Workfront.

## Gestion des enregistrements dans la section Planification

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur la carte d’un type d’enregistrement connecté à un projet, un portfolio ou un programme Workfront.
1. Accédez à un champ d’enregistrement connecté qui a une connexion avec un objet Workfront, soit en mode Tableau, soit à partir de la page de détails d’un enregistrement. Pour plus d’informations, consultez la section [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).
1. Cliquez sur le nom d’un objet Workfront dans le champ d’enregistrement connecté.
La page des objets s’ouvre dans Workfront.

1. Cliquez sur **Planning** dans le panneau de gauche.

   >[!NOTE]
   >
   >   L’administrateur de Workfront ou de groupe doit ajouter la section Planification à votre modèle de mise en page avant qu’elle ne s’affiche pour un projet, un portfolio ou un programme Worfront.

   La section Planification affiche les informations suivantes :

   * Les enregistrements connectés s’affichent sur des cartes individuelles contenant les informations suivantes :
      * Nom de l’enregistrement
      * Miniature de l’enregistrement
      * Nom du champ d’enregistrement connecté tel qu’il s’affiche dans Workfront Planning.
   * Les enregistrements s’affichent sous leur espace de travail respectif.

   ![](assets/planning-section-on-project.png)

1. (Facultatif) Cliquez sur **Afficher toutes les connexions** pour afficher tous les types d’enregistrements connectés, y compris ceux sans enregistrements connectés. Par défaut, les types d’enregistrements sans enregistrements connectés ne s’affichent pas.
1. Cliquez sur une carte d’enregistrement pour afficher plus d’informations sur l’enregistrement. La zone d’aperçu des enregistrements s’affiche.
1. (Facultatif) Commencez à modifier les champs dans la zone d’aperçu de l’enregistrement. Vos modifications sont enregistrées automatiquement.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de la zone d’aperçu pour ouvrir la page de détails de l’enregistrement. La page de détails de l’enregistrement s’ouvre dans Workfront Planning.
1. Pointez sur une carte d’enregistrement, puis cliquez sur l’icône de déconnexion d’enregistrement **-**, puis cliquez sur **Déconnecter**.
Les événements suivants se produisent :
   * L’enregistrement n’est plus connecté à l’objet Workfront.
   * L’objet Workfront est également supprimé du champ connecté de l’enregistrement de Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont également supprimées.
1. Cliquez sur **Connect** pour connecter plus d’enregistrements pour les types d’enregistrements connectés. Pour plus d’informations, consultez [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).

   Les événements suivants se produisent :

   * Les enregistrements sont immédiatement connectés à l’objet Workfront et s’affichent dans la section Planification .
   * L’objet Workfront est ajouté au champ connecté de l’enregistrement Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont renseignées dans Workfront Planning.


