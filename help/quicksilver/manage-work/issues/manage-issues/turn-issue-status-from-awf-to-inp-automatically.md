---
product-area: projects
navigation-topic: manage-issues
title: Mettre à jour automatiquement les statuts des problèmes de Commentaires en attente à En cours.
description: Lorsque le contact par Principal d’un problème effectue une mise à jour du problème en mettant à jour un champ (y compris un champ personnalisé) ou en ajoutant un commentaire, l’état du problème est automatiquement mis à jour vers En cours .
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 7%

---

# Mettre à jour automatiquement les statuts des problèmes de Commentaires en attente à En cours.

Lorsque le contact par Principal d’un problème effectue une mise à jour du problème en mettant à jour un champ (y compris un champ personnalisé) ou en ajoutant un commentaire, l’état du problème est automatiquement mis à jour vers En cours .

Pour que ce changement d’état automatique se produise, les éléments suivants sont requis :

* Le problème doit être saisi par le biais d’une file d’attente de requêtes.

  Pour plus d’informations sur la création de files d’attente de requêtes, voir la section [Créer et gérer des files d’attente de requêtes](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) . Pour plus d’informations sur la création de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Les détails de la file d’attente dans la file d’attente des demandes doivent avoir les paramètres suivants :
   * **Lorsqu’une personne fait une demande, l’attribution automatique** est définie sur **Accès Contribute**
   * **Modifier l’état** est sélectionné sous Paramètres avancés

  ![ Les détails de la file d’attente donnent accès à Contribute et l’état de modification est sélectionné.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Lors de la configuration d’une file d’attente de demandes, vous pouvez définir l’accès des contacts principaux aux problèmes qu’ils envoient.
  >
  >Lorsque vous désélectionnez le paramètre Modifier l’état lors de la configuration de la file d’attente des demandes, n’oubliez pas que les administrateurs système ont toujours accès à la modification de l’état des problèmes, même si l’option Modifier l’état est désélectionnée dans les paramètres de la file d’attente des demandes.

  Pour plus d’informations sur les détails de la file d’attente, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Le problème doit se trouver dans l’état Commentaires en attente .
* Un état Await Feedback (AWF) doit être disponible pour les problèmes au niveau du système.

  Pour plus d’informations sur les états au niveau du système, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
