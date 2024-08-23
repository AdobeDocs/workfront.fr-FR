---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Accéder aux files d’attente de demande
description: Lorsque vous accordez l’accès à une file d’attente de demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente de demandes dans la zone Demandes d’Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 15%

---

# Fournir un accès aux files d’attente des demandes

Lorsque vous accordez l’accès à une file d’attente de demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente de demandes dans la zone Demandes d’Adobe Workfront.

Vous pouvez accorder à différents utilisateurs l’accès à une file d’attente des demandes, selon qu’ils font partie de l’équipe de projet, du groupe de projets ou de la société de projets. Vous pouvez également permettre à tous les membres du système d’accéder à une file d’attente de requêtes. 

Cela s’avère utile dans les organisations qui invitent des parties prenantes externes dans Workfront et qui souhaitent limiter l’accès des utilisateurs à des zones spécifiques : dans ce cas, une file d’attente de requêtes ouverte uniquement aux utilisateurs associés à la société ou au groupe du projet limite la visibilité des parties prenantes externes. L’accès à tout le monde rend la demande visible pour les parties prenantes internes et externes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Nouvelle licence : standard </p>
   Ou
   <p>Licence actuelle : plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant que la file d’attente des demandes ne soit disponible pour les utilisateurs de la zone Demandes , vous devez créer un projet avec les paramètres suivants :

* Désignez-le comme file d’attente des demandes. Pour plus d’informations sur la création d’une file d’attente de requêtes, voir [Création d’une file d’attente de requêtes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Mettez à jour l’état du projet sur Actuel.

## Accéder à une file d’attente de requêtes

1. Accédez au projet dans lequel vous souhaitez accorder l’accès aux files d’attente de requête.

   >[!NOTE]
   >
   >Seuls les projets dont l’état est Actuel sont visibles dans la zone Demandes .

1. Cliquez sur **Détails de la file d’attente** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Détails de la file d’attente**.
1. Sélectionnez **Publish comme file d’attente de demande d’aide** pour désigner le projet comme file d’attente de demande.
1. Sélectionnez l’une des options suivantes :

   * **N’importe qui** : n’importe quel utilisateur peut afficher et ajouter des requêtes à la file d’attente des demandes.
   * **Personnes ayant accès aux vues de ce projet** : les utilisateurs disposant d’autorisations d’affichage sur le projet peuvent afficher et ajouter des requêtes à la file d’attente des demandes. 
   * **Personnes dans la société de ce projet** : les utilisateurs associés à la société du projet peuvent afficher et ajouter des requêtes. La Société associée au projet est répertoriée entre parenthèses en regard de cette option. 
   * **Personnes du groupe de ce projet** : les utilisateurs associés au groupe du projet peuvent afficher et ajouter des requêtes. Le groupe associé au projet est répertorié entre parenthèses en regard de cette option.

     Les files d’attente de groupe sont utiles lorsque plusieurs départements partagent un compte Workfront pour atteindre des objectifs organisationnels uniques. Chaque service peut avoir ses propres files d’attente que les membres d’autres groupes ne devraient pas pouvoir voir.

     Pour plus d’informations sur qui dispose d’autorisations sur un projet, voir [Partage d’un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
     Les groupes et les entreprises peuvent être associés au projet lors de sa modification. Pour plus d’informations sur la modification de projets, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquer sur **Enregistrer**.
