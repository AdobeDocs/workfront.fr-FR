---
title: Configuration des préférences de tâche et de problème pour un groupe
user-type: administrator
product-area: system-administration;user-management;setup
keywords: group,preferences,task,issue,unlock
navigation-topic: create-and-manage-groups
description: Si des groupes de votre entreprise doivent configurer une tâche ou une préférence d’émission indépendamment de la façon dont elle est configurée au niveau du système, un administrateur Adobe Workfront peut déverrouiller la préférence. Ensuite, en tant qu’administrateur de groupe, vous pouvez configurer les préférences de votre groupe, ce qui aura une incidence sur toutes les tâches ou tous les problèmes associés à votre groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 8%

---

# Configuration des préférences de tâche et de problème pour un groupe

Si des groupes de votre entreprise doivent configurer une tâche ou une préférence d’émission indépendamment de la façon dont elle est configurée au niveau du système, un administrateur Adobe Workfront peut déverrouiller la préférence. Ensuite, en tant qu’administrateur de groupe, vous pouvez configurer les préférences de votre groupe, ce qui aura une incidence sur toutes les tâches ou tous les problèmes associés à votre groupe.

S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur la façon dont l’administrateur Workfront déverrouille les préférences, voir [Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Une configuration au niveau du groupe est également possible pour les préférences du projet. Pour plus d’informations, voir [Configuration des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* En règle générale, une préférence déverrouillée reste déverrouillée indéfiniment. Si l’administrateur Workfront le reverrouille, le paramètre système prend à nouveau effet et les paramètres de la préférence accordée par les administrateurs du groupe sont perdus.
>* Les préférences définies pour le groupe associé à un projet sont prioritaires sur celles définies pour le groupe d’accueil de l’utilisateur qui crée le projet.
>* Certaines préférences au niveau du groupe affectent les modèles de projet que vous créez pour le groupe. Pour plus d’informations, reportez-vous à la section [Affichage, utilisation et création de modèles pour votre groupe à partir de la zone Groupes](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) de l’article [Création et modification de modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Une fois qu’un administrateur Workfront a déverrouillé une préférence au niveau du système, vous pouvez la configurer, puis la verrouiller pour vous assurer que tous les membres de votre groupe et de ses sous-groupes utilisent la même configuration. Cela est parallèle à la possibilité qu’un administrateur de Workfront a de configurer et de verrouiller une préférence pour tous les utilisateurs du système. Pour plus d’informations, voir [Verrouillage ou déverrouillage d’un projet, d’une tâche ou de préférences d’émission pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

+++

## Configuration des préférences de tâche déverrouillée et de problème pour un groupe de niveau supérieur

>[!TIP]
>
>Si vous êtes administrateur de Workfront, vous pouvez ignorer les étapes 1 à 4 en accédant à Configuration > Préférences du projet > Tâches et problèmes, puis en recherchant le nom du groupe dans la zone située en haut de la page.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez configurer la tâche déverrouillée et les préférences d’émission.
1. Sur la page qui s’affiche pour le groupe, dans le panneau de gauche, cliquez sur **Task &amp; Issue Preferences**.
1. Sur la page qui s’affiche, passez à l’une des 5 sections répertoriées ci-dessous pour configurer les paramètres des zones Nouvelles tâches par défaut, Problèmes, Suppression, Dates réelles et Accès, puis cliquez sur **Enregistrer**.

   Si vous passez la souris sur l’icône de verrouillage ![](assets/lock-toggle-button-dimmed.png) pour une préférence que vous devez configurer et qu’une info-bulle s’affiche pour vous indiquer que est verrouillé, vous pouvez demander à votre administrateur Workfront de la déverrouiller pour tous les groupes de l’organisation.

   Lorsqu’il est déverrouillé, vous et d’autres administrateurs de groupe pouvez le configurer séparément pour vos propres groupes. Vous pouvez également le verrouiller pour votre groupe et tous les sous-groupes situés sous votre groupe.

   * [Nouvelles valeurs par défaut de tâche](#new-task-defaults)
   * [Événements](#issues)
   * [Suppression](#deletion)
   * [Dates effectives](#actual-dates)

     <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [Accès](#access)

### Paramètres par défaut de la nouvelle tâche {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Date de début pour les nouvelles tâches</td> 
      <td> <p>Détermine la date de début par défaut des nouvelles tâches pour les gestionnaires de projet. La date de début des nouvelles tâches peut être la date de début prévue du projet ou le jour de création de la tâche.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Type de durée </p> </td> 
      <td> <p>Détermine la relation entre le nombre de ressources (et leur pourcentage d’allocation) et la durée ou l’effort total de la tâche. Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Task Duration and Duration Types : article index</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de revenus</td> 
      <td> <p>Calcule les estimations de recettes prévues et réelles pour une tâche. Lorsque le <strong>Type de revenu</strong> est défini sur <strong>Non facturable</strong>, les heures planifiées et les heures réelles enregistrées ne génèrent pas d’estimation de recettes pour la tâche, et le travail sur la tâche ne contribue pas aux recettes au niveau du projet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de coût</td> 
      <td> <p>Calcule les estimations de coûts prévues et réelles pour une tâche. Lorsque la valeur est définie sur <strong>Aucun coût</strong>, les heures planifiées et les heures réelles enregistrées ne génèrent pas d’estimation de coût planifiée ou réelle de la tâche, et le travail sur la tâche ne contribue pas aux coûts au niveau du projet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Problèmes {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mettre à jour automatiquement le statut des événements pouvant être résolus lorsque le statut de l'objet de résolution change</td> 
      <td> <p>Lorsqu’une personne convertit un problème en projet ou tâche, le problème d’origine et le projet ou la tâche converti deviennent des objets de résolution. Ce paramètre vous permet de mettre en corrélation la résolution du problème d’origine avec la résolution de son objet résolvable. Pour plus d’informations sur la résolution d’objets, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution d’objets résolvables </a>.</p> <p>Pour que ce paramètre ait un effet, l’option <strong>Conserver le problème d’origine et lier sa résolution à la tâche</strong> doit être sélectionnée.</p> 
       <ul> 
        <li>Lorsque ce paramètre est activé, vous pouvez créer des états personnalisés avec la même clé pour les problèmes, les projets ou les tâches. Lorsque le projet ou la tâche (en tant qu’objet résolvable) devient un état personnalisé, la modification se répercute également sur l’état du problème. La clé d’état doit être la même pour le problème et les états du projet ou de la tâche.</li> 
        <li>Lorsque ce paramètre est désactivé, les statuts des objets de résolution sont automatiquement définis sur l’état par défaut, au lieu des statuts personnalisés. Pour plus d’informations sur les états par défaut, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accès à la liste des états des problèmes système</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lors de la conversion d’un problème en tâche</td> 
      <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion, d’un problème à l’autre :</p> 
       <ul> 
        <li><strong>Conserver le problème d’origine et lier sa résolution à la tâche</strong> : lorsque vous convertissez le problème, il reste visible en tant que problème jusqu’à ce que la tâche soit terminée. Le statut du problème passe automatiquement à Fermé lorsque la tâche est terminée.</li> 
        <li><strong>Autoriser les contacts de Principal à avoir accès à la tâche</strong> : permet au contact principal (créateur du problème) d’accéder à la tâche pour examiner la tâche, effectuer des mises à jour et rester informé de son avancement.</li> 
        <li> <p><strong>Autoriser la modification de ces paramètres lors de la conversion</strong> : permet à l’utilisateur qui convertit le problème de modifier ces options lors de la conversion d’un problème en tâche.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lors de la conversion d’un problème en projet</td> 
      <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion d’un problème à l’autre :</p> 
       <ul> 
        <li><strong>Conserver le problème d’origine et lier sa résolution au projet</strong> : lorsque vous convertissez le problème, il reste visible en tant que problème jusqu’à la fin du projet. Le statut du problème passe automatiquement à Fermé lorsque le projet est terminé.</li> 
        <li><strong>Autoriser les contacts de Principal à avoir accès au projet</strong> : donne au contact principal (créateur du problème) l’accès au projet pour examiner le projet, effectuer des mises à jour et rester informé de son avancement.</li> 
        <li><strong>Autoriser la modification de ces paramètres lors de la conversion</strong> : permet à l’utilisateur qui convertit le problème de modifier les options répertoriées lors de la conversion d’un problème en projet.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Suppression {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Autoriser les utilisateurs à supprimer les tâches et les événements comportant des heures consignées</td> 
      <td> <p> Permet de déterminer si vous autorisez la suppression de tâches ou de problèmes lorsque des heures sont enregistrées. Cette option est sélectionnée par défaut.</p> 
       <div> 
        <p><b>Conseil</b> : ce paramètre s’applique également à la suppression de projets comportant des tâches ou des problèmes avec des heures de connexion. Ce paramètre ne s’applique pas à la suppression de projets pour lesquels le temps est consigné directement pour le projet. </p> 
        <p>Tenez compte des points suivants :</p> 
        <ul> 
         <li> <p>Lorsqu’elle est sélectionnée, vous recevez un avertissement informatif lorsque vous supprimez une tâche ou un problème. L’avertissement vous rappelle que si la tâche ou le problème a des heures enregistrées, elles seront déplacées vers le projet ou supprimées. Vous pouvez définir si les heures sont supprimées ou déplacées vers le projet dans la zone Préférences de la feuille de temps et des heures de la configuration. Une fois que vous avez confirmé l’affichage de l’avertissement, la tâche ou le problème est supprimé. Pour plus d’informations sur la configuration des préférences de la feuille de temps et des heures, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref"> Configuration des préférences de la feuille de temps et de l’heure</a>. </p> <p>Conseil : <span>Lorsque vous supprimez un projet avec des tâches et des problèmes ayant des heures journalisées, les heures journalisées sont supprimées ou elles sont conservées conformément aux paramètres de la zone Préférences de la feuille de temps et des heures de la configuration</span>. </p> </li> 
         <li><span>Lorsque vous désélectionnez cette option, vous recevez un avertissement prohibitif lorsque vous supprimez une tâche ou un problème avec les heures enregistrées, ou lorsque vous supprimez un projet avec les heures enregistrées pour ses tâches ou problèmes</span> <span>.</span> L’avertissement indique que l’administrateur n’autorise pas la suppression de tâches ou de problèmes avec les heures enregistrées. Les tâches, problèmes<span> ou projets dont les heures sont enregistrées pour les tâches et problèmes</span> ne peuvent pas être supprimés. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Dates effectives {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lorsqu’une tâche ou un problème passe de "Nouveau" à "En cours", définissez la Date de début réelle sur</td> 
      <td> <p>Sélectionnez l’une des options suivantes lorsque la Date de début réelle est enregistrée dans Workfront lorsqu’une tâche ou un problème passe de <strong>New</strong> à <strong>En cours</strong> :</p> 
       <ul> 
        <li><strong>Maintenant :</strong> La date de début réelle est définie sur la date actuelle.</li> 
        <li><strong>Date de début planifiée :</strong> La date de début réelle est définie sur la date de début planifiée de la tâche ou du problème.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsqu’une tâche ou un problème est terminé, définissez la Date de fin réelle sur</td> 
      <td> <p>Sélectionnez l’une des options suivantes lorsque la Date de fin réelle est enregistrée dans Workfront lorsqu’une tâche ou un problème est terminé :</p> 
       <ul> 
        <li><strong>Maintenant : </strong> La date d’achèvement réelle est définie sur la date actuelle.</li> 
        <li> <p><strong>Date d’achèvement planifiée :</strong> La date d’achèvement réelle est définie sur la date d’achèvement planifiée de la tâche ou du problème.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Accès {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lorsqu’une personne est affectée à une tâche</td> 
      <td> 
       <ul> 
        <li><strong>Donnez-leur ... accès à une tâche</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour la tâche à laquelle il est affecté. Pour plus d’informations sur les autorisations de tâche, voir<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Octroi de l’accès aux utilisateurs</a>.</li> 
        <li> <p><strong>Leur accorder également ... l’accès au projet</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour le projet auquel une tâche lui est affectée. Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsqu’une personne est affectée à un problème</td> 
      <td> 
       <ul> 
        <li><strong>Donnez-leur ... accès à une tâche</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour la tâche à laquelle il est affecté. Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Octroi de l’accès aux utilisateurs</a>.</li> 
        <li> <p><strong>Leur accorder également ... l’accès au projet</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour le projet auquel une tâche lui est affectée. Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsqu’une personne envoie une requête</td> 
      <td> 
       <ul> 
        <li><strong>Donnez-leur ... accès au problème</strong> : définit l’autorisation par défaut d’un utilisateur sur une demande qu’il a envoyée. Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème</a>.</li> 
        <li> <p><strong>Les personnes d’une même société hériteront des mêmes autorisations pour toutes les requêtes</strong> : permet aux utilisateurs d’afficher les requêtes envoyées par d’autres utilisateurs de la même société qu’eux. Ils disposent des mêmes autorisations sur ces demandes que sur leurs propres demandes envoyées.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
