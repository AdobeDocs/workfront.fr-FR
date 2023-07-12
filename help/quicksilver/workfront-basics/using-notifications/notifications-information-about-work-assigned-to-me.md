---
content-type: reference
navigation-topic: notifications
title: 'Notifications : Informations sur le travail qui m''est assigné'
description: Les notifications suivantes vous alertent sur les activités qui se produisent sur une tâche qui vous est affectée.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 901605917347297a1ee077f00905b03427582650
workflow-type: tm+mt
source-wordcount: '2090'
ht-degree: 6%

---

# Notifications : Informations sur le travail qui m&#39;est assigné

Les notifications suivantes vous alertent sur les activités qui se produisent sur une tâche qui vous est affectée.

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Activation ou désactivation de vos propres notifications d’événement](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Une tâche antérieure d’une tâche affectée à mon équipe est terminée</strong> </p> <p>L’équipe affectée reçoit une notification par courrier électronique lorsqu’un prédécesseur de l’une de ses tâches est terminé. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Terminé : &lt;task name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom de la tâche du prédécesseur<br>Projet de tâche du prédécesseur<br>Numéro de référence de la tâche du prédécesseur<br>Nom de l’utilisateur qui a terminé la tâche du prédécesseur<br>État de la tâche précédente<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche précédente<br><strong>Voir Plus de détails</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de prédécesseurs terminés<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </p> </td> 
   <td><strong>Chaque jour</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Lorsqu'une tâche est terminée, envoyer un e-mail aux cessionnaires principaux de toute les tâches dépendantes</strong> </p> <p>La personne désignée pour la tâche reçoit une notification par courrier électronique lorsqu’un prédécesseur de l’une de ses tâches est terminé. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom de la tâche du prédécesseur<br>Projet de tâche du prédécesseur<br>Numéro de référence de la tâche du prédécesseur<br>Nom de l’utilisateur qui a terminé la tâche du prédécesseur<br>État de la tâche précédente<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de prédécesseurs terminés<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </p> </td> 
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
   <td> <p><strong>Lorsqu'une tâche d'approbation est approuvée ou rejetée, envoyer un e-mail au cessionnaire</strong> </p> <p>La personne désignée pour la tâche reçoit une notification par e-mail lorsque la tâche est approuvée ou rejetée.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a accordé la validation<br>New Task Status<br>Date et heure auxquelles la tâche a été approuvée ou rejetée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches approuvées ou rejetées<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a approuvé ou rejeté la tâche<br>*Décision D’Approbation ([!UICONTROL Approuvé]/ [!UICONTROL Refusé])<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Quand une tâche est terminée, envoyer un e-mail au cessionnaire</strong> </p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique une fois la tâche terminée.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Remarque : Si la tâche est modifiée et passe à un état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "Terminé".</p> </p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Toutes les tâches antérieures d’une tâche affectée à mon équipe sont terminées</strong> </p> <p>L’équipe affectée reçoit une notification par courrier électronique lorsqu’un prédécesseur de l’une de ses tâches est marqué comme terminé.</p> <p>Les utilisateurs disposant d’une licence de vérification ou de demandeur ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Fin de la tâche : &lt;name&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> Résumé du travail qui vous est assigné &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Projet de tâche<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche du prédécesseur<br>État de la tâche précédente<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche précédente<br><strong>Voir Plus de détails</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </td>
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
   <td> <p><strong>Toutes les tâches antérieures de mes tâches sont terminées</strong> </p> <p>La personne désignée pour la tâche reçoit une notification par courrier électronique pour chaque prédécesseur qui est terminé.</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt;</em><br></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Projet de tâche<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche du prédécesseur<br>État de la tâche précédente<br>Date et heure auxquelles le prédécesseur a été terminé<br>État précédent de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </td> 
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
   <td> <p><strong>Lorsqu'un événement est approuvé ou rejeté, envoyer un e-mail au cessionnaire</strong> </p> <p>La personne désignée pour un problème reçoit une notification par courrier électronique lorsqu’une décision d’approbation est prise (approuvée ou rejetée).</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Problème en attente d’approbation : &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> Résumé du travail qui vous est assigné &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a approuvé ou rejeté le problème<br>Décision d’approbation (approuvée ou rejetée)<br>État du problème<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes approuvés ou rejetés<br>*Nom du problème<br>*Nom de l’utilisateur qui a approuvé ou rejeté le problème<br>*Décision d’approbation (approuvée ou rejetée)<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Lorsqu'un événement est conclu, envoyer e-mail au cessionnaire</strong> </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Terminé : &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p><em> L’objet de la notification quotidiennement Digest est : Résumé du travail qui vous est assigné &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur ayant terminé le problème<br>Nouveau statut du problème<br>Date et heure auxquelles le problème s’est terminé<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom de l’utilisateur ayant terminé le problème<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Les documents sont chargés ou modifiés à ma demande</strong> </p> <p>La personne désignée pour le problème reçoit une notification par courrier électronique lorsque des documents sont téléchargés ou que les détails du document sont modifiés sur un problème qu’elle a ajouté.</p> <p>Une notification par courrier électronique n’est pas envoyée si l’utilisateur qui a déclenché le problème est la personne désignée pour le problème.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et si le projet est configuré comme une file d’attente de demande d’aide (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requête</a>).</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Document ajouté à] &lt;request name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom de la requête<br>Nom du projet (nom de la file d’attente des demandes)<br>Numéro de référence du document <br>Nom de l’utilisateur qui a téléchargé le document.<br>Document Name <br>Ajout de la date "À"<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Téléchargement]</strong> boutons<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents chargés ou modifiés<br>*Nom du document<br>*Nom de l’objet<br>*Nom de l’utilisateur qui a téléchargé le document.<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque la date de fin prévue d'une tâche est modifiée, envoyer un e-mail à l'utilisateur affecté</strong> </p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique lorsque la [!UICONTROL Date d’achèvement planifiée] de la tâche change, sauf si l’utilisateur qui a modifié la date d’achèvement planifiée est également le cessionnaire de la tâche.</p> <p>Une notification est envoyée uniquement si l’état du projet est autre que [!UICONTROL Planning].</p> <p>Aucune notification n’est envoyée concernant les tâches personnelles.</p> <p> Les utilisateurs disposant d’une licence de vérification ou de demandeur ne reçoivent pas de notification. </p> <p> L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL La date d’échéance a été modifiée.]</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nouvelle date d’échéance ([!UICONTROL Date d’achèvement prévue])<br>Date et heure de modification de la date d’échéance<br>Nom de l’utilisateur qui a modifié la date d’échéance<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches pour lesquelles la date d’échéance (date d’achèvement prévue) a été modifiée<br>*Nom de la tâche<br>*Nouvelle date d’achèvement prévue<br>*Nom de l’utilisateur qui a modifié la date d’échéance<br>*Date du résumé quotidien </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque la date de fin prévue d'un événement est modifiée, envoyer un e-mail à  l'utilisateur affecté</strong> </p> <p>La personne désignée par le problème reçoit une notification par courrier électronique lorsque la [!UICONTROL Date d’achèvement planifiée] change, sauf si l’utilisateur qui a modifié la [!UICONTROL Date d’achèvement planifiée] est également la personne désignée.</p> <p>Une notification est envoyée uniquement si l’état du projet est autre que [!UICONTROL Planning].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL La date d’échéance a été modifiée]</em></p> <p> </p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nouvelle date d’échéance ([!UICONTROL Date d’achèvement prévue])<br>Date et heure de modification de la date d’échéance<br>Nom de l’utilisateur qui a modifié la date d’échéance<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes où la date d’échéance ([!UICONTROL Date d’achèvement prévue]) a changé<br>*Nom du problème<br>*Nouvelle [!UICONTROL Date d’achèvement planifiée]<br>*Nom de l’utilisateur qui a modifié la date d’échéance<br>*Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Le statut est remplacé sur une tâche que l'on m'a affectée par</strong> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique lorsque l’état de la tâche change, sauf si l’utilisateur qui a modifié l’état est également la personne désignée.</p> <p>Remarque : Cette notification n’est pas envoyée lorsque l’état de la tâche devient terminé. Une notification distincte est utilisée pour les tâches terminées. Voir <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Une tâche à laquelle je suis affecté est terminée.</a>, ci-dessus.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;task name=""&gt; de &lt;project name=""&gt; is &lt;new status=""&gt;</em></p> <p> </p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a modifié l’état<br>Nouveau statut<br>Date et heure de modification de l’état<br>État de l’aperçu<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches pour lesquelles l’état a changé<br>*Nom de la tâche<br>*État de la tâche précédente<br>*New Task Status<br>*Nom de l’utilisateur qui a modifié l’état<br>*Date du résumé quotidien<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le statut a été modifié dans l'un de mes éléments de travail.</strong> </p> <p>Vous recevez une notification par courrier électronique lorsque l’état change pour un problème auquel vous êtes affecté, sauf si vous modifiez vous-même l’état. </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ou [!UICONTROL Requestor] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;issue name=""&gt; de &lt;project name=""&gt; is &lt;new status=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé du travail qui vous a été attribué] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a modifié l’état<br>Nouveau statut<br>Date et heure de modification de l’état<br>État du problème précédent<br><strong>Voir Plus de détails</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes où l’état a changé<br>*Nom de la tâche<br>*État du problème précédent<br>*Nouveau statut du problème<br>*Nom de l’utilisateur qui a modifié l’état<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
 </tbody> 
</table>
