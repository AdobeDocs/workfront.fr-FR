---
product-area: projects
navigation-topic: manage-issues
title: Mettre automatiquement à jour les statuts des événements de En attente de commentaires à En cours
description: Lorsque le contact principal d’un problème effectue une mise à jour du problème en mettant à jour un champ (y compris un champ personnalisé) ou en ajoutant un commentaire, le statut du problème est automatiquement mis à jour vers En cours.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
TQID: https://experienceleague.adobe.com/axgDUT8M6p79omHTSO8OrvM7qAM81AjG0Fug2JUl4ck
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 76%

---

# Mettre à jour automatiquement les statuts des problèmes de Commentaires en attente à En cours.

<!--Audited: 109/2025-->

Lorsque le contact principal d’un problème effectue une mise à jour du problème en mettant à jour un champ (y compris un champ personnalisé) ou en ajoutant un commentaire, le statut du problème est automatiquement mis à jour vers En cours.

Pour que ce changement d’état automatique se produise, les éléments suivants sont requis :

* Le problème doit être ajouté à l’aide d’une file d’attente de demandes.

  Pour plus d’informations sur la création de files d’attente des demandes, consultez la section [Créer et gérer des files d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md).

  Pour plus d’informations sur l’envoi de demandes à une file d’attente des demandes, voir [Création et envoi de demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Les détails de la file d’attente des demandes doivent avoir les paramètres suivants :
   * **Lorsqu’une personne émet une demande, il lui est automatiquement accordé** un **Accès en contribution**
   * **Modifier le statut** est sélectionné

  ![Les détails de la file d’attente accordent un accès en contribution et Modifier le statut est sélectionné.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Lors de la configuration d’une file d’attente de demandes, vous pouvez définir l’accès des contacts principaux aux problèmes qu’ils envoient.
  >
  >Lorsque vous désélectionnez le paramètre Modifier le statut lorsque vous configurez la file d’attente des demandes, gardez à l’esprit que les administrateurs et les administratrices système disposent toujours de l’accès leur permettant de modifier le statut des problèmes, même si l’option Modifier le statut est désélectionnée dans les paramètres de la file d’attente des demandes.

  Pour plus d’informations sur les détails de la file d’attente, consultez [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Le problème doit avoir le statut En attente de feedback.
* Un statut En attente de feedback doit être disponible pour les problèmes au niveau du système.

  Pour plus d’informations sur les statuts au niveau du système, voir [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
