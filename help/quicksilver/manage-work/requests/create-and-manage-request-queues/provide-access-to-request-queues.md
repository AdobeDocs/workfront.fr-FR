---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Accéder aux files d’attente de demandes
description: Lorsque vous accordez l’accès à une file d’attente de demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente de demandes dans la zone Demandes d’Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Accéder aux files d’attente de demandes

Lorsque vous accordez l’accès à une file d’attente de demandes, vous déterminez qui, au sein de votre organisation, peut afficher la file d’attente de demandes dans la zone Demandes d’Adobe Workfront.

Vous pouvez accorder à différents utilisateurs l’accès à une file d’attente des demandes, selon qu’ils font partie de l’équipe de projet, du groupe de projets ou de la société de projets. Vous pouvez également permettre à tous les membres du système d’accéder à une file d’attente de requêtes. 

Cela s’avère utile dans les organisations qui invitent des parties prenantes externes dans Workfront et qui souhaitent limiter l’accès des utilisateurs à des zones spécifiques : dans ce cas, une file d’attente de requêtes ouverte uniquement aux utilisateurs associés à la société ou au groupe du projet limite la visibilité des parties prenantes externes. L’accès à tout le monde rend la demande visible pour les parties prenantes internes et externes.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Gestion des autorisations pour le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant que la file d’attente des demandes ne soit disponible pour les utilisateurs de la zone Demandes , vous devez créer un projet avec les paramètres suivants :

* Désignez-le comme file d’attente des demandes. Pour plus d’informations sur la création d’une file d’attente de requêtes, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Mettez à jour l’état du projet sur Actuel.

## Accéder à une file d’attente de requêtes

1. Accédez au projet dans lequel vous souhaitez accorder l’accès aux files d’attente de requête.

   >[!NOTE]
   >
   >Seuls les projets dont l’état est Actuel sont visibles dans la zone Demandes .

1. Cliquez sur **Détails de la file** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis **Détails de la file**.
1. Sélectionner **Publier en tant que file d’attente de demande d’aide** pour désigner le projet comme file d’attente des demandes.
1. Sélectionnez l’une des options suivantes :

   * **Personne**: Tout utilisateur peut afficher et ajouter des requêtes à la file d’attente des requêtes.
   * **Personnes ayant accès à ce projet**: les utilisateurs disposant des autorisations d’affichage sur le projet peuvent afficher et ajouter des requêtes à la file d’attente des demandes. 
   * **Personnes de l’entreprise de ce projet**: les utilisateurs associés à la société du projet peuvent afficher et ajouter des requêtes. La Société associée au projet est répertoriée entre parenthèses en regard de cette option. 
   * **Personnes dans le groupe de ce projet**: les utilisateurs associés au groupe du projet peuvent afficher et ajouter des requêtes. Le groupe associé au projet est répertorié entre parenthèses en regard de cette option.

      Les files d’attente de groupe sont utiles lorsque plusieurs départements partagent un compte Workfront pour atteindre des objectifs organisationnels uniques. Chaque service peut avoir ses propres files d’attente que les membres d’autres groupes ne devraient pas pouvoir voir.

      Pour plus d’informations sur les autorisations d’un projet, voir [Partage d’un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      Les groupes et les entreprises peuvent être associés au projet lors de sa modification. Pour plus d’informations sur la modification de projets, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquer sur **Enregistrer**.
