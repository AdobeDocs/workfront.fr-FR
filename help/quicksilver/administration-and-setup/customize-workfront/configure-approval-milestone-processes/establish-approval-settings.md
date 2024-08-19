---
title: Configuration des paramètres d’approbation globaux
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: En tant qu’administrateur Adobe Workfront, vous pouvez déterminer les paramètres globaux des processus d’approbation dans Workfront. Ces paramètres ont un impact sur tous les processus d’approbation des tâches de votre système.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 17%

---

# Configuration des paramètres d’approbation globaux

En tant qu’administrateur Adobe Workfront, vous pouvez déterminer les paramètres globaux des processus d’approbation dans Workfront. Ces paramètres ont un impact sur tous les processus d’approbation des tâches de votre système.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur système ou disposer d’une licence Plan avec un accès administratif aux processus d’approbation.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configuration des paramètres d’approbation globaux

{{step-1-to-setup}}

1. Cliquez sur **Traitements** > **Validations**.

1. Cliquez sur l’icône **Paramètres** ![](assets/gear-icon-settings.png) en regard du nom de la zone **Approbations** .

1. Dans la zone **Approval Settings** (Paramètres d’approbation) qui s’affiche, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ajoutez &lt;nombre&gt; jours à la date d’achèvement prévue pour s’adapter aux processus d’approbation.</td> 
      <td> <p>Spécifiez le nombre de minutes, heures, jours, semaines ou mois à ajouter à la date d’achèvement prévue de la tâche qui doit être approuvée. Sélectionnez l’option "Temps écoulé" (minutes, heures, jours ou semaines) pour ajouter une heure incluant les week-ends, jours fériés et heures non travaillées qui ont été désignés dans le calendrier de travail du système.</p> 
      <p>Par exemple, si une tâche est affectée le vendredi et a une durée de 3 jours écoulés, la date d’achèvement de la tâche est définie pour le lundi (en supposant que le samedi et le dimanche soient un week-end). Si la tâche a une durée de 3 jours (non écoulés), la date d’achèvement de la tâche est définie pour le mercredi.</p>
      <p><b>REMARQUE</b> : l’activation de l’ajout de temps supplémentaire pour s’adapter à l’approbation des tâches affecte le calendrier de la tâche et celui du projet.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">L’approbateur ne doit pas appartenir à l’équipe du projet (pour les processus d’approbation qui incluent un rôle).</td> 
      <td> <p>Sélectionnez cette option si aucun approbateur n’est nécessaire pour faire partie de l’équipe du projet lorsqu’un processus d’approbation inclut un rôle. Lorsque vous attribuez la décision d’approbation à un rôle de tâche, seuls les utilisateurs auxquels un rôle est associé dans le projet voient l’approbation. Si vous activez ce paramètre, tout utilisateur disposant de ce rôle de tâche reçoit la demande d’approbation, qu’il fasse ou non partie de l’équipe de projet. Pour plus d’informations sur la modification du rôle de projet d’un utilisateur, voir <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gérer l’équipe de projet</a>. </p> 
      <p><b>TIP</b> : lorsque vous affectez une approbation à un rôle et que l’option <b>Approbateur non requis pour faire partie de l’équipe de projet (pour les processus d’approbation qui incluent un rôle)</b> est désactivée, mais qu’aucun rôle ne correspond au rôle sur l’approbation, l’approbation est réaffectée au propriétaire du projet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactiver la délégation d'approbation</td> 
      <td> <p>Sélectionnez cette option pour désactiver la fonctionnalité permettant aux utilisateurs de votre système de déléguer les approbations à un autre utilisateur. Lorsque cette option est sélectionnée, l’option permettant de déléguer les approbations est supprimée de Workfront et toutes les délégations d’approbation existantes sont arrêtées.</p> <p>Pour plus d’informations sur la délégation des approbations dans Workfront, voir <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Déléguer la demande d’approbation</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser la modification du formulaire personnalisé lorsque le projet, la tâche ou le problème est à l’état d’approbation en attente</td> 
      <td> <p>Sélectionnez cette option pour permettre aux utilisateurs de modifier le formulaire personnalisé de projets, de tâches et de problèmes lorsqu’ils se trouvent dans l’état Autorisation en attente . Il s’agit du paramètre par défaut.</p> 
      <p>Lorsque cette option est sélectionnée :</p> 
       <ul> 
       <li>Tous les approbateurs (et tous les autres utilisateurs ayant accès à la modification du formulaire personnalisé) peuvent apporter des modifications au formulaire personnalisé lorsque l’objet est en attente d’approbation, quel que soit le chemin d’approbation actuel ou l’étape d’approbation.</li> 
       <li>Les modifications apportées au formulaire personnalisé au cours d’un processus d’approbation n’ont aucune incidence sur les décisions d’approbation prises avant la modification.</li> 
       <li> <p>Toutes les modifications apportées au projet, à la tâche ou au problème sont suivies de la même manière, quel que soit ce paramètre. </p> <p>Par exemple, si vous avez ajouté des champs de formulaire personnalisés à suivre dans le flux de mise à jour, toutes les modifications apportées au formulaire sont suivies dans le flux de mise à jour de l’objet.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser les utilisateurs à rappeler les demandes récemment créées en attente d'approbation</td> 
      <td> <p>Sélectionnez cette option pour configurer si les utilisateurs peuvent rappeler un problème ou une demande en attente d’approbation pour leur premier état. Vous pouvez associer le premier état d’un problème ou d’une demande à un processus d’approbation en configurant les files d’attente de demandes. </p> 
      <p>Pour plus d’informations sur les files d’attente de requête, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requête</a>.</p> 
      <p>Utilisez l’une des méthodes suivantes :</p> 
       <ul> 
       <li>Sélectionnez cette option pour permettre aux utilisateurs de rappeler une approbation pour le premier état d’un problème ou d’une demande. Dans ce cas, il peut voir un bouton Rappeler&lt; sur un nouveau problème ou une demande en attente d’approbation. Lorsqu’ils choisissent de rappeler le problème, ils reçoivent un avertissement indiquant que le problème sera également supprimé. Le problème est supprimé après qu'ils aient confirmé qu'ils le rappelaient. </li> 
       <li> <p>Désélectionnez cette option pour empêcher les utilisateurs de rappeler un problème ou une demande dont le premier état est en attente d’approbation. Ils ne peuvent pas voir de bouton Rappel&lt; sur le nouveau problème ou la nouvelle demande et la validation doit être accordée. Il s’agit de l’option par défaut.</p> 
       <p>Pour plus d’informations sur la révision des éléments en attente d’approbation, voir <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Affichage des approbations </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer les modifications.**
