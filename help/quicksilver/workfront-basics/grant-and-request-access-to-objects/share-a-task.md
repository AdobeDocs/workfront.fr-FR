---
title: Partager une tâche
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Votre administrateur Adobe Workfront peut vous accorder l’accès aux tâches d’affichage ou de modification lorsqu’il affecte des niveaux d’accès. Pour plus d’informations sur l’octroi de l’accès aux tâches, voir Octroi de l’accès aux tâches.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 11%

---

# Partager une tâche

Votre administrateur Adobe Workfront peut vous accorder l’accès aux tâches d’affichage ou de modification lorsqu’il affecte des niveaux d’accès. Pour plus d’informations sur l’octroi de l’accès aux tâches, voir [Octroi de l’accès aux tâches](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Outre le niveau d’accès qui est accordé aux utilisateurs, vous pouvez leur accorder des autorisations pour Afficher, Contribute ou Gérer des tâches spécifiques que vous avez accès au partage.

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

## Remarques concernant le partage d’une tâche

Outre les considérations ci-dessous, reportez-vous également à la section [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Par défaut, le créateur d’une tâche dispose des autorisations Gérer .
* Vous pouvez partager des tâches individuellement ou partager plusieurs tâches à la fois, en bloc.\
  Le partage de tâches est identique au partage d&#39;autres objets. Pour plus d’informations sur le partage d’éléments dans Workfront, voir [Partage d’un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Vous pouvez accorder les autorisations suivantes à une tâche : 

   * Afficher
   * Gérer
   * Contribuer\
     ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* Lorsque vous partagez une tâche, les utilisateurs héritent par défaut des mêmes autorisations sur tous les objets enfants associés à la tâche. Par exemple, ils héritent des mêmes autorisations sur les tâches, problèmes et documents enfants associés à la tâche.\
  Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir  [Comprendre les objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  L’administrateur de Workfront peut indiquer si les documents doivent hériter des autorisations des objets de niveau supérieur au niveau d’accès de l’utilisateur. Pour plus d’informations sur la limitation des autorisations héritées sur les documents, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Vous pouvez supprimer les autorisations héritées d’une tâche.\
  Pour plus d’informations sur la suppression des autorisations héritées des objets, voir  [Supprimer des autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Méthodes de partage d’une tâche

Vous pouvez partager une tâche de la manière suivante :

* Manuellement, individuellement ou en bloc. Le partage manuel de tâches est similaire au partage de tout autre objet dans Workfront.

  Pour plus d’informations sur le partage d’objets dans Workfront, voir  [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automatiquement, en procédant comme suit :

   * Spécifiez les autorisations sur l’un des objets parents de la tâche : projet, programme ou portfolio. Les tâches héritent des autorisations de leurs objets parents. Pour plus d’informations sur l’affichage des autorisations héritées sur les objets, voir [Affichage des autorisations héritées sur les objets](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Ajoutez des entités au partage de projet sur un modèle utilisé pour créer le projet sur lequel la tâche est effectuée. Pour plus d’informations sur le partage de projets à partir de modèles, voir [Partage d’un modèle](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Spécifiez les autorisations sur toutes les tâches d’un projet lorsque vous le modifiez. Pour plus d’informations sur la gestion de l’accès aux tâches du projet en fonction des autorisations d’un utilisateur pour le projet, reportez-vous à la section [](../../manage-work/projects/manage-projects/edit-projects.md#access) de l’article [Modifier les projets](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Si vous ne spécifiez pas les autorisations de tâche que les utilisateurs doivent posséder lorsqu’ils sont affectés aux tâches du projet, ils reçoivent par défaut les mêmes autorisations que celles dont ils disposent sur le projet.

## Autorisations de tâche

Le tableau suivant affiche les autorisations que vous pouvez accorder aux utilisateurs lorsqu’ils peuvent afficher, Contribute ou gérer une tâche :

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong> </th> 
   <th><strong>Gérer</strong> </th> 
   <th><strong>Contribute</strong> </th> 
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
   <td scope="row">Ajout de prédécesseurs</td> 
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
   <td scope="row"> <p>Modification de la tâche générale<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier l’état de la tâche</td> 
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
   <td scope="row">Modifier les dates planifiées</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Assignation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Effectuer une affectation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Joindre un formulaire personnalisé</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier les champs personnalisés</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Création d’un processus d’approbation</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Approuver Une Tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier Finance*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter/Modifier des dépenses</td> 
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
   <td scope="row">Mises à jour/commentaires</td> 
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
