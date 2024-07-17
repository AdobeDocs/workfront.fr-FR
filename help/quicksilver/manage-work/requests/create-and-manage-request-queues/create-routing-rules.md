---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer des règles de routage
description: Les règles de routage contrôlent ce qu’Adobe Workfront fait avec les problèmes lorsqu’elles sont envoyées à une file d’attente de requêtes. Pour plus d’informations sur la création de files d’attente de requête, voir Création d’une file d’attente de requête.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 12%

---

# Créer des règles de routage

<!-- Audited: 12/2023 -->

Les règles de routage contrôlent ce qu’Adobe Workfront fait avec les problèmes lorsqu’ils sont envoyés vers une file d’attente de demandes. Pour plus d’informations sur la création de files d’attente de requête, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Les règles de routage envoient des problèmes à des utilisateurs spécifiques ou à des rôles de tâche les mieux équipés pour résoudre le problème ou la requête envoyée. Les règles de routage sont généralement associées aux rubriques de la file d’attente, qui sont utilisées pour contrôler la règle de routage qui sera appliquée au problème ou à la requête.

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

## Création d’une règle de routage

1. Accédez au projet dans lequel vous souhaitez ajouter les règles de routage pour vos requêtes.
1. Cliquez sur **Règles de routage** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Règles de routage**.
1. Cliquez sur **Nouvelle règle de routage** pour ajouter la nouvelle règle.
1. Saisissez les informations suivantes pour la règle de routage :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nom</strong> </td> 
      <td>Nom de la règle de routage. Vous pouvez voir la règle de routage si vous avez accès à ces informations sur le projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Ajoutez une description pour la règle de routage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cessionnaire par défaut*</strong> </td> 
      <td>Ajoutez un utilisateur actif ou un rôle de tâche actif auquel les nouveaux problèmes doivent être affectés. Vous ne pouvez avoir qu’une seule personne désignée par défaut dans ce champ. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Équipe par défaut*</strong> </td> 
      <td>Ajoutez une équipe active à laquelle le nouveau problème doit être affecté. Vous ne pouvez avoir qu’une seule équipe par défaut dans ce champ.

   <p><b>NOTE</b></p>

   Une fois le problème envoyé, vous pouvez modifier ses affectations et affecter d’autres utilisateurs, rôles ou équipes. Pour plus d’informations, voir <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Affecter des problèmes</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Itinéraire vers le projet</strong> </td> 
      <td>Il s’agit du projet sur lequel le problème est ajouté.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Si un utilisateur, un rôle de tâche ou une équipe sont désactivés après qu’ils ont été associés à une règle de routage, les demandes continuent à leur être acheminées. Vous devez régulièrement dresser un inventaire de toutes les règles de routage et remplacer les affectations désactivées par les affectations actives.

   Lorsque vous acheminez un problème vers un projet, les utilisateurs disposant d’autorisations sur le problème reçoivent les autorisations définies sur ce projet. Pour plus d’informations sur la définition des autorisations sur les projets, voir [Partage d’un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![Nouvelle zone de règle de routage](assets/new-routing-rule-box.png)

1. Cliquer sur **Enregistrer**.

   Ce processus définit uniquement la règle de routage. Pour vous assurer que le problème est acheminé lorsqu’il est envoyé vers la file d’attente des demandes, vous devez sélectionner la règle de routage sur l’onglet **Détails de la file d’attente** sous **Itinéraire par défaut**.

   Pour plus d’informations sur l’ajout d’un itinéraire par défaut à une file d’attente de requêtes, voir [Création d’une file d’attente de requêtes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Si vous souhaitez associer plusieurs règles de routage à la file d’attente des demandes, vous devez créer plusieurs rubriques de file d’attente et associer chacune d’elles à une règle de routage distincte. Pour plus d’informations sur la création d’une rubrique de file d’attente, voir [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
