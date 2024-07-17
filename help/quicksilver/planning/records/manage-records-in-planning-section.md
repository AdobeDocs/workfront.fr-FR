---
title: Gestion des enregistrements dans la section Planification des objets Adobe Workfront
description: Vous pouvez afficher les enregistrements connectés aux objets Adobe Workfront dans la section Planification d’un objet Workfront, dans le panneau de gauche.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 10%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->

<!-- opening the Details preview and page is not possible yet - hid those steps, but add them when released-->


# Gestion des enregistrements dans la section Planification des objets Adobe Workfront

{{planning-important-intro}}

Vous pouvez afficher les enregistrements connectés aux objets Adobe Workfront dans la section Planification d’un objet Workfront, dans le panneau de gauche.

La section Planification est disponible pour les objets Workfront suivants :

* Projet
* Portfolio
* Programme
<!--* Group
* Company-->

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouvelle : standard</p>
   Ou
   <p>Actuelle : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Affichage ou accès supérieur à Projets, programmes et Portfolios</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Dans Workfront, affichez ou autorisations supérieures à un projet, un portfolio ou un programme</a> </p> 
   <p>Dans Workfront Planning, Contribute ou autorisations supérieures à un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail de planification Workfront, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans le menu principal et la section Planning dans le panneau de gauche à votre modèle de mise en page. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Points à prendre en compte concernant la section Planification des objets Workfront

* Tout d’abord, vous devez connecter les types d’enregistrements aux types d’objets Workfront et les enregistrements aux objets Workfront pour les afficher dans Workfront.

  Pour plus d’informations, voir les articles suivants :

   * [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md)
* Vous pouvez afficher la section Planification dans un objet Workfront, même lorsqu’aucun enregistrement n’est associé à l’objet Workfront.
* Vous pouvez connecter des enregistrements de planification à des objets Workfront de Workfront, dans la section Planification lorsqu’au moins un enregistrement est connecté à l’objet Workfront.

## Gestion des enregistrements dans la section Planification

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur la carte d’un type d’enregistrement connecté à un projet, un portfolio ou un programme Workfront.
1. Accédez à un champ d’enregistrement connecté qui a une connexion avec un objet Workfront, soit en mode Tableau, soit à partir de la page de détails d’un enregistrement. Pour plus d’informations, voir [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).
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

1. Cliquez sur une carte d’enregistrement pour afficher plus d’informations sur l’enregistrement. La zone d’aperçu des enregistrements s’affiche.
1. (Facultatif) Commencez à modifier les champs dans la zone d’aperçu de l’enregistrement. Vos modifications sont enregistrées automatiquement.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de la zone d’aperçu pour ouvrir la page de détails de l’enregistrement. La page de détails de l’enregistrement s’ouvre dans Workfront Planning.
1. Pointez sur une carte d’enregistrement, puis cliquez sur l’icône de déconnexion d’enregistrement **-**, puis cliquez sur **Déconnecter**.
Les événements suivants se produisent :
   * L’enregistrement n’est plus connecté à l’objet Workfront.
   * L’objet Workfront est également supprimé du champ connecté de l’enregistrement de Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont également supprimées.
1. Cliquez sur **Se connecter** pour connecter d&#39;autres enregistrements.

   >[!NOTE]
   >
   >   Le bouton Se connecter s’affiche uniquement pour les espaces de travail dans lesquels vous disposez des autorisations Contribute. <!--they might replace this with one button at the top of the page. Rephrase-->

1. Cliquez sur les enregistrements que vous souhaitez connecter. Les événements suivants se produisent :

   * Les enregistrements sont immédiatement connectés à l’objet Workfront et s’affichent dans la section Planification .
   * L’objet Workfront est ajouté au champ connecté de l’enregistrement Workfront Planning.
   * Les valeurs des champs de recherche Workfront connectés à l’enregistrement Planning sont renseignées dans Workfront Planning.

<!--add more steps here for what happens after clicking Connect-->
