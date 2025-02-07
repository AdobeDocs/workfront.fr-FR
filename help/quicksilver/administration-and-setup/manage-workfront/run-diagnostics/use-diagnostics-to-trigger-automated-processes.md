---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Utiliser les diagnostics pour déclencher des processus automatisés
description: Vous pouvez utiliser les Diagnostics pour déclencher manuellement des processus automatisés, tels que des scripts temporels, des recalculs ou des notifications par e-mail.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 94%

---

# Utiliser les diagnostics pour déclencher des processus automatisés

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Vous pouvez utiliser les Diagnostics pour déclencher manuellement des processus automatisés, tels que des scripts temporels, des recalculs ou des notifications par e-mail.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utiliser les diagnostics pour déclencher des processus automatisés

1. Cliquez sur l’icône **Menu principal** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![Icône des paramètres d’engrenage](assets/gear-icon-settings.png).

1. Développer **Système**, puis cliquez sur **Diagnostics**.
1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Envoyer des notifications de retard</td> 
      <td> <p>Envoie manuellement les notifications de rappel automatique pour les tâches et les problèmes en retard. </p> <p>Pour plus d’informations sur la configuration des rappels automatiques, voir <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurer des rappels automatiques</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer des notifications précoces</td> 
      <td> <p>Envoie manuellement les notifications de rappel automatique pour les tâches et les problèmes qui approchent les dates d’échéance.</p> <p>Pour plus d’informations sur la configuration des rappels automatiques, voir <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurer des rappels automatiques</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer des notifications de rappel</td> 
      <td> <p>Envoie manuellement des notifications de rappel. </p> <p>Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurer des notifications de rappel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Examiner tous les comptes POP</td> 
      <td> <p>Recherche de nouveaux e-mails envoyés aux comptes POP liés à Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recalculer les chronologies</td> 
      <td> <p>Recalcule la chronologie de tous les projets Workfront qui ont le statut Actif. </p> <p>Pour plus d’informations sur le calcul automatique ou manuel de la chronologie des projets, projet par projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculer les chronologies des projets</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rétablir les rapports clients par défaut</td> 
      <td>Restaure les rapports par défaut qui ont été initialement fournis avec Workfront, de sorte qu’ils soient visibles dans la section <strong>Rapports</strong> pour tous les utilisateurs et toutes les utilisatrices.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Générer des feuilles de temps</td> 
      <td>Générer des feuilles de temps pour des personnes selon leur profil de feuille de temps récurrente Cette option ne doit être exécutée que si le profil de feuille de temps a été modifié de manière significative une fois qu’il a été attribué aux personnes, et uniquement après la suppression de toutes les feuilles de temps actuelles et futures.</td> 
     </tr> 
    </tbody> 
   </table>
