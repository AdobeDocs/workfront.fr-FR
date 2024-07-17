---
content-type: reference
navigation-topic: notifications
title: "Notifications : informations sur les projets que je possède"
description: Les notifications suivantes vous alertent sur les activités qui ont lieu sur un projet dont vous êtes responsable. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Modification de vos propres notifications par e-mail.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 9%

---

# Notifications : informations sur les projets dont je suis propriétaire

Les notifications suivantes vous alertent sur les activités qui ont lieu sur un projet dont vous êtes responsable. Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong> Un document est ajouté à un projet dont je suis propriétaire</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un document est ajouté au projet, sauf si la personne qui a ajouté le document est également propriétaire du projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et que le document n’est pas Privé.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Document ajouté à] &lt;Nom du projet&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a ajouté le document<br>Nom du document<br>ajouté à la date<br>Détails du document (format, taille, numéro de version)<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Télécharger]</strong><br>*Nom du projet<br> 2}*Nombre total de documents ajoutés<br>*Nom du document<br>*Nom de l’utilisateur ayant ajouté le document<br>*Date du résumé quotidien<br><br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche de jalon est terminée sur un projet dont je suis propriétaire</strong> </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Terminé] : &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p>Remarque : Si la tâche est modifiée et passe à l’état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".</p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>Nouvel état de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>}}}*Nom de la tâche}*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand un projet passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au propriétaire du projet</strong> </p> <p>Le propriétaire du projet reçoit une notification par e-mail lorsque le projet est en retard sur la planification. Un projet est en retard de planification lorsque l’état de progression est "[!UICONTROL En danger]", "[!UICONTROL Derrière]" ou "[!UICONTROL En retard]".</p> <p>La bonne pratique consiste à maintenir cette notification active. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Changement de progression du projet] : &lt;Nom du projet&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>État d’avancement du projet<br>Date de début planifiée du projet]<br>Date d’achèvement prévue du projet [!UICONTROL]<br>État d’avancement du projet [!UICONTROL Date de début prévue]<br>Date d’achèvement prévue du projet]<br>Pourcentage d’achèvement du projet<br>État du projet<br>Propriétaire du projet 0}*Nom du projet<br>*Numéro de référence du projet<br>*État d’avancement du projet<br>*Date du résumé quotidien<br><br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'un événement est ajouté.</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Problème ajouté à] &lt;Nom du projet&gt;</em></p> <p> </p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date d’entrée<br>Priorité du problème<br>Attribué au nom <br>État du problème<br>Contact du Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>}}*Nombre total du nombre total de problèmes ajouté au projet<br>}}}}}}}}}}*Nombre total de problèmes *Nom du problème<br>*Nom de l’utilisateur qui a ajouté le problème<br>*Date du résumé quotidien</p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche est terminée sur un projet dont je suis propriétaire</strong> </p> <p>Le propriétaire du projet reçoit une notification lorsqu’une tâche se termine sur son projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Terminé] : &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p> <p>Remarque : Si la tâche est modifiée et passe à l’état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".</p> </p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche <br>État de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées <br>*Nom de la tâche *Nom de la tâche<br> Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche sur un projet dont je suis propriétaire se trouve derrière</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’une tâche du projet est en retard sur le planning. Une tâche est en retard de planification lorsque l’état de progression est "[!UICONTROL En danger]" ou "[!UICONTROL Derrière]" ou "[!UICONTROL En retard]".</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Changement de progression de la tâche] : &lt;Nom de la tâche&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> Nom De La Tâche <br>Nom Du Projet<br>Numéro De Référence De La Tâche<br>État De La Nouvelle Tâche<br>Date De Démarrage Prévue De La Tâche]<br>Date D’Achèvement Prévue De La Tâche [!UICONTROL Date D’Achèvement Prévue]<br>État De La Tâche [!UICONTROL Date D’Achèvement Prévue]<br>Pourcentage De La Tâche<br>État De La Tâche<br>Nom Affecté 10}Entré par nom<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches en retard de planification<br>*Nom de la tâche<br>*Affecté à un nom<br>*Date du résumé quotidien<br><br> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème est terminé sur un projet dont je suis propriétaire</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un problème se termine sur son projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification. </p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Terminé] : &lt;Nom du problème&gt; sur &lt;Nom du projet&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a terminé le problème<br>État du problème<br>Date et heure auxquelles le problème a été terminé<br>État du problème précédent<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>}}*Nom du problème<br>}*Nom du projet*Nom de l’utilisateur affecté à la publication<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème non attribué est ajouté à un projet dont je suis propriétaire</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Qui doit être affecté à ce nouveau problème sur] &lt;Nom du projet&gt; ?</em></p> <p> </p> <p> L’objet de la notification de résumé quotidien est : <em> Résumé des projets que vous possédez &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date d’entrée<br>Priorité du problème<br>Affecté à un nom (vide)<br>État du problème<br>Contact du Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total}*État du problème Nombre total de problèmes de problèmes de problèmes de problèmes }}}}}}}}*Nombre total de problèmes de problèmes ajouté}}}}}*Nombre total de problèmes de problèmes de problèmes de problèmes <br> *Nom du problème<br>*Nom de l’utilisateur qui a ajouté le problème<br>*Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Je suis défini comme propriétaire d’un nouveau projet</strong> </p> <p>Lorsqu’un utilisateur ou une utilisatrice est désigné comme la personne propriétaire d’un projet, il ou elle reçoit une notification par e-mail.</p> <p>Si le propriétaire du projet est le même utilisateur que celui qui a effectué l’affectation, aucune notification par courrier électronique n’est envoyée.</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>Activez-le parce qu'ils sont affectés à quelque chose. </p> <p> Attribuer quelque chose, partager quelque chose, avoir accès à quelque chose.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Vous êtes maintenant le propriétaire du projet de] &lt;Nom du projet&gt;</em></p> <p>Le texte suivant est inclus dans le corps de la notification électronique :<em><br></em></p> <p><em>[!UICONTROL Bonjour] &lt;Votre nom&gt;,<br></em><em>&lt;Nom de l’utilisateur qui vous a affecté en tant que propriétaire du projet&gt; [!UICONTROL vous a désigné propriétaire de] &lt;Nom du projet&gt;. [!UICONTROL En tant que propriétaire du projet, vous pouvez recevoir des notifications par e-mail supplémentaires sur l’activité du projet, être tenu d’approuver les heures du projet ou être impliqué dans l’approbation des travaux liés au projet. Tout est à vous.]</em> </p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> <p> </p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Date d’achèvement du projet<br>*Nom du projet<br>*Numéro de référence du projet<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date de validation change pour une tâche sur l’un de mes projets</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement d’une tâche sur le projet est modifiée, sauf si l’utilisateur ou l’utilisatrice qui a modifié la date d’engagement est également la personne propriétaire du projet.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Date de validation pour] &lt;Nom de la tâche&gt; [!UICONTROL est maintenant] &lt;Nouvelle date de validation&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> Résumé des projets que vous possédez &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a modifié la date de validation<br>Date de nouvelle validation<br>Date de validation planifiée de la tâche]<br>Informations sur la façon dont la chronologie du projet est affectée par cette modification<br>Affectée à un nom<br>Entrée par le nom<br>Propriétaire du projet<br><strong>[!UICONTROL Voir plus de détails]{10 Bouton <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches dont la date de validation a changé<br>*Nom de la tâche<br>*Date du résumé quotidien</strong><br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date de validation change pour un problème sur l’un de mes projets</strong> </p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement d’un problème sur le projet change, sauf si la personne qui modifie la date d’engagement est la même que la personne propriétaire du projet.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Date de validation pour] &lt;Nom du problème&gt; [!UICONTROL est maintenant] &lt;Nouvelle date de validation&gt;</em></p> <p> L’objet de la notification de résumé quotidien est : <em> [!UICONTROL Résumé des projets que vous possédez] &lt;Date de résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a modifié la date de validation<br>Nouvelle date de validation<br>Date d’achèvement prévue du problème<br>Attribué au nom<br>Entré par nom<br>Propriétaire du projet<br><strong>[!UICONTROL Voir plus de détails]</strong>}<br>*Nom du projet<br>*Numéro de référence du projet<br>*Numéro de projet}}*Numéro de référence du projet}*Nombre total de problèmes dont la date de validation a changé<br>*Nom du problème<br>*Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
