---
content-type: reference
navigation-topic: notifications
title: "Notifications : informations sur les projets que je sponsorise"
description: Les notifications suivantes vous alertent sur les activités qui se produisent sur un projet que vous sponsorisez.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 6%

---

# Notifications : informations sur les projets que je sponsorise

Les notifications suivantes vous alertent sur les activités qui se produisent sur un projet que vous sponsorisez.

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Envoyer un e-mail au sponsor du projet lorsqu'un document est ajouté.</strong> </p> <p>Le parrain du projet reçoit une notification par courrier électronique lorsqu’un document est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et si le document n’est pas [!UICONTROL Privé].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Document ajouté à] &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Résumé des projets que vous sponsorisez] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du document<br>Nom de l’utilisateur qui a ajouté le document<br>Document Name<br>Ajout de la date "À"<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Téléchargement]</strong> boutons<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents ajoutés<br>*Nom du document<br>*Nom de l’utilisateur qui a ajouté le document<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au sponsor du projet lorsqu'une tâche jalonnée est terminée.</strong> </p> <p>Le parrain du projet reçoit une notification par courrier électronique lorsqu’une tâche de jalon est terminée sur un projet qu’il sponsorise.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>Remarque : Si la tâche est modifiée et passe à l’état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".<br></p> <p>L’objet de la notification quotidiennement Digest est :<em> Résumé des projets que vous sponsorisez &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Task Name<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>New Task Status<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Task Name<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand un projet passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au sponsor du projet</strong> </p> <p>Le parrain du projet reçoit une notification par e-mail lorsque le projet est en retard sur le planning. Un projet est en retard dans le calendrier lorsque l’état de progression est "[!UICONTROL En danger]" ou "[!UICONTROL En danger]".</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Modification de l’état d’avancement du projet] : &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est : <em>[!UICONTROL Résumé des projets que vous sponsorisez] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>État d’avancement du projet<br>[!UICONTROL Date de début planifiée] du projet<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Projet [!UICONTROL Date de début prévue]<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Pourcentage du projet terminé<br>État du projet<br>Propriétaire du projet<br>*Nom du projet<br>*Numéro de référence du projet<br>*État d’avancement du projet<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au sponsor du projet lorsqu'une tâche est terminée.</strong> </p> <p>Le sponsor du projet reçoit une notification par email.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Remarque : Si la tâche est modifiée et passe à l’état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".</p> </p> <p>L’objet de la notification quotidiennement Digest est :<em> Résumé des projets que vous sponsorisez &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Task Name<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>État de la tâche<br>Date et heure de modification de l’état de la tâche<br>État de la tâche précédente<br><strong>Voir Plus de détails</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Task Name<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand une tâche passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au sponsor du projet</strong> </p> <p>Le parrain du projet reçoit une notification par e-mail lorsqu’une tâche du projet est en retard sur le planning. Une tâche est en retard de planification lorsque l’état de progression est "[!UICONTROL En danger]" ou "[!UICONTROL Derrière]" ou "[!UICONTROL En retard]".</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Task Progress Change] : &lt;task name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Résumé des projets que vous sponsorisez] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Task Name<br>Nom du projet<br>Numéro de référence de tâche<br>Nouveau statut d’avancement de la tâche<br>Tâche [!UICONTROL Date de début planifiée]<br>Tâche [!UICONTROL Date d’achèvement prévue]<br>Tâche [!UICONTROL Date de début prévue]<br>Tâche [!UICONTROL Date d’achèvement prévue]<br>Pourcentage de la tâche terminé<br>État de la tâche<br>Nom attribué<br>Saisi par nom<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches en retard sur le planning<br>*Task Name<br>*Nom de l’utilisateur qui a participé à la tâche<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au sponsor du projet lorsqu'un événement est ajouté.</strong> </p> <p>Le parrain du projet reçoit une notification par courrier électronique lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Problème ajouté à] &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est : <em>[!UICONTROL Résumé des projets que vous sponsorisez] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom attribué <br>État du problème<br>Contact Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés au projet<br>*Nom du problème<br>*Nom de l’utilisateur affecté à la publication<br>*Date du résumé quotidien<br><br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au sponsor du projet lorsqu'un événement est conclu.</strong> </p> <p>Le sponsor du projet reçoit une notification par email.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> Résumé des projets que vous sponsorisez &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur ayant terminé le problème<br>État du problème<br>Date et heure auxquelles le problème a été terminé<br>État du problème précédent<br><strong>Voir Plus de détails</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom de l’utilisateur affecté à la publication<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au sponsor du projet lorsqu'un événement non affecté est ajouté.</strong> </p> <p>Le parrain du projet reçoit une notification par courrier électronique lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Qui doit être affecté à ce nouveau problème le] &lt;project name=""&gt;?</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Résumé des projets que vous sponsorisez] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom attribué (vide)<br>État du problème<br>Contact Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés<br>*Nom du problème<br>*Nom de l’utilisateur qui a ajouté le problème<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le sponsor du projet change ou lors de la création du projet, envoyer un e-mail au nouveau sponsor affecté</strong> </p> <p>Le sponsor du projet reçoit une notification par email lorsqu’il est défini comme sponsor d’un projet.<br></p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Project Sponsor] : &lt;project name=""&gt;</em></p> <p>Le texte suivant est inclus dans le corps de la notification électronique :</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL vous a fait parrainer] &lt;project name=""&gt;. [!UICONTROL En tant que parrain du projet, vous pouvez recevoir des notifications par e-mail supplémentaires sur l’activité du projet ou être impliqué dans l’approbation des travaux liés au projet. Bonne lecture.]</em> </p> <p>L’objet de la notification quotidiennement Digest est : <em>Résumé des projets que vous sponsorisez &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Date d’achèvement prévue du projet<br>*Nom du projet<br>*Numéro de référence du projet<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
 </tbody> 
</table>
