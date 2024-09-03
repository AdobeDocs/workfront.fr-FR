---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Accéder aux files d’attente de demande
description: Lorsque vous accordez l’accès à une file d’attente des demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente des demandes dans la zone Demandes d’Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 99%

---

# Accorder l’accès aux files d’attente des demandes

Lorsque vous accordez l’accès à une file d’attente des demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente des demandes dans la zone Demandes d’Adobe Workfront.

Vous pouvez accorder à différentes personnes l’accès à une file d’attente des demandes, selon qu’elles font partie de l’équipe du projet, du groupe du projet ou de l’entreprise du projet. Vous pouvez également permettre à tous les membres du système d’accéder à une file d’attente des demandes. 

Cela s’avère utile dans les organisations qui invitent des parties prenantes externes dans Workfront et qui souhaitent limiter l’accès des personnes à des zones spécifiques : dans ce cas, une file d’attente des demandes ouverte uniquement aux personnes associées à l’entreprise ou au groupe du projet limite la visibilité des parties prenantes externes. Donner accès à tout le monde rend la demande visible pour les parties prenantes internes et externes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
   <p>Nouvelle licence : Standard </p>
   Ou
   <p>Licence actuelle : plan </p> </td> 
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

* Désignez-le comme file d’attente des demandes. Pour plus d’informations sur la création d’une file d’attente des demandes, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Mettez à jour le statut du projet sur Actif.

## Accorder l’accès à une file d’attente des demandes

1. Accédez au projet dans lequel vous souhaitez accorder l’accès aux files d’attente des demandes.

   >[!NOTE]
   >
   >Seuls les projets dont le statut est Actif sont visibles dans la zone Demandes.

1. Cliquez sur **Détails de la file d’attente** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Détails de la file d’attente**.
1. Sélectionnez **Publier en tant que file d’attente des demandes d’aide** pour désigner le projet comme file d’attente des demandes.
1. Sélectionnez l’une des options suivantes :

   * **N’importe qui** : tout le monde peut afficher et ajouter des demandes à la file d’attente des demandes.
   * **Personnes ayant un accès en affichage à ce projet** : les personnes disposant des autorisations d’affichage sur le projet peuvent afficher et ajouter des demandes à la file d’attente des demandes.
   * **Personnes de l’entreprise de ce projet** : les personnes associées à l’entreprise du projet peuvent afficher et ajouter des demandes. L’entreprise associée au projet est répertoriée entre parenthèses en regard de cette option.
   * **Personnes dans le groupe de ce projet** : les personnes associées au groupe du projet peuvent afficher et ajouter des demandes. Le groupe associé au projet est répertorié entre parenthèses en regard de cette option.

     Les files d’attente des groupes sont utiles lorsque plusieurs départements partagent un compte Workfront pour atteindre des objectifs organisationnels uniques. Chaque service peut avoir ses propres files d’attente que les membres d’autres groupes ne devraient pas pouvoir voir.

     Pour plus d’informations sur les autorisations d’un projet, voir [Partager un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
     Les groupes et les entreprises peuvent être associés au projet lors de sa modification. Pour plus d’informations sur la modification de projets, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquer sur **Enregistrer**.
