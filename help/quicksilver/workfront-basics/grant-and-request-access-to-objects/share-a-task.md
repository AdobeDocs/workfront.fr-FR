---
title: Partager une tâche
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: La personne chargée de votre administration Adobe Workfront peut vous accorder l’accès en affichage ou en modification aux tâche lorsqu’elle attribue des niveaux d’accès. Pour plus d’informations sur l’octroi de l’accès aux tâches, voir Accorder un accès aux tâches.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 100%

---

# Partager une tâche

La personne chargée de votre administration Adobe Workfront peut vous accorder l’accès en affichage ou en modification aux tâche lorsqu’elle attribue des niveaux d’accès. Pour plus d’informations sur l’octroi de l’accès aux tâches, voir [Accorder un accès aux tâches](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

En plus du niveau d’accès qui est accordé aux personnes, vous pouvez leur accorder des autorisations d’affichage, de contribution ou de gestion de tâches spécifiques que vous pouvez partager.

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

## Remarques concernant le partage d’une tâche

Outre les considérations ci-dessous, voir [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Par défaut, la personne ayant créé une tâche dispose des autorisations de gestion.
* Vous pouvez partager des tâches individuellement ou partager plusieurs tâches à la fois, en masse.\
  Le partage de tâches est identique au partage d’autres objets. Pour plus d’informations sur le partage d’éléments dans Workfront, voir [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Vous pouvez accorder les autorisations suivantes sur une tâche :

   * Afficher
   * Gérer
   * Contribuer
* Lorsque vous partagez une tâche, les personnes héritent par défaut des mêmes autorisations sur tous les objets enfant associés à la tâche. Par exemple, elles héritent des mêmes autorisations sur les tâches, problèmes et documents enfant associés à la tâche.\
  Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir [Comprendre les objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  L’administrateur ou l’administratrice Workfront peut indiquer si les documents doivent hériter des autorisations des objets supérieurs dans le niveau d’accès de l’utilisateur ou de l’utilisatrice. Pour plus d’informations sur la restriction des autorisations héritées sur les documents, voir [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Vous pouvez supprimer les autorisations héritées d’une tâche.\
  Pour plus d’informations sur la suppression des autorisations héritées des objets, voir [Supprimer les autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Méthodes de partage d’une tâche

Vous pouvez partager une tâche de l’une des manières suivantes :

* Manuellement, individuellement ou en masse. Le partage manuel de tâches est similaire au partage de tout autre objet dans Workfront.

  Pour plus d’informations sur le partage d’objets dans Workfront, voir [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automatiquement, en procédant comme suit :

   * Spécifiez les autorisations sur l’un des objets parent de la tâche : projet, programme ou portfolio. Les tâches héritent des autorisations de leurs objets parent. Pour plus d’informations sur l’affichage des autorisations héritées sur les objets, voir [Afficher les autorisations héritées sur les objets](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Ajoutez des entités au partage de projet sur un modèle utilisé pour créer le projet sur lequel la tâche est effectuée. Pour plus d’informations sur le partage de projets à partir de modèles, voir [Partager un modèle](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Spécifiez les autorisations sur toutes les tâches d’un projet lorsque vous le modifiez.Pour plus d’informations sur la gestion de l’accès aux tâches du projet en fonction des autorisations d’une personne sur le projet, voir la section [](../../manage-work/projects/manage-projects/edit-projects.md#access) dans l’article [Modifier des projets](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Si vous ne spécifiez pas les autorisations de tâche que les personnes doivent posséder lorsqu’elles sont affectées aux tâches du projet, elles reçoivent par défaut les mêmes autorisations que celles dont elles disposent sur le projet.

## Autorisations sur la tâche

Le tableau suivant affiche les autorisations que vous pouvez accorder aux personnes lorsque vous leur permettez d’afficher, de contribuer ou de gérer une tâche :

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong> </th> 
   <th><strong>Gérer</strong> </th> 
   <th><strong>Contribuer</strong> </th> 
   <th><strong>Afficher</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Ajouter une ou plusieurs tâches</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter des tâches antérieures</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter un ou plusieurs problèmes</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Supprimer tâche</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Modifier la tâche générale<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier le statut de la tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier la contrainte de tâche</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Afficher tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter un ou plusieurs documents</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Copier la tâche*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Déplacer la tâche*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Consigner les heures</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier les dates prévues</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Accepter l’affectation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Créer une affectation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Joindre un formulaire personnalisé</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier les champs personnalisés</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Créer un processus d’approbation</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Approuver une tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier les finances*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter/modifier des dépenses</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Afficher Finance</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Mises à jour / commentaires</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Partager</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Partager sur le système</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Contrôlé par le niveau d’accès et les autorisations sur le projet.
