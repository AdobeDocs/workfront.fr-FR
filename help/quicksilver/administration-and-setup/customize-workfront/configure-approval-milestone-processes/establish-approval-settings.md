---
title: Configurer les paramètres de validation globale
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: En tant qu’équipe d’administration Adobe Workfront, vous pouvez déterminer les paramètres globaux des processus d’approbation dans Workfront. Ces paramètres ont un impact sur tous les processus d’approbation des éléments de travail de votre système.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: 1397702a6b50953e7abcfe491b95aeb8b981df5b
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 94%

---

# Configurer des paramètres d’approbation globaux

En tant qu’équipe d’administration Adobe Workfront, vous pouvez déterminer les paramètres globaux des processus d’approbation dans Workfront. Ces paramètres ont un impact sur tous les processus d’approbation des éléments de travail de votre système.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être administrateur ou administratrice système ou disposer d’une licence Plan avec un accès administratif aux processus d’approbation.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configurer des paramètres d’approbation globaux

{{step-1-to-setup}}

1. Cliquez sur **Processus** > **Validations**.

1. Cliquez sur l’icône **Paramètres** ![Icône des paramètres d’engrenage](assets/gear-icon-settings.png) en regard du nom de la zone **Validations**.

1. Dans la zone **Paramètres d’approbation** qui s’affiche, indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ajoutez le &lt;number&gt; de jours jusqu’à la date d’achèvement prévue pour permettre les processus d’approbation.</td> 
      <td> <p>Indiquez le nombre de minutes, heures, jours, semaines ou mois à ajouter à la date d’achèvement prévue de la tâche qui doit être approuvée. Sélectionnez les minutes, heures, jours ou semaines « écoulés » pour ajouter le temps incluant les week-ends, jours fériés et heures non travaillées qui ont été désignés dans le calendrier de travail du système.</p> 
      <p>Par exemple, si une tâche est affectée le vendredi et a une durée de 3 jours écoulés, la date d’achèvement de la tâche est définie pour le lundi (en supposant que le samedi et le dimanche soient un week-end). Si la tâche a une durée de 3 jours (non écoulés), la date d’achèvement de la tâche est définie pour le mercredi.</p>
      <p><b>NOTE</b> : l’activation de l’ajout de temps supplémentaire pour permettre l’approbation des tâches affecte le calendrier de la tâche et celui du projet.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">La personne chargée de l’approbation n’a pas besoin de faire partie de l’équipe du projet (quand un processus d’approbation comprend un rôle).</td> 
      <td> <p>Sélectionnez cette option s’il n’est pas nécessaire d’inclure un approbateur ou une approbatrice dans l’équipe du projet lorsqu’un processus d’approbation comprend un rôle. Tout utilisateur disposant de cette fonction reçoit la demande d’approbation, qu’il fasse partie ou non de l’équipe du projet, bien que l’accès au projet ne lui soit pas automatiquement accordé. Pour plus d’informations sur la modification du rôle de projet d’un utilisateur ou d’une utilisatrice, voir <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gérer l’équipe de projet</a>. </p> 
      <p><b>CONSEIL</b> : lorsque vous affectez une approbation à un rôle et que l’option <b>La personne chargée de l’approbation n’a pas besoin de faire partie de l’équipe du projet (quand un processus d’approbation comprend un rôle)</b> est désactivée, mais qu’aucun rôle de l’équipe de projet ne correspond au rôle de l’approbation, l’approbation est réattribuée à la personne propriétaire du projet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactiver la délégation d'approbation</td> 
      <td> <p>Sélectionnez cette option pour désactiver la fonctionnalité permettant aux utilisateurs et utilisatrices de votre système de déléguer les approbations à d’autres personnes. Lorsque cette option est sélectionnée, l’option permettant de déléguer les approbations est supprimée de Workfront et toutes les délégations d’approbation existantes sont interrompues.</p> <p>Pour plus d’informations sur la délégation des approbations dans Workfront, voir <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Déléguer une demande d’approbation</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser la modification du formulaire personnalisé lorsque le projet, la tâche ou le problème a le statut Approbation en attente</td> 
      <td> <p>Sélectionnez cette option pour permettre aux utilisateurs et utilisatrices de modifier le formulaire personnalisé de projets, de tâches et de problèmes lorsqu’ils ont le statut Appobation en attente. Il s’agit du paramètre par défaut.</p> 
      <p>Lorsque cette option est sélectionnée :</p> 
       <ul> 
       <li>Tous les approbateurs et approbatrices (et toutes les autres personnes ayant accès à la modification du formulaire personnalisé) peuvent apporter des modifications au formulaire personnalisé lorsque l’objet est en attente d’approbation, quel que soit le chemin ou l’étape d’approbation actuels.</li> 
       <li>Les modifications apportées au formulaire personnalisé au cours d’un processus d’approbation n’ont aucune incidence sur les décisions d’approbation prises avant la modification.</li> 
       <li> <p>Toutes les modifications apportées au projet, à la tâche ou au problème sont suivies de la même manière, quel que soit ce paramètre. </p> <p>Par exemple, si vous avez ajouté des champs de formulaire personnalisés à suivre dans le flux de mise à jour, toutes les modifications apportées au formulaire sont suivies dans le flux de mise à jour de l’objet.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser les utilisateurs à rappeler les demandes récemment créées en attente d'approbation</td> 
      <td> <p>Sélectionnez cette option pour configurer si les utilisateurs et utilisatrices peuvent rappeler un problème ou une demande en attente d’approbation pour leur premier statut. Vous pouvez associer le premier statut d’un problème ou d’une demande à un processus d’approbation en configurant les files d’attente de demandes. </p> 
      <p>Pour plus d’informations sur les files d’attente des demandes, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente des demandes</a>.</p> 
      <p>Utilisez l’une des méthodes suivantes :</p> 
       <ul> 
       <li>Sélectionnez cette option pour permettre aux personnes de rappeler une approbation pour le premier statut d’un problème ou d’une demande. Dans ce cas, ces personnes peuvent voir un bouton Rappeler&lt; sur un nouveau problème ou une nouvelle demande en attente d’approbation. Lorsqu’elles choisissent de rappeler le problème, elles reçoivent un avertissement indiquant que le problème sera également supprimé. Le problème est supprimé après qu’elles aient confirmé qu’elles le rappelaient. </li> 
       <li> <p>Désélectionnez cette option pour empêcher les personnes de rappeler un problème ou une demande dont le premier statut est en attente d’approbation. Elles ne peuvent pas voir de bouton Rappeler&lt; sur le nouveau problème ou la nouvelle demande et l’approbation doit être accordée. Il s’agit de l’option par défaut.</p> 
       <p>Pour plus d’informations sur la révision des éléments en attente d’approbation, voir <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Afficher les approbations </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer les modifications**.
