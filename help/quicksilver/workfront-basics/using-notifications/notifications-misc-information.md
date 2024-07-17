---
content-type: reference
navigation-topic: notifications
title: "Notifications : informations diverses"
description: Les notifications suivantes vous alertent sur les activités qui se produisent sur un projet que vous sponsorisez.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 2%

---

# Notifications : informations diverses

Les notifications suivantes vous alertent sur les activités qui se produisent sur un projet que vous sponsorisez.

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voir aussi [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Vous ne pouvez pas activer ou désactiver les notifications quotidiennes et vous ne recevez pas de courriers électroniques condensés quotidiens pour les événements de cette catégorie. Vous pouvez activer ou désactiver des notifications instantanées individuelles pour la catégorie [!UICONTROL Divers].

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
   <td> <p><strong>Un message est envoyé au [!UICONTROL Annonce Center]</strong> </p> <p>Vous recevez une notification par e-mail lorsqu’un nouveau message a été envoyé au [!UICONTROL Annonce Center]. </p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL [!DNL Adobe Workfront] Annonce] : &lt;Objet de l’annonce&gt;</em></p> </td> 
   <td> Objet de l’annonce <br>Texte du message inclus dans l’annonce<br>Document(s) joint(s)<br>Nom de l’utilisateur qui a envoyé l’annonce<br>Date et heure d’envoi de l’annonce </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une modification de l’affectation d’une tâche affecte l’une de mes personnes</strong> </p> <p>Lorsque l’un des rapports directs d’un utilisateur désigné en tant que responsable est affecté à une nouvelle tâche, le responsable reçoit un courrier électronique à propos de l’affectation. </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Affectation de ressource de tâche] : &lt;Nom de la tâche&gt;</em></p> </td> 
   <td>Nom du projet<br>Nom de la tâche<br>Date et heure de création de la tâche<br>Nom de l’utilisateur qui a créé la tâche<br>Nom de l’affectation<br>Date d’échéance (date d’achèvement prévue)<br>État de la tâche<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Après avoir reçu une demande de téléchargement de document, la demande est annulée</strong> </p> <p>Le demandeur ou la demandeuse de document reçoit une notification par e-mail lorsqu’ une demande de document est annulée.</p> <p>L'objet de l'email de notification instantanée est : <em>&lt;Nom de l'utilisateur qui a annulé la demande&gt; a annulé la demande de document. </em></p> <p>Le texte suivant est inclus dans le corps de la notification électronique :</p> <p><em>[!UICONTROL Bonjour] &lt;Votre nom&gt;, <br><br>&lt;Nom de l’utilisateur qui a annulé la demande&gt;[!UICONTROL n’a plus besoin que vous téléchargiez quelque chose concernant la demande que vous avez reçue précédemment. Nous voulions juste vous le faire savoir.]</em> </p> </td> 
   <td>Nom de l’utilisateur qui a annulé la demande<br>Le texte de la demande de téléchargement de document d’origine<br>Une bannière "[!UICONTROL CANCELED]" sur la demande de document d’origine<br>Date et heure de la demande de document d’origine<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une erreur qui nécessite mon attention a été trouvée</strong> </p> <p>L'utilisateur qui répond à un commentaire par email reçoit une notification par email lorsque la réponse ne parvient pas à être diffusée.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Échec du traitement sur] &lt;objet du message d’origine&gt;</em></p> <p>Pour plus d’informations sur l’utilisation du courrier électronique pour répondre aux commentaires, voir <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Réponse aux notifications par courrier électronique</a>.</p> </td>
   <td> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une modification de l’affectation d’un problème affecte l’une de mes personnes</strong> </p> <p>Le responsable d’un utilisateur affecté à un problème reçoit une notification par courrier électronique lorsqu’il est supprimé d’un problème ou affecté à un problème. </p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>Attribution de problèmes : &lt;Nom du problème&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a effectué l’affectation<br>Type de problème<br>Nom de l’utilisateur affecté au problème<br>Date d’entrée du problème<br>Priorité du problème<br>Contact de Principal<br>Problème [!UICONTROL Date d’achèvement prévue]<br>État du problème<br><strong>[!UICONTROL Voir Plus de détails]</strong></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une de mes personnes est ajoutée à un projet</strong> </p> <p>Un responsable reçoit une notification par courrier électronique lorsqu’un de ses utilisateurs est ajouté à un projet. Cette notification est envoyée quel que soit l’état du projet. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>L’objet de l’e-mail est : <em>Attribution de projets : &lt;Nom utilisateur&gt;[&lt;GUID de projet&gt;_ &lt;GUID utilisateur&gt;]</em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a ajouté la personne au projet<br>Nom de l’utilisateur qui a été ajouté au projet<br>Date de début planifiée du projet]<br>Date de début prévue du projet [!UICONTROL Date d’achèvement prévue]<br>Pourcentage du projet terminé<br>Noms des autres sur le projet<br>État du projet<br>Propriétaire du projet{10 Bouton}[!UICONTROL Voir plus de détails]</strong><br><strong><br><br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un ajoute un projet à un portefeuille ou à un programme que je possède</strong> </p> <p>Le portefeuille et/ou le propriétaire du programme reçoivent une notification lorsqu’un nouveau projet est ajouté à un portfolio ou à un programme.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Projet ajouté à] &lt;nom du Portfolio&gt;[GUID du projet]</em></p> </td> 
   <td> Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a ajouté le projet au portefeuille/programme<br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un partage un objet avec moi</strong> </p> <p>Vous recevez une notification par e-mail lorsqu’une personne vous ajoute à la liste des autorisations de [!UICONTROL Partage] sur un objet.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Accès accordé]: &lt;Nom de l’objet&gt;</em></p> <p>Une notification N’est envoyée que si le projet est à l’état [!UICONTROL Actuel].</p> </td> 
   <td> Nom de l’objet <br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Accès initial à l’objet<br>Nouvel accès accordé à l’objet<br>Date et heure auxquelles l’accès a été accordé <br>Nom de l’utilisateur qui a accordé l’accès </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un partage un objet avec mon équipe</strong> </p> <p>Vous recevez une notification par e-mail lorsqu’une personne ajoute votre équipe à la liste des autorisations de partage sur un objet.</p> <p>L’objet de l’email de notification instantanée est : <em>[!UICONTROL Accès accordé]: &lt;Nom de l’objet&gt; [GUID de la règle d’accès]</em></p> </td> 
   <td> Nom de l’objet <br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Ancien accès<br>Nouvel accès<br>Date et heure auxquelles l’accès a été accordé<br>Nom de votre équipe<br>Nom de l’utilisateur qui a accordé l’accès </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une mise à jour est effectuée sur une tâche, un problème ou un projet auquel je suis abonné </strong> </p> <p>Vous recevez une notification par courrier électronique lorsqu’une personne fait un commentaire sur un article auquel vous êtes abonné.</p> <p>L’objet de l’email d’abonnement est : <em>[!UICONTROL Une mise à jour a été effectuée sur le] &lt;Type d’objet&gt; auquel vous êtes abonné : &lt;Nom de l’objet&gt;</em></p> </td> 
   <td> Nom de l’objet<br> Numéro de référence de l’objet<br> Nom de l’utilisateur qui a fait un commentaire sur l’élément abonné<br> Date à laquelle le commentaire a été fait<br> Commentaire ajouté à l’élément abonné.  </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
