---
content-type: reference
navigation-topic: notifications
title: '« Notifications : informations sur les projets dont je suis propriétaire »'
description: Les notifications suivantes vous alertent sur les activités qui ont lieu sur un projet dont vous êtes propriétaire. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Modifier vos propres notifications par e-mail.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 100%

---

# Notifications : informations sur les projets dont je suis propriétaire

Les notifications suivantes vous alertent sur les activités qui ont lieu sur un projet dont vous êtes propriétaire. Pour plus d’informations sur la configuration des notifications que vous recevez, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Un document est ajouté à un projet dont je suis propriétaire</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un document est ajouté au projet, sauf si c’est elle qui l’a ajouté.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] et que le document n’est pas Privé.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Document added to] &lt;Project Name&gt;</em></p> <p> L’objet de la notification de synthèse quotidienne est : <em> [!UICONTROL Digest of Projects You Own] &lt;Date de la synthèse quotidienne&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Nom de la personne qui a ajouté le document<br>Nom du document<br>Date d’ajout<br>Détails du document (format, taille, numéro de version)<br><strong>Boutons [!UICONTROL Preview]</strong> et <strong>[!UICONTROL Download]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents ajoutés<br>*Nom du document<br>*Nom de la personne qui a ajouté le document<br>*Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche jalonnée est achevée sur un projet dont je suis propriétaire</strong> </p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p>Remarque : si la tâche passe à un statut qui correspond à [!UICONTROL Complete], l’objet de l’e-mail affiche toujours « [!UICONTROL Complete] ».</p> <p> L’objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Projects You Own] &lt;Date de la synthèse quotidienne&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de la personne qui a terminé la tâche<br>Nouveau statut de tâche<br>Date et heure auxquelles la tâche a été terminée<br>Précédent statut de la tâche<br><strong>Bouton [!UICONTROL See More Details]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de la personne qui a terminé la tâche<br>*Date de la synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand un projet passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au propriétaire du projet</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque le projet est en retard. Un projet est en retard lorsque le statut de la progression est « [!UICONTROL At Risk] », « [!UICONTROL Behind] » ou « [!UICONTROL Late] ».</p> <p>La bonne pratique consiste à maintenir cette notification active. </p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Project Progress Change] : &lt;Nom du projet&gt;</em></p> <p> L’objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Projects You Own] &lt;Date de la synthèse quotidienne&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Statut de la progression du projet<br>[!UICONTROL Planned Start Date] du projet<br>[!UICONTROL Planned Completion Date] du projet<br>[!UICONTROL Projected Start Date] du projet<br>[!UICONTROL Projected Completion Date] du projet<br>Pourcentage du projet terminé<br>Statut du projet<br>Personne propriétaire du projet<br>*Nom du projet<br>*Numéro de référence du projet<br>*Statut de la progression du projet<br>*Date de la synthèse quotidienne<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'un événement est ajouté.</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Issue added to] &lt;Nom du projet&gt;</em></p> <p> </p> <p> L’objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Projects You Own] &lt;Date de la synthèse quotidienne&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du portfolio<br>Numéro de référence du problème<br>Nom de la personne qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom de la personne cessionnaire<br>Statut du problème<br>Contact principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés au projet<br>*Nom du problème<br>*Nom de la personne qui a ajouté le problème<br>*Date de la synthèse quotidienne</p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et quotidienne</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche est achevée sur un projet dont je suis propriétaire</strong> </p> <p>La personne propriétaire du projet reçoit une notification lorsqu’une tâche se termine sur son projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Complete] : &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p> <p>Remarque : si la tâche passe à un statut qui correspond à [!UICONTROL Complete], l’objet de l’e-mail affiche toujours « [!UICONTROL Complete] ».</p> </p> <p> L’objet de la notification de la synthèse quotidienne est : <em> [!UICONTROL Digest of Projects You Own] &lt;Date de la synthèse quotidienne&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de la personne qui a terminé la tâche <br>Statut de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>Précédent statut de la tâche<br><strong>Bouton [!UICONTROL See More Details]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de la personne qui a terminé la tâche<br>*Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche d’un projet que je possède est en retard</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’une tâche du projet est en retard sur le planning. Une tâche est en retard sur le planning lorsque le statut de la progression est « [!UICONTROL At Risk] » ou « [!UICONTROL Behind] » ou « [!UICONTROL Late] ».</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Task Progress Change] : &lt;Task Name&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est le suivant : <em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche <br>Statut de progression de la nouvelle tâche<br>[!UICONTROL Planned Start Date]de la tâche<br>[!UICONTROL Planned Completion Date]de la tâche<br>[!UICONTROL Projected Start Date] de la tâche<br>[!UICONTROL Projected Completion Date] de la tâche<br>Pourcentage terminé de la tâche<br>Statut de la tâche<br>Nom de la personne affectée<br>Nom de la personne ayant saisi la tâche<br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total des tâches qui sont en retard<br>* Nom de la tâche<br>* Nom de la personne affectée<br>* Date de la synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème est terminé sur un projet que je possède</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème se termine sur son projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification. </p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;Issue Name&gt; de &lt;Project Name&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est le suivant : <em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la personne ayant terminé le problème<br>Statut du problème<br>Date et heure auxquelles le problème a été terminé<br>Statut précédent du problème<br><strong>Bouton [!UICONTROL See More Details]</strong> <br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de problèmes terminés<br>* Nom du problème<br>* Nom de la personne affectée au problème<br>* Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème non affecté est ajouté à un projet que je possède </strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Qui doit être affecté à ce nouveau problème le] &lt;p&gt; ?</em></p> <p> </p> <p> L’objet de la notification de synthèse quotidienne est le suivant : <em> Synthèse des projets que vous possédez &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de la personne qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom attribué (vide)<br>Statut du problème<br>Contact principal<br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de problèmes ajoutés<br>* Nom du problème<br>* Nom de la personne qui a ajouté le problème<br>* Date de la synthèse quotidienne<br></p> </td> 
   <td> <p><strong>Instantanée</strong> </p> <p><strong>et quotidienne</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Je suis propriétaire d’un nouveau projet</strong> </p> <p>Lorsqu’une personne est définie comme propriétaire d’un projet, elle reçoit une notification par e-mail.</p> <p>Si la personne propriétaire du projet est la même personne que celle qui a effectué l’affectation, aucune notification par e-mail n’est envoyée.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>Activez cela parce que ces personnes sont affectées à quelque chose. </p> <p> Affecter quelque chose, partager quelque chose, avoir accès à quelque chose.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL You're now the project owner of] &lt;Project Name&gt;</em>.</p> <p>Le texte suivant est inclus dans le corps de la notification par e-mail :<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;Your Name&gt;,<br></em><em>&lt;Name of the user who assigned you as the Project Owner&gt; [!UICONTROL made you the owner of] &lt;Project Name&gt;. [!UICONTROL As the Project Owner, you might receive additional email notifications about project activity, be required to approve hours for the project, or be involved in approving work related to the project. It's all yours.]</em> </p> <p> L’objet de la notification de synthèse quotidienne est le suivant : <em> [!UICONTROL Digest of Projects You Own] &lt;date of daily digest&gt; </em></p> <p> </p> </td> 
   <td> <p>Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Date d’achèvement du projet<br>* Nom du projet<br>* Numéro de référence du projet<br>* Date de la synthèse quotidienne</p> </td> 
   <td><strong>Instantanée</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date d’engagement est modifiée pour une tâche sur un de mes projets</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement est modifiée pour une tâche du projet, sauf si la personne qui a modifié la date d’engagement est également la personne propriétaire du projet.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Commit date for] &lt;Task Name&gt; [!UICONTROL is now] &lt;New Commit Date&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est le suivant : <em> Synthèse des projets que vous possédez &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de la personne qui a modifié la date d’engagement<br>Nouvelle date d’engagement<br>[!UICONTROL Planned Completion Date] de la tâche<br>Informations sur l’impact de cette modification sur la chronologie du projet<br>Nom de la personne affectée<br>Nom de la personne ayant saisi la tâche<br>Propriétaire du projet<br><strong>Bouton [!UICONTROL See More Details]</strong> <br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de tâches dont la date d’engagement a changé<br>* Nom de la tâche<br>* Date de la synthèse quotidienne<br></p> </td> 
   <td> <p><strong>Instantanée</strong> </p> <p><strong>et [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date d’engagement est modifiée sur un problème d‘un de mes projets</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement change pour un problème sur le projet, sauf si c’est elle qui l’a modifiée.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Commit date for] &lt;Issue Name&gt; [!UICONTROL is now] &lt;New Commit Date&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est le suivant : <em> [!UICONTROL Digest of Projects You Own] &lt;date of daily digest &gt; </em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la personne qui a modifié la date d’engagement<br>Nouvelle date d’engagement<br>Date d’achèvement prévue du problème<br>Nom de la personne affectée<br>Nom de la.personne ayant saisi le problème<br>Propriétaire du projet<br><strong>Bouton [!UICONTROL See More Details]</strong> <br>* Nom du projet<br>* Numéro de référence du projet<br>* Nombre total de problèmes dont la date d’engagement a changé<br>* Nom du problème<br>* Date de la synthèse quotidienne<br></p> </td> 
   <td> <p><strong>Instantanée</strong> </p> <p><strong>et [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
