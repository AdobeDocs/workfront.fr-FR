---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Définition des types de requête pour un projet
description: Vous pouvez organiser le type de problèmes ou de requêtes connectés dans Adobe Workfront par types de requêtes.
author: Lisa
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 22%

---

# Définir les types de demandes pour un projet

Vous pouvez organiser le type de problèmes ou de requêtes connectés dans Adobe Workfront par types de requêtes.

Cette organisation est utile pour des raisons de création de rapports et pour aider les utilisateurs à comprendre le type de travail inattendu qui peut se produire pendant la durée de vie d’un projet.

## Conditions d’accès

+++

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
    <p>Nouvelle : standard</p>
    <p>ou</p>
    <p>Actuelle : formule</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez effectuer les opérations suivantes :

* Avoir ou créer un projet

  Pour plus d’informations sur la création de projets, voir [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md).

## Considérations sur les types de requête

* Vous pouvez spécifier le type de problèmes ou de requêtes pouvant être consignés dans un projet lorsque vous configurez la zone **Détails de la file d’attente** pour le projet.
* Vous n’avez pas besoin d’activer le projet pour qu’il devienne une file d’attente de requêtes afin de pouvoir définir des types de requêtes pour un projet. Les problèmes consignés pour un projet peuvent être étiquetés avec un type de requête différent.
* Si vous ajoutez des rubriques de file d’attente à votre projet, vous devez définir des types de requêtes sur chaque rubrique de file d’attente pour l’afficher lors de l’ajout d’un nouveau problème ou d’une nouvelle requête. Pour plus d’informations, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Définition du problème ou des types de requête pour un projet

{{step1-to-projects}}

1. Cliquez sur le nom du projet pour l’ouvrir.
1. Dans le panneau de gauche, cliquez sur **Détails de la file d’attente**.
1. Dans la section **Propriétés de la file d’attente**, sélectionnez les **types de requête** que vous souhaitez pour le projet.

   >[!NOTE]
   >
   >Vous devez avoir sélectionné au moins un type de requête. Vous pouvez sélectionner plusieurs types de requête.

   Choisissez parmi les types suivants :

   * Rapport sur les bogues
   * Modifier l’ordre
   * Problème
   * Demande

   >[!TIP]
   >
   >Votre administrateur Workfront a peut-être renommé certaines de ces options. Pour plus d’informations, voir [Configuration des types de requête](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Cliquer sur **Enregistrer**.

   Les types de requêtes que vous avez spécifiés seront disponibles pour sélection lorsque vous saisissez un nouveau problème sur une tâche ou un projet, ou lorsque vous envoyez une nouvelle requête au projet, si le projet est activé en tant que file d’attente de requêtes.
