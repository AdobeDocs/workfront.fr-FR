---
product-area: projects
navigation-topic: manage-issues
title: Mettre automatiquement à jour les états des problèmes depuis l’état En attente de retour vers En cours
description: Lorsque le contact Principal d’un problème effectue une mise à jour du problème en mettant à jour un champ (y compris un champ personnalisé) ou en ajoutant un commentaire, l’état du problème est automatiquement mis à jour vers En cours .
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Mettre automatiquement à jour les états des problèmes depuis l’état En attente de retour vers En cours

Lorsque le contact Principal d’un problème effectue une mise à jour du problème en mettant à jour un champ (y compris un champ personnalisé) ou en ajoutant un commentaire, l’état du problème est automatiquement mis à jour vers En cours .

Pour que ce changement d’état automatique se produise, les éléments suivants sont requis :

* Le problème doit être saisi via une file d’attente de requêtes.

   Pour plus d’informations sur la création de files d’attente, voir la section [Création et gestion des files d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) . Pour plus d’informations sur la création de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Les détails de la file d’attente dans la file d’attente des demandes doivent avoir les paramètres suivants :
   * **Lorsqu’une personne émet une demande, elle accorde automatiquement** est défini sur **Accès aux contributions**
   * **Modifier l’état** est sélectionné sous Paramètres avancés.

   ![Détails de la file d’attente : attribuez l’accès au contributeur et l’état de modification est sélectionné.](assets/queuedetails-contributeaccess-changestatus.png)

   Pour plus d’informations sur les détails de la file d’attente, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Le problème doit se trouver dans l’état Commentaires en attente .
* Un état Await Feedback (AWF) doit être disponible pour les problèmes au niveau du système.

   Pour plus d’informations sur les états au niveau du système, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
