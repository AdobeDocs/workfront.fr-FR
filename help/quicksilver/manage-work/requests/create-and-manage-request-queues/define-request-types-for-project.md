---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Définition des types de requête pour un projet
description: Vous pouvez organiser le type de problèmes ou de requêtes connectés dans Adobe Workfront par types de requêtes.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 2%

---

# Définition des types de requête pour un projet

Vous pouvez organiser le type de problèmes ou de requêtes connectés dans Adobe Workfront par types de requêtes.

Cette organisation est utile pour des raisons de création de rapports et pour aider les utilisateurs à comprendre le type de travail inattendu qui peut se produire pendant la durée de vie d’un projet.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Formule Adobe Workfront</a>*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Présentation des licences</a>*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez effectuer les opérations suivantes :

* Avoir ou créer un projet

  Pour plus d’informations sur la création de projets, voir [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md).

## Considérations sur les types de requête

* Vous pouvez spécifier le type de problèmes ou de requêtes pouvant être consignés dans un projet lorsque vous configurez la variable **Détails de la file** zone du projet.
* Vous n’avez pas besoin d’activer le projet pour qu’il devienne une file d’attente de requêtes afin de pouvoir définir des types de requêtes pour un projet. Les problèmes consignés pour un projet peuvent être étiquetés avec un type de requête différent.
* Si vous ajoutez des rubriques de file d’attente à votre projet, vous devez définir des types de requêtes sur chaque rubrique de file d’attente pour l’afficher lors de l’ajout d’un nouveau problème ou d’une nouvelle requête. Pour plus d’informations, voir [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Définition du problème ou des types de requête pour un projet

1. Cliquez sur **Projets** dans le menu principal. ![](assets/main-menu-icon.png)

1. Cliquez sur le nom du projet pour l’ouvrir.
1. Dans le panneau de gauche, cliquez sur **Détails de la file**.
1. Dans le **Propriétés de la file d’attente** , sélectionnez **Types de requête** vous voulez le projet.

   >[!NOTE]
   >
   >Vous devez avoir sélectionné au moins un type de requête. Vous pouvez sélectionner plusieurs types de requête.

   Choisissez parmi les types suivants :

   * Rapport sur les bogues
   * Modifier l&#39;ordre
   * Problème
   * Demande

   >[!TIP]
   >
   >Votre administrateur Workfront a peut-être renommé certaines de ces options. Pour plus d’informations, voir [Configuration des types de requête](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Cliquer sur **Enregistrer**.

   Les types de requêtes que vous avez spécifiés seront disponibles pour sélection lorsque vous saisissez un nouveau problème sur une tâche ou un projet, ou lorsque vous envoyez une nouvelle requête au projet, si le projet est activé en tant que file d’attente de requêtes.
