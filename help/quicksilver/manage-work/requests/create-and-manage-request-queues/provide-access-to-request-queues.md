---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Fournir l’accès aux files d’attente des demandes
description: Lorsque vous accordez l’accès à une file d’attente des demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente des demandes dans la zone Demandes d’Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 55%

---

# Accorder l’accès aux files d’attente des demandes

<!-- Audited: 6/2025 -->

Lorsque vous accordez l’accès à une file d’attente des demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente des demandes dans la zone Demandes d’Adobe Workfront.

Vous pouvez fournir à différents utilisateurs l’accès à une file d’attente des demandes, selon qu’ils font partie de l’équipe du projet, du groupe de projets ou de l’entreprise du projet. Vous pouvez également fournir un accès à la file d’attente des demandes à tous les membres du système.

Cela s’avère utile dans les organisations qui invitent des parties prenantes externes dans Workfront et souhaitent limiter l’accès des utilisateurs à des zones spécifiques. Dans ce cas, une file d’attente de demandes ouverte uniquement aux utilisateurs associés à la société ou au groupe du projet limite la visibilité aux parties prenantes externes. Donner accès à tout le monde rend la demande visible pour les parties prenantes internes et externes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Nouveau : Standard </p>
   <p>Actuel : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant que la file d’attente des demandes ne soit disponible pour les personnes de la zone Demandes, vous devez créer un projet avec les paramètres suivants :

* Désignez-le comme file d’attente des demandes. Pour plus d’informations, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Mettez à jour le statut du projet sur Actif.

## Accorder l’accès à une file d’attente des demandes

1. Accédez au projet dans lequel vous souhaitez accorder l’accès aux files d’attente des demandes.

   >[!NOTE]
   >
   >Seuls les projets dont le statut est Actif sont visibles dans la zone Demandes.

1. Cliquez sur **Détails de la file d’attente** dans le panneau de gauche.
1. Sélectionnez **Publier en tant que file d’attente des demandes d’aide** pour désigner le projet comme une file d’attente des demandes.
1. Sélectionnez l’une des options suivantes qui s’affichent :

   * **N’importe qui** : tout le monde peut afficher et ajouter des demandes à la file d’attente des demandes.
   * **Personnes disposant d’un accès en affichage à ce projet** : les utilisateurs disposant d’autorisations en affichage pour le projet peuvent afficher et ajouter des demandes à la file d’attente des demandes.
   * **Personnes de l’entreprise associées à ce projet** : les utilisateurs et utilisatrices associés à l’entreprise associée au projet peuvent afficher et ajouter des demandes. La société associée au projet est indiquée entre parenthèses en regard de cette option.
   * **Personnes du groupe de ce projet** : les utilisateurs associés au groupe du projet peuvent afficher et ajouter des demandes. Le groupe associé au projet est indiqué entre parenthèses en regard de cette option.

     Les files d’attente des groupes sont utiles lorsque plusieurs départements partagent un compte Workfront pour atteindre des objectifs organisationnels uniques. Chaque ministère peut avoir ses propres files d&#39;attente que les membres d&#39;autres groupes ne devraient pas être en mesure de voir.

     Pour plus d’informations sur les autorisations d’un projet, voir [Partager un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

     Les groupes et les entreprises peuvent être associés au projet lors de sa modification. Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquer sur **Enregistrer**.
