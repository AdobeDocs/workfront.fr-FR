---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Types de notification d’événement
description: Les notifications d’événements sont des e-mails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches et des problèmes. Cet article répertorie et décrit les types de notifications d’événements disponibles.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '5201'
ht-degree: 97%

---

# Types de notifications d’événements

<!-- Audited: 1/2024 -->

Les notifications d’événements sont des e-mails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches et des problèmes, comme expliqué dans la section [Notifications d’événements](../../../workfront-basics/using-notifications/event-notifications.md).

Ces notifications peuvent être configurées au niveau du système et du groupe :

* Pour plus d’informations sur la configuration des notifications d’événements au niveau du système, voir [Configurer les notifications d’événement pour tous les utilisateurs et les utilisatrices du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Pour plus d’informations sur la configuration des notifications d’événements au niveau du groupe, voir [Afficher et configurer les notifications d’événements pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Les utilisateurs et utilisatrices individuels peuvent également activer et désactiver leurs notifications d’événements individuelles dans leur profil individuel. Pour plus d’informations, consultez [Modifier vos propres notifications par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Les tableaux suivants répertorient toutes les notifications d’événements Adobe Workfront, une brève description de l’événement et si l’événement est actif ou inactif par défaut.

>[!NOTE]
>
>Les notifications dont la valeur est &quot;Actif&quot; dans la colonne État par défaut sont actives par défaut pour les notifications instantanées et quotidiennes, sauf indication contraire.

## Action nécessaire

Voir aussi [Notifications : action nécessaire](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th>État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Demande d'accès</p> </td> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Quelqu’un me demande un accès</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> <p> </p> </td> 
   <td> <p>Ajout de demande de document</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel ou à laquelle le document est demandé</p> </td> 
   <td> <p>Quelqu’un m’a demandé de charger un ou des documents.</p> <p>Le demandeur ou la demandeuse de document reçoit une notification par e-mail lorsqu’il ou elle reçoit une demande de chargement d’un document.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document en attente d’approbation</p> </td> 
   <td> <p>Approbateurs</p> </td> 
   <td> <p>Je dois approuver un document.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Affectation de problème</p> </td> 
   <td> <p>L’utilisateur ou l’utilisatrice auquel ou à laquelle ce problème est affecté</p> </td> 
   <td> <p>On m’affecte à un problème.</p> <p>La personne désignée pour le problème ne reçoit une notification par e-mail que si le projet est Actuel et que le statut du problème n’est pas Fermé ou similaire à Fermé.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light, de contributeur ou contributrice, révision ou demande ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Événement en attente d'approbation</p> </td> 
   <td> <p>Approbateurs</p> </td> 
   <td> <p>Je dois approuver un problème.</p> <p>Les utilisateurs et les utilisatrices qui reçoivent une notification par e-mail pour cet événement varient selon que le paramètre « L’approbateur ou l’approbatrice ne doit pas nécessairement faire partie de l’équipe du projet (pour les processus d’approbation incluant un rôle » est activé ou désactivé (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer les paramètres d’approbation globaux</a>). </p> <p>Si cette option est activée</strong>, une notification par e-mail est envoyée à tous les utilisateurs et à toutes les utilisatrices du système ayant la fonction « Approbateur ou approbatrice ».</p> <p>Si cette option est désactivée</strong>, seules les personnes membres de l’équipe du projet ayant la fonction « Approbateur ou approbatrice » reçoivent une notification par e-mail.</p> <p>Une notification est envoyée si le projet est au statut Planification ou Actuel. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Événement en attente d'approbation</p> </td> 
   <td> <p>Approbateur ou approbatrice délégué</p> </td> 
   <td> <p>Je dois passer en revue une approbation de problème qui m'a été déléguée.</p> <p>Lorsqu’une personne délègue l’approbation d’un problème à un autre utilisateur ou une autre utilisatrice, cet utilisateur ou cette utilisatrice en est informé. </p> <p>Une notification n’est envoyée que lorsque le projet est au statut Actuel.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Projet en attente d'approbation</p> </td> 
   <td> <p>Approbateurs</p> </td> 
   <td> <p>Je dois approuver un projet.</p> <p>Les utilisateurs et les utilisatrices qui reçoivent une notification par e-mail pour cet événement varient selon que le paramètre « L’approbateur ou l’approbatrice ne doit pas nécessairement faire partie de l’équipe de projet (pour les processus d’approbation incluant un rôle) » est activé ou désactivé (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer les paramètres d’approbation globaux</a>).</p> <p>Si cette option est activée</strong>, une notification par e-mail est envoyée à tous les utilisateurs et à toutes les utilisatrices du système ayant la fonction « Approbateur ou approbatrice ».</p> <p>Si cette option est désactivée</strong>, seules les personnes membres de l’équipe du projet ayant la fonction « Approbateur ou approbatrice » reçoivent une notification par e-mail.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Projet en attente d'approbation</td> 
   <td>Approbateur ou approbatrice délégué</td> 
   <td> <p>J’ai besoin de vérifier une approbation de projet qui m’a été déléguée.</p> </td> 
   <td> Actif</td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Affectation de tâche</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel ou à laquelle la tâche est affectée</p> </td> 
   <td> <p>Je suis la personne cessionnaire principale d’une tâche.</p> <p>La personne cessionnaire d’une tâche reçoit une notification par e-mail si elle est désignée comme personne cessionnaire principale de la tâche, sauf si la personne cessionnaire est l’utilisateur ou l’utilisatrice qui a effectué l’affectation.</p> <p>Une notification est envoyée si le statut du projet est Actuel et que la tâche n’est pas marquée comme terminée.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Tâche en attente d'approbation</p> </td> 
   <td> <p>Approbateurs</p> </td> 
   <td> <p>Je dois approuver une tâche.</p> <p>Les utilisateurs et les utilisatrices qui reçoivent une notification par e-mail pour cet événement varient selon que le paramètre « L’approbateur ou l’approbatrice ne doit pas nécessairement faire partie de l’équipe de projet (pour les processus d’approbation incluent un rôle) » est activé ou désactivé (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer les paramètres d’approbation globaux</a>). </p> <p>Si cette option est activée</strong>, une notification par e-mail est envoyée à tous les utilisateurs et à toutes les utilisatrices du système ayant la fonction « Approbateur ou approbatrice ».</p> <p>Si cette option est désactivée</strong>, seules les personnes membres de l’équipe du projet ayant la fonction « Approbateur ou approbatrice » reçoivent une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel au moment de la demande.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Tâche en attente d'approbation</p> </td> 
   <td> <p>Approbateur ou approbatrice délégué</p> </td> 
   <td> <p>J’ai besoin de vérifier une approbation de tâche qui m’a été déléguée.</p> <p>Lorsqu’une personne délègue l’approbation d’un problème à un autre utilisateur ou une autre utilisatrice, cet utilisateur ou cette utilisatrice en est informé. </p> <p>Une notification n’est envoyée que si le statut du projet est Actuel au moment de la demande.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Feuille de temps rouverte</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel ou à laquelle la feuille de temps appartient</p> </td> 
   <td> <p>Ma feuille de temps est rouverte.</p> <p>La personne propriétaire de la feuille de temps reçoit une notification par e-mail lorsque la feuille de temps est rouverte, sauf si la personne qui a rouvert la feuille de temps est également propriétaire de la feuille de temps.</p> <p>Une notification par e-mail n’est envoyée que si le statut de la feuille de temps est Ouverte.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Rejet de la feuille de temps</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel ou à laquelle la feuille de temps appartient</p> </td> 
   <td> <p>Ma feuille de temps est rejetée.</p> <p>Le ou la propriétaire de la feuille de temps reçoit une notification par e-mail lorsque la feuille de temps est rejetée, sauf si la personne qui a rejeté la feuille de temps est également la propriétaire.</p> <p>Une notification par e-mail n’est envoyée que si le statut de la feuille de temps est Rejeté.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Envoi de la feuille de temps</p> </td> 
   <td> <p>Approbateur</p> </td> 
   <td> <p>Je dois approuver une feuille de temps.</p> <p>La personne approbatrice de la feuille de temps reçoit une notification par e-mail lorsqu’une feuille de temps qu’elle doit approuver est envoyée, sauf si l’utilisateur ou l’utilisatrice qui l’a envoyée est également l’approbateur ou l’approbatrice de la feuille de temps.</p> <p>Une notification n’est envoyée que si le statut de la feuille de temps est Envoyé.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affectation</p> </td> 
   <td> <p>Demande d’élément de travail</p> </td> 
   <td> <p>Membres de l’équipe pour lesquels l’élément est demandé</p> </td> 
   <td> <p>Mon équipe reçoit une nouvelle demande de travail.</p> <p>Les personnes membres de l’équipe reçoivent une notification par e-mail lorsque l’équipe reçoit une nouvelle demande de travail. (La personne qui a soumis la demande ne reçoit pas de notification si elle est membre de l’équipe.)</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel au moment de la demande de travail et que le statut de la demande de travail est Nouvelle.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affectation</p> </td> 
   <td> <p>Demande d’élément de travail</p> </td> 
   <td> <p>Utilisateur ou utilisatrice pour lequel ou laquelle l’élément de travail est demandé</p> </td> 
   <td> <p>Je reçoit une nouvelle nouvelle demande de travail.</p> <p>La personne cessionnaire de l’élément de travail reçoit une notification par e-mail, sauf si la personne qui dépose la demande est également la personne cessionnaire. </p> <p>La notification n’est pas envoyée si le statut de la tâche est Terminé ou si le statut du problème est Fermé.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel au moment de la demande.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Demandes que j’ai effectuées

Voir aussi [Notifications : demandes que j’ai effectuées](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Changement de statut d’approbation de document</p> </td> 
   <td> <p>Demandeur</p> </td> 
   <td> <p>Une demande d’approbation de document est remplie.</p> <p>Le demandeur ou la demandeuse de document reçoit une notification par e-mail lorsque la demande d’approbation de document est remplie.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Demande de document remplie</p> </td> 
   <td> <p>Demandeur</p> </td> 
   <td> <p>Une demande de chargement de document est honorée.</p> <p>Le demandeur ou la demandeuse de document reçoit une notification par e-mail lorsqu’une demande de chargement d’un document est honorée.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout de problème</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>J’ajoute un problème à un projet.</p> <p>Le contact principal sur un problème reçoit une notification lorsqu’il ajoute un problème dans un projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>Affectation de problème</td> 
   <td>Contact principal du problème</td> 
   <td> <p>Une personne a été affectée à un problème dont je suis le contact principal.</p> <p>Le contact principal sur un problème reçoit une notification lorsque le problème est affecté à un utilisateur ou une utilisatrice. </p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> Inactif</td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement de problème</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>Un problème dont je suis le contact principal est terminé.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut de projet</p> </td> 
   <td> <p>Utilisateur ou utilisatrice ayant créé le projet (Entré par)</p> </td> 
   <td> <p>Le statut d’un projet que j’ai créé a changé.</p> <p>La personne qui a créé le projet reçoit une notification par e-mail lorsque le statut du projet change.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout de demande</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>J’envoie une demande (confimation).</p> <p>Le contact principal sur le problème reçoit une notification par e-mail lorsqu’un problème est envoyé.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si le projet utilise une vue « Est le Help Desk ».</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Affectation de demande</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>Une personne est affectée à ma demande.</p> <p>Le contact principal du problème reçoit une notification par e-mail lorsqu’une personne est affectée au problème, sauf si le contact principal et la personne affectée sont le même utilisateur ou la même utilisatrice.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si le projet utilise une vue « Est le Help Desk ».</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Demande close</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>Ma demande est close.</p> <p>Le contact principal du problème reçoit une notification par e-mail lorsque la demande est close.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si le projet utilise une vue « Est le Help Desk ».</p> <p>Si les notifications d’« achèvement de problème » sont activées, elles se déclenchent toujours au lieu de la « demande au contact principal du problème close ». Si vous souhaitez que cette notification se déclenche, vous devez désactiver les notifications d’« achèvement de problème ».</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de demande de document</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>Un document est modifié ou chargé sur un problème pour lequel je suis le contact principal.</p> <p>Le contact principal du problème reçoit une notification par e-mail lorsqu’un document est chargé ou modifié sur le problème, sauf si la personne qui a chargé ou modifié le document est également le contact principal.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si l’option « Publier en tant que file d’attente des demandes d’aide » est activée pour le projet dans l’onglet Configuration de la file d’attente.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut de demande</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>Le statut dans ma demande change.</p> <p>Le contact principal du problème reçoit une notification par e-mail lorsque le statut du problème change, sauf si l’utilisateur ou l’utilisatrice qui a modifié le statut est également le contact principal.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et que le projet utilise une vue « Est le Help Desk ».</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Communication

Voir aussi [Notifications : communication](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Commentaire sur le document</p> </td> 
   <td> <p>Propriétaire du document</p> </td> 
   <td> <p>Un commentaire a été ajouté sur mon document.</p> <p>La personne propriétaire d’un document dans Workfront reçoit une notification par e-mail lorsqu’un commentaire est publié sur le document, sauf si l’utilisateur ou l’utilisatrice qui a publié le commentaire est également la personne propriétaire du document.</p> <p>Tous les utilisateurs et toutes les utilisatrices qui sont directement inclus dans le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel. </p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Commentaire sur &lt;Nom de la demande&gt; sur &lt;Nom du projet&gt; (réf# &lt;Numéro de référence de la demande&gt;)</em>.</p> <p> L’objet de la notification de synthèse quotidienne est : <em>Synthèse de la communication &lt;Date de synthèse quotidienne&gt;</em>.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Ajout de note de demande</p> </td> 
   <td> <p>Contact principal du problème</p> </td> 
   <td> <p>Lorsqu’un commentaire est publié sur une demande, envoyez un e-mail au contact principal du problème.</p> <p>Le contact principal d’un problème reçoit une notification par e-mail lorsqu’un commentaire est publié sur une demande, sauf si l’utilisateur ou l’utilisatrice qui a publié le commentaire est également le contact principal du problème.</p> <p>Tous les utilisateurs et toutes les utilisatrices qui sont directement inclus dans le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td>Mise à jour dirigée</td> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Une personne m’a inclus dans une mise à jour dirigée.</p> <p>Une mise à jour dirigée réside dans le fait qu’une personne inclut spécifiquement un autre utilisateur ou une autre utilisatrice dans une mise à jour, comme décrit dans <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Taguer d’autres personnes sur les mises à jour</a>.</p> <p>Dans ce cas, l’utilisateur ou l’utilisatrice qui est inclus dans la mise à jour dirigée reçoit une notification par e-mail concernant la mise à jour.</p> <p>La notification par e-mail n’est envoyée que si l’utilisateur ou l’utilisatrice dispose de droits d’accès à l’objet et s’il la garde activée dans son profil.  </p> <p>Cette notification d’événement est activée par défaut et ne peut pas être désactivée.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Mise à jour dirigée</p> </td> 
   <td> <p>Membres d'équipe</p> </td> 
   <td> <p>Une personne inclut mon équipe dans une mise à jour dirigée.</p> <p>Une mise à jour dirigée réside dans le fait qu’une personne inclut spécifiquement un autre utilisateur ou une autre utilisatrice dans une mise à jour, comme décrit dans <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Taguer d’autres personnes sur les mises à jour</a>.</p> <p>Dans ce cas, tout membre de l’équipe inclus dans la mise à jour dirigée reçoit une notification par e-mail concernant la mise à jour.</p> <p>La notification par e-mail n’est envoyée qu’aux utilisateurs et utilisatrices disposant de droits d’accès à l’objet de la mise à jour.</p> <p>Si la personne qui envoie la mise à jour dirigée est un membre de l’équipe en cours d’inclusion, la personne qui envoie la mise à jour ne reçoit pas de notification par e-mail.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Commentaire sur l’élément de travail</p> </td> 
   <td> <p>Participantes et participants au thread</p> </td> 
   <td> <p>Quelqu’un commente un thread auquel je participe.</p> <p>Les participantes et participants au thread et les utilisateurs et utilisatrices inclus dans un message direct reçoivent une notification par e-mail lorsqu’une personne fait un commentaire dans le thread.</p> <p>Les utilisateurs et utilisatrices doivent disposer d’un accès en affichage pour recevoir une notification.</p> <p>Les utilisateurs et utilisatrices suivants ne reçoivent pas de notification :</p> 
    <ul> 
     <li> <p>Équipes incluses dans un message direct</p> </li> 
     <li> <p>Personne propriétaire de la note</p> </li> 
     <li> <p>Contact principal</p> </li> 
    </ul> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Commentaire sur l’élément de travail</p> </td> 
   <td> <p>Personne cessionnaire d’élément de travail</p> </td> 
   <td> <p>Une personne commente l’un de mes éléments de travail.</p> <p>La personne cessionnaire de l’élément de travail reçoit une notification par e-mail chaque fois qu’une personne ajoute une mise à jour à un élément de travail, sauf si la personne qui ajoute la mise à jour est également la personne cessionnaire.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Réponse à la demande de travail</p> </td> 
   <td> <p> Demandeuse ou demandeur de travail</p> </td> 
   <td> <p>Une personne répond à ma demande.</p> <p>Une fois qu’un utilisateur ou une utilisatrice a envoyé une demande et qu’une autre personne a répondu à cette demande, l’utilisateur ou l’utilisatrice qui a envoyé la demande reçoit une notification par e-mail.</p> <p>Une notification par e-mail n’est pas envoyée si :</p> 
    <ul> 
     <li> <p>L’utilisateur ou l’utilisatrice qui envoie la réponse est la même personne que celle qui a effectué la demande.</p> </li> 
     <li> <p>L’utilisateur ou l’utilisatrice n’a pas accès en affichage à la note.</p> </li> 
    </ul> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Informations d’approbation

Voir aussi [Notifications : informations d’approbation](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Délégation d'approbation</p> </td> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>J’ai reçu une délégation en tant que personne approbatrice.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut de l'approbation d'événement déléguée</p> </td> 
   <td> <p>Utilisateur ou utilisatrice ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation de problème déléguée a été remplie. </p> <p>Lorsque vous déléguez l’approbation d’un problème à une autre personne, vous recevez une notification par e-mail une fois cette approbation terminée (qu’elle approuve ou rejette l’approbation du problème). </p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut de l'approbation de projet déléguée</p> </td> 
   <td> <p>Utilisateur ou utilisatrice ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation de projet déléguée a été remplie.</p> <p>Lorsque vous déléguez l’approbation d’un projet à une autre personne, vous recevez une notification par e-mail une fois cette approbation terminée (qu’elle approuve ou rejette l’approbation du projet).</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Changement de statut de l'approbation de tâche déléguée</p> </td> 
   <td> <p>Utilisateur ou utilisatrice ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation de tâche déléguée a été remplie.</p> <p>Lorsque vous déléguez l’approbation d’une tâche à une autre personne, vous recevez une notification par e-mail une fois cette approbation terminée (qu’elle approuve ou rejette l’approbation de la tâche).</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Annuler l'approbation du document pour l'approbateur</p> </td> 
   <td> <p>Utilisateur ou utilisatrice ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation de document a été annulée.</p> <p>L’approbateur ou l’approbatrice du document reçoit une notification par e-mail lorsque la demande d’approbation du document est annulée.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Approbation de feuille de temps</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel ou à laquelle la feuille de temps appartient</p> </td> 
   <td> <p>Ma feuille de temps est approuvée.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur le travail qui m’a été affecté

Voir aussi [Notifications : informations sur le travail qui m’a été affecté](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Tâche</td> 
   <td>Achèvement de toutes les tâches antérieures</td> 
   <td>Membres de l’équipe affectés aux tâches dépendantes</td> 
   <td> <p>Toutes les tâches antérieures des tâches de l’équipe sont terminées.</p> <p>Les personnes cessionnaires de la tâche (tous les membres de l’équipe) reçoivent une notification par e-mail.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td>Inactif</td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de toutes les tâches antérieures</p> </td> 
   <td> <p>Utilisateur ou utilisatrice affecté aux tâches dépendantes</p> </td> 
   <td> <p>Toutes les tâches antérieures de mes tâches sont terminées.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Décision d’approbation</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel le problème est affecté</p> </td> 
   <td> <p>Un problème que j’ai résolu est approuvé ou rejeté</p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsqu’une décision d’approbation est prise (approuvée ou rejetée).</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Décision d’approbation</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel la tâche est affectée</p> </td> 
   <td> <p>Une tâche que j’ai terminée est approuvée ou rejetée.</p> <p>La personne cessionnaire pour la tâche reçoit une notification par e-mail lorsque la tâche est approuvée ou refusée.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement de problème</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel le problème est affecté</p> </td> 
   <td> <p>Un problème qui m’a été affecté est terminé.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>La date d'achèvement planifiée pour l'événement a changé</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel le problème est affecté</p> </td> 
   <td> <p>La date d’échéance d’un problème qui m’a été affecté est modifiée.</p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsque la date d’achèvement prévue est modifiée, sauf si l’utilisateur ou l’utilisatrice qui a modifié la date d’achèvement prévue est également la personne cessionnaire.</p> <p>Une notification n’est envoyée que si le statut du projet est autre que Planification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut de problème</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel le problème est affecté</p> </td> 
   <td> <p>Le statut de l’un de mes éléments de travail a changé.</p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsque le statut est modifié, sauf si l’utilisateur ou l’utilisatrice qui a modifié le statut est également la personne cessionnaire.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de demande de document</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel le problème est affecté</p> </td> 
   <td> <p>Des documents sont chargés ou modifiés sur des demandes qui me sont affectées.</p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsque des documents sont chargés ou ont été modifiés sur un problème qu’elle a ajouté.</p> <p>Une notification par e-mail n’est pas envoyée si la personne qui a entré le problème est la personne cessionnaire du problème.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si l’option « Publier en tant que file d’attente des demandes d’aide » est activée pour le projet dans l’onglet Configuration de la file d’attente.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel la tâche est affectée</p> </td> 
   <td> <p>Une tâche qui m’a été affectée est terminée.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque la tâche est terminée. Les notifications ne sont pas envoyées lorsqu’une tâche personnelle est terminée.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light, de contributeur ou contributrice, révision ou demandeuse ou demandeur ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche</p> </td> 
   <td> <p>Utilisateur ou utilisatrice affecté à une tâche dépendante</p> </td> 
   <td> <p>Une tâche antérieure de l’une des mes tâches est terminée.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque l’une des tâches antérieures de ses tâches est terminée.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>La date d'achèvement prévue pour la tâche a changé</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel la tâche est affectée</p> </td> 
   <td> <p>La date d’échéance d’une tâche qui m’a été affectée est modifiée.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque la date d’achèvement prévue de la tâche est modifiée, sauf si l’utilisateur ou l’utilisatrice qui a modifié la date d’achèvement prévue est également la personne cessionnaire de la tâche.</p> <p>Une notification n’est envoyée que si le statut du projet est autre que Planification.</p> <p>Aucune notification n’est envoyée concernant les tâches personnelles.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Changement de statut de la tâche</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel la tâche est affectée</p> </td> 
   <td> <p>Le statut est modifié sur une tâche qui m’a été affectée.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque le statut de la tâche est modifié, sauf si l’utilisateur ou l’utilisatrice qui a modifié le statut est également la personne cessionnaire.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Informations sur les projets auxquels je participe

Voir aussi [Notifications : informations sur les projets auxquels je participe](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Statut de projet Actuel</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un projet sur lequel je travaille devient actif.</p> <p>Les utilisateurs et utilisatrices sur le projet reçoivent une notification par e-mail lorsque le projet devient actif.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un document est ajouté au projet sur lequel je travaille.</p> <p>Les utilisateurs et utilisatrices de l’équipe de projet reçoivent une notification par e-mail lorsqu’un document est ajouté au projet, à l’exception de l’utilisateur ou l’utilisatrice qui a ajouté le document.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si le document n’est pas Privé. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout de problème</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet sur lequel je travaille.</p> <p>Les utilisateurs et utilisatrices d’un projet reçoivent une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement de problème</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un problème sur un projet sur lequel je travaille est résolu.</p> <p>Toute personne sur le projet reçoit une notification.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche jalonnée</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Une tâche jalonnée sur un projet sur lequel je travaille est terminée.</p> <p>Toutes les personnes de l’équipe de projet reçoivent une notification lorsqu’une tâche jalonnée est terminée. </p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Achèvement de projet</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un projet sur lequel je travaille est terminé.</p> <p>Les utilisateurs et utilisatrices d’une équipe de projet reçoivent une notification par e-mail lorsque le statut du projet est Terminé.</p> <p>Conseil : si les projets sont terminés régulièrement, l’activation de cette option peut générer un grand nombre d’e-mails pour les utilisateurs et utilisatrices qui ont un nombre limité de tâches sur de nombreux projets. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut de projet</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Le statut d’un projet sur lequel je travaille est modifié.</p> <p>Les utilisateurs et utilisatrices de l’équipe de projet reçoivent une notification par e-mail lorsque le statut du projet change. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur du projet</p> </td> 
   <td> <p>Ajout d’utilisateur et d’utilisatrice de projet</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>J’ai été ajouté à un projet.</p> <p>L’utilisateur ou l’utilisatrice qui a été ajouté au projet reçoit une notification par e-mail lorsqu’il ou elle est ajouté, sauf s’il ou elle s’est ajouté lui-même ou elle-même au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Une tâche sur un projet sur lequel je travaille est terminée.</p> <p>Les membres de l’équipe de projet reçoivent une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Problème non affecté ajouté</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un problème non affecté est ajouté à un projet sur lequel je travaille.</p> <p>Les utilisateurs et utilisatrices d’un projet reçoivent une notification par e-mail lorsqu’un problème non affecté est ajouté au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur les projets dont je suis propriétaire

Voir aussi [Notifications : informations sur les projets dont je suis propriétaire](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un document est ajouté à un projet dont je suis propriétaire.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un document est ajouté au projet, sauf si la personne qui a ajouté le document est également propriétaire du projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si le document n’est pas Privé.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout de problème</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet dont je suis propriétaire.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Modification de la date d'engagement pour l'événement</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>La date d’engagement d’un problème sur l’un de mes projets est modifiée.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement d’un problème sur le projet change, sauf si la personne qui modifie la date d’engagement est la même que la personne propriétaire du projet.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement de problème</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un problème sur un projet dont je suis propriétaire est terminé.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche jalonnée</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Une tâche jalonnée sur un projet dont je suis propriétaire est terminée.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Affectation de propriétaire de projet</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Je suis désigné comme la personne propriétaire d’un nouveau projet.</p> <p>Lorsqu’un utilisateur ou une utilisatrice est désigné comme la personne propriétaire d’un projet, il ou elle reçoit une notification par e-mail.</p> <p>Si la personne propriétaire du projet est la même personne que celle qui a effectué l’affectation, aucune notification par e-mail n’est envoyée.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Modification de la progression du projet</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un projet que je possède est en retard.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque le projet est en retard par rapport au planning.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la date d'engagement pour la tâche</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>La date d’engagement pour une tâche d’un de mes projets est modifiée.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement d’une tâche sur le projet est modifiée, sauf si l’utilisateur ou l’utilisatrice qui a modifié la date d’engagement est également la personne propriétaire du projet.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Une tâche est terminée sur un projet que je possède.</p> <p>La personne propriétaire du projet reçoit une notification. </p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la progression de la tâche</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Une tâche d’un projet que je possède est en retard.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’une tâche du projet est en retard sur le planning.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème non attribué</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un problème non attribué est ajouté à un projet que je possède.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur les projets que je sponsorise

Voir aussi [Notifications : informations sur les projets que je sponsorise](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un document est ajouté à un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’un document est ajouté au projet, sauf si le document est ajouté par la personne sponsor du projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel et si le document n’est pas Privé.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout de problème</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un problème est ajouté au projet que je sponsorise</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement de problème</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un problème est résolu sur un projet que je sponsorise</p> <p>La personne sponsor du projet reçoit une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche jalonnée</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Envoyer un e-mail à la personne sponsor du projet lorsqu’une tâche jalonnée est terminée.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’une tâche jalonnée est terminée sur un projet qu’elle sponsorise.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Modification de la progression du projet</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un projet que je sponsorise est en retard.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsque le projet est en retard par rapport au planning.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Affectation de la personne sponsor du projet</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Je sponsorise un projet.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’elle est définie comme sponsor d’un projet.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Une tâche jalonnée est terminée dans un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la progression de la tâche</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un tâche d’un projet que je sponsorise est en retard.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’une tâche du projet est en retard sur le planning.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème non attribué</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un problème non attribué est ajouté à un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations diverses

Voir aussi [Notifications : informations diverses](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Annonce</td> 
   <td> <p>L'annonce a été ajoutée</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Un message est envoyé au Centre des annonces.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Annulation de demande de documents</p> </td> 
   <td> <p>Utilisateur ou utilisatrice auquel ou à laquelle le document est demandé</p> </td> 
   <td> <p>Annuler une demande de chargement de documents de ma part.</p> <p>Le demandeur ou la demandeuse de document reçoit une notification par e-mail lorsqu’ une demande de document est annulée.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Notification d'erreur</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Une erreur a été détectée et requiert votre attention</p> <p>Une notification par e-mail est générée une fois que Workfront a tenté de se connecter à un compte POP sans y parvenir. Après 25 tentatives, Workfront désactive la connexion au compte POP afin de préserver les ressources et envoie une notification. </p> <p>La notification est envoyée par e-mail à la personne propriétaire du projet, si l’e-mail POP est associé à une file d’attente des demandes, ou à l’équipe d’administration Workfront, si le compte POP est associé à la fonction « Courrier entrant » dans la configuration de la messagerie.
   </p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Affectation de problème</p> </td> 
   <td> <p>Propriétaire de la ressource</p> </td> 
   <td> <p>L’attribution d’un problème affecte une personne dont je suis responsable.</p> <p>Le Gestionnaire des cessionnaires des problèmes reçoit une notification par e-mail lorsqu’une modification affecte un utilisateur ou une utilisatrice sous sa responsabilité.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Nouvel utilisateur</p> </td> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Lorsqu’un utilisateur ou une utilisatrice est créé dans Workfront, envoyez-lui un e-mail.</p> <p>Une fois créé, l’utilisateur ou l’utilisatrice reçoit une invitation par e-mail l’informant qu’un compte Workfront a été créé et lui demandant de configurer son mot de passe.</p> <p>Lors de la création d’un utilisateur ou d’une utilisatrice, les utilisateurs et utilisatrices peuvent sélectionner l’option « Envoyer un e-mail d’invitation à cette personne » (comme décrit dans la section <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajouter des utilisateurs et utilisatrices</a><span style="font-weight: 400;">). Cependant, lorsque l’option « Nouvel utilisateur ou utilisatrice à utilisateur ou utilisatrice » est activée globalement, les nouveaux utilisateurs et utilisatrices reçoivent l’invitation par e-mail, que l’option « Envoyer un e-mail d’invitation à cette personne » soit sélectionnée ou non.</span></p> </td> 
   <td> Inactif </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Partage d’objets</p> </td> 
   <td> <p>Membres de l’équipe avec lesquels l’objet a été partagé</p> </td> 
   <td> <p>Quelqu’un partage un objet avec mon équipe.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Partage d’objets</p> </td> 
   <td> <p>Personne avec laquelle l’objet a été partagé</p> </td> 
   <td> <p>Quelqu’un partage un objet avec moi.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur du projet</p> </td> 
   <td> <p>Ajout d’utilisateur et d’utilisatrice de projet</p> </td> 
   <td> <p>Propriétaire de la ressource</p> </td> 
   <td> <p>Une des personnes dont je suis responsable est ajoutée à un projet.</p> <p>Une personne responsable reçoit une notification par e-mail lorsqu’un de ses rapports directs est ajouté à un projet.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence light ou de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Projet ajouté à un portefeuille ou un programme</p> </td> 
   <td> <p>Propriétaire du portfolio ou du programme</p> </td> 
   <td> <p>Quelqu’un ajoute un projet à un portfolio ou un programme dont je suis propriétaire.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Affectation de tâche</p> </td> 
   <td> <p>Propriétaire de la ressource</p> </td> 
   <td> <p>L’attribution d’une tâche affecte une personne dont je suis responsable.</p> <p>Le responsable du cessionnaire de la tâche reçoit une notification par e-mail.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> Projet <br>Tâche <br>Problème</td> 
   <td>Nouvelle mise à jour</td> 
   <td>Abonné </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Un e-mail est envoyé lorsqu’une mise à jour est effectuée sur une tâche, un problème ou un projet auquel je suis abonné ou abonnée.</span> </p> </td> 
   <td>Actif (instantané uniquement)</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## Délégation

Voir aussi [Notifications : délégation](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Type d&#39;objet | Événement | Destinataire | Description | État par défaut |
|------------------|--------------------------------------------|-----------|--------------------------------------------------------------|-----------------------|
| Tâches et événements | Délégation des tâches et des problèmes | Cessionnaire | Je délègue mes tâches et problèmes (confirmation). | Actif (instantané uniquement) |
| Tâches et événements | Arrêter la délégation des tâches et des problèmes | Cessionnaire | J’arrête de déléguer mes tâches et problèmes (confirmation). | Actif (instantané uniquement) |
| Tâches et événements | Délégation des tâches et des problèmes | Déléguer | Quelqu’un me délègue ses tâches et problèmes. | Actif (instantané uniquement) |
| Tâches et événements | Arrêter la délégation des tâches et des problèmes | Déléguer | Quelqu’un cesse de me déléguer ses tâches et problèmes. | Actif (instantané uniquement) |
