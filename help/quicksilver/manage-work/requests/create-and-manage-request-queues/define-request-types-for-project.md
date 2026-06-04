---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Définition des types de demande pour un projet
description: Vous pouvez organiser le type de problèmes ou de demandes consignés dans Adobe Workfront par types de demandes.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 64%

---

# Définir les types de demandes pour un projet

<!-- Audited: 6/2025 -->

Vous pouvez organiser le type de problèmes ou de demandes consignés dans Adobe Workfront par types de demandes. Cela s’avère utile pour signaler des raisons et aider les utilisateurs et les utilisatrices à comprendre le type de travail inattendu qui peut se produire au cours du cycle de vie d’un projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
    <p>Standard</p>
    <p>Plan</p></td>  
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

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez effectuer les opérations suivantes :

* posséder ou créer un projet ;

  Pour plus d’informations sur la création de projets, voir [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

## Considérations relatives aux types de demandes

* Vous pouvez spécifier le type d’événements ou de demandes qui peuvent être consignés dans un projet lorsque vous configurez la zone Détails de la file d’attente pour le projet.
* Vous n’avez pas besoin d’activer le projet pour qu’il devienne une file d’attente de demandes pour pouvoir définir des types de demandes pour un projet. Les problèmes consignés pour un projet peuvent être étiquetés avec un type de demande différent.
* Si vous ajoutez des rubriques de file d’attente à votre projet, vous devez définir des types de demandes sur chaque rubrique de file d’attente pour l’afficher lors de l’ajout d’un nouveau problème ou d’une nouvelle demande. Pour plus d’informations, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Définir les types de problèmes ou de demandes pour un projet

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Dans le panneau de gauche, cliquez sur **Détails de la file d’attente**.
1. Dans la section **Propriétés de la file d’attente**, sélectionnez les **Types de demande** souhaités pour le projet :
   * Rapport sur les bogues
   * Modifier l&#39;ordre
   * Problème
   * Demande

   >[!NOTE]
   >
   >* Vous devez disposer d’au moins un type de demande sélectionné. Vous pouvez sélectionner plusieurs types.
   >* Votre équipe d’administration Workfront a peut-être renommé certaines de ces options. Pour plus d’informations, voir [Configurer les types de demande](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Cliquer sur **Enregistrer**. Les types de demande que vous avez spécifiés seront disponibles pour sélection lorsque vous entrez un nouveau problème sur une tâche ou un projet, ou lorsque vous soumettez une nouvelle demande au projet (si le projet est activé comme une file d&#39;attente de demandes).
