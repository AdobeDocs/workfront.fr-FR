---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Utiliser les diagnostics pour déclencher des processus automatisés
description: Vous pouvez utiliser l’option Diagnostics pour déclencher manuellement des processus automatisés, tels que des scripts temporels, des recalculs ou des notifications par courrier électronique.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 16%

---

# Utiliser les diagnostics pour déclencher des processus automatisés

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Vous pouvez utiliser l’option Diagnostics pour déclencher manuellement des processus automatisés, tels que des scripts temporels, des recalculs ou des notifications par courrier électronique.

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">Formule Adobe Workfront</a> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences</a> </td> 
   <td> <p>Plan </p>Vous devez être un administrateur Workfront. Pour plus d’informations sur les administrateurs de Workfront, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès d’administration complet à un utilisateur</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Utiliser des diagnostics pour déclencher des processus automatisés

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Développez **Système**, puis cliquez sur **Diagnostics**.
1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Envoyer des notifications de retard</td> 
      <td> <p>Envoie manuellement les notifications de rappel automatique pour les tâches en retard et les problèmes. </p> <p>Pour plus d’informations sur la configuration des rappels automatiques, voir <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configuration des rappels automatiques</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer des notifications précoces</td> 
      <td> <p>Envoie manuellement les notifications de rappel automatique pour les tâches et les problèmes qui approchent les dates d’échéance.</p> <p>Pour plus d’informations sur la configuration des rappels automatiques, voir <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configuration des rappels automatiques</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer des notifications de rappel</td> 
      <td> <p>Envoie manuellement des notifications de rappel. </p> <p>Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuration des notifications de rappel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Examiner tous les comptes POP</td> 
      <td> <p>Vérifie les nouveaux emails envoyés aux comptes POP liés à Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recalculer les chronologies</td> 
      <td> <p>Recalcule la chronologie de tous les projets Workfront qui sont à l’état Actuel. </p> <p>Pour plus d’informations sur le calcul automatique ou manuel de la chronologie des projets, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculer la chronologie des projets</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rétablir les rapports clients par défaut</td> 
      <td>Restaure les rapports par défaut qui ont été initialement fournis avec Workfront, de sorte qu’ils soient visibles dans la section <strong>Rapports</strong> pour tous les utilisateurs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Générer des feuilles de temps</td> 
      <td>Génère des feuilles de temps pour les utilisateurs en fonction de leurs profils de feuilles de temps récurrents. Cette option ne doit être exécutée que si le profil de la feuille de temps a été modifié de manière significative une fois qu’il a été attribué aux utilisateurs, et uniquement après la suppression de toutes les feuilles de temps actuelles et futures.</td> 
     </tr> 
    </tbody> 
   </table>
