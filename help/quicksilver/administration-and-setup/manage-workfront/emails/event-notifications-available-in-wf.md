---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Notifications d’événements disponibles dans Adobe Workfront
description: Les notifications d’événement sont des emails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches et des problèmes, comme expliqué dans la section Notifications d’événement .
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '5070'
ht-degree: 25%

---

# Notifications d’événements disponibles dans Adobe Workfront

Les notifications d’événement sont des emails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches et des problèmes, comme expliqué dans la section [Notifications d’événements](../../../workfront-basics/using-notifications/event-notifications.md).

Ces notifications peuvent être configurées au niveau du système et du groupe :

* Pour plus d’informations sur la configuration des notifications d’événement au niveau du système, voir [Configuration des notifications d’événement pour tous les membres du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Pour plus d’informations sur la configuration des notifications d’événement au niveau du groupe, voir [Affichage et configuration des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Les utilisateurs individuels peuvent également activer et désactiver leurs notifications d’événement individuelles dans leur profil individuel. Pour plus d’informations, voir [Activation ou désactivation de vos propres notifications d’événement](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Les tableaux suivants répertorient toutes les notifications d’événement Adobe Workfront, une brève description de l’événement et si l’événement est principal ou inactif par défaut.

## Action nécessaire

Voir aussi [Notifications : Action nécessaire](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th>État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Utilisateur</p> </td> 
   <td> <p>Demande d’accès à l’utilisateur</p> </td> 
   <td> <p>Quelqu'un me demande un accès.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> <p> </p> </td> 
   <td> <p>:</p> </td> 
   <td> <p>Me demander de télécharger un ou plusieurs documents.</p> <p>Le demandeur de document reçoit une notification par courrier électronique lorsqu’il reçoit une demande de téléchargement d’un document.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Document en attente d'approbation des approbateurs</p> </td> 
   <td> <p>Je dois approuver un document.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Affectation d'événement envoyée au cessionnaire</p> </td> 
   <td> <p>En cas de modification de l'affectation d'un événement, envoyer un e-mail au nouveau cessionnaire.</p> <p>La personne désignée pour le problème ne reçoit une notification par courrier électronique que si l’état du projet est Actuel et que l’état du problème n’est pas Fermé ou que l’état du problème est Terminé.</p> <p>Les utilisateurs disposant d’une licence de vérification ou de requête ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Événement en attente d'approbation par les approbateurs</p> </td> 
   <td> <p>Lorsqu'un événement est en attente d'approbation, envoyer un e-mail à l'approbateur.</p> <p>Les utilisateurs qui reçoivent une notification par courrier électronique pour cet événement dépendent de l’activation du paramètre "L’approbateur n’a pas besoin d’appartenir à l’équipe de projet (pour les processus d’approbation qui incluent un rôle)" (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuration des paramètres d’approbation globaux</a>). </p> <p>Si cette option est activée</strong>, une notification électronique est envoyée à tous les utilisateurs du système avec le rôle de tâche "approbateur".</p> <p>Si cette option est désactivée</strong>, seuls les membres de l’équipe de projet ayant le rôle d’approbateur reçoivent une notification par e-mail.</p> <p>Une notification est envoyée si le projet est à l’état Planification ou En cours . </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Événement en attente d'approbation envoyé à l'approbateur délégué</p> </td> 
   <td> <p>Je dois passer en revue une approbation de problème qui m’a été déléguée.</p> <p>Lorsqu’une personne délègue l’approbation d’un problème à un autre utilisateur, cet utilisateur en est informé. </p> <p>Une notification est envoyée uniquement lorsque le projet est à l’état En cours .</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Projet en attente d'approbation par les approbateurs</p> </td> 
   <td> <p>Lorsqu'un projet est en attente d'approbation, envoyer un e-mail à l'approbateur.</p> <p>Les utilisateurs qui reçoivent une notification par courrier électronique pour cet événement dépendent de l’activation du paramètre "L’approbateur n’a pas besoin d’être membre de l’équipe de projet (pour les processus d’approbation qui incluent un rôle de tâche)" (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuration des paramètres d’approbation globaux</a>).</p> <p>Si cette option est activée</strong>, une notification électronique est envoyée à tous les utilisateurs du système avec le rôle de tâche "approbateur".</p> <p>Si cette option est désactivée</strong>, seuls les membres de l’équipe de projet ayant le rôle d’approbateur reçoivent une notification par e-mail.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Projet en attente d'approbation envoyé à l'approbateur délégué</td> 
   <td> <p>J'ai besoin de vérifier une approbation de projet qui m'a été déléguée.</p> </td> 
   <td> Actif</td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Affectation de la tâche envoyée au cessionnaire</p> </td> 
   <td> <p>En cas de modification de l'affectation principale d'une tâche, envoyer un e-mail au nouveau cessionnaire.</p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique s’il est nommé responsable Principal de la tâche, sauf si le cessionnaire est l’utilisateur qui a effectué l’affectation.</p> <p>Une notification est envoyée si l’état du projet est Actuel et que la tâche n’est pas marquée Terminée.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Tâche en attente d'approbation par les approbateurs</p> </td> 
   <td> <p>Lorsqu'une tâche est en attente d'approbation, envoyer un e-mail à l'approbateur.</p> <p>Les utilisateurs qui reçoivent une notification par courrier électronique pour cet événement dépendent de l’activation du paramètre "L’approbateur n’a pas besoin d’appartenir à l’équipe de projet (pour les processus d’approbation qui incluent un rôle)" (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuration des paramètres d’approbation globaux</a>). </p> <p>Si cette option est activée</strong>, une notification électronique est envoyée à tous les utilisateurs du système avec le rôle de tâche "approbateur".</p> <p>Si cette option est désactivée</strong>, seuls les membres de l’équipe de projet ayant le rôle d’approbateur reçoivent une notification par e-mail.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel au moment de la demande.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Tâche en attente d'approbation envoyée à l'approbateur délégué</p> </td> 
   <td> <p>J'ai besoin de vérifier une approbation de tâche qui m'a été déléguée.</p> <p>Lorsqu’une personne délègue l’approbation d’un problème à un autre utilisateur, cet utilisateur en est informé. </p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel au moment de la demande.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Feuille de temps rouverte pour l'utilisateur</p> </td> 
   <td> <p>Ma feuille de temps est rouverte.</p> <p>Le propriétaire de la feuille de temps reçoit une notification par e-mail lorsque la feuille de temps est rouverte, sauf si l’utilisateur qui l’a rouverte est également propriétaire de la feuille de temps.</p> <p>Une notification par e-mail n'est envoyée que si l'état de la feuille de temps est Ouverte.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Refus de la feuille de temps envoyée à l'utilisateur</p> </td> 
   <td> <p>Lorsqu'une feuille de temps est rejetée, envoyer un e-mail à l'utilisateur.</p> <p>Le propriétaire de la feuille de temps reçoit une notification par e-mail lorsque la feuille de temps est rejetée, sauf si l’utilisateur qui a rejeté la feuille de temps est également le propriétaire.</p> <p>Une notification par e-mail n’est envoyée que si l’état de la feuille de temps est Refusé.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Envoi de feuille de temps à l'approbateur</p> </td> 
   <td> <p>Lorsqu'une feuille de temps est soumise, envoyer un e-mail à l'approbateur.</p> <p>L’approbateur de la feuille de temps reçoit une notification par courrier électronique lorsqu’une feuille de temps qu’il doit approuver est envoyée, sauf si l’utilisateur qui l’a envoyée est également l’approbateur de la feuille de temps.</p> <p>Une notification n'est envoyée que si l'état de la feuille de temps est Envoyé.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affectation</p> </td> 
   <td> <p>Demande d'élément de travail à l'équipe</p> </td> 
   <td> <p>Lorsque l'équipe reçoit une nouvelle demande de travail, envoyer un e-mail à l'équipe.</p> <p>Les membres de l’équipe reçoivent une notification par e-mail lorsqu’ils reçoivent une nouvelle demande de travail. (L’utilisateur qui a soumis la demande ne reçoit pas de notification s’il est membre de l’équipe.)</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel au moment de la demande de travail et que l’état de la demande de travail est Nouveau.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affectation</p> </td> 
   <td> <p>Demande d'élément de travail au cessionnaire de l'élément de travail</p> </td> 
   <td> <p>Lorsqu'un utilisateur reçoit une nouvelle demande de travail, envoyer un e-mail au cessionnaire.</p> <p>La personne désignée de l’élément de travail reçoit une notification par courrier électronique, sauf si l’utilisateur qui effectue la demande est également la personne désignée. </p> <p>Une notification n’est pas envoyée si l’état de la tâche est Terminé ou si l’état du problème est Fermé.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel au moment de la demande.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Demandes que j’ai faites

Voir aussi [Notifications : Demandes que j’ai faites](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Le statut d'approbation du document a été modifié pour le demandeur</p> </td> 
   <td> <p>Une demande d'approbation du document est remplie.</p> <p>Le demandeur du document reçoit une notification par courrier électronique une fois la demande d’approbation du document terminée.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Demande de document remplie envoyée au demandeur</p> </td> 
   <td> <p>Une demande de chargement de document est honorée.</p> <p>Le demandeur de document reçoit une notification par courrier électronique lorsqu’une demande de téléchargement d’un document est satisfaite.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d'événement envoyé au créateur de l'événement</p> </td> 
   <td> <p>J’ajoute un problème à un projet.</p> <p>Le contact Principal sur un problème reçoit une notification lorsqu’il ajoute un problème dans un projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>Affectation d'événement au contact principal de l'événement</td> 
   <td> <p>Une personne a été affectée à un événement dont je suis le contact principal.</p> <p>Le contact Principal sur un problème reçoit une notification lorsque le problème est assigné à un utilisateur. </p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> Inactif</td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Conclusion de l'événement envoyée au créateur de l'événement</p> </td> 
   <td> <p>Lorsqu'un événement est conclu, envoyer un e-mail au créateur de l'événement.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut du projet envoyé à l'utilisateur ayant saisi le projet</p> </td> 
   <td> <p>Lorsque le statut d'un projet est modifié, envoyer un e-mail à l'utilisateur qui a entré le projet.</p> <p>L’utilisateur qui a créé le projet reçoit une notification par courrier électronique lorsque l’état du projet change.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout de demande de bureau d'aide - Envoi au créateur du problème</p> </td> 
   <td> <p>Je soumets une demande (confirmation).</p> <p>Le contact Principal sur le problème reçoit une notification par courrier électronique lorsqu’il envoie un problème.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet utilise une vue "Is Help Desk".</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Affectation de demande de bureau d'aide - Envoi au créateur du problème</p> </td> 
   <td> <p>Quelqu'un est affecté à ma demande.</p> <p>Le contact Principal de la publication reçoit une notification par courrier électronique lorsqu’un utilisateur est affecté à la publication, sauf si le contact Principal et l’utilisateur affecté sont le même.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet utilise une vue "Is Help Desk".</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Clôture de demande de bureau d'aide - Envoi au créateur du problème</p> </td> 
   <td> <p>Ma demande est close (confirmation).</p> <p>Le contact Principal du problème reçoit une notification par e-mail à la fermeture de la demande.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le projet utilise une vue "Is Help Desk".</p> <p>Si les notifications relatives à la "fin du problème" sont activées, elles se déclenchent toujours au lieu de la "demande fermée pour le contact Principal du problème". Si vous souhaitez que cette notification se déclenche, vous devez désactiver les notifications "achèvement du problème".</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document à une demande de bureau d'aide - Envoi au créateur du problème</p> </td> 
   <td> <p>Un document est modifié ou téléchargé sur un problème pour lequel je suis le contact principal.</p> <p>Le contact Principal du problème reçoit une notification par e-mail lorsqu’un document est téléchargé ou modifié sur le problème, sauf si l’utilisateur qui a téléchargé ou modifié le document est également le contact Principal.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si l’option "Publier en tant que file d’attente de demande d’aide" est activée pour le projet dans l’onglet Configuration de la file d’attente . <!-- BROUILLÉ DANS FLARE : Pour plus d’informations sur la publication d’un projet en tant que file d’attente des demandes d’aide, voir 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Présentation de l’onglet Détails de la file d’attente dans un projet</a>.

    --></p> </td>
<td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut de la demande de bureau d'aide - Envoi au créateur du problème</p> </td> 
   <td> <p>L’état change à ma demande.</p> <p>Le Principal contact de la question reçoit une notification par courrier électronique lorsque l’état de la question change, sauf si l’utilisateur qui a modifié l’état est également le contact Principal.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et que le projet utilise une vue "Is Help Desk" (Est le service d’assistance).</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Communication

Voir aussi [Notifications : Communication](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Commentaire sur le document au propriétaire du document</p> </td> 
   <td> <p>Un commentaire a été ajouté sur mon document.</p> <p>Le propriétaire d’un document dans Workfront reçoit une notification par courrier électronique lorsqu’un commentaire est publié sur le document, sauf si l’utilisateur qui a publié le commentaire est également le propriétaire du document.</p> <p>Tous les utilisateurs qui sont directement inclus dans le commentaire reçoivent également une notification par courrier électronique.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel. </p> <p>L'objet de l'email de notification instantanée est le suivant : <em>Commentaire sur &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> L’objet de la notification quotidiennement Digest est :<em> Résumé de la communication &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Actif </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Ajout de note à la demande de bureau d'aide - Envoi au créateur du problème</p> </td> 
   <td> <p>Lorsqu’un commentaire est publié sur une demande, envoyez un email Principal au problème.</p> <p>Le Principal contact pour un problème reçoit une notification par courrier électronique lorsqu’un commentaire est publié sur une demande, sauf si l’utilisateur qui a publié le commentaire est également le Principal contact pour le problème.</p> <p>Tous les utilisateurs inclus directement dans le commentaire reçoivent également une notification par courrier électronique.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur</p> </td> 
   <td>Mise à jour dirigée vers l’utilisateur</td> 
   <td> <p>Quelqu'un m'inclut sur une mise à jour dirigée.</p> <p>Une mise à jour ciblée est effectuée lorsqu’un utilisateur inclut spécifiquement un autre utilisateur dans une mise à jour, comme décrit dans la section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Balisage des autres sur les mises à jour</a>.</p> <p>Dans ce cas, l’utilisateur inclus dans la mise à jour redirigée reçoit une notification par courrier électronique concernant la mise à jour.</p> <p>La notification électronique n’est envoyée que si l’utilisateur dispose des droits d’accès à l’objet&lt;!&gt;— BROUILLÉ DANS FLARE : et n’est pas le même utilisateur que celui qui saisit la mise à jour

    -->. &lt;/p> &lt;p>Cette notification d’événement est activée par défaut et ne peut pas être désactivée.&lt;/p> &lt;/td>
<td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Équipe</p> </td> 
   <td> <p>Mise à jour dirigée vers l’équipe</p> </td> 
   <td> <p>Quelqu'un inclut mon équipe dans une mise à jour dirigée.</p> <p>Une mise à jour ciblée est effectuée lorsqu’un utilisateur inclut spécifiquement un autre utilisateur dans une mise à jour, comme décrit dans la section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Balisage des autres sur les mises à jour</a>.</p> <p>Dans ce cas, tout membre de l’équipe inclus dans la mise à jour ciblée reçoit une notification par courrier électronique à propos de la mise à jour.</p> <p>La notification électronique est envoyée uniquement aux utilisateurs disposant de droits d’accès à l’objet de la mise à jour.</p> <p>Si l’utilisateur qui envoie la mise à jour redirigée est membre de l’équipe en cours d’inclusion, l’utilisateur qui envoie la mise à jour ne reçoit pas de notification par courrier électronique.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Commentaire d'élément de travail pour les participants du thread</p> </td> 
   <td> <p>Lorsque quelqu'un fait un commentaire sur un élément de travail, envoyer un e-mail à tous ceux qui ont également fait un commentaire sur cet élément de travail.</p> <p>Les participants au thread et les utilisateurs inclus dans un message direct reçoivent une notification par email lorsqu’un utilisateur fait un commentaire dans le thread.</p> <p>Les utilisateurs doivent disposer de l’accès Affichage pour recevoir une notification.</p> <p>Les utilisateurs suivants ne reçoivent pas de notification :</p> 
    <ul> 
     <li> <p>Équipes incluses dans un message direct</p> </li> 
     <li> <p>Propriétaire de la note</p> </li> 
     <li> <p>Contact Principal</p> </li> 
    </ul> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Commentaire d'élément de travail pour le cessionnaire de l'élément de travail</p> </td> 
   <td> <p>Lorsque quelqu'un fait un commentaire sur un élément de travail, envoyer un e-mail au cessionnaire.</p> <p>La personne désignée de l’élément de travail reçoit une notification par courrier électronique chaque fois qu’un utilisateur ajoute une mise à jour à un élément de travail, sauf si l’utilisateur qui ajoute la mise à jour est également la personne désignée.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Réponse à une demande de travail au demandeur de travail</p> </td> 
   <td> <p>Quelqu'un répond à ma demande.</p> <p>Une fois qu’un utilisateur a envoyé une requête et qu’un autre utilisateur a répondu à cette requête, l’utilisateur qui l’a envoyée reçoit une notification par courrier électronique.</p> <p>Une notification électronique n’est pas envoyée si :</p> 
    <ul> 
     <li> <p>L’utilisateur qui envoie la réponse est le même utilisateur qui a effectué la demande.</p> </li> 
     <li> <p>L’utilisateur n’a pas accès à l’affichage de la note.</p> </li> 
    </ul> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations de validation

Voir aussi [Notifications : Informations de validation](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Utilisateur</p> </td> 
   <td> <p>Délégation d'approbation envoyée à un autre utilisateur</p> </td> 
   <td> <p>Je suis délégué en tant qu'approbateur.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut de l'approbation d'événement déléguée</p> </td> 
   <td> <p>Une demande d'approbation d'événement déléguée a été remplie. </p> <p>Lorsque vous déléguez l’approbation d’un problème à quelqu’un d’autre, vous recevez une notification par courrier électronique une fois cette approbation terminée (qu’il approuve ou refuse l’approbation du problème). </p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut de l'approbation de projet déléguée</p> </td> 
   <td> <p>Une demande d'approbation de projet déléguée a été remplie.</p> <p>Lorsque vous déléguez l’approbation d’un projet à une autre personne, vous recevez une notification par e-mail une fois cette approbation terminée (qu’elle approuve ou refuse l’approbation du projet).</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Changement de statut de l'approbation de tâche déléguée</p> </td> 
   <td> <p>Un état d’approbation de tâche déléguée est terminé.</p> <p>Lorsque vous déléguez une validation de tâche à une autre personne, vous recevez un email de notification une fois cette validation terminée (qu’elle valide ou refuse la validation de la tâche).</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Annuler l'approbation du document pour l'approbateur</p> </td> 
   <td> <p>Une demande d'approbation du document est annulée.</p> <p>L’approbateur du document reçoit une notification par courrier électronique lorsque la demande d’approbation du document est annulée.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Approbation de feuille de temps pour l'utilisateur</p> </td> 
   <td> <p>Lorsqu'une feuille de temps est acceptée et fermée, envoyer un e-mail à l'utilisateur.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur le travail qui m&#39;est assigné

Voir aussi [Notifications : Informations sur le travail qui m&#39;est assigné](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Tâche</td> 
   <td>Toutes les tâches antérieures terminées envoyées aux tâches dépendantes de l’équipe affectée</td> 
   <td> <p>Tous les prédécesseurs des tâches de l'équipe sont terminés.</p> <p>Les personnes désignées pour la tâche (tous les membres de l’équipe) reçoivent une notification par e-mail.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td>Inactif</td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Tous les achèvements de tâches antérieures envoyés aux tâches dépendantes</p> </td> 
   <td> <p>Toutes les tâches antérieures de mes tâches sont terminées.</p> <p>La personne désignée pour la tâche reçoit une notification par courrier électronique.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Décision d’approbation d’émettre attribuée à</p> </td> 
   <td> <p>Lorsqu'un événement est approuvé ou rejeté, envoyer un e-mail au cessionnaire.</p> <p>La personne désignée pour un problème reçoit une notification par courrier électronique lorsqu’une décision d’approbation est prise (approuvée ou rejetée).</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Décision d’approbation de la tâche affectée à</p> </td> 
   <td> <p>Lorsqu'une tâche d'approbation est approuvée ou rejetée, envoyer un e-mail au cessionnaire.</p> <p>La personne désignée pour la tâche reçoit une notification par e-mail lorsque la tâche est approuvée ou rejetée.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Conclusion de l'événement envoyée au cessionnaire</p> </td> 
   <td> <p>Lorsqu'un événement est conclu, envoyer e-mail au cessionnaire.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>La date d'achèvement planifiée pour l'événement a changé</p> </td> 
   <td> <p>Lorsque la date de fin prévue d'un événement est modifiée, envoyer un e-mail à  l'utilisateur affecté.</p> <p>La personne désignée par le problème reçoit une notification par courrier électronique lorsque la date de fin planifiée change, sauf si l’utilisateur qui a modifié la date de fin planifiée est également la personne désignée.</p> <p>Une notification est envoyée uniquement si l’état du projet est autre que Planification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Le statut de l'événement a été remplacé par Affecté à</p> </td> 
   <td> <p>L’état change pour l’une de mes tâches.</p> <p>La personne désignée de la publication reçoit une notification par courrier électronique lorsque l’état change, sauf si l’utilisateur qui a modifié l’état est également la personne désignée.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document à une demande de bureau d'aide - Envoi à la personne chargée du problème</p> </td> 
   <td> <p>Les documents sont téléchargés ou modifiés à ma demande.</p> <p>La personne désignée pour le problème reçoit une notification par courrier électronique lorsque des documents sont chargés ou modifiés sur un problème qu’elle a ajouté.</p> <p>Une notification par courrier électronique n’est pas envoyée si l’utilisateur qui a participé au problème est la personne désignée pour le problème.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si l’option "Publier en tant que file d’attente de demande d’aide" est activée pour le projet dans l’onglet Configuration de la file d’attente .<!-- BROUILLÉ DANS FLARE : Pour plus d’informations sur la publication d’un projet en tant que file d’attente des demandes d’aide, voir 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Présentation de l’onglet Détails de la file d’attente dans un projet</a>.

    --></p> </td>
<td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche à Tâche affectée à</p> </td> 
   <td> <p>Quand une tâche est terminée, envoyer un e-mail au cessionnaire.</p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique une fois la tâche terminée. Les notifications ne sont pas envoyées lorsqu’une tâche personnelle est terminée.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> <p>Les utilisateurs disposant d’une licence de vérification ou de demandeur ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche envoyé aux tâches dépendantes</p> </td> 
   <td> <p>Lorsqu'une tâche est terminée, envoyer un e-mail aux cessionnaires principaux de toute les tâches dépendantes.</p> <p>La personne désignée pour la tâche reçoit une notification par e-mail lorsque l’un des prédécesseurs de la tâche est terminé.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>La date d'achèvement prévue pour la tâche a changé</p> </td> 
   <td> <p>Lorsque la date de fin prévue d'une tâche est modifiée, envoyer un e-mail à l'utilisateur affecté.</p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique lorsque la date d’achèvement planifiée de la tâche change, sauf si l’utilisateur qui a modifié la date d’achèvement planifiée est également le cessionnaire de la tâche.</p> <p>Une notification est envoyée uniquement si l’état du projet est autre que Planification.</p> <p>Aucune notification n’est envoyée concernant les tâches personnelles.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Le statut de la tâche a été remplacé par Affecté(e) à.</p> </td> 
   <td> <p>Le statut est remplacé sur une tâche que l'on m'a affectée par.</p> <p>Le cessionnaire de la tâche reçoit une notification par courrier électronique lorsque l’état de la tâche change, sauf si l’utilisateur qui a modifié l’état est également la personne désignée.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur les projets sur lesquels je travaille

Voir aussi [Notifications : Informations sur les projets sur lesquels je travaille](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement du statut du projet courant envoyé à l'équipe du projet</p> </td> 
   <td> <p>Lorsque le statut d'un projet passe du statut idée/approuvé/rejeté/demandé/planifié à courant, envoyez un e-mail à l'équipe.</p> <p>Les utilisateurs du projet reçoivent une notification par e-mail lorsque le projet devient principal.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document envoyé à l'équipe de projet</p> </td> 
   <td> <p>Un document est ajouté à un projet sur lequel je travaille.</p> <p>Les utilisateurs de l’équipe de projet reçoivent une notification par courrier électronique lorsqu’un document est ajouté au projet, à l’exception de l’utilisateur qui a ajouté le document.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et que le document n’est pas Privé. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d'événement envoyé à l'équipe de projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet sur lequel je travaille.</p> <p>Les utilisateurs d’un projet reçoivent une notification par courrier électronique lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Conclusion d'événement envoyée à l'équipe de projet</p> </td> 
   <td> <p>Lorsqu'un événement est conclu, envoyer un e-mail à l'équipe.</p> <p>Tout utilisateur du projet reçoit une notification.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche jalonnée envoyé à l'équipe de projet</p> </td> 
   <td> <p>Une tâche de jalon est effectuée sur un projet sur lequel je travaille.</p> <p>Tous les utilisateurs de l’équipe de projet reçoivent une notification lorsqu’une tâche de jalon est terminée. </p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Achèvement du projet envoyé à l'équipe de projet</p> </td> 
   <td> <p>Quand un projet est terminé, envoyer un e-mail à l'équipe.</p> <p>Les utilisateurs d’une équipe de projet reçoivent une notification par courrier électronique lorsque l’état du projet est terminé.</p> <p>Conseil : Si les projets sont terminés régulièrement, l’activation de cette option peut créer de nombreux courriers électroniques pour les utilisateurs qui ont un nombre limité de tâches sur de nombreux projets. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut du projet envoyé à l'équipe du projet</p> </td> 
   <td> <p>Lorsque le statut d'un projet est modifié, envoyer un e-mail à l'équipe.</p> <p>Les utilisateurs de l’équipe de projet reçoivent une notification par e-mail lorsque l’état du projet change. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur du projet</p> </td> 
   <td> <p>Ajout d'un utilisateur de projet envoyé à l'utilisateur du projet</p> </td> 
   <td> <p>Lorsqu'un utilisateur est ajouté à l'équipe de projet, envoyer un e-mail à l'utilisateur.</p> <p>L’utilisateur qui a été ajouté au projet reçoit une notification par courrier électronique lorsqu’il est ajouté, sauf s’il a été ajouté lui-même au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche envoyé à l'équipe de projet</p> </td> 
   <td> <p>Quand une tâche est terminée, envoyer un e-mail à l'équipe.</p> <p>Les membres de l’équipe de projet reçoivent une notification par e-mail.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d'événement non affecté envoyé à l'équipe du projet</p> </td> 
   <td> <p>Un problème non assigné est ajouté à un projet sur lequel je travaille.</p> <p>Les utilisateurs d’un projet reçoivent une notification par courrier électronique lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur les projets que je possède

Voir aussi [Notifications : Informations sur les projets que je possède](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document envoyé au propriétaire du projet</p> </td> 
   <td> <p>Un document est ajouté à un projet que je possède.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un document est ajouté au projet, sauf si l’utilisateur qui a ajouté le document est également le propriétaire du projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et que le document n’est pas Privé.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d'événement envoyé au propriétaire du projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet que je possède.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Modification de la date d'engagement pour un événement envoyée au propriétaire du projet</p> </td> 
   <td> <p>Lorsque la date d'engagement pour un événement est modifiée, envoyer un e-mail au propriétaire du projet.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsque la date de validation change pour un problème sur le projet, sauf si l’utilisateur qui modifie la date de validation est le même que le propriétaire du projet.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Conclusion de l'événement envoyée au propriétaire du projet</p> </td> 
   <td> <p>Envoyer un e-mail au propriétaire du projet lorsqu'un événement est terminé.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche jalonnée envoyé au propriétaire du projet</p> </td> 
   <td> <p>Une tâche de jalon est effectuée sur un projet que je possède.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Affectation du propriétaire du projet envoyé au propriétaire du projet</p> </td> 
   <td> <p>Lorsque le propriétaire du projet change ou lors de la création du projet, envoyer un e-mail au nouveau propriétaire affecté.</p> <p>Lorsqu’un utilisateur est désigné propriétaire d’un projet, il reçoit une notification par courrier électronique.</p> <p>Si le propriétaire du projet est le même utilisateur que celui qui a effectué l’affectation, aucune notification par courrier électronique n’est envoyée.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Modification de la progression du projet envoyée au propriétaire du projet</p> </td> 
   <td> <p>Quand un projet passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au propriétaire du projet.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsque le projet est en retard sur le planning.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la date d'engagement pour une tâche envoyée au propriétaire du projet</p> </td> 
   <td> <p>Lorsque la date d'engagement pour une tâche est modifiée, envoyer un e-mail au propriétaire du projet.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsque la date de validation change pour une tâche du projet, sauf si l’utilisateur qui a modifié la date de validation est également le propriétaire du projet.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche envoyé au propriétaire du projet</p> </td> 
   <td> <p>Envoyer un e-mail au propriétaire du projet lorsqu'une tâche est terminée.</p> <p>Le propriétaire du projet reçoit une notification. </p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la progression de la tâche envoyée au propriétaire du projet</p> </td> 
   <td> <p>Quand une tâche passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au propriétaire du projet.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’une tâche du projet est en retard sur le planning.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d'événement non affecté envoyé au propriétaire du projet</p> </td> 
   <td> <p>Un problème non attribué est ajouté à un projet que je possède.</p> <p>Le propriétaire du projet reçoit une notification par courrier électronique lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur les projets que je sponsorise

Voir aussi [Notifications : Informations sur les projets que je sponsorise](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de document envoyé au sponsor du projet</p> </td> 
   <td> <p>Un document est ajouté à un projet que je sponsorise.</p> <p>Le parrain du projet reçoit une notification par courrier électronique lorsqu’un document est ajouté au projet, sauf si le parrain du projet l’ajoute.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel et si le document n’est pas Privé.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d'événement envoyé au sponsor du projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet que je sponsorise.</p> <p>Le parrain du projet reçoit une notification par courrier électronique lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Conclusion d'événement envoyée au sponsor du projet</p> </td> 
   <td> <p>Un problème est terminé sur un projet que je sponsorise.</p> <p>Le sponsor du projet reçoit une notification par email.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche jalonnée envoyé au sponsor du projet</p> </td> 
   <td> <p>Une tâche de jalon est effectuée sur un projet que je sponsorise.</p> <p>Le sponsor du projet reçoit une notification par e-mail lorsqu’une tâche de jalon est terminée sur un projet qu’il sponsorise.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Modification de la progression du projet envoyée au sponsor du projet</p> </td> 
   <td> <p>Quand un projet passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au sponsor du projet.</p> <p>Le parrain du projet reçoit une notification par e-mail lorsque le projet est en retard sur le planning.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Affectation de sponsor du projet envoyée au sponsor de projet</p> </td> 
   <td> <p>Lorsque le sponsor du projet change ou lors de la création du projet, envoyer un e-mail au nouveau sponsor affecté.</p> <p>Le sponsor du projet reçoit une notification par email lorsqu’il est défini comme sponsor d’un projet.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement de tâche envoyé au sponsor du projet</p> </td> 
   <td> <p>Une tâche est effectuée sur un projet que je sponsorise.</p> <p>Le sponsor du projet reçoit une notification par email.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la progression de la tâche envoyée au sponsor du projet</p> </td> 
   <td> <p>Quand une tâche passe d'un statut de progression positive (Dans les délais) à un statut de progression négative (En retard), envoyer un e-mail au sponsor du projet.</p> <p>Le parrain du projet reçoit une notification par e-mail lorsqu’une tâche du projet est en retard sur le planning.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d'événement non affecté envoyé au sponsor du projet</p> </td> 
   <td> <p>Un problème non attribué est ajouté à un projet que je sponsorise.</p> <p>Le parrain du projet reçoit une notification par courrier électronique lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations diverses

Voir aussi [Notifications : Informations diverses](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d'objet</th> 
   <th>Événement</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Annonce</td> 
   <td> <p>L'annonce a été ajoutée</p> </td> 
   <td> <p>Un message est envoyé au Centre des annonces.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Annuler la demande de document envoyée au destinataire de la demande</p> </td> 
   <td> <p>Annuler une demande de téléchargement de document de ma part.</p> <p>L’utilisateur reçoit une notification par courrier électronique lorsqu’une demande de document est annulée.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Notification d'erreur</p> </td> 
   <td> <p>Une erreur qui nécessite votre attention a été trouvée.</p> <p>Une notification par courrier électronique est générée une fois que Workfront a tenté de se connecter à un compte POP et qu’il n’y a pas réussi. Après 25 tentatives, Workfront désactive la connexion au compte POP afin de préserver les ressources et envoie une notification. </p> <p>La notification est envoyée par courrier électronique au propriétaire du projet, si le courrier électronique POP est associé à une file d’attente de requêtes, ou aux administrateurs Workfront, si le compte POP est associé à la fonction "Courrier entrant" dans la configuration des emails.
     <!--
      DRAFTED IN FLARE:
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      --></p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Affectation d'un événement envoyée au propriétaire de la ressource</p> </td> 
   <td> <p>En cas de modification de l'affectation d'un événement, envoyer un e-mail au propriétaire de la ressource.</p> <p>Le Gestionnaire des personnes concernées reçoit une notification par e-mail lorsqu’une modification affecte un utilisateur qu’il gère.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur</p> </td> 
   <td> <p>Nouvel utilisateur envoyé à l'utilisateur</p> </td> 
   <td> <p>Lorsqu'un nouvel utilisateur est créé dans Workfront, envoyer un e-mail à l'utilisateur.</p> <p>Une fois le nouvel utilisateur créé, il reçoit une invitation par courrier électronique l’informant qu’un compte Workfront a été créé et lui demandant de définir son mot de passe.</p> <p>Lors de la création d’un nouvel utilisateur, les utilisateurs peuvent sélectionner l’option "Envoyer un courrier électronique d’invitation à cette personne" (comme décrit dans la section <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajout d’utilisateurs</a><span style="font-weight: 400;">). Cependant, lorsque l’option "Nouvel utilisateur à l’utilisateur" est activée globalement, tous les nouveaux utilisateurs reçoivent l’invitation par courrier électronique, que l’option "Envoyer un courrier électronique d’invitation à cette personne" soit sélectionnée ou non.</span></p> </td> 
   <td> Inactif </td> 
  </tr> 
  <tr> 
   <td> <p>Équipe</p> </td> 
   <td> <p>Partage d'objet envoyé à l'équipe</p> </td> 
   <td> <p>Quelqu'un partage un objet avec mon équipe.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur</p> </td> 
   <td> <p>Partage d'objet envoyé à l'utilisateur</p> </td> 
   <td> <p>Quelqu'un partage un objet avec moi.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur du projet</p> </td> 
   <td> <p>Ajout d'un utilisateur de projet envoyé au propriétaire de la ressource</p> </td> 
   <td> <p>Lorsqu'un utilisateur est ajouté à une équipe de projet, envoyer un e-mail au propriétaire de la ressource.</p> <p>Un responsable reçoit une notification par e-mail lorsqu’un de ses rapports directs est ajouté à un projet.</p> <p>Les utilisateurs disposant d’une licence de révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Projet ajouté à un portefeuille ou un programme</p> </td> 
   <td> <p>Quelqu'un ajoute un projet à un portefeuille ou un programme dont je suis propriétaire.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Affectation d'une tâche envoyée au propriétaire de la ressource</p> </td> 
   <td> <p>En cas de modification de l'affectation primaire d'une tâche, envoyer un e-mail au propriétaire de la ressource.</p> <p>Le responsable du cessionnaire de la tâche reçoit une notification par courrier électronique.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> Projet <br>Tâche <br>Problème</td> 
   <td>Nouvelle mise à jour pour l'abonné </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Un email est envoyé lorsqu’une mise à jour est effectuée sur une tâche, un problème ou un projet auquel je suis abonné.</span> </p> </td> 
   <td>Actif</td> 
  </tr> 
 </tbody> 
</table>

## Délégation

Voir aussi [Notifications : Délégation](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Type d&#39;objet | Événement | Description | État par défaut |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Tâches et événements | Délégation de tâches et problèmes à la personne assignée | Je délègue mes tâches et problèmes (confirmation). | Actif |
| Tâches et événements | Arrêter la délégation de tâches et de problèmes à la personne assignée | J’arrête de déléguer mes tâches et problèmes (confirmation). | Actif |
| Tâches et événements | Délégation de tâches et problèmes à la personne assignée | Quelqu’un me délègue ses tâches et problèmes. | Actif |
| Tâches et événements | Arrêter les tâches et émettre la délégation à déléguer | Quelqu’un cesse de me déléguer ses tâches et problèmes. | Actif |
