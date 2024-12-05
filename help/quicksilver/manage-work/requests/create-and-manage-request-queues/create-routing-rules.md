---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer des règles de routage
description: Les règles de routage contrôlent ce qu’Adobe Workfront fait avec les problèmes lorsqu’elles sont envoyées à une file d’attente de requêtes.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 8ec279ece400c10a37e67664b77b1e0df6639724
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 90%

---

# Créer des règles de routage

<!-- Audited: 12/2023 -->

Les règles de routage contrôlent ce qu’Adobe Workfront fait des problèmes lorsqu’ils sont soumis à une file d’attente des demandes. Pour plus d’informations sur la création de files d’attente des demandes, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Les règles de routage envoient les problèmes aux personnes ou aux fonctions spécifiques les mieux équipées pour résoudre le problème ou la demande soumis. Les règles de routage sont généralement associées à des rubriques de file d’attente, qui sont utilisées pour contrôler la règle de routage qui sera appliquée au problème ou à la demande.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Formule Adobe Workfront</p></td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle licence : Standard </p> 
   Ou
   <p>Licence actuelle : plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une règle de routage

1. Accédez au projet dans lequel vous souhaitez ajouter des règles de routage pour vos requêtes.
1. Cliquez sur **Règles de routage** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Règles de routage**.
1. Cliquez sur **Nouvelle règle de routage** pour ajouter la nouvelle règle. La zone **Nouvelle règle de routage** s’ouvre.

   ![Zone Nouvelle règle de routage](assets/new-routing-rule-box.png)
1. Saisissez les informations suivantes pour la règle de routage :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nom</strong> </td> 
      <td>Le nom de la règle de routage. Vous pouvez voir la règle de routage si vous avez accès à cette information sur le projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Ajoutez une description pour la règle de routage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cessionnaire par défaut*</strong> </td> 
      <td>Ajoutez une personne active ou une fonction active à qui les nouveaux problèmes doivent être attribués. Ce champ ne peut contenir qu’une seule personne cessionnaire par défaut. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Équipe par défaut*</strong> </td> 
      <td>Ajouter une équipe active à laquelle le nouveau problème doit être attribué. Ce champ ne peut contenir qu’une seule équipe par défaut.

   <p><b>NOTE</b></p>

   Une fois le problème soumis, vous pouvez modifier ses affectations et affecter d’autres personnes, fonctions ou équipes. Pour plus d’informations, voir <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Attribuer des problèmes</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Transmettre au projet</strong> </td> 
      <td>Il s’agit du projet dans lequel le problème est ajouté.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Si une personne, une fonction ou une équipe est désactivée après avoir été associée à une règle de routage, les demandes continuent de lui être transmises. Vous devez périodiquement faire l’inventaire de toutes les règles de routage et remplacer les affectations désactivées par des affectations actives.

   Lorsque vous transmettez un problème vers un projet, les personnes ayant des autorisations sur le problème reçoivent les autorisations définies pour ce projet. Pour plus d’informations sur la définition des autorisations sur les projets, voir [Partager un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

1. Cliquer sur **Enregistrer**.

   Ce processus ne définit que la règle de routage. Pour garantir que le problème est acheminé lorsqu’il est soumise à la file d’attente, vous devez sélectionner la règle de transmission dans l’onglet **Détails de la file d’attente** sous **Route par défaut**.

   Pour plus d’informations sur l’ajout d’une route par défaut à une file d’attente, voir [Créer une file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Si vous souhaitez associer plusieurs règles de transmission à la file d’attente, vous devez créer plusieurs rubriques de file d’attente et associer chacune d’elles à une règle de transmission distincte. Pour plus d’informations sur la création d’une rubrique de file d’attente, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
