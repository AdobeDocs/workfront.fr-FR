---
content-type: reference
navigation-topic: notifications
title: "Notifications : informations sur les projets sur lesquels je me trouve"
description: Les notifications suivantes vous alertent sur les activités qui se produisent dans les projets sur lesquels vous travaillez.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 6%

---

# Notifications : informations sur les projets sur lesquels je travaille

Les notifications suivantes vous alertent sur les activités qui se produisent dans les projets sur lesquels vous travaillez.

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
   <td> <p><strong>Envoyer un e-mail à l'équipe lorsqu'un document est ajouté.</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par courrier électronique lorsqu’un document est ajouté au projet, à l’exception de l’utilisateur qui a ajouté le document.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et que le document n’est pas Privé.</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Document ajouté à] &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est <em>[!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du document<br>Nom de l’utilisateur qui a ajouté le document<br>Document Name<br>Ajout de la date "À"<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Téléchargement]</strong> boutons<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents ajoutés<br>*Nom du document<br>*Nom de l’utilisateur qui a téléchargé le document.<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail à l'équipe lorsqu'une tâche jalonnée est terminée.</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification lorsqu’une tâche de jalon sur le projet est terminée. Les notifications ne sont pas envoyées lorsqu’une tâche personnelle est terminée.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet est <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Task Name<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>État de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Task Name<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le statut d'un projet passe du statut idée/approuvé/rejeté/demandé/planifié à courant, envoyez un e-mail à l'équipe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsque l’état du projet est défini sur [!UICONTROL Actuel].</p> <p>Remarque : Les utilisateurs doivent être répertoriés dans l’onglet Personnel d’un projet pour recevoir une notification lorsqu’un état de projet est défini sur [!UICONTROL Actuel]. Pour plus d’informations sur l’ajout d’utilisateurs à une équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gérer l’équipe de projet</a>.</p> <p>L'objet de l'email de notification instantanée est <em>&lt;project name=""&gt; [!UICONTROL is Current - Accédez à votre projet et voyez vos tâches !]</em></p> <p> L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>État du projet<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Propriétaire du projet<br>Liste des tâches qui vous sont affectées, à l’un de vos rôles de tâche ou à l’une de vos équipes<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*État du projet<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Un projet auquel mon équipe participe est devenu actif</strong> <p>Les membres d’une équipe reçoivent une notification par e-mail lorsqu’un projet devient actif. L'équipe doit être affectée à au moins une tâche pour recevoir la notification.</p><p>Si un utilisateur individuel et une équipe sont tous deux affectés à une tâche sur le projet. l’équipe ne recevra pas de notification.</p><p>L'objet de l'email de notification instantanée est <i>&lt;project name=""&gt; [!UICONTROL est actif : accédez à votre projet et voyez vos tâches !]</i></p><p>L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>État du projet<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Propriétaire du projet<br>Liste des tâches affectées à votre équipe<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*État du projet<br>*Date du résumé quotidien</td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand un projet est terminé, envoyer un e-mail à l'équipe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsque l’état du projet est [!UICONTROL Terminé].</p> <p>Conseil : Si les projets sont terminés régulièrement, l’activation de cette option peut créer de nombreux courriers électroniques pour les utilisateurs qui ont un nombre limité de tâches sur de nombreux projets.</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Modification de l’état du projet] : &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur ayant terminé le projet<br>État du projet<br>Date et heure auxquelles le projet a été terminé<br>État précédent du projet<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*État du projet<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quand une tâche est terminée, envoyer un e-mail à l'équipe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’une tâche est terminée sur leur projet. <br>Pour plus d’informations sur l’équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Présentation de l’équipe de projet</a>.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Complete] : &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Remarque : Si la tâche est modifiée et passe à l’état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".</p> </p> <p><em> Le sujet de la notification quotidiennement est le suivant : [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>Task Name<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>État de la tâche<br>Date et heure de modification de l’état de la tâche<br>État de la tâche précédente<br><strong>Voir Plus de détails</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Task Name<br>*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail à l'équipe lorsqu'un événement est ajouté.</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est Actuel.</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Problème ajouté à] &lt;project name=""&gt;</em></p> <p> </p> <p> L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Type de problème<br>Nom du problème<br>Date de saisie<br>Priorité du problème<br>Nom attribué <br>État du problème<br>Contact Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés au projet<br>*Nom du problème<br>*Nom de l’utilisateur affecté à la publication<br>*Date du résumé quotidien </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'un événement est conclu, envoyer un e-mail à l'équipe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par courrier électronique lorsqu’un problème est survenu sur leur projet.<br>Pour plus d’informations sur l’équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Présentation de l’équipe de projet</a>.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Complete] : &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Nom de l’utilisateur ayant terminé le problème<br>État du problème<br>Date et heure auxquelles le problème a été terminé<br>État du problème précédent<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom de l’utilisateur affecté à la publication<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Envoyer un e-mail à l'équipe lorsqu'un événement non affecté est ajouté.</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Qui doit être affecté à ce nouveau problème le] &lt;project name=""&gt;?</em></p> <p> L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom attribué (vide) <br>État du problème<br>Contact Principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés<br>*Nom du problème<br>*Nom de l’utilisateur qui a ajouté le problème<br>*Date du résumé quotidien<br></td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'un utilisateur est ajouté à l'équipe de projet, envoyer un e-mail à l'utilisateur</strong> </p> <p>L’utilisateur qui a été ajouté au projet reçoit une notification par courrier électronique lorsqu’il est ajouté, sauf s’il s’est ajouté lui-même au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Vous avez été ajouté au projet] &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui vous a ajouté au projet<br>[!UICONTROL Date de début planifiée] du projet<br>[!UICONTROL Date d’achèvement prévue du projet]<br>Pourcentage du projet terminé<br>Noms d’autres sur le projet <br>Propriétaire du projet<br><strong>Voir Plus de détails</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le statut d'un projet est modifié, envoyer un e-mail à l'équipe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par courrier électronique lorsque l’état du projet change. <br>Pour plus d’informations sur l’équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Présentation de l’équipe de projet</a>.</p> <p>L'objet de l'email de notification instantanée est <em>[!UICONTROL Modification de l’état du projet] : &lt;project name=""&gt;</em></p> <p> L’objet de la notification quotidiennement Digest est <em> [!UICONTROL Résumé des projets sur lesquels vous vous trouvez] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a modifié l’état du projet<br>Nouvel état du projet<br>Date et heure de modification du statut du projet<br>État précédent du projet<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Nom du projet<br>*Numéro de référence du projet<br>*État du projet<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
 </tbody> 
</table>
