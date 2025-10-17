---
content-type: reference
navigation-topic: notifications
title: 'Notifications : Demandes que j’ai effectuées'
description: Les notifications suivantes vous informent sur les demandes que vous avez effectuées dans Adobe Workfront.
author: Courtney
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 98%

---

# Notifications : Demandes que j’ai effectuées

Les notifications suivantes vous informent sur les demandes que vous avez effectuées dans [!DNL Adobe Workfront].

Pour plus d’informations sur la configuration des notifications que vous recevez, voir la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voir aussi [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Demandes que j’ai effectuées</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d’approbation de document est remplie</strong> </p> <p>La personne qui a demandé une approbation sur un document reçoit une notification par e-mail une fois la demande d’approbation terminée.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant :<em> &lt;Approver Name&gt; a &lt;Approval Decision ([!UICONTROL Approved], [!UICONTROL Approved with Changes], [!UICONTROL Rejected])&gt; ce document.</em></p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un e-mail de synthèse quotidienne.</p> </td> 
   <td> Nom du document<br>Nom de l’approbateur ou l’approbatrice </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un document est modifié ou chargé sur un problème dont je suis le contact principal</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail lorsqu’un document est chargé ou modifié sur le problème, sauf si la personne qui a chargé ou modifié le document est également le contact principal.</p> <p>Une notification n’est envoyée que si le projet est configuré en tant que [!UICONTROL Help Request Queue] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Document ajouté à &lt;Issue Name&gt;</em></p> <p>L’objet de la notification de synthèse quotidienne est : <em>Synthèse de vos demandes &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Nom de l’objet dans lequel le document a été chargé<br>Nom de l’objet parent<br>Numéro de référence du document<br>Nom de la personne qui a chargé le document<br>Nom du document<br>Date de l’ajout<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>Boutons [!UICONTROL Preview]</strong> et <strong>[!UICONTROL Download]</strong> <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents chargés<br>*Nom du document<br>*Nom de l’objet parent<br>*Nom de la personne qui a ajouté le document<br>*Date de la synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande de chargement de document est honorée</strong> </p> <p>La personne ayant demandé le document reçoit une notification par e-mail lorsqu’une demande de chargement de document est honorée.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Your document request from] &lt;User Name&gt; a été honorée</em></p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un e-mail de synthèse quotidienne.</p> </td> 
   <td> <p>Nom de la personne qui a chargé le document<br>Nom de l’objet dans lequel le document a été chargé<br>Nom du document<br><br></p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche personnelle que j’ai affectée à une autre personne est terminée</strong> </p> <p>Une notification est envoyée à l’utilisateur qui a affecté une demande de travail personnelle à une autre personne lorsque cette demande est terminée. </p>  <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Fin de tâche : &lt;Task Name&gt;</em></p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un e-mail de synthèse quotidienne.</p> </p> </td> 
   <td> Nom de la tâche<br>Nom du projet par défaut (Projet personnel de la personne qui a reçu la tâche personnelle)<br>Numéro de référence de tâche<br>Nom de la personne propriétaire de la tâche<br>Nouveau statut de tâche<br>Date et heure auxquelles la tâche a été terminée<br>Statut de la tâche précédente<br><strong>Bouton [!UICONTROL See More Details]</strong><br><br><br></td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème pour lequel je suis le contact principal est terminé</strong> </p> <p>Le contact principal sur un problème reçoit une notification une fois le problème terminé.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Issue Completion] : &lt;Issue Name&gt;</em></p> <p>L’objet de la notification de synthèse quotidienne est :<em> Synthèse de vos demandes &lt;Date of the daily digest&gt;</em></p> <p> </p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur ou l’utilisatrice ayant terminé le problème<br>Nouveau statut<br>Date et heure auxquelles le problème a été terminé<br>Statut du problème précédent<br><strong>Bouton [!UICONTROL See More Details]</strong> <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom de l’utilisateur ou l’utilisatrice ayant terminé le problème<br>*Date de la synthèse quotidienne </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>J’ajoute un problème à un projet</strong> </p> <p>Le contact principal sur un problème reçoit une notification lorsqu’il ajoute un problème dans un projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Issue submitted] : &lt;Issue Name&gt; sur &lt;Project Name&gt;</em></p> <p>L’objet de la notification de synthèse quotidienne est :<em> Synthèse de vos demandes &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du portfolio<br>Numéro de référence du problème<br>Votre nom<br>Nom du problème<br>Date de saisie<br>Priorité du problème<br>Statut du problème<br>Nom de la personne assignée<br>Contact principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés<br>*Nom du problème<br>*Date de la synthèse quotidienne </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>J’envoie une demande (confirmation)</strong> </p> <p>Le contact principal sur le problème reçoit une notification par e-mail lorsqu’il envoie un problème.</p> <p>Une notification n’est envoyée que si le statut du projet est [!UICONTROL Current] et si le projet est configuré en tant que [!UICONTROL Help Request Queue] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Request Submitted] : &lt;Request Name&gt; sur &lt;Project (Request Queue) Name&gt;</em></p> <p>L’objet de la notification de synthèse quotidienne est le suivant :<em> Synthèse de vos demandes &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>Nom du projet (nom de la file d’attente des demandes)<br>Nom du portfolio<br>Numéro de référence du problème<br>Nom du problème<br>Date de saisie<br>Priorité du problème<br>Statut du problème<br>Nom de la personne assignée<br>Contact principal<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total de demandes envoyées<br>*Nom de la demande<br>*Priorité de la demande<br>*Date de la synthèse quotidienne</p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ma demande est fermée (confirmation)</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail à la fermeture de la demande.</p> <p>Une notification est envoyée uniquement si le statut du projet est défini comme Actuel et si le projet est configuré en tant que [!UICONTROL Help Request Queue] (comme décrit dans <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente de demandes</a>).</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Your request has been closed] : « &lt;Request Name&gt; »</em></p> <p>L’objet de la notification de synthèse quotidienne est : <em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Nom de la demande<br>Nom du projet<br>Numéro de référence de la demande<br>Nom de l’utilisateur ou de l’utilisatrice qui a fermé la demande<br>Statut du problème<br>Date et heure de fermeture de la demande<br>Staut de la demande précédente<br><strong>Bouton</strong> [!UICONTROL See More Details]<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total de demandes fermées<br>*Nom de la demande<br>*Nom de l’utilisateur ou de l’utilisatrice qui a fermé la demande<br>*Date de synthèse quotidienne </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une personne est affectée à ma demande</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail lorsque quelqu’un est affecté au problème, sauf si le contact principal et l’utilisateur ou l’utilisatrice affecté sont la même personne.</p> <p>Une notification est envoyée uniquement si le statut du projet est défini comme Actuel et si le projet est configuré en tant que [!UICONTROL Help Request Queue] (comme décrit dans <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L’objet de l’e-mail de notification instantanée est : <em>&lt;Name of the user who is assigned to your request&gt; [!UICONTROL has been assigned to your request] : « &lt;Request Name&gt; »</em></p> <p>L’objet de la notification de synthèse quotidienne est :<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la demande<br>Type de demande<br>Date entrée<br>Priorité du problème<br>Contact principal<br>Date d’achèvement prévue<br>Statut du problème<br><strong>Bouton</strong>Plus de détails<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de demandes affectées<br>*Nom de la demande<br>*Nom d’affectation<br>*Date de la synthèse quotidienne</p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le statut d’un projet que j’ai créé est modifié</strong> </p> <p>L’utilisateur ou l’utilisatrice qui a créé le projet reçoit une notification par e-mail lorsque le statut du projet est modifié.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Project Status Change]: &lt;Project Name&gt;</em></p> <p>L’objet de la notification de synthèse quotidienne est :<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur ou de l’utilisatrice qui a modifié le statut<br>Nouveau statut<br>Date et heure de modification du statut du projet<br>Statut précédent du projet<br><strong>Bouton</strong> [!UICONTROL See More Details]<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nouveau statut du projet<br>*Nom de l’utilisateur ou de l’utilisatrice qui a modifié le statut du projet<br>*Date de synthèse quotidienne</p> </td> 
   <td> <p><strong>Instantané</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le statut est modifié à ma demande</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail lorsque le statut du problème est modifié, sauf si l’utilisateur ou l’utilisatrice à l’origine de la modification est également le contact principal.</p> <p>Une notification est envoyée uniquement si le statut du projet est défini comme Actuel et si le projet est configuré en tant que [!UICONTROL Help Request Queue] (comme décrit dans <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>&lt;Request Name&gt; est &lt;New Status&gt;</em></p> <p>L’objet de la synthèse quotidienne est :<em> Synthèse de vos demandes &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Nom de la demande<br>Nom du projet<br>Numéro de référence de la demande<br>Nom de l’utilisateur ou de l’utilisatrice qui a modifié le statut de la demande<br>Nouveau statut<br>Date et heure de modification du statut de la demande<br>Statut de la demande précédente<br><strong>Bouton</strong> [!UICONTROL See More Details]<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de demandes dont le statut a été modifié<br>*Nom de la demande<br>*Statut de la demande précédente<br>*Staut de la nouvelle demande<br>*Nom de l’utilisateur ou de l’utilisatrice qui a modifié le statut<br>*Date de synthèse quotidienne<br></td> 
   <td> <p><strong>Chaque jour</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
