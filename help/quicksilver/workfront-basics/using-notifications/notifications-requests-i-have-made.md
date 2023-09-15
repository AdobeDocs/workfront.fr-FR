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
ht-degree: 7%

---

# Notifications : demandes que j’ai effectuées

Les notifications suivantes vous informent sur les demandes que vous avez effectuées dans [!DNL Adobe Workfront].

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voir aussi [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Demandes que j'ai effectuées</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d'approbation du document est remplie</strong> </p> <p>L’utilisateur qui a demandé une approbation sur un document reçoit une notification par courrier électronique une fois la demande d’approbation terminée.</p> <p>L'objet de l'email de notification instantanée est le suivant :<em> &lt;approver name=""&gt; has &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; ce document.</em></p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </td> 
   <td> Document Name<br>Nom du validant </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un document est modifié ou chargé sur un problème pour lequel je suis le contact principal</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail lorsqu’un document est téléchargé ou modifié sur le problème, sauf si l’utilisateur qui a téléchargé ou modifié le document est également le contact principal.</p> <p>Une notification est envoyée uniquement si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de requête]</a>).</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Document ajouté à &lt;issue name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est : <em>Résumé de vos requêtes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom de l’objet dans lequel le document a été téléchargé.<br>Nom de l’objet parent<br>Numéro de référence du document<br>Nom de l’utilisateur qui a téléchargé le document.<br>Document Name<br>Ajout de la date "À"<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Téléchargement]</strong> boutons<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents téléchargés<br>*Nom du document<br>*Nom de l’objet parent<br>*Nom de l’utilisateur qui a ajouté le document<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande de chargement de document est honorée</strong> </p> <p>Le demandeur de document reçoit une notification par courrier électronique lorsqu’une demande de téléchargement de document est satisfaite.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Votre demande de document auprès de] &lt;user name=""&gt; a été accompli</em></p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </td> 
   <td> <p>Nom de l’utilisateur qui a téléchargé le document.<br>Nom de l’objet dans lequel le document a été téléchargé.<br>Document Name<br><br></p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche personnelle que j'ai affectée à quelqu'un d'autre est terminée</strong> </p> <p>Une notification est envoyée à l’utilisateur qui a assigné une tâche ad hoc à quelqu’un d’autre une fois cette tâche terminée. </p> <p>Pour plus d’informations sur les tâches ad hoc, voir <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Création d’éléments de travail à partir de la zone [!UICONTROL Accueil]</a>.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Fin de tâche : &lt;task name=""&gt;</em></p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> Task Name<br>Nom de projet par défaut (Projet personnel de l’utilisateur qui a reçu la tâche personnelle)<br>Numéro de référence de tâche<br>Nom du propriétaire de la tâche<br>New Task Status<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br><br><br></td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'un événement est conclu, envoyer un e-mail au créateur de l'événement</strong> </p> <p>Le contact principal sur un problème reçoit une notification une fois le problème terminé.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Fin du problème] : &lt;issue name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> Résumé de vos requêtes &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur ayant terminé le problème<br>Nouveau statut<br>Date et heure auxquelles le problème a été terminé<br>État du problème précédent<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom de l’utilisateur ayant terminé le problème<br>*Date du résumé quotidien </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'un événement est ajouté, envoyer un e-mail au créateur de l'événement.</strong> </p> <p>Le contact principal sur un problème reçoit une notification lorsqu’il ajoute un problème dans un projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Problème soumis] : &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> Résumé de vos requêtes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Votre nom<br>Nom du problème<br>Date de saisie<br>Priorité du problème<br>État du problème<br>Nom attribué<br>Contact Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés<br>*Nom du problème<br>*Date du résumé quotidien </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'une demande de bureau d'aide est ajoutée, envoyer un e-mail au créateur du problème.</strong> </p> <p>Le contact par Principal sur le problème reçoit une notification par courrier électronique lorsqu’il envoie un problème.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de requête]</a>).</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Demande envoyée] : &lt;request name=""&gt; on &lt;project request="" queue="" name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> Résumé de vos requêtes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nom du projet (nom de la file d’attente des demandes)<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom du problème<br>Date de saisie<br>Priorité du problème<br>État du problème<br>Nom attribué<br>Contact Principal<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total de demandes soumises<br>*Nom de la demande<br>*Priorité de la requête<br>*Date du résumé quotidien</p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'une demande de bureau d'aide est close, envoyer un e-mail au créateur du problème.</strong> </p> <p>Le contact principal du problème reçoit une notification par e-mail à la fermeture de la demande.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requête</a>).</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Votre demande a été fermée] :"&lt;request name=""&gt;"</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Résumé de vos requêtes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom de la requête<br>Nom du projet<br>Numéro de référence de la requête<br>Nom de l’utilisateur qui a fermé la requête<br>État du problème<br>Date et heure de fermeture de la requête<br>État de la requête précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total de demandes clôturées<br>*Nom de la demande<br>*Nom de l’utilisateur qui a fermé la demande<br>*Date du résumé quotidien </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'une demande de bureau d'aide est affectée, envoyer un e-mail au créateur du problème.</strong> </p> <p>Le contact principal de la question reçoit une notification par courrier électronique lorsqu’un utilisateur est affecté à la question, sauf si le contact principal et l’utilisateur affecté sont le même utilisateur.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de requête]</a>).</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL a été affecté à votre demande] : "&lt;request name=""&gt;"</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Résumé de vos requêtes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la requête<br>Type de requête<br>Date de saisie<br>Priorité du problème<br>Contact Principal<br>Date d’achèvement prévue<br>État du problème<br><strong>Voir Plus de détails</strong> button <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de demandes affectées<br>*Nom de la demande<br>*Attribué au nom<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le statut d'un projet est modifié, envoyer un e-mail à l'utilisateur qui a entré le projet</strong> </p> <p>L’utilisateur qui a créé le projet reçoit une notification par courrier électronique lorsque l’état du projet change.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Modification de l’état du projet] : &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Résumé de vos requêtes] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a modifié l’état<br>Nouveau statut<br>Date et heure de modification de l’état du projet<br>État précédent du projet<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nouveau état du projet<br>*Nom de l’utilisateur qui a modifié l’état du projet<br>*Date du résumé quotidien</p> </td> 
   <td> <p><strong>Instantané</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le statut est modifié dans une demande de bureau d'aide, envoyer un e-mail au créateur du problème.</strong> </p> <p>Le contact principal de la question reçoit une notification par courrier électronique lorsque l’état de la question change, sauf si l’utilisateur qui a modifié l’état est également le contact principal.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet est configuré en tant que [!UICONTROL File d’attente des demandes d’aide] (comme décrit dans la section <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Créer une file d’attente de requête]</a>).</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;request name=""&gt; is &lt;new status=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> Résumé de vos requêtes &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom de la requête<br>Nom du projet<br>Numéro de référence de la requête<br>Nom de l’utilisateur qui a modifié l’état de la requête<br>Nouveau statut<br>Date et heure de modification de l’état de la requête<br>État de la requête précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de demandes dont l’état a changé<br>*Nom de la demande<br>*État de la requête précédente<br>*New Request Status<br>*Nom de l’utilisateur qui a modifié l’état<br>*Date du résumé quotidien<br></td> 
   <td> <p><strong>Chaque jour</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
