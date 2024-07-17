---
content-type: reference
navigation-topic: notifications
title: "Notifications : informations sur le travail qui m’est assigné"
description: Les notifications suivantes vous alertent sur les activités qui se produisent sur une tâche qui vous est affectée.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 5%

---

# Notifications : informations sur le travail qui m’a été affecté

Les notifications suivantes vous alertent sur les activités qui se produisent sur une tâche qui vous est affectée.

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voir aussi [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>Champs inclus </p> <p> *Champs de résumé quotidien uniquement</p> </th> 
   <th>État par défaut</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Un prédécesseur d'une tâche affectée à mon équipe est terminé</strong> </p> <p>L’équipe affectée reçoit une notification par courrier électronique lorsqu’un prédécesseur de l’une de ses tâches est terminé. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>Terminé : &lt;Nom de la tâche&gt;</em></p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom de la tâche du prédécesseur <br>Prédécesseur Projet de tâche<br>Prédécesseur Numéro de référence de la tâche<br>Nom de l’utilisateur ayant terminé la tâche du prédécesseur<br>État de la tâche du prédécesseur<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche du prédécesseur<br><strong>Voir Plus de détails</strong> bouton<br>*Nom du projet<br>}*Numéro de référence du projet<br>}}}*10}*État de la fonction de référence du précédent}*10}*10}*État de la fonction <br>*État de référence du prédécesseur}*État de la fonction}*État de la fonction}*État de référence du prédécesseur*État de référence du prédécesseur}*État de la tâche de la tâche 1}*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </p> </td> 
   <td><strong>Chaque jour</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Lorsqu'une tâche est terminée, envoyer un e-mail aux cessionnaires principaux de toute les tâches dépendantes</strong> </p> <p>La personne désignée pour la tâche reçoit une notification par courrier électronique lorsqu’un prédécesseur de l’une de ses tâches est terminé. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Terminé] : &lt;Nom de la tâche&gt;</em></p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom de la tâche du prédécesseur<br>Prédécesseur Tâche Projet<br>Prédécesseur Numéro de référence de la tâche<br>Nom de l’utilisateur ayant terminé la tâche du prédécesseur<br>État de la tâche du prédécesseur<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche du prédécesseur<br><strong>[!UICONTROL Voir plus de détails]</strong>} bouton<br>*Nom du projet<br>}}*Numéro de référence du projet*Numéro de référence du projet<br>}}}}}}}*Numéro de la tâche de référence du prédécesseur  de prédécesseurs ont terminé<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </p> </td> 
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
   <td> <p><strong>Une tâche que j’ai terminée est approuvée ou rejetée</strong> </p> <p>La personne cessionnaire pour la tâche reçoit une notification par e-mail lorsque la tâche est approuvée ou refusée.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Terminé] : &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a accordé l’approbation<br>Nouveau statut de la tâche<br>Date et heure auxquelles la tâche a été approuvée ou rejetée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>}*Nombre total de tâches approuvées ou rejetées<br>}*Nom de tâche<br>*Nom de l’utilisateur qui a approuvé ou rejeté la tâche<br>*Décision d’approbation ([!UICONTROL Approuvé]/ [!UICONTROL Refusé])<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Une tâche à laquelle je suis assigné est terminée</strong> </p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique une fois la tâche terminée.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Terminé] : &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p> <p>Remarque : si la tâche est modifiée et passe à l’état [!UICONTROL Terminé], l’objet du courrier électronique continue à afficher "Terminé".</p> </p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>}}*Nom de la tâche*Nom de l’utilisateur la tâche<br>*Date du résumé quotidien<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Tous les prédécesseurs d'une tâche affectée à mon équipe sont terminés</strong> </p> <p>L’équipe affectée reçoit une notification par courrier électronique lorsqu’un prédécesseur de l’une de ses tâches est marqué comme terminé.</p> <p>Les utilisateurs disposant d’une licence de vérification ou de demandeur ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>Fin de tâche : &lt;Nom&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> Résumé du travail qui vous a été attribué &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Projet de tâche<br>Numéro de référence de la tâche<br>Nom de l’utilisateur ayant terminé la tâche précédente<br>État de la tâche précédente<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche précédente<br><strong>Voir plus de détails</strong> bouton<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>}*Nom de la tâche<br>}*Nom de la tâche*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </td>
   <td><strong>Instant</strong> </td> 
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
   <td> <p><strong>Tous les prédécesseurs de mes tâches sont terminés</strong> </p> <p>La personne désignée pour la tâche reçoit une notification par courrier électronique pour chaque prédécesseur qui est terminé.</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Terminé] : &lt;Nom de la tâche&gt;</em><br></p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Projet de tâche<br>Numéro de référence de la tâche<br>Nom de l’utilisateur ayant terminé la tâche précédente<br>État de la tâche précédente<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong> bouton<br>*Nom du projet<br>*Numéro de référence du projet<br>}*Nombre total de tâches terminées Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Un problème que je résolve est approuvé ou rejeté</strong> </p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsqu’une décision d’approbation est prise (approuvée ou rejetée).</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>Problème en attente d’approbation : &lt;Date de début planifiée&gt; &lt;Numéro de référence du problème&gt; - &lt;Nom du problème&gt; dans &lt;Nom du projet&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> Résumé du travail qui vous a été attribué &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a approuvé ou rejeté le problème<br>Décision d’approbation (approuvée ou rejetée)<br>État du problème<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>}}*Nombre total 1}*Nom du problème<br>*Nom de l’utilisateur qui a approuvé ou rejeté le problème<br>*Décision d’approbation (approuvée ou rejetée)<br>*Date du résumé quotidien<br><br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Un problème auquel je suis affecté est terminé</strong> </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>Terminé : &lt;Nom du problème&gt; sur &lt;Nom du projet&gt;</em></p> <p><em> L’objet de la notification quotidiennement de résumé est : Résumé du travail qui vous a été attribué &lt;Date du résumé quotidien&gt; </em> </p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a terminé le problème<br>État du nouveau problème<br>Date et heure auxquelles le problème s’est terminé<br>État de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong>} <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>}*Nom du problème}*Nom du problème<br>*Nom du problème*Nom de l’utilisateur ayant terminé le problème<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Les documents sont téléchargés ou modifiés sur les demandes auxquelles je suis affecté à </strong> </p> <p>La personne désignée pour le problème reçoit une notification par courrier électronique lorsque des documents sont téléchargés ou que les détails du document sont modifiés sur un problème qu’elle a ajouté.</p> <p>Une notification par courrier électronique n’est pas envoyée si l’utilisateur qui a déclenché le problème est la personne désignée pour le problème.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et si le projet est configuré comme une file d’attente de demande d’aide (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente de demande</a>).</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Document ajouté à] &lt;Nom de la demande&gt;</em></p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom de la requête<br>Nom du projet (Nom de la file d’attente de la requête)<br>Numéro de référence du document <br>Nom de l’utilisateur qui a téléchargé le document<br>Nom du document <br> ajouté à la date<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Télécharger]</strong> 1}*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents téléchargés ou modifiés<br>*Nom du document<br>*Nom de l’objet<br>*Nom de l’utilisateur ayant téléchargé le document<br>*Date du résumé quotidien<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date d’échéance d’une tâche qui m’a été affectée est modifiée</strong> </p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique lorsque la [!UICONTROL Date d’achèvement planifiée] de la tâche change, sauf si l’utilisateur qui a modifié la date d’achèvement planifiée est également le cessionnaire de la tâche.</p> <p>Une notification est envoyée uniquement si l’état du projet est autre que [!UICONTROL Planning].</p> <p>Aucune notification n’est envoyée concernant les tâches personnelles.</p> <p> Les utilisateurs disposant d’une licence de vérification ou de demandeur ne reçoivent pas de notification. </p> <p> L'objet de l'email de notification instantanée est : <em>[!UICONTROL La date d'échéance a été modifiée.]</em></p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Date d’échéance ([!UICONTROL Date d’achèvement prévue])<br>Date et heure auxquelles la date d’échéance a été modifiée<br>Nom de l’utilisateur qui a modifié la date d’échéance<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches où la date d’échéance (date d’achèvement prévue) a changé<br>*Nom de tâche *Nom de la date d’exécution <br>*Nom de tâche *Nom de la date d’exécution *Nom de la date d’échéance (date d’exécution prévue) Date d’achèvement prévue<br>*Nom de l’utilisateur qui a modifié la date d’échéance<br>*Date du résumé quotidien </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date d’échéance change pour un problème auquel je suis affecté </strong> </p> <p>La personne désignée par le problème reçoit une notification par courrier électronique lorsque la [!UICONTROL Date d’achèvement planifiée] change, sauf si l’utilisateur qui a modifié la [!UICONTROL Date d’achèvement planifiée] est également la personne désignée.</p> <p>Une notification est envoyée uniquement si l’état du projet est autre que [!UICONTROL Planning].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL La date d’échéance a été modifiée]</em></p> <p> </p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Date d’échéance ([!UICONTROL Date d’achèvement prévue])<br>Date et heure auxquelles la date d’échéance a été modifiée<br>Nom de l’utilisateur qui a modifié la date d’échéance<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes où la date d’échéance ([!UICONTROL Date d’achèvement planifiée]) a changé<br>) Nom<br>*Nouvelle [!UICONTROL Date d’achèvement prévue]<br>*Nom de l’utilisateur qui a modifié la date d’échéance<br>*Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>L’état change sur une tâche à laquelle je suis assigné</strong> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque le statut de la tâche est modifié, sauf si l’utilisateur ou l’utilisatrice qui a modifié le statut est également la personne cessionnaire.</p> <p>Remarque : Cette notification n’est pas envoyée lorsque l’état de la tâche devient terminé. Une notification distincte est utilisée pour les tâches terminées. Voir <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Une tâche à laquelle je suis assigné est terminée</a>, ci-dessus.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>&lt;Nom de la tâche&gt; de &lt;Nom du projet&gt; est &lt;Nouvel état&gt;</em></p> <p> </p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a modifié l’état<br>Nouveau statut<br>Date et heure auxquelles l’état a été modifié<br>État de prévisualisation<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches où l’état a changé<br>}} 2}*État de la tâche précédente<br>*État de la nouvelle tâche<br>*Nom de l’utilisateur qui a modifié l’état<br>*Date du résumé quotidien<br><br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>L’état change sur l’une de mes tâches</strong> </p> <p>Vous recevez une notification par courrier électronique lorsque l’état change pour un problème auquel vous êtes affecté, sauf si vous modifiez vous-même l’état. </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L’objet de l’email de notification instantanée est : <em>&lt;Nom du problème&gt; de &lt;Nom du projet&gt; est &lt;Nouvel état&gt;</em></p> <p> Le sujet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a modifié l’état<br>Nouveau statut<br>Date et heure auxquelles l’état a été modifié<br>État du problème précédent<br><strong>Voir Plus de détails</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes où l’état a changé<br>}*Nom de la tâche<br>*État précédent<br>*Nouvel état de problème<br>*Nom de l’utilisateur qui a modifié l’état<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
 </tbody> 
</table>
