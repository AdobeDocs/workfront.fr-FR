---
content-type: reference
navigation-topic: notifications
title: 'Notifications : Informations sur le travail qui m’a été affecté'
description: Les notifications suivantes vous alertent sur les activités qui se produisent sur un élément de travail qui vous est affecté.
author: Courtney
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 100%

---

# Notifications : Informations sur le travail qui m’a été affecté

Les notifications suivantes vous alertent sur les activités qui se produisent sur un élément de travail qui vous est affecté.

Pour plus d’informations sur la configuration des notifications que vous recevez, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consultez également la section [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>Champs inclus </p> <p> * Champs de résumé quotidien uniquement</p> </th> 
   <th>Statut par défaut</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Une tâche antérieure d’une tâche affectée à mon équipe est terminée.</strong> </p> <p>L’équipe affectée reçoit une notification par e-mail lorsqu’une tâche antérieure de l’une de ses tâches est terminé. </p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Terminé : &lt;Task Name&gt;</em>.</p> <p> L’objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> <p>Nom de la tâche antérieure<br>Projet de tâche antérieure<br>Numéro de référence de la tâche antérieure<br>Nom de la personne qui a terminé la tâche antérieure<br>Statut de la tâche antérieure<br>Date et heure auxquelles la tâche antérieure a été terminée<br>Statut précédent de la tâche antérieure<br><strong>Bouton Plus de détails</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches antérieures terminées<br>* Nom de la tâche<br>* Nom de la personne qui a terminé la tâche<br>* Date de la synthèse quotidienne </p> </td> 
   <td><strong>Chaque jour</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Lorsqu'une tâche est terminée, envoyer un e-mail aux cessionnaires principaux de toute les tâches dépendantes</strong> </p> <p>La personne désignée pour la tâche reçoit une notification par e-mail lorsqu’une tâche antérieure de l’une de ses tâches est terminé. </p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;Task Name&gt;</em>.</p> <p> L’objet de la notificationde la synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> <p>Nom de la tâche antérieure<br>Projet de tâche antérieure<br>Numéro de référence de la tâche antérieure<br>Nom dela personne qui a terminé la tâche antérieure<br>Statut de la tâche antérieure<br>Date et heure auxquelles la tâche antérieure a été terminée<br>Statut précédent de la tâche antérieure<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches antérieures terminées<br>* Nom de la tâche<br>* Nom de la personne qui a terminé la tâche<br>* Date de la synthèse quotidienne </p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>Lorsqu’une tâche d’approbation est approuvée ou rejetée, envoyer un e-mail à la personne cessionnaire</strong> </p> <p>La personne cessionnaire pour la tâche reçoit une notification par e-mail lorsque la tâche est approuvée ou refusée.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;Task Name&gt; de &lt;Project Name&gt;</em>.</p> <p> L’objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de la personne qui a accordé la validation<br>Nouveau statut de la tâche<br>Date et heure auxquelles la tâche a été approuvée ou refusée<br>Statut de la tâche précédente<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches approuvées ou refusées<br>* Nom de la tâche<br>* Nom de la personne qui a approuvé ou refusé la tâche<br>* Décision d’approbation ([!UICONTROL Approved]/[!UICONTROL Rejected])<br>* Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Une tâche qui m’a été affectée est terminée</strong> </p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail une fois la tâche terminée.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L‘objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;Task Name&gt; de &lt;Project name&gt;</em>.</p> <p> <p>Remarque : si la tâche est modifiée et passe à l’équivalent du statut [!UICONTROL Complete], l’objet de l’e-mail affiché reste « Terminé ».</p> </p> <p> L‘objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de la personne qui a terminé la tâche<br>Date et heure auxquelles la tâche a été terminée<br>Statut de la tâche précédente<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches terminées<br>* Nom de la tâche<br>* Nom de la personne qui a terminé la tâche<br>* Date de la synthèse quotidienne<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Toutes les tâches antérieures d’une tâche affectée à mon équipe sont terminées</strong> </p> <p>L’équipe affectée reçoit une notification par e-mail lorsqu’une tâche antérieure de l’une de ses tâches est marquée comme terminée.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence Réviseur ou Demandeur ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Tâche terminée : &lt;Name&gt;</em>.</p> <p> L’objet de la notification de la synthèse quotidienne est : <em> Résumé du travail qui vous a été affecté &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom de la tâche<br>Projet de tâche<br>Numéro de référence de tâche<br>Nom de la personne qui a terminé la tâche antérieure<br>Statut de la tâche antérieure<br>Date et heure auxquelles la tâche antérieure a été terminée<br>Statut précédent de la tâche antérieure<br><strong>Bouton Plus de détails</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches terminées<br>* Nom de la tâche<br>* Nom de la personne qui a terminé la tâche<br>* Date de la synthèse quotidienne </td>
   <td><strong>Instantané</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Toutes les tâches antérieures de mes tâches sont terminées</strong> </p> <p>La personne à qui la tâche a été affectée reçoit une notification par e-mail pour chaque tâche antérieure qui est terminée.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;Task Name&gt;</em><br>.</p> <p> L’objet de la notification de synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom de la tâche<br>Projet de tâche<br>Numéro de référence de tâche<br>Nom de la personne qui a terminé la tâche antérieure<br>Statut de la tâche antérieure<br>Date et heure auxquelles la tâche antérieure a été terminée<br>Statut précédent de la tâche antérieure<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches terminées<br>* Nom de la tâche<br>* Nom de la personne qui a terminé la tâche<br>* Date de la synthèse quotidienne </td> 
   <td><strong>Instantané</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Lorsqu’un événement est approuvé ou rejeté, envoyer un e-mail à la personne cessionnaire</strong> </p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsqu’une décision d’approbation est prise (approuvée ou rejetée).</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Problème en attente d’approbation : &lt;Planned Start Date&gt; &lt;Issue Reference Number&gt; - &lt;Issue Name&gt; de &lt;Project Name&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est : <em> Résumé du travail qui vous a été affecté &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la personne qui a approuvé ou rejeté le problème<br>Décision d’approbation (approuvée ou rejetée)<br>Statut du problème<br>Nom de la personne qui a demandé l’approbation<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de problèmes approuvés ou rejetés<br>* Nom du problème<br>* Nom de la personne qui a approuvé ou rejeté le problème<br>* Décision d’approbation (approuvée ou rejetée)<br>* Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Lorsqu’un événement est conclu, envoyer e-mail à la personne cessionnaire</strong> </p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Terminé : &lt;Issue Name&gt; de &lt;Project Name&gt;</em>.</p> <p><em> L’objet de la notification de synthèse quotidienne est : Résumé du travail qui vous a été affecté &lt;Date of daily digest&gt; </em>. </p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la personne ayant terminé le problème<br>Nouveau statut du problème<br>Date et heure auxquelles le problème a été terminé<br>Statut de la tâche précédente<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de problèmes terminés<br>* Nom du problème<br>* Nom de la personne ayant terminé le problème<br>* Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Les documents sont chargés ou modifiés à ma demande</strong> </p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsque des documents sont chargés ou que les détails du document sont modifiés sur un problème qu’elle a ajouté.</p> <p>Une notification par e-mail n’est pas envoyée si la personne qui a déclenché le problème est la personne cessionnaire du problème.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] et si le projet est configuré comme une file d’attente des demandes d’aide (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente des demandes</a>).</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Document added to] &lt;Request Name&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> <p>Nom de la demande<br>Nom du projet (nom de la file d’attente des demandes)<br>Numéro de référence du document<br>Nom de la personne qui a chargé le document<br>Nom du document<br>Ajouté le<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Preview]</strong> et <strong>[!UICONTROL Download]</strong> boutons<br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de documents chargés ou modifiés<br>* Nom du document<br>* Nom de l’objet<br>* Nom de la personne qui a chargé le document<br>* Date de la synthèse quotidienne</p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date d’échéance d’une tâche qui m’a été affectée est modifiée</strong> </p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque la [!UICONTROL Planned Completion Date] de la tâche est modifiée, sauf si l’utilisateur ou l’utilisatrice qui a modifié la date d’achèvement prévue est également la personne cessionnaire de la tâche.</p> <p>Une notification est envoyée uniquement si le statut du projet est autre que [!UICONTROL Planning].</p> <p>Aucune notification n’est envoyée concernant les tâches personnelles.</p> <p> Les utilisateurs et utilisatrices disposant d’une licence Réviseur ou Demandeur ne reçoivent pas de notification. </p> <p> L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Due Date has been changed.]</em>.</p> <p> L’objet de la notification de synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de tâche<br>Nouvelle date d’échéance ([!UICONTROL Planned Completion Date])<br>Date et heure de la modification de la date d’échéance<br>Nom de la personne qui a modifié la date d’échéance<br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches pour lesquelles la date d’échéance (date d’achèvement prévue) a été modifiée<br>* Nom de la tâche<br>* Nouvelle date d’achèvement prévue<br>* Nom de la personne qui a modifié la date d’échéance<br>* Date de la synthèse quotidienne </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date d’échéance d’une tâche qui m’a été affectée est modifiée</strong> </p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsque la [!UICONTROL Planned Completion Date] est modifiée, sauf si l’utilisateur ou l’utilisatrice qui a modifié la [!UICONTROL Planned Completion Date] est également la personne cessionnaire.</p> <p>Une notification est envoyée uniquement si le statut du projet est autre que [!UICONTROL Planning].</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Due Date has been changed]</em>.</p> <p> </p> <p> L’objet de la notification de synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt;</em>.</p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nouvelle date d’échéance ([!UICONTROL Planned Completion Date])<br>Date et heure de la modification de la date d’échéance<br>Nom de la personne qui a modifié la date d’échéance<br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de problèmes où la date d’échéance ([!UICONTROL Planned Completion Date]) a été modifiée<br>* Nom du problème<br>* Nouvelle [!UICONTROL Planned Completion Date]<br>* Nom de la personne qui a modifié la date d’échéance<br>* Date de la synthèse quotidienne<br></p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Le statut est remplacé sur une tâche que l’on m’a affectée par</strong> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque le statut de la tâche est modifié, sauf si l’utilisateur ou l’utilisatrice qui a modifié le statut est également la personne cessionnaire.</p> <p>Remarque : cette notification n’est pas envoyée lorsque le statut de la tâche devient terminé. Une notification distincte est utilisée pour les tâches terminées. Consultez <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Une tâche qui m’a été affectée est terminée</a> ci-dessus.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>&lt;Task Name&gt; de &lt;Project Name&gt; est &lt;New Status&gt;</em>.</p> <p> </p> <p> L’objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de la personne qui a modifié l’état<br>Nouveau statut<br>Date et heure de modification du statut<br>Prévisualisation du statut<br><strong>Bouton [!UICONTROL See More Details]</strong> <br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches pour lesquelles le statut a changé<br>* Nom de la tâche<br>* Statut précédent de la tâche<br>* Nouveau statut de la tâche<br>* Nom de la personne qui a modifié le statut<br>* Date de la synthèse quotidienne<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le statut a été modifié pour l’un de mes éléments de travail</strong> </p> <p>Vous recevez une notification par e-mail lorsque le statut d’un problème qui vous est affecté est modifié, sauf si vous modifiez vous-même le statut. </p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>&lt;Issue Name&gt; de &lt;Project Name&gt; est &lt;New Status&gt;</em>.</p> <p> L’objet de la notification de la synthèse quotidienne est le suivant : <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la personne qui a modifié le statut<br>Nouveau statut<br>Date et heure de modification du statut<br>Statut précédent du problème<br><strong>Bouton Plus de détails</strong><br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de problèmes pour lesquels le statut a changé<br>* Nom de la tâche<br>* Statut précédent du problème<br>* Nouveau statut du problème<br>* Nom de la personne qui a modifié le statut<br>* Date de la synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
 </tbody> 
</table>
