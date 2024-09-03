---
content-type: reference
navigation-topic: notifications
title: '« Notifications : informations sur les projets auxquels je participe »'
description: Les notifications suivantes vous alertent sur les activités qui se produisent dans les projets sur lesquels vous travaillez.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 100%

---

# Notifications : informations sur les projets auxquels je participe

Les notifications suivantes vous alertent sur les activités qui se produisent dans les projets sur lesquels vous travaillez.

Pour plus d’informations sur la configuration des notifications que vous recevez, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consultez également la section [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>Champs inclus </p> <p> * Champs de résumé quotidien uniquement</p> </th> 
   <th>Statut par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Un document est ajouté à un projet auquel je participe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un document est ajouté au projet, à l’exception de l’utilisateur ou de l’utilisatrice qui a ajouté le document.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] et que le document n’est pas Privé.</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Document added to] &lt;Project Name&gt;</em></p> <p>L’objet de la notification de synthèse quotidienne est <em>[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du portfolio<br>Numéro de référence du document<br>Nom de l’utilisateur ou de l’utilisatrice qui a ajouté le document<br>Nom du document<br>Date de l’ajout<br>Détails du document (format, taille, numéro de version)<br>Miniature du document<br><strong>Boutons [!UICONTROL Preview]</strong> et <strong>[!UICONTROL Download]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de documents ajoutés<br>*Nom du document<br>*Nom de l’utilisateur ou de l’utilisatrice qui a chargé le document.<br>*Date de la synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche jalonnée est terminée sur un projet auquel je participe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification lorsqu’une tâche jalonnée sur le projet est terminée. Les notifications ne sont pas envoyées lorsqu’une tâche personnelle est terminée.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>La ligne d’objet est <em>[!UICONTROL Complete] : &lt;Task Name&gt; sur &lt;Project Name&gt;</em></p> <p>L’objet de la notification de synthèse quotidienne est <em>[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de l’utilisateur ou de l’utilisatrice qui a terminé la tâche<br>Statut de la tâche<br>Date et heure auxquelles la tâche a été terminée<br>Statut de la tâche précédente<br><strong>Bouton</strong> [!UICONTROL See More Details] <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de l’utilisateur ou de l’utilisatrice qui a terminé la tâche<br>*Date de la synthèse quotidienne<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque le statut d'un projet passe du statut idée/approuvé/rejeté/demandé/planifié à courant, envoyez un e-mail à l'équipe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsque le statut du projet est défini sur [!UICONTROL Current].</p> <p>Remarque : les utilisateurs et utilisatrices doivent être répertoriés dans l’onglet Personnel d’un projet pour recevoir une notification lorsqu’un statut de projet est défini sur [!UICONTROL Current]. Pour plus d’informations sur l’ajout d’utilisateurs et d’utilisatrices à une équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gérer l’équipe de projet</a>.</p> <p>L’objet de l’e-mail de notification instantanée est <em>&lt;Project Name&gt; [!UICONTROL is Current - Go to your project and see your tasks!]</em></p> <p> L’objet de la notification de synthèse quotidienne est <em>[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Statut du projet<br>[!UICONTROL Planned Completion Date] du projet<br>Propriétaire du projet<br>Une liste des tâches qui vous sont affectées, à l’une de vos fonctions ou à l’une de vos équipes<br><strong>Bouton [!UICONTROL See More Details]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Statut du projet<br>*Date de synthèse quotidienne</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Un projet auquel mon équipe participe est devenu actif</strong> <p>Les membres d’une équipe reçoivent une notification par e-mail lorsqu’un projet devient actif. L’équipe doit être affectée à au moins une tâche pour recevoir la notification.</p><p>Si un utilisateur ou une utilisatrice individuel et une équipe sont tous deux affectés à une tâche sur le projet, l’équipe ne recevra pas de notification.</p><p>L’objet de l’e-mail de notification instantanée est <i>&lt;Project Name&gt; [!UICONTROL is Active - Go to your project and see your tasks!]</i></p><p>L’objet de la notification de synthèse quotidienne est <em>[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p></td> 
   <td>Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Statut du projet<br>[!UICONTROL Planned Completion Date] du projet<br>Propriétaire du projet<br>Une liste des tâches affectées à votre équipe<br><strong>Bouton</strong> [!UICONTROL See More Details]<br>*Nom du projet<br>*Numéro de référence du projet<br>*Statut du projet<br>*Date de synthèse quotidienne</td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un projet auquel je participe est terminé</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsque le statut du projet est [!UICONTROL Complete].</p> <p>Conseil : si des projets sont terminés régulièrement, l’activation de cette option peut créer de nombreux e-mails pour les personnes qui ont un nombre limité de tâches sur de nombreux projets.</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Project Status Change] : &lt;Project Name&gt;</em></p> <p> L’objet de la notification de synthèse quotidienne est <em>[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Nom de l’utilisateur ou de l’utilisatrice qui a terminé le projet<br>Statut du projet<br>Date et heure d’achèvement du projet<br>Statut précédent du projet<br><strong>Bouton</strong> [!UICONTROL See More Details]<br>*Nom du projet<br>*Numéro de référence du projet<br>*Statut du projet<br>*Date de synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une tâche est terminée sur un projet auquel je participe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’une tâche est terminée sur leur projet. <br>Pour plus d’informations sur l’équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Vue d’ensemble de l’équipe d’un projet</a>.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Complete] : &lt;Task Name&gt; on &lt;Project Name&gt;</em></p> <p> <p>Remarque : si la tâche passe à un statut qui correspond à [!UICONTROL Complete], l’objet de l’e-mail affiche toujours « [!UICONTROL Complete] ».</p> </p> <p><em>L’objet de la notification de synthèse quotidienne est le suivant : [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em> </p> </td> 
   <td> <p>Nom de la tâche<br>Nom du projet<br>Numéro de référence de tâche<br>Nom de l’utilisateur ou de l’utilisatrice qui a terminé la tâche<br>Statut de la tâche<br>Date et heure de modification du statut de la tâche<br>Statut précédent de la tâche<br><strong>Bouton Voir Plus de détails</strong> <br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de tâches terminées<br>*Nom de la tâche<br>*Nom de l’utilisateur ou de l’utilisatrice qui a terminé la tâche<br>*Date de la synthèse quotidienne<br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème est ajouté à un projet auquel je participe</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un problème est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est Actuel.</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Issue added to] &lt;Project Name&gt;</em></p> <p> </p> <p> L’objet de la notification de synthèse quotidienne est <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Nom du projet<br>Nom du portfolio<br>Numéro de référence du problème<br>Nom de l’utilisateur ou de l’utilisatrice qui a ajouté le problème<br>Type de problème<br>Nom du problème<br>Date de saisie<br>Priorité du problème<br>Nom de la personne cessionnaire <br>Statut du problème<br>Contact principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés au projet<br>*Nom du problème<br>*Nom de la personne affectée à la publication<br>*Date de la synthèse quotidienne </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème est terminé sur un projet auquel je participe.</strong> </p> <p>Les membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un problème est terminé sur leur projet.<br>Pour plus d’informations sur l’équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Vue d’ensemble de l’équipe de projet</a>.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current] ou [!UICONTROL Planning].</p> <p>L’objet de l’e-mail de notification instantanée est le suivant <em>[!UICONTROL Complete]: &lt;Issue Name&gt; sur &lt;Project Name&gt;</em></p> <p> L’objet de la notification de synthèse quotidienne est <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom du problème<br>Nom du projet<br>Nom de la personne ayant terminé le problème<br>Statut du problème<br>Date et heure auxquelles le problème a été terminé.<br>Statut précédent du problème<br><strong>Bouton [!UICONTROL See More Details]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes terminés<br>*Nom du problème<br>*Nom de la personne affectée au problème<br>*Date de la synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un problème non affecté est ajouté à un projet auquel je participe</strong>. </p> <p>Les personnes membres d’une équipe de projet reçoivent une notification par e-mail lorsqu’un problème non affecté est ajouté au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Who should be assigned to this new issue on] &lt;Project Name&gt;?</em>.</p> <p> L’objet de la notification de synthèse quotidienne est <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom du projet<br>Nom du portfolio<br>Numéro de référence du problème<br>Nom de la personne qui a ajouté le problème.<br>Nom du problème<br>Type de problème<br>Date de saisie<br>Priorité du problème<br>Nom de la personne cessionnaire (vide)<br>Statut du problème<br>Contact principal<br>*Nom du projet<br>*Numéro de référence du projet<br>*Nombre total de problèmes ajoutés<br>*Nom du problème<br>*Nom de la personne qui a ajouté le problème.<br>*Date de la synthèse quotidienne<br></td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>On m’ajoute à un projet</strong> </p> <p>La personne qui a été ajoutée au projet reçoit une notification par e-mail lorsqu’elle est ajoutée, sauf si elle s’est ajoutée elle-même au projet.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL You've been added to the project] &lt;Project Name&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> <p>Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Nom de la personne qui vous a ajouté(e) au projet.<br>[!UICONTROL Planned Start Date] du projet<br>[!UICONTROL Planned Completion Date]<br>Pourcentage du projet terminé<br>Noms d’autres personnes sur le projet<br>Personne propriétaire du projet<br><strong>Bouton Voir Plus de détails</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Date de la synthèse quotidienne</p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Le statut d’un projet auquel je participe est modifié</strong>. </p> <p>Les personnes membres d’une équipe de projet reçoivent une notification par e-mail lorsque le statut du projet change. <br>Pour plus d’informations sur l’équipe de projet, voir <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Vue d’ensemble de l’équipe de projet</a>.</p> <p>L’objet de l’e-mail de notification instantanée est <em>[!UICONTROL Project Status Change] : &lt;Project Name&gt;</em>.</p> <p> L’objet de la notification de synthèse quotidienne est <em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em>.</p> </td> 
   <td> Nom du projet<br>Nom du portfolio<br>Numéro de référence du projet<br>Nom de la personne qui a modifié le statut du projet.<br>Nouveau statut du projet<br>Date et heure de modification du statut du projet<br>Statut précédent du projet<br><strong>Bouton [!UICONTROL See More Details]</strong><br>*Nom du projet<br>*Numéro de référence du projet<br>*Statut du projet<br>*Date de synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
 </tbody> 
</table>
