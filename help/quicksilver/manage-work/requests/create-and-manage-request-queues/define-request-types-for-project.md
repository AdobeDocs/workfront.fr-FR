---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Définition des types de demande pour un projet
description: Vous pouvez organiser le type de problèmes ou de demandes consignés dans Adobe Workfront par types de demandes.
author: Lisa
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 6d9583f8a0e1e0c3712c8a47d68c5d5d321679f9
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 87%

---

# Définir les types de demandes pour un projet

Vous pouvez organiser le type de problèmes ou de demandes consignés dans Adobe Workfront par types de demandes.

Cette organisation est utile pour des raisons de reporting et pour aider les utilisateurs et utilisatrices à comprendre le type de travail inattendu qui peut survenir pendant la durée de vie d’un projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
    <p>Nouveau : Standard</p>
    <p>ou</p>
    <p>Actuel : formule</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez effectuer les opérations suivantes :

* Avoir ou créer un projet

  Pour plus d’informations sur la création de projets, voir [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

## Considérations relatives aux types de demandes

* Vous pouvez spécifier le type de problèmes ou de demandes pouvant être consignés dans un projet lorsque vous configurez la zone **Détails de la file d’attente** du projet.
* Vous n’avez pas besoin d’activer le projet pour qu’il devienne une file d’attente de demandes pour pouvoir définir des types de demandes pour un projet. Les problèmes consignés pour un projet peuvent être étiquetés avec un type de demande différent.
* Si vous ajoutez des rubriques de file d’attente à votre projet, vous devez définir des types de demandes sur chaque rubrique de file d’attente pour l’afficher lors de l’ajout d’un nouveau problème ou d’une nouvelle demande. Pour plus d’informations, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Définir les types de problèmes ou de demandes pour un projet

{{step1-to-projects}}

1. Cliquez sur le nom du projet pour l’ouvrir.
1. Dans le panneau de gauche, cliquez sur **Détails de la file d’attente**.
1. Dans la section **Propriétés de file d’attente**, sélectionnez les **Types de demande** que vous voulez pour le projet.

   >[!NOTE]
   >
   >Vous devez disposer d’au moins un type de demande sélectionné. Vous pouvez sélectionner plusieurs types de demandes.

   Choisissez parmi les types suivants :

   * Rapport sur les bogues
   * Modifier l&#39;ordre
   * Problème
   * Demande

   >[!TIP]
   >
   >Votre équipe d’administration Workfront a peut-être renommé certaines de ces options. Pour plus d’informations, voir [Configurer les types de demande](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Cliquer sur **Enregistrer**.

   Les types de demandes que vous avez spécifiés pourront être sélectionnés lorsque vous conclurez un nouveau problème sur une tâche ou un projet, ou lorsque vous soumettrez une nouvelle demande au projet, si le projet est activé comme une file d&#39;attente de demandes.
