---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Types de notification d’événement
description: Les notifications d’événement sont des e-mails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches et des problèmes. Cet article répertorie et décrit les types de notifications d’événement disponibles.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: f3016e77f086d221dc11398ec06cc7435ad82278
workflow-type: tm+mt
source-wordcount: '5237'
ht-degree: 99%

---

# Types de notification d’événement

<!-- Audited: 1/2024 -->

Les notifications d’événement sont des e-mails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches et des problèmes, comme expliqué dans la section [Notifications d’événements](../../../workfront-basics/using-notifications/event-notifications.md).

Ces notifications peuvent être configurées au niveau du système et du groupe :

* Pour plus d’informations sur la configuration des notifications d’événement au niveau du système, voir [Configurer des notifications d’événement pour toutes les personnes membres du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Pour plus d’informations sur la configuration des notifications d’événement au niveau du groupe, voir [Afficher et configurer des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Les utilisateurs et utilisatrices peuvent également activer et désactiver leurs notifications d’événement particulières dans leur profil. Pour plus d’informations, voir [Modifier vos propres notifications par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Les tableaux suivants répertorient toutes les notifications d’événement Adobe Workfront, une brève description de l’événement et indiquent si l’événement est actif ou inactif par défaut.

>[!NOTE]
>
>Sauf indication contraire, les notifications dont la valeur dans la colonne État par défaut est « Actif » sont actives par défaut pour les notifications instantanées et quotidiennes.

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
   <th>Type d’objet</th> 
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
   <td> <p>Une personne me demande un accès.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> <p> </p> </td> 
   <td> <p>Ajout de demande de document</p> </td> 
   <td> <p>Utilisateur ou utilisatrice dont le document est demandé.</p> </td> 
   <td> <p>Une personne m’a demandé de charger le ou les documents.</p> <p>La personne qui a demandé le document reçoit une notification par e-mail lorsqu’elle reçoit une demande de chargement d’un document.</p> </td> 
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
   <td> <p>Attribution de problèmes</p> </td> 
   <td> <p>L’utilisateur ou utilisatrice à qui ce problème est affecté.</p> </td> 
   <td> <p>Un problème m’a été affecté.</p> <p>La personne cessionnaire pour le problème ne reçoit une notification par e-mail que si le statut du projet est Actuel et que le statut du problème n’est pas Fermé ou équivalent.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence Light, Contribution, Révision ou Demande ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Événement en attente d'approbation</p> </td> 
   <td> <p>Approbateurs</p> </td> 
   <td> <p>Je dois approuver un problème.</p> <p>Les utilisateurs et utilisatrices qui reçoivent une notification par e-mail pour cet événement dépendent de l’activation du paramètre « L’approbateur ou approbatrice n’a pas besoin d’appartenir à l’équipe de projet (pour les processus d’approbation qui incluent un rôle) » (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer les paramètres d’approbation globaux</a>). </p> <p>Si cette option est activée</strong>, une notification par e-mail est envoyée à tous les utilisateurs et utilisatrices du système avec la fonction « Approbateur ou approbatrice ».</p> <p>Si cette option est désactivée</strong>, seules les personnes membres de l’équipe de projet ayant une fonction d’approbateur ou approbatrice reçoivent une notification par e-mail.</p> <p>Une notification est envoyée si le projet a le statut Prévu ou Actuel. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Événement en attente d'approbation</p> </td> 
   <td> <p>Personne approbatrice déléguée</p> </td> 
   <td> <p>J’ai besoin de vérifier l’approbation d’un problème qui m’a été déléguée.</p> <p>Lorsqu’une personne délègue l’approbation d’un problème à une autre personne, cette dernière en est informée. </p> <p>Une notification est envoyée uniquement lorsque le projet a le statut En cours.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Projet en attente d'approbation</p> </td> 
   <td> <p>Approbateurs</p> </td> 
   <td> <p>J’ai besoin d’approuver un projet.</p> <p>Les personnes qui reçoivent une notification par e-mail pour cet événement dépendent de l’activation du paramètre « La personne approbatrice n’a pas besoin d’être membre de l’équipe de projet (pour les processus d’approbation qui incluent une fonction) » (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer des paramètres d’approbation globaux</a>).</p> <p>Si cette option est activée</strong>, une notification par e-mail est envoyée à toutes les personnes du système avec la fonction « personne approbatrice ».</p> <p>Si cette option est désactivée</strong>, seules les personnes membres de l’équipe de projet ayant le rôle de « personne approbatrice » reçoivent une notification par e-mail.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Projet en attente d'approbation</td> 
   <td>Personne approbatrice déléguée</td> 
   <td> <p>J’ai besoin de vérifier une approbation de projet qui m’a été déléguée.</p> </td> 
   <td> Actif</td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Affectation de la tâche</p> </td> 
   <td> <p>Personne à laquelle la tâche est affectée.</p> </td> 
   <td> <p>Je suis la personne cessionnaire principale d’une tâche.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail si elle est désignée comme principale personne cessionnaire de la tâche, sauf si la personne cessionnaire est celle qui a effectué l’affectation.</p> <p>Une notification est envoyée si le statut du projet est En cours et que la tâche n’est pas marquée comme Terminée.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Tâche en attente d'approbation</p> </td> 
   <td> <p>Approbateurs</p> </td> 
   <td> <p>J’ai besoin d’approuver une tâche.</p> <p>Les personnes qui reçoivent une notification par e-mail pour cet événement dépendent de l’activation du paramètre « La personne approbatrice n’a pas besoin d’appartenir à l’équipe de projet (pour les processus d’approbation qui incluent une fonction) » (comme décrit dans la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer des paramètres d’approbation globaux</a>). </p> <p>Si cette option est activée</strong>, une notification par e-mail est envoyée à tous les utilisateurs et utilisatrices du système avec la fonction « Approbateur ou approbatrice ».</p> <p>Si cette option est désactivée</strong>, seules les personnes membres de l’équipe de projet ayant la fonction de personne approbatrice reçoivent une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est En cours au moment de la demande.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Tâche en attente d'approbation</p> </td> 
   <td> <p>Personne approbatrice déléguée</p> </td> 
   <td> <p>J’ai besoin de vérifier une approbation de tâche qui m’a été déléguée.</p> <p>Lorsqu’une personne délègue l’approbation d’un problème à une autre personne, cette dernière en est informée. </p> <p>Une notification est envoyée uniquement si le statut du projet est En cours au moment de la demande.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Feuille de temps rouverte</p> </td> 
   <td> <p>Utilisateur ou utilisatrice qui possède la feuille de temps</p> </td> 
   <td> <p>Ma feuille de temps est rouverte.</p> <p>La personne propriétaire de la feuille de temps reçoit une notification par e-mail lorsque la feuille de temps est rouverte, sauf si la personne qui a rouvert la feuille de temps est également propriétaire de la feuille de temps.</p> <p>Une notification par e-mail n’est envoyée que si le satut de la feuille de temps est Ouvert.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Rejet de la feuille de temps</p> </td> 
   <td> <p>Utilisateur ou utilisatrice qui possède la feuille de temps</p> </td> 
   <td> <p>Ma feuille de temps a été rejetée.</p> <p>Le ou la propriétaire de la feuille de temps reçoit une notification par e-mail lorsque la feuille de temps est rejetée, sauf si la personne qui a rejeté la feuille de temps est également la propriétaire.</p> <p>Une notification par e-mail n’est envoyée que si le statut de la feuille de temps est Rejetée.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Envoi de la feuille de temps</p> </td> 
   <td> <p>Approbateur</p> </td> 
   <td> <p>Je dois approuver une feuille de temps.</p> <p>La personne approbatrice de la feuille de temps reçoit une notification par e-mail lorsqu’une feuille de temps qu’elle doit approuver est envoyée, sauf si l’utilisateur ou l’utilisatrice qui l’a envoyée est également l’approbateur ou l’approbatrice de la feuille de temps.</p> <p>Une notification n’est envoyée que si le statut de la feuille de temps est Envoyée.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affectation</p> </td> 
   <td> <p>Demande d’élément de travail</p> </td> 
   <td> <p>Personnes membres de l’équipe pour laquelle l’élément est demandé.</p> </td> 
   <td> <p>Mon équipe reçoit une nouvelle demande de travail.</p> <p>Les personnes membres de l’équipe reçoivent une notification par e-mail lorsque l’équipe reçoit une nouvelle demande de travail. (Les utilisateurs et utilisatrices qui ont soumis la demande ne reçoivent pas de notification s’ils sont membres de l’équipe.)</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel au moment de la demande de travail et que le statut de la demande de travail est Nouvelle.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affectation</p> </td> 
   <td> <p>Demande d’élément de travail</p> </td> 
   <td> <p>Utilisateur ou utilisatrice pour qui un élément de travail est demandé.</p> </td> 
   <td> <p>Je reçois une nouvelle demande de travail.</p> <p>La personne cessionnaire de l’élément de travail reçoit une notification par e-mail, sauf si la personne qui dépose la demande est également la personne cessionnaire. </p> <p>Une notification n’est pas envoyée si le statut de la tâche est Terminée ou si le statut du problème est Fermé.</p> <p>Une notification est envoyée uniquement si le statut du projet est En cours au moment de la demande.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Demandes que j’ai effectuées.

Voir aussi [Notifications : demandes que j’ai effectuées](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Changement de statut d’approbation du document</p> </td> 
   <td> <p>Demandeur</p> </td> 
   <td> <p>Une demande d’approbation du document est terminée.</p> <p>La personne qui a demandé le document reçoit une notification par e-mail une fois la demande d’approbation du document terminée.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Demande de document terminée</p> </td> 
   <td> <p>Demandeur</p> </td> 
   <td> <p>Une demande de chargement de document est honorée.</p> <p>La personne qui a demandé le document reçoit une notification par e-mail lorsqu’une demande de chargement d’un document est honorée.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>J’ajoute un problème au projet.</p> <p>La personne à l’origine du problème reçoit une notification lorsqu’elle l’ajoute dans un projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>Attribution de problèmes</td> 
   <td>Créateur ou créatrice du problème</td> 
   <td> <p>Une personne a été affectée à un problème dont je suis le créateur ou la créatrice.</p> <p>Le créateur ou la créatrice d’un problème reçoit une notification lorsque le problème est attribué à un utilisateur ou une utilisatrice. </p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> Inactif</td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement du problème</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>Un problème dont je suis le créateur ou la créatrice est terminé.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut d’un projet</p> </td> 
   <td> <p>Utilisateur ou utilisatrice ayant créé le projet (saisi par)</p> </td> 
   <td> <p>Le statut d’un projet que j’ai créé change.</p> <p>L’utilisateur ou l’utilisatrice qui a créé le projet reçoit une notification par e-mail lorsque le statut du projet est modifié.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’une demande</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>J’ai soumis une demande (confirmation).</p> <p>Le créateur ou la créatrice du problème reçoit une notification par e-mail lors de l’envoi d’un problème.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel et si le projet utilise une vue « Centre d’assistance ».</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Affectation d’une demande</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>Une personne est affectée à ma demande.</p> <p>Le créateur ou la créatrice du problème reçoit une notification par e-mail lorsque le problème est affecté à une personne, sauf si cette personne est le créateur ou la créatrice.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel et si le projet utilise une vue « Centre d’assistance ».</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Demande fermée</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>Ma demande est fermée (confirmation).</p> <p>Le contact principal du problème reçoit une notification par e-mail à la fermeture de la demande.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel et si le projet utilise une vue « Centre d’assistance ».</p> <p>Si les notifications pour « conclusion de problème » sont activées, elles se déclenchent toujours au lieu de « Clôture de demande de bureau d’aide - Envoi au créateur ou à la créatrice du problème ». Si vous souhaitez que cette notification se déclenche, vous devez désactiver les notifications « conclusion de problème ».</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de docuement de demande</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>Un document est modifié ou chargé sur un problème dont je suis créateur ou créatrice.</p> <p>Le contact principal du problème reçoit une notification par e-mail lorsqu’un document est chargé ou modifié sur le problème, sauf si la personne qui a chargé ou modifié le document est également le contact principal.</p> <p>Une notification est envoyée uniquement si le statut du projet est En cours et si l’option « Publier en tant que file d’attente des demandes d’aide » est activée pour le projet dans l’onglet Configuration de la file d’attente.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut de la demande</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>Le statut est modifié dans ma demande.</p> <p>Le contact principal du problème reçoit une notification par e-mail lorsque le statut du problème est modifié, sauf si l’utilisateur ou l’utilisatrice à l’origine de la modification est également le contact principal.</p> <p>Une notification est envoyée uniquement si le statut du projet est En cours et que le projet utilise une vue « Centre d’assistance ».</p> </td> 
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
   <th>Type d’objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Commenter sur le document</p> </td> 
   <td> <p>Propriétaire du document</p> </td> 
   <td> <p>Un commentaire a été ajouté sur mon document.</p> <p>La personne propriétaire d’un document dans Workfront reçoit une notification par e-mail lorsqu’un commentaire est publié sur le document, sauf si la personne qui a publié le commentaire est également propriétaire du document.</p> <p>Tous les utilisateurs et utilisatrices directement concernés par le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel. </p> <p>L’objet de l’e-mail de notification instantanée est : <em>Commentaire sur &lt;Request name&gt; sur &lt;Project Name&gt; (n° de réf. &lt;Request Reference Number&gt;)</em>.</p> <p> L’objet de la notification de résumé quotidien est :<em> Résumé des communications &lt;Date of daily digest&gt;</em>.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Ajout de note à une demande</p> </td> 
   <td> <p>Créateur ou créatrice du problème</p> </td> 
   <td> <p>Lorsqu’un commentaire est publié sur une requête, envoyez un e-mail au contact principal du problème.</p> <p>Le contact principal d’un problème reçoit une notification par e-mail lorsqu’un commentaire est publié sur une requête, sauf si la personne qui a publié le commentaire est également le contact principal du problème.</p> <p>Toutes les personnes qui sont directement incluses dans le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td>Mise à jour dirigée</td> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Une personne m’inclut dans une mise à jour dirigée.</p> <p>Une mise à jour est dirigée lorsqu’une personne inclut spécifiquement une autre personne dans une mise à jour, comme décrit dans la section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Baliser d’autres personnes sur les mises à jour</a>.</p> <p>Dans ce cas, l’utilisateur ou utilisatrice qui est inclus dans la mise à jour dirigée reçoit une notification par e-mail concernant la mise à jour.</p> <p>La notification par e-mail n’est envoyée que si la personne dispose des droits d’accès à l’objet et si ce dernier est activé dans son profil.  </p> <p>Cette notification d’événement est activée par défaut et ne peut pas être désactivée.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Mise à jour dirigée</p> </td> 
   <td> <p>Membres d'équipe</p> </td> 
   <td> <p>Une personne inclut mon équipe dans une mise à jour dirigée.</p> <p>Une mise à jour dirigée a lieu lorsqu’un utilisateur ou une utilisatrice inclut spécifiquement une autre personne dans une mise à jour, comme décrit dans la section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Taguer d’autres personnes sur les mises à jour</a>.</p> <p>Dans ce cas, toute personne membre de l’équipe incluse dans la mise à jour dirigée reçoit une notification par e-mail concernant la mise à jour.</p> <p>La notification par e-mail est envoyée uniquement aux utilisateurs et utilisatrices disposant de droits d’accès à l’objet de la mise à jour.</p> <p>Si la personne qui envoie la mise à jour dirigée est membre de l’équipe incluse, la personne qui envoie la mise à jour ne reçoit pas de notification par e-mail.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Commentaire d’un élément de travail</p> </td> 
   <td> <p>Personne participantes du thread</p> </td> 
   <td> <p>Une personne fait un commentaire dans un thread auquel je participe.</p> <p>Les personnes participant au thread et les utilisateurs et utilisatrices inclus dans un message direct reçoivent une notification par e-mail lorsque quelqu’un fait un commentaire dans le thread.</p> <p>Les utilisateurs et utilisatrices doivent disposer de l’accès en affichage pour recevoir une notification.</p> <p>Les utilisateurs et utilisatrices suivants ne reçoivent pas de notification :</p> 
    <ul> 
     <li> <p>Les équipes incluses dans un message direct</p> </li> 
     <li> <p>La personne propriétaire de la note</p> </li> 
     <li> <p>Le contact principal</p> </li> 
    </ul> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Commentaire d’un élément de travail</p> </td> 
   <td> <p>Personne cessionnaire d’un élément de travail</p> </td> 
   <td> <p>Une personne fait un commentaire sur l’un de mes éléments de travail.</p> <p>La personne assignée de l’élément de travail reçoit une notification par e-mail chaque fois qu’une personne ajoute une mise à jour à un élément de travail, sauf si la personne qui ajoute la mise à jour est également la personne assignée.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Note</p> </td> 
   <td> <p>Réponse à la demande de travail</p> </td> 
   <td> <p> Personne qui a demandé le travail.</p> </td> 
   <td> <p>Une personne répond à ma demande.</p> <p>L’utilisateur ou l’utilisatrice qui a envoyé la demande reçoit une notification par e-mail lorsqu’une autre personne y a répondu.</p> <p>Une notification par e-mail n’est pas envoyée si :</p> 
    <ul> 
     <li> <p>L’utilisateur ou utilisatrice qui répond est celui qui a fait la demande.</p> </li> 
     <li> <p>L’utilisateur ou utilisatrice n’a pas accès à la note</p> </li> 
    </ul> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Informations sur l’approbation

Voir aussi [Notifications : informations sur l’approbation](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’objet</th> 
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
   <td> <p>Je fait l’objet d’une délégation en tant qu’approbateur ou approbatrice.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut de l'approbation d'événement déléguée</p> </td> 
   <td> <p>Personne ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation d’un problème déléguée a été remplie. </p> <p>Lorsque vous déléguez l’approbation d’un problème à une autre personne, vous recevez une notification par e-mail une fois cette approbation terminée (que la personne approuve ou refuse l’approbation du problème). </p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut de l'approbation de projet déléguée</p> </td> 
   <td> <p>Personne ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation de projet déléguée a été remplie.</p> <p>Lorsque vous déléguez l’approbation d’un projet à une autre personne, vous recevez une notification par e-mail une fois cette approbation terminée (que la personne approuve ou refuse l’approbation du projet).</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Changement de statut de l'approbation de tâche déléguée</p> </td> 
   <td> <p>Personne ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation de tâche déléguée a été remplie.</p> <p>Lorsque vous déléguez une approbation de tâche à une autre personne, vous recevez une notification par e-mail une fois cette approbation terminée (que la personne approuve ou refuse l’approbation de la tâche).</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Annuler l'approbation du document pour l'approbateur</p> </td> 
   <td> <p>Personne ayant délégué l’approbation</p> </td> 
   <td> <p>Une demande d’approbation du document est annulée.</p> <p>L’approbateur ou l’approbatrice du document reçoit une notification par e-mail lorsque la demande d’approbation du document est annulée.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feuille de temps</p> </td> 
   <td> <p>Approbation de la feuille de temps</p> </td> 
   <td> <p>Utilisateur ou utilisatrice qui possède la feuille de temps</p> </td> 
   <td> <p>Ma feuille de temps est approuvée.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur le travail qui m&#39;a été affecté

Voir aussi [Notifications : informations sur le travail qui m’a été affecté](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Tâche</td> 
   <td>Toutes les tâches antérieures terminées</td> 
   <td>Personnes membres de l’équipe affectées à des tâches dépendantes</td> 
   <td> <p>Toutes les tâches antérieures à celles de l’équipe sont terminées.</p> <p>Les personnes cessionnaires pour la tâche (toutes les personnes membres de l’équipe) reçoivent une notification par e-mail.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td>Inactif</td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Toutes les tâches antérieures terminées</p> </td> 
   <td> <p>Personne affectée aux tâches dépendantes</p> </td> 
   <td> <p>Toutes les tâches antérieures aux miennes sont terminées.</p> <p>La personne cessionnaire pour la tâche reçoit une notification par e-mail.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Décision d’approbation</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui le problème est affecté.</p> </td> 
   <td> <p>Un problème que je résous est approuvé ou rejeté.</p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsqu’une décision d’approbation est prise (approuvée ou rejetée).</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Décision d’approbation</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui la tâche est affectée.</p> </td> 
   <td> <p>Une tâche que j’effectue est approuvée ou rejetée.</p> <p>La personne cessionnaire pour la tâche reçoit une notification par e-mail lorsque la tâche est approuvée ou refusée.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement du problème</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui le problème est affecté.</p> </td> 
   <td> <p>Un problème qui m’est affecté est terminé.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>La date d'achèvement planifiée pour l'événement a changé</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui le problème est affecté.</p> </td> 
   <td> <p>La date d’échéance d’un problème qui m’est affecté change.</p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsque la date d’achèvement prévue change, sauf si c’est elle qui a modifié la date d’achèvement prévue.</p> <p>Une notification est envoyée uniquement si le statut du projet est autre que Planification.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Changement de statut du problème</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui le problème est affecté.</p> </td> 
   <td> <p>Le statut de l’un de mes éléments de travail change.</p> <p>La personne cessionnaire du problème reçoit une notification par e-mail lorsque le statut change, sauf si c’est elle qui a l’a modifié.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout de docuement de demande</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui le problème est affecté.</p> </td> 
   <td> <p>Les documents sont chargés ou modifiés sur des demandes qui me sont affectées.</p> <p>La personne cessionnaire pour le problème reçoit une notification par e-mail lorsque des documents sont chargés ou modifiés sur un problème qu’elle a ajouté.</p> <p>Une notification par e-mail n’est pas envoyée si l’utilisateur ou utilisatrice qui a créé le problème est la personne cessionnaire du problème.</p> <p>Une notification est envoyée uniquement si le statut du projet est En cours et si l’option « Publier en tant que file d’attente des demandes d’aide » est activée pour le projet dans l’onglet Configuration de la file d’attente.</p> </td> 
   <td> <p>Actif (quotidien uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui la tâche est affectée.</p> </td> 
   <td> <p>Une tâche qui m’est affectée est terminée.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail une fois la tâche terminée. Les notifications ne sont pas envoyées lorsqu’une tâche personnelle est terminée.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> <p>Les utilisateurs et utilisatrices disposant d’une licence Light, Contribution, Révision ou Demande ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche</p> </td> 
   <td> <p>Personne affectée à une tâche dépendante</p> </td> 
   <td> <p>Une tâche antérieure à ma tâche est terminée.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque l’une des tâches antérieures est terminée.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>La date d'achèvement prévue pour la tâche a changé</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui la tâche est affectée.</p> </td> 
   <td> <p>La date d’échéance d’une tâche qui m’est affectée change.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque la date d’achèvement prévue de la tâche change, sauf si c’est elle qui l’a modifiée.</p> <p>Une notification est envoyée uniquement si le statut du projet est autre que Planification.</p> <p>Aucune notification n’est envoyée concernant les tâches personnelles.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Changement de statut de la tâche</p> </td> 
   <td> <p>Utilisateur ou utilisatrice à qui la tâche est affectée.</p> </td> 
   <td> <p>Le statut d’une tâche qui m’est affectée change.</p> <p>La personne cessionnaire de la tâche reçoit une notification par e-mail lorsque le statut de la tâche est modifié, sauf si l’utilisateur ou l’utilisatrice qui a modifié le statut est également la personne cessionnaire.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Informations sur les projets auxquels je participe

Voir aussi [Notifications : informations sur les projets sur lesquels je travaille](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Statut actuel du projet</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un projet sur lequel je travaille devient actif.</p> <p>Les utilisateurs et utilisatrices du projet reçoivent une notification par e-mail lorsqu’il devient actif.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout d’un document</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un document est ajouté à un projet sur lequel je travaille.</p> <p>Les utilisateurs et utilisatrices de l’équipe de projet reçoivent une notification par e-mail lorsqu’un document est ajouté au projet, à l’exception de la personne qui a ajouté le document.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel et que le document n’est pas privé. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet sur lequel je travaille.</p> <p>Les utilisateurs et utilisatrices d’un projet reçoivent une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement du problème</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un problème est achevé sur un projet sur lequel je travaille.</p> <p>Toute personne sur le projet reçoit une notification.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche jalonnée</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Une tâche jalonnée est achevée sur un projet sur lequel je travaille.</p> <p>Toutes les personnes de l’équipe de projet reçoivent une notification lorsqu’une tâche jalonnée est achevée. </p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Achèvement du projet</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un projet sur lequel je travaille est achevé.</p> <p>Les personnes d’une équipe de projet reçoivent une notification par e-mail lorsque le statut du projet est Terminé.</p> <p>Conseil : si des projets sont terminés régulièrement, l’activation de cette option peut créer de nombreux e-mails pour les personnes qui ont un nombre limité de tâches sur de nombreux projets. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Changement de statut d’un projet</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Le statut est modifié sur un projet sur lequel je travaille.</p> <p>Les personnes de l’équipe de projet reçoivent une notification par e-mail lorsque le statut du projet est modifié. </p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
     <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Statut actuel du projet</p> </td> 
   <td> <p>Membres de l’équipe affectée</p> </td> 
   <td> <p>Un projet auquel mon équipe participe est devenu actif.</p> <p>Les membres d’une équipe Workfront affectée reçoivent une notification par e-mail lorsque le projet qui leur a été affecté devient actif.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur du projet</p> </td> 
   <td> <p>Ajout d’utilisateurs et utilisatrices au projet</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Je fais l’objet d’un ajout à un projet.</p> <p>La personne qui a été ajoutée au projet reçoit une notification par e-mail lorsqu’elle est ajoutée, sauf si elle s’est ajoutée elle-même au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Une tâche est terminée sur un projet sur lequel je travaille.</p> <p>Les personnes membres de l’équipe de projet reçoivent une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème non attribué</p> </td> 
   <td> <p>Membres de l’équipe de projet</p> </td> 
   <td> <p>Un problème non attribué est ajouté à un projet sur lequel je travaille.</p> <p>Les personnes sur un projet reçoivent une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
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
   <th>Type d’objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout d’un document</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un document est ajouté à un projet dont je suis propriétaire.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un document est ajouté au projet, sauf si c’est elle qui l’a ajouté.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel et que le document n’est pas privé.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet dont je suis propriétaire.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Modification de la date d'engagement pour l'événement</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>La date d’engagement d’un problème sur l’un de mes projets change.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement change pour un problème sur le projet, sauf si c’est elle qui l’a modifiée.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement du problème</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un problème est terminé sur un projet dont je suis propriétaire.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche jalonnée</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Une tâche jalonnée est terminée sur un projet dont je suis propriétaire.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Affectation de la personne propriétaire du projet</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>On me définit comme personne propriétaire d’un nouveau projet.</p> <p>Lorsqu’une personne est définie comme propriétaire d’un projet, elle reçoit une notification par e-mail.</p> <p>Si la personne propriétaire du projet est la personne qui a effectué l’affectation, aucune notification par e-mail n’est envoyée.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Modification de la progression du projet</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un projet dont je suis propriétaire prend du retard.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque le projet est en retard sur le planning.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la date d'engagement pour la tâche</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>La date d’engagement est modifiée pour une tâche sur l’un de mes projets.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsque la date d’engagement est modifiée pour une tâche du projet, sauf si la personne qui a modifié la date d’engagement est également la personne propriétaire du projet.</p> </td> 
   <td> <p>Actif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Une tâche est terminée sur un projet dont je suis propriétaire.</p> <p>La personne propriétaire du projet reçoit une notification. </p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la progression de la tâche</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Une tâche sur un projet dont je suis propriétaire prend du retard.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’une tâche du projet est en retard sur le planning.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème non attribué</p> </td> 
   <td> <p>Propriétaire du projet</p> </td> 
   <td> <p>Un problème non attribué est ajouté à un projet dont je suis propriétaire.</p> <p>La personne propriétaire du projet reçoit une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informations sur les projets que je sponsorise.

Voir aussi [Notifications : informations sur les projets que je sponsorise](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’objet</th> 
   <th>Événement</th> 
   <th>Destinataire</th> 
   <th>Description</th> 
   <th> État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Document</p> </td> 
   <td> <p>Ajout d’un document</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un document est ajouté à un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’un document est ajouté au projet, sauf si c’est elle qui a jouté le document.</p> <p>Une notification est envoyée uniquement si le statut du projet est En cours et si le document n’est pas privé.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un problème est ajouté à un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Achèvement du problème</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un problème est terminé sur un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche jalonnée</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Une tâche jalonnée est terminée sur un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’une tâche jalonnée est terminée sur un projet qu’elle sponsorise.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Modification de la progression du projet</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un projet que je sponsorise prend du retard.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsque le projet est en retard sur le planning.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Affectation d’une personne sponsor du projet</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Je suis la personne sponsor d’un projet.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’elle est définie comme sponsor d’un projet.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Achèvement d’une tâche</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Une tâche est terminée sur un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Modification de la progression de la tâche</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Une tâche sur un projet que je sponsorise prend du retard.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’une tâche du projet est en retard sur le planning.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Ajout d’un problème non attribué</p> </td> 
   <td> <p>Sponsor du projet</p> </td> 
   <td> <p>Un problème non attribué est ajouté sur un projet que je sponsorise.</p> <p>La personne sponsor du projet reçoit une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
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
   <th>Type d’objet</th> 
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
   <td> <p>Annulation de demande de document</p> </td> 
   <td> <p>Utilisateur ou utilisatrice dont le document est demandé.</p> </td> 
   <td> <p>Une demande de chargement de document de ma part est annulée.</p> <p>La personne reçoit une notification par e-mail lorsque sa demande de document est annulée.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Notification d’erreur</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Une erreur a été détectée et requiert mon attention.</p> <p>Une notification par e-mail est générée si Workfront a tenté de se connecter à un compte POP et a échoué. Après 25 tentatives, Workfront désactive la connexion au compte POP afin de préserver les ressources et envoie une notification. </p> <p>La notification est envoyée par e-mail à la personne propriétaire du projet, si l’adresse e-mail POP est associée à une file d’attente de demandes, ou aux administrateurs et administratrices Workfront, si le compte POP est associé à la fonction « Courrier entrant » dans la configuration des e-mails.
   </p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problème</p> </td> 
   <td> <p>Attribution de problèmes</p> </td> 
   <td> <p>Personne propriétaire de la ressource</p> </td> 
   <td> <p>Un changement d’affectation de problème affecte un de mes collaborateurs ou une de mes collaboratrices.</p> <p>La personne responsable des personnes cessionnaires du problème reçoit une notification par e-mail lorsqu’une modification affecte un utilisateur ou une utilisatrice qu’elle gère.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel ou Planification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Nouvel utilisateur</p> </td> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Lors de la création d’un utilisateur ou d’une utilisatrice dans Workfront, lui envoyer un e-mail.</p> <p>Une fois la création de l’utilisateur ou de l’utilisatrice effectuée, une invitation par e-mail l’informant qu’un compte Workfront a été créé et lui demandant de définir son mot de passe lui est envoyé.</p> <p>Lors de la création d’un utilisateur ou d’une utilisatrice, les personnes peuvent sélectionner l’option « Envoyer un e-mail d’invitation à cette personne » (comme décrit dans <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajouter des utilisateurs et utilisatrices</a><span style="font-weight: 400;">). Cependant, lorsque l’option « Nouvel utilisateur ou nouvelle utilisatrice envoyé à l’utilisateur ou à l’utilisatrice » est activée globalement, tous les nouveaux utilisateurs et utilisatrices reçoivent l’invitation par e-mail, que l’option « Envoyer un e-mail d’invitation à cette personne » soit sélectionnée ou non.</span></p> </td> 
   <td> Inactif </td> 
  </tr> 
  <tr> 
   <td> <p>Equipe</p> </td> 
   <td> <p>Partage d’objets</p> </td> 
   <td> <p>Personnes membres de l’équipe avec lesquelles l’objet a été partagé.</p> </td> 
   <td> <p>Une personne partage un objet avec mon équipe.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Partage d’objets</p> </td> 
   <td> <p>Utilisateur ou utilisatrice avec qui l’objet a été partagé.</p> </td> 
   <td> <p>Une personne partage un objet avec moi.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur du projet</p> </td> 
   <td> <p>Ajout d’utilisateurs et utilisatrices au projet</p> </td> 
   <td> <p>Personne propriétaire de la ressource</p> </td> 
   <td> <p>Un de mes collaborateurs ou une de mes collaboratrices fait l’objet d’un ajout au projet.</p> <p>Une personne gestionnaire reçoit une notification par e-mail lorsqu’une personne de ses rapports directs est ajoutée à un projet.</p> <p>Les personnes disposant d’une licence Light ou Révision ne reçoivent pas de notification.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>Projet ajouté à un portefeuille ou un programme</p> </td> 
   <td> <p>Personne propriétaire du portfolio ou du programme</p> </td> 
   <td> <p>Une personne ajoute un projet à un portfolio ou un programme dont je suis propriétaire.</p> </td> 
   <td> <p>Actif (instantané uniquement)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche</p> </td> 
   <td> <p>Affectation de la tâche</p> </td> 
   <td> <p>Personne propriétaire de la ressource</p> </td> 
   <td> <p>Un changement d’affectation d’une tâche affecte un de mes collaborateurs ou une de mes collaboratrices.</p> <p>La personne responsable de la personne cessionnaire de la tâche reçoit une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> </td> 
   <td> <p>Inactif</p> </td> 
  </tr> 
  <tr> 
   <td> Projet <br>Tâche <br>Problème</td> 
   <td>Nouvelle mise à jour</td> 
   <td>Abonné </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Un e-mail est envoyé lorsqu’une mise à jour est effectuée sur un objet (tâche, problème ou projet) auquel j’ai un abonnement.</span> </p> </td> 
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

| Type d’objet | Événement | Destinataire | Description | État par défaut |
|------------------|--------------------------------------------|-----------|--------------------------------------------------------------|-----------------------|
| Tâches et événements | Délégation de tâches et de problèmes | Cessionnaire | Je délègue mes tâches et problèmes (confirmation). | Actif (instantané uniquement) |
| Tâches et événements | Arrêter la délégation de tâches et de problèmes | Cessionnaire | J’arrête de déléguer mes tâches et problèmes (confirmation). | Actif (instantané uniquement) |
| Tâches et événements | Délégation de tâches et de problèmes | Déléguer | Quelqu’un me délègue ses tâches et problèmes. | Actif (instantané uniquement) |
| Tâches et événements | Arrêter la délégation de tâches et de problèmes | Déléguer | Quelqu’un cesse de me déléguer ses tâches et problèmes. | Actif (instantané uniquement) |
