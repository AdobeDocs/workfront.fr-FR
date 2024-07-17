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
ht-degree: 4%

---

# Notifications : informations sur les projets auxquels je participe

Les notifications suivantes vous alertent sur les activités qui se produisent dans les projets sur lesquels vous travaillez.

Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Un document est ajouté à un projet sur lequel je me trouve </strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par courrier électronique lorsqu’un document est ajouté au projet, à l’exception de l’utilisateur qui a ajouté le document.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] et que le document n’est pas Privé.</p> <p>L’objet de l’email de notification instantanée est <em>[!UICONTROL Document ajouté à] &lt;Nom du projet&gt;</em></p> <p>L’objet de la notification quotidiennement de résumé est <em>[!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du document<br>Nom de l’utilisateur qui a ajouté le document<br>Nom du document<br>Ajout à la date<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>[!UICONTROL Aperçu]</strong> et <strong>[!UICONTROL Télécharger]</strong> 12}*Numéro de référence du projet<br>*Nombre total de documents ajoutés<br>*Nom du document<br>*Nom de l’utilisateur ayant téléchargé le document<br>*Date du résumé quotidien<br><br> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche de jalon est terminée sur un projet sur lequel je me trouve</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification lorsqu’une tâche de jalon sur le projet est terminée. Les notifications ne sont pas envoyées lorsqu’une tâche personnelle est terminée.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet est <em>[!UICONTROL Complete]: &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p>L’objet de la notification de résumé quotidien est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>État de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>État de la tâche précédente<br><strong>[!UICONTROL Voir plus de détails]</strong> <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche *Nom de la tâche <br>*Nom de la tâche *Nom de la tâche*Nom de l’utilisateur qui a terminé la tâche<br>*Date du résumé quotidien<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le statut d'un projet passe du statut idée/approuvé/rejeté/demandé/planifié à courant, envoyez un e-mail à l'équipe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsque l’état du projet est défini sur [!UICONTROL Actuel].</p> <p>Remarque : Les utilisateurs doivent être répertoriés dans l’onglet Personnel d’un projet pour recevoir une notification lorsqu’un état de projet est défini sur [!UICONTROL Actuel]. Pour plus d’informations sur l’ajout d’utilisateurs à une équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gérer l’équipe de projet</a>.</p> <p>L’objet de l’e-mail de notification instantanée est <em>&lt;Nom du projet&gt; [!UICONTROL est Actuel - Accédez à votre projet et consultez vos tâches !]</em></p> <p> Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>État du projet<br>Date d’achèvement prévue du projet]<br>Propriétaire du projet<br>Liste des tâches qui vous ont été affectées, à l’un de vos rôles de travail ou à l’une de vos équipes<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>}*Numéro de référence du projet<br>}}} État du projet<br>*Date du résumé quotidien</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Un projet sur lequel mon équipe est active</strong> <p>Les membres d’une équipe reçoivent une notification par e-mail lorsqu’un projet devient actif. L'équipe doit être affectée à au moins une tâche pour recevoir la notification.</p><p>Si un utilisateur individuel et une équipe sont tous deux affectés à une tâche sur le projet. l’équipe ne recevra pas de notification.</p><p>L’objet de l’e-mail de notification instantanée est <i>&lt;Nom du projet&gt; [!UICONTROL est actif - Accédez à votre projet et consultez vos tâches !]</i></p><p>Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p></td> 
   <td>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>État du projet<br>Date d’achèvement prévue du projet]<br>Propriétaire du projet<br>Liste des tâches affectées à votre équipe<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*État du projet<br>}</td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un projet sur lequel je suis en cours est terminé</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsque l’état du projet est [!UICONTROL Terminé].</p> <p>Conseil : si les projets sont terminés régulièrement, l’activation de cette option peut générer un grand nombre d’e-mails pour les utilisateurs et utilisatrices qui ont un nombre limité de tâches sur de nombreux projets.</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Modification de l’état du projet] : &lt;Nom du projet&gt;</em></p> <p> Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a terminé le projet<br>État du projet<br>Date et heure auxquelles le projet a été terminé<br>État du projet précédent<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*État du projet<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche est terminée sur un projet sur lequel je suis sur</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’une tâche est terminée sur leur projet. <br>Pour plus d’informations sur l’équipe de projet, consultez la <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">présentation de l’équipe de projet</a>.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Complete] : &lt;Nom de la tâche&gt; sur &lt;Nom du projet&gt;</em></p> <p> <p>Remarque : Si la tâche est modifiée et passe à l’état qui correspond à [!UICONTROL Terminé], l’objet de l’email affiche toujours "[!UICONTROL Terminé]".</p> </p> <p><em> Le sujet de la notification quotidiennement de résumé est : [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em> </p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a terminé la tâche<br>État de la tâche<br>Date et heure auxquelles l’état de la tâche a été modifié<br>État de la tâche précédente<br><strong>Voir plus de détails</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche *Nom de la tâche<br>}*Nom de la tâche utilisateur ayant terminé la tâche<br>*Date du résumé quotidien<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème est ajouté à un projet sur lequel je me trouve </strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification n’est envoyée que si le statut du projet est Actuel.</p> <p>L’objet de l’email de notification instantanée est <em>[!UICONTROL Problème ajouté à] &lt;Nom du projet&gt;</em></p> <p> </p> <p> Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Type de problème<br>Nom du problème<br>Date d’entrée<br>Priorité du problème<br>Attribué au nom <br>État du problème<br>Principal Contact<br>*Nom du projet<br>*Numéro de référence du projet<br>}}*Nombre total du nombre total de problèmes ajouté au projet<br>}}}}}}}}}}}}}*Nombre total de problèmes *Nom du problème<br>*Nom de l’utilisateur affecté à la publication<br>*Date du résumé quotidien </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème est survenu sur un projet sur lequel je suis sur</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par courrier électronique lorsqu’un problème est survenu sur leur projet.<br>Pour plus d’informations sur l’équipe de projet, consultez la <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">présentation de l’équipe de projet</a>.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel] ou [!UICONTROL Planification].</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Complete] : &lt;Nom du problème&gt; sur &lt;Nom du projet&gt;</em></p> <p> Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Nom de l’utilisateur ayant terminé le problème<br>État du problème<br>Date et heure auxquelles le problème a été terminé<br>État du problème précédent<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom du projet de l’utilisateur affecté<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème non attribué est ajouté à un projet sur lequel je me trouve </strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un problème non attribué est ajouté au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L’objet de l’email de notification instantanée est <em>[!UICONTROL Qui doit être affecté à ce nouveau problème sur] &lt;Nom du projet&gt; ?</em></p> <p> Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a ajouté le problème<br>Nom du problème<br>Type de problème<br>Date d’entrée<br>Priorité du problème<br>Affecté à un nom (vide) <br>État du problème<br>Principal Contact<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total}}*État du problème Nombre total de problèmes de problèmes d’ajout<br>}}}}}}*Nombre total de problèmes }}}}}*Nombre total *Nom du problème<br>*Nom de l’utilisateur qui a ajouté le problème<br>*Date du résumé quotidien<br></td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Je suis ajouté à un projet</strong> </p> <p>L’utilisateur qui a été ajouté au projet reçoit une notification par courrier électronique lorsqu’il est ajouté, sauf s’il s’est ajouté lui-même au projet.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L’objet de l’email de notification instantanée est <em>[!UICONTROL Vous avez été ajouté au projet] &lt;Nom du projet&gt;</em></p> <p> Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> <p>Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui vous a ajouté au projet<br>Projet [!UICONTROL Date de début planifiée]<br>Date de fin planifiée du projet]<br>Pourcentage du projet terminé<br>Noms des autres sur le projet <br>Propriétaire du projet<br><strong>Voir Plus de détails</strong>}*Nom du projet<br> *Numéro de référence du projet<br>*Date du résumé quotidien<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>L’état change sur un projet sur lequel je me trouve</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par courrier électronique lorsque l’état du projet change. <br>Pour plus d’informations sur l’équipe de projet, consultez la <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">présentation de l’équipe de projet</a>.</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Modification de l’état du projet] : &lt;Nom du projet&gt;</em></p> <p> Le sujet de la notification quotidiennement de résumé est <em> [!UICONTROL Résumé des projets que vous utilisez] &lt;Date du résumé quotidien&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du Portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur qui a modifié l’état du projet<br>Nouvel état du projet<br>Date et heure auxquelles l’état du projet a changé<br>État du projet précédent<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>}*État du projet <br>*État du projet digest </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
 </tbody> 
</table>
