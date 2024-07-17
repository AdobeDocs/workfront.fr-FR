---
content-type: reference
navigation-topic: notifications
title: "Notifications : demandes que j’ai effectuées"
description: Les notifications suivantes vous informent sur les demandes que vous avez effectuées dans Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 6%

---

# Notifications : demandes que j’ai effectuées

Les notifications suivantes vous permettent de connaître les demandes que vous avez effectuées dans [!DNL Adobe Workfront].

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voir aussi [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Demandes Que J’Ai Effectuées</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d'approbation de document est terminée</strong> </p> <p>L’utilisateur qui a demandé une approbation sur un document reçoit une notification par courrier électronique une fois la demande d’approbation terminée.</p> <p>L’objet de l’e-mail de notification instantanée est :<em> &lt;Nom de l’approbateur&gt; a &lt;Décision d’approbation ([!UICONTROL Approuvé], [!UICONTROL Approuvé avec des modifications], [!UICONTROL Refusé])&gt; ce document.</em></p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </td> 
   <td> Nom du document<br>Nom de l’approbateur </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un document est modifié ou téléchargé sur un problème pour lequel je suis le contact principal</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail lorsqu’un document est chargé ou modifié sur le problème, sauf si la personne qui a chargé ou modifié le document est également le contact principal.</p> <p>Une notification est envoyée uniquement si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de demandes]</a>).</p> <p>L'objet de l'email de notification instantanée est : <em>Document ajouté à &lt;Nom du problème&gt;</em></p> <p>L’objet de la notification de résumé quotidienne est : <em>Digest of Your Requests &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> Nom d’objet où le document a été téléchargé<br>Nom d’objet parent<br>Numéro de référence du document<br>Nom de l’utilisateur qui a téléchargé le document<br>Nom du document<br>ajouté à la date<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Téléchargement]</strong> 11}*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents téléchargés<br>*Nom du document<br>*Nom de l’objet parent<br>*Nom de l’utilisateur ayant ajouté le document<br>*Date du résumé quotidien<br> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une requête de téléchargement de document est satisfaite</strong> </p> <p>Le demandeur de document reçoit une notification par courrier électronique lorsqu’une demande de téléchargement de document est satisfaite.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Votre demande de document auprès de] &lt;Nom d’utilisateur&gt; a été satisfaite</em></p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </td> 
   <td> <p>Nom de l’utilisateur qui a téléchargé le document<br>Nom de l’objet dans lequel le document a été téléchargé<br>Nom du document<br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche personnelle que j'ai assignée à quelqu'un d'autre est terminée</strong> </p> <p>Une notification est envoyée à l’utilisateur qui a assigné une tâche ad hoc à quelqu’un d’autre une fois cette tâche terminée. </p> <p>Pour plus d’informations sur les tâches ad hoc, voir <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Création d’éléments de travail à partir de la zone [!UICONTROL Accueil]</a>.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>Fin de tâche : &lt;Nom de la tâche&gt;</em></p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> Nom de la tâche<br>Nom de projet par défaut (Projet personnel de l’utilisateur qui a reçu la tâche personnelle)<br>Numéro de référence de la tâche<br>Nom du propriétaire de la tâche<br>Nouvel état de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong><br><br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème pour lequel je suis le contact principal est terminé</strong> </p> <p>Le contact principal sur un problème reçoit une notification une fois le problème terminé.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Fin du problème] : &lt;Nom du problème&gt;</em></p> <p>L’objet de la notification de résumé quotidien est :<em> Digest de vos requêtes &lt;Date du résumé quotidien&gt;</em></p> <p> </p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a terminé le problème<br>Nouveau statut<br>Date et heure auxquelles le problème a été terminé<br>État du problème précédent<br><strong>[!UICONTROL Voir plus de détails]</strong> <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>}*Nom du problème<br>}*Nom du projet *Nom de l’utilisateur ayant terminé le problème<br>*Date du résumé quotidien </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>J’ajoute un problème à un projet</strong> </p> <p>Le contact principal sur un problème reçoit une notification lorsqu’il ajoute un problème dans un projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Problème envoyé] : &lt;Nom du problème&gt; sur &lt;Nom du projet&gt;</em></p> <p>L’objet de la notification de résumé quotidien est :<em> Digest de vos requêtes &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Votre nom<br>Nom du problème<br>Date d’entrée<br>Priorité du problème<br>État du problème<br>Affecté au nom<br>Contact du Principal<br>}*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés<br>*Nom du problème<br>*Nom du problème}*Nom du projet}*Nom du projet*Date de résumé </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>J'envoie une demande (confirmation)</strong> </p> <p>Le contact par Principal sur le problème reçoit une notification par courrier électronique lorsqu’il envoie un problème.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de demandes]</a>).</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Demande envoyée] : &lt;Nom de la demande&gt; sur &lt;Nom de la demande (file d’attente de la demande)&gt;</em></p> <p>L’objet de la notification de résumé quotidien est :<em> Digest de vos requêtes &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> <p>Nom du projet (Nom de la file d’attente des demandes)<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom du problème<br>Date d’entrée<br>Priorité du problème<br>État du problème<br>Affecté au nom<br>Contact du Principal<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total de demandes envoyées<br>*Nom de demande<br>*Priorité de demande}*12}*Priorité de demande}*13}*Priorité de demande Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ma demande est fermée (confirmation)</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail lorsque la demande est close.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente de demandes</a>).</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Votre demande a été fermée]:"&lt;Nom de la demande&gt;"</em></p> <p>Le sujet de la notification de résumé quotidien est :<em> [!UICONTROL Digest de vos requêtes] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Nom de la requête<br>Nom du projet<br>Numéro de référence de la requête<br>Nom de l’utilisateur qui a fermé la requête<br>État du problème<br>Date et heure de fermeture de la requête<br>État de la requête précédente<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total de requêtes fermées<br>}}*Nom de la requête <br>*Nom de la requête }*Nom de la requête *Nom de l’utilisateur qui a fermé la demande<br>*Date du résumé quotidien </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu’un est affecté à ma requête</strong> </p> <p>Le contact principal de la question reçoit une notification par courrier électronique lorsqu’un utilisateur est affecté à la question, sauf si le contact principal et l’utilisateur affecté sont le même utilisateur.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet est configuré en tant que [!UICONTROL File d’attente de demande d’aide] (comme décrit dans <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de demande]</a>).</p> <p>L’objet de l’e-mail de notification instantanée est : <em>&lt;Nom de l’utilisateur affecté à votre demande&gt; [!UICONTROL a été affecté à votre demande] : "&lt;Nom de la demande&gt;"</em></p> <p>Le sujet de la notification de résumé quotidien est :<em> [!UICONTROL Digest de vos requêtes] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la demande<br>Type de demande<br>Date d’entrée<br>Priorité du problème<br>Contact de Principal<br>Date d’achèvement prévue<br>État du problème<br><strong>Voir Plus de détails</strong> <br>*Nom du projet<br>*Numéro de référence du projet<br>}}*Nombre total du nombre total de demande<br>}}*Nombre total de demande affectée<br>*Nom attribué<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le statut change sur un projet que j’ai créé</strong> </p> <p>La personne qui a créé le projet reçoit une notification par e-mail lorsque le statut du projet change.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Modification de l’état du projet] : &lt;Nom du projet&gt;</em></p> <p>Le sujet de la notification de résumé quotidien est :<em> [!UICONTROL Digest de vos requêtes] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a modifié l’état<br>Nouveau statut<br>Date et heure auxquelles l’état du projet a été modifié<br>État du projet précédent<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nouveau statut du projet<br>*Nom de l’utilisateur état du projet<br>*Date du résumé quotidien</p> </td> 
   <td> <p><strong>Instant</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le statut change sur ma requête</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail lorsque le statut du problème change, sauf si l’utilisateur ou l’utilisatrice qui a modifié le statut est également le contact principal.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et que le projet est configuré en tant que [!UICONTROL File d’attente de demande d’aide] (comme décrit dans <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de demande]</a>).</p> <p>L’objet de l’email de notification instantanée est : <em>&lt;Nom de la requête&gt; est &lt;Nouveau statut&gt;</em></p> <p>L’objet de la notification de résumé quotidien est :<em> Digest de vos requêtes &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Nom de la requête<br>Nom du projet<br>Numéro de référence de la requête<br>Nom de l’utilisateur qui a modifié l’état de la requête<br>Nouvel état<br>Date et heure auxquelles l’état de la requête a été modifié<br>État de la requête précédente<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>}}*Nombre total de requête <br>}*Nombre total de requête *Nombre total de requêtes dont l’état de requête }}*Nombre total de requêtes dont l’état de requêtes dont l’état ont changé *Nom de la requête<br>*État de la requête précédente<br>*État de la nouvelle requête<br>*Nom de l’utilisateur qui a modifié l’état<br>*Date du résumé quotidien<br></td> 
   <td> <p><strong>Chaque jour</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
