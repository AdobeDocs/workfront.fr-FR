---
content-type: reference
navigation-topic: notifications
title: 'Notifications : Informations diverses'''
description: Les notifications suivantes vous alertent sur les activités qui se produisent sur un projet que vous sponsorisez.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# Notifications : Informations diverses

Les notifications suivantes vous alertent sur les activités qui se produisent sur un projet que vous sponsorisez.

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Activation ou désactivation de vos propres notifications d’événement](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voir aussi [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Vous ne pouvez pas activer ou désactiver les notifications quotidiennes et vous ne recevez pas de courriers électroniques condensés quotidiens pour les événements de cette catégorie. Vous pouvez activer ou désactiver des notifications instantanées individuelles pour le [!UICONTROL Divers] catégorie.

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
   <td> <p><strong>Un message est envoyé au [!UICONTROL Annonce Center]</strong> </p> <p>Vous recevez une notification par e-mail lorsqu’un nouveau message a été envoyé au [!UICONTROL Annonce Center]. </p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL [!DNL Adobe Workfront] Annonce] : &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Objet de l'annonce<br>Texte du message inclus dans l’annonce<br>Document(s) joint(s)<br>Nom de l’utilisateur qui a envoyé l’annonce<br>Date et heure d’envoi de l’annonce </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En cas de modification de l'affectation primaire d'une tâche, envoyer un e-mail au propriétaire de la ressource</strong> </p> <p>Lorsque l’un des rapports directs d’un utilisateur désigné en tant que responsable est affecté à une nouvelle tâche, le responsable reçoit un courrier électronique à propos de l’affectation. </p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Task Resource Assignment] : &lt;task name=""&gt;</em></p> </td> 
   <td>Nom du projet<br>Nom de la tâche<br>Date et heure de création de la tâche<br>Nom de l’utilisateur qui a créé la tâche<br>Noms d’affectation<br>Date d’échéance (date d’achèvement prévue)<br>État de la tâche<br></td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Après réception de la demande de chargement de document, la demande est annulée</strong> </p> <p>L’utilisateur reçoit une notification par courrier électronique lorsqu’une demande de document est annulée.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; annulation de la demande de document. </em></p> <p>Le texte suivant est inclus dans le corps de la notification électronique :</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL n’a plus besoin que vous téléchargiez quelque chose à propos de la demande que vous avez reçue précédemment. Nous voulions juste vous le faire savoir.]</em> </p> </td> 
   <td>Nom de l’utilisateur qui a annulé la demande<br>Texte de la requête de téléchargement de document d’origine<br>Bannière "[!UICONTROL ANNULÉ]" sur la demande de document d’origine<br>Date et heure de la requête de document d’origine<br></td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une erreur a été détectée et requiert mon attention</strong> </p> <p>L'utilisateur qui répond à un commentaire par email reçoit une notification par email lorsque la réponse ne parvient pas à être diffusée.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Échec du traitement le] &lt;subject of="" original="" message=""&gt;</em></p> <p>Pour plus d’informations sur l’utilisation des emails pour répondre aux commentaires, voir .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>En cas de modification de l'affectation d'un événement, envoyer un e-mail au propriétaire de la ressource</strong> </p> <p>Le responsable d’un utilisateur affecté à un problème reçoit une notification par courrier électronique lorsqu’il est supprimé d’un problème ou affecté à un problème. </p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Attribution de problèmes : &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a effectué l’affectation<br>Type de problème<br>Nom de l’utilisateur affecté au problème<br>Date de publication saisie<br>Priorité du problème<br>Contact Principal<br>Problème [!UICONTROL Date d’achèvement prévue]<br>État du problème<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'un utilisateur est ajouté à une équipe de projet, envoyer un e-mail au propriétaire de la ressource</strong> </p> <p>Un responsable reçoit une notification par courrier électronique lorsqu’un de ses utilisateurs est ajouté à un projet. Cette notification est envoyée quel que soit l’état du projet. </p> <p>Les utilisateurs disposant d’une licence [!UICONTROL Review] ne reçoivent pas de notification.</p> <p>L'objet de l'email est le suivant : <em>Attribution de projets : &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a ajouté la personne au projet<br>Nom de l’utilisateur qui a été ajouté au projet<br>[!UICONTROL Date de début planifiée] du projet<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Pourcentage du projet terminé<br>Noms d’autres sur le projet<br>État du projet<br>Propriétaire du projet<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br><br><br></p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un ajoute un projet à un portefeuille ou un programme dont je suis propriétaire</strong> </p> <p>Le portefeuille et/ou le propriétaire du programme reçoivent une notification lorsqu’un nouveau projet est ajouté à un portfolio ou à un programme.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Projet [!UICONTROL ajouté à] &lt;portfolio name=""&gt;[GUID du projet]</em></p> </td> 
   <td> Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a ajouté le projet au portefeuille/programme<br><br></td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un partage un objet avec moi</strong> </p> <p>Vous recevez une notification par e-mail lorsqu’une personne vous ajoute à la liste des autorisations de [!UICONTROL Partage] sur un objet.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Accès accordé] : &lt;object name=""&gt;</em></p> <p>Une notification N’est envoyée que si le projet est à l’état [!UICONTROL Actuel].</p> </td> 
   <td> Nom de l’objet<br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Accès initial à l’objet<br>Nouvel accès accordé à l’objet<br>Date et heure auxquelles l’accès a été accordé <br>Nom de l’utilisateur qui a accordé l’accès </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un partage un objet avec mon équipe</strong> </p> <p>Vous recevez une notification par e-mail lorsqu’une personne ajoute votre équipe à la liste des autorisations de partage sur un objet.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Accès accordé] : &lt;object name=""&gt; [Accéder au GUID de règle]</em></p> </td> 
   <td> Nom de l’objet<br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Ancien accès<br>Accès<br>Date et heure auxquelles l’accès a été accordé<br>Nom de votre équipe<br>Nom de l’utilisateur qui a accordé l’accès </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une mise à jour est apportée à une tâche, un problème ou un projet auquel je suis abonné.</strong> </p> <p>Vous recevez une notification par courrier électronique lorsqu’une personne fait un commentaire sur un article auquel vous êtes abonné.</p> <p>L'objet de l'email d'abonnement est le suivant : <em>[!UICONTROL Une mise à jour a été apportée au] &lt;object type=""&gt; vous êtes abonné à : &lt;object name=""&gt;</em></p> </td> 
   <td> Nom de l’objet<br> Numéro de référence de l’objet<br> Nom de l’utilisateur qui a fait un commentaire sur l’élément abonné<br> Commentaire de date<br> Commentaire ajouté à l’élément abonné  </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
 </tbody> 
</table>
