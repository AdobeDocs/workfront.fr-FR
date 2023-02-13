---
content-type: reference
navigation-topic: notifications
title: 'Notifications : Informations sur les projets que je possède'
description: Les notifications suivantes vous alertent sur les activités qui ont lieu sur un projet dont vous êtes responsable. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Activation ou désactivation de vos propres notifications d’événement.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# Notifications : Informations sur les projets que je possède

Les notifications suivantes vous alertent sur les activités qui ont lieu sur un projet dont vous êtes responsable. Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Activation ou désactivation de vos propres notifications d’événement](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'un document est ajouté.</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un document est ajouté au projet, sauf si l’utilisateur qui a ajouté le document est également le propriétaire du projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et que le document n’est pas Privé.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Document ajouté à] &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a ajouté le document<br>Document Name<br>Ajout de la date "À"<br>Détails du document (format, taille, numéro de version)<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Téléchargement]</strong> boutons<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents ajoutés<br>*Nom du document<br>*Nom de l’utilisateur qui a ajouté le document<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'une tâche jalonnée est terminée.</strong> </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>Remarque : Si la tâche est modifiée et passe à un état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".</p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>New Task Status<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand un projet passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au propriétaire du projet</strong> </p> <p>Le propriétaire du projet reçoit une notification par e-mail lorsque le projet est en retard sur la planification. Un projet est en retard de planification lorsque l’état de progression est "[!UICONTROL En danger]", "[!UICONTROL Derrière]" ou "[!UICONTROL En retard]".</p> <p>La bonne pratique consiste à conserver cette notification principale. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Modification de la progression du projet] : &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>État d’avancement du projet<br>[!UICONTROL Date de début planifiée] du projet<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Projet [!UICONTROL Date de début prévue]<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Pourcentage du projet terminé<br>État du projet<br>Propriétaire du projet<br>*Nom du projet<br>*Numéro de référence du projet<br>*État d’avancement du projet<br>*Date du résumé quotidien<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'un événement est ajouté.</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Problème ajouté à] &lt;project name=""&gt;</em></p> <p> </p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom attribué <br>État du problème<br>Contact Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés au projet<br>*Nom du problème<br>*Nom de l’utilisateur qui a ajouté le problème<br>*Date du résumé quotidien</p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'une tâche est terminée</strong> </p> <p>Le propriétaire du projet reçoit une notification lorsqu’une tâche se termine sur son projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Remarque : Si la tâche est modifiée et passe à un état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".</p> </p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche <br>État de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées <br>*Nom de la tâche<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand une tâche passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au propriétaire du projet</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’une tâche du projet est en retard sur le planning. Une tâche est en retard de planification lorsque l’état de progression est "[!UICONTROL En danger]" ou "[!UICONTROL Derrière]" ou "[!UICONTROL En retard]".</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Task Progress Change] : &lt;task name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nouveau statut d’avancement de la tâche<br>Tâche [!UICONTROL Date de début planifiée]<br>Tâche [!UICONTROL Date d’achèvement prévue]<br>Tâche [!UICONTROL Date de début prévue]<br>Tâche [!UICONTROL Date d’achèvement prévue]<br>Pourcentage de la tâche terminé<br>État de la tâche<br>Nom attribué<br>Saisi par nom<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches en retard sur le planning<br>*Nom de la tâche<br>*Attribué au nom<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'un événement est terminé</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un problème se termine sur son projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification. </p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Complete] : &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur ayant terminé le problème<br>État du problème<br>Date et heure auxquelles le problème a été terminé<br>État du problème précédent<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom de l’utilisateur affecté à la publication<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail au propriétaire du projet lorsqu'un événement non affecté est ajouté.</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Qui doit être affecté à ce nouveau problème le] &lt;project name=""&gt;?</em></p> <p> </p> <p> L’objet de la notification quotidiennement Digest est : <em> Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom attribué (vide)<br>État du problème<br>Contact Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés<br>*Nom du problème<br>*Nom de l’utilisateur qui a ajouté le problème<br>*Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le propriétaire du projet change ou lors de la création du projet, envoyer un e-mail au nouveau propriétaire affecté</strong> </p> <p>Lorsqu’un utilisateur est désigné propriétaire d’un projet, il reçoit une notification par courrier électronique.</p> <p>Si le propriétaire du projet est le même utilisateur que celui qui a effectué l’affectation, aucune notification par courrier électronique n’est envoyée.</p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>Activez-le parce qu'ils sont affectés à quelque chose. </p> <p> Attribuer quelque chose, partager quelque chose, avoir accès à quelque chose.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Vous êtes maintenant le propriétaire du projet de] &lt;project name=""&gt;</em></p> <p>Le texte suivant est inclus dans le corps de la notification électronique :<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL vous a fait devenir propriétaire de] &lt;project name=""&gt;. [!UICONTROL En tant que propriétaire du projet, vous pouvez recevoir des notifications par e-mail supplémentaires sur l’activité du projet, être tenu d’approuver les heures du projet ou être impliqué dans l’approbation des travaux liés au projet. C'est tout à vous.]</em> </p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Date d’achèvement du projet<br>*Nom du projet<br>*Numéro de référence du projet<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque la date d'engagement pour une tâche est modifiée, envoyer un e-mail au propriétaire du projet</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsque la date de validation change pour une tâche du projet, sauf si l’utilisateur qui a modifié la date de validation est également le propriétaire du projet.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Date de validation pour] &lt;task name=""&gt; [!UICONTROL est maintenant] &lt;new commit="" date=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a modifié la date de validation<br>Nouvelle date de validation<br>Tâche [!UICONTROL Date d’achèvement prévue]<br>Informations sur l’impact de cette modification sur la chronologie du projet<br>Nom attribué<br>Saisi par nom<br>Propriétaire du projet<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches dont la date de validation a changé<br>*Nom de la tâche<br>*Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque la date d'engagement pour un événement est modifiée, envoyer un e-mail au propriétaire du projet</strong> </p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsque la date de validation change pour un problème sur le projet, sauf si l’utilisateur qui modifie la date de validation est le même que le propriétaire du projet.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Date de validation pour] &lt;issue name=""&gt; [!UICONTROL est maintenant] &lt;new commit="" date=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est : <em> [!UICONTROL Résumé des projets que vous possédez &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a modifié la date de validation<br>Nouvelle date de validation<br>Date d’achèvement prévue du problème<br>Nom attribué<br>Saisi par nom<br>Propriétaire du projet<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes dont la date de validation a changé<br>*Nom du problème<br>*Date du résumé quotidien<br></p> </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
