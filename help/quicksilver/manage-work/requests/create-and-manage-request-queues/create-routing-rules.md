---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer des règles de routage
description: Les règles de routage contrôlent ce qu’Adobe Workfront fait des problèmes lorsqu’ils sont soumis à une file d’attente des demandes. Pour plus d’informations sur la création de files d’attente des demandes, voir Créer une file d’attente des demandes.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 100%

---

# Créer des règles de routage

<!-- Audited: 12/2023 -->

Les règles de routage contrôlent ce qu’Adobe Workfront fait des problèmes lorsqu’ils sont soumis à une file d’attente des demandes. Pour plus d’informations sur la création de files d’attente des demandes, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Les règles de routage envoient les problèmes aux personnes ou aux fonctions spécifiques les mieux équipées pour résoudre la demande ou le problème soumis. Les règles de routage sont généralement associées à des rubriques de file d’attente, qui sont utilisées pour contrôler la règle de routage qui sera appliquée au problème ou à la demande.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<!--drafted - replace the table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
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
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de gestion pour le projet</p> </td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une règle de routage

1. Accédez au projet dans lequel vous souhaitez ajouter les règles de routage pour vos demandes.
1. Cliquez sur Règles de routage dans le panneau de gauche. **** Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Règles de routage**.
1. Cliquez sur **Nouvelle règle de routage** pour ajouter la nouvelle règle.
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

   ![Zone Nouvelle règle de routage](assets/new-routing-rule-box.png)

1. Cliquer sur **Enregistrer**.

   Ce processus ne définit que la règle de routage. Pour garantir que le problème est acheminé lorsqu’il est soumise à la file d’attente des demandes, vous devez sélectionner la règle de routage dans l’onglet **Détails de la file d’attente** sous **Route par défaut**.

   Pour plus d’informations sur l’ajout d’une route par défaut à une file d’attente des demandes, voir [Créer une file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Si vous souhaitez associer plusieurs règles de routage à la file d’attente, vous devez créer plusieurs rubriques de file d’attente et associer chacune d’elles à une règle de routage distincte. Pour plus d’informations sur la création d’une rubrique de file d’attente, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
