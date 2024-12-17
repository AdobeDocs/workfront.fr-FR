---
title: Configuration des préférences de tâche et de problème pour un groupe
user-type: administrator
product-area: system-administration;user-management;setup
keywords: groupe,préférences,tâche,problème,déverrouiller
navigation-topic: create-and-manage-groups
description: Si des groupes de votre entreprise doivent configurer une préférence de tâche ou de problème indépendamment de sa configuration au niveau du système, un administrateur ou une administratrice Adobe Workfront peut déverrouiller la préférence. Ensuite, en tant qu’administrateur ou administratrice de groupes, vous pouvez configurer les préférences de votre groupe, ce qui aura une incidence sur toutes les tâches associées ou tous les problèmes associés à votre groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1885'
ht-degree: 98%

---

# Configurer les préférences de tâches et de problèmes pour un groupe

Si des groupes de votre entreprise doivent configurer une préférence de tâche ou de problème indépendamment de sa configuration au niveau du système, un administrateur ou une administratrice Adobe Workfront peut déverrouiller la préférence. Ensuite, en tant qu’administrateur ou administratrice de groupes, vous pouvez configurer les préférences de votre groupe, ce qui aura une incidence sur toutes les tâches associées ou tous les problèmes associés à votre groupe.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur le déverrouillage des préférences par l’administrateur ou l’administratrice Workfront, voir [Verrouiller ou déverrouiller les préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Une configuration au niveau du groupe est également possible pour les préférences de projet. Pour plus d’informations, voir [Configurer les préférences des projets de groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* En règle générale, une préférence déverrouillée reste déverrouillée indéfiniment. Si l’administrateur ou l’administratrice Workfront la verrouille à nouveau, le paramètre système prend à nouveau effet et les paramètres de la préférence définie par les administrateurs et administratrices de groupes sont perdus.
>* Les préférences définies pour le groupe associé à un projet sont prioritaires sur celles définies pour le groupe principal de l’utilisateur ou de l’utilisatrice qui crée le projet.
>* Certaines préférences au niveau du groupe affectent les modèles de projet que vous créez pour le groupe. Pour plus d’informations, voir la section [Afficher, utiliser et créer des modèles pour votre groupe à partir de la zone Groupes](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) dans l’article [Créer et modifier des modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Une fois qu’un administrateur ou une administratrice Workfront a déverrouillé une préférence au niveau du système, vous pouvez la configurer, puis la verrouiller pour vous assurer que toutes les personnes membres de votre groupe et de ses sous-groupes utilisent la même configuration. Ceci vient en parallèle de la capacité qu’a un administrateur ou une administratrice Workfront de configurer et de verrouiller une préférence pour tous les utilisateurs et utilisatrices du système. Pour plus d’informations, voir [Verrouiller ou déverrouiller une préférence de projet, de tâche ou de problème pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

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
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer les préférences de tâche et de problème déverrouillées pour un groupe de niveau supérieur

>[!TIP]
>
>Si vous êtes un administrateur ou une administratrice Workfront, vous pouvez ignorer les étapes 1 à 4 en accédant à Configuration > Préférences du projet > Tâches et problèmes, puis en recherchant le nom du groupe dans la zone située en haut de la page.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez configurer les préférences de tâche et de problème déverrouillées.
1. Sur la page qui s’affiche pour le groupe, dans le panneau de gauche, cliquez sur **Préférences de tâche et de problème**.
1. Sur la page qui s’affiche, passez à l’une des 5 sections répertoriées ci-dessous pour configurer les paramètres des zones Paramètres par défaut de la nouvelle tâche, Problèmes, Suppression, Dates effectives et Accès, puis cliquez sur **Enregistrer**.

   Si vous pointez sur l’icône de verrouillage ![](assets/lock-toggle-button-dimmed.png) d’une préférence que vous devez configurer et qu’une info-bulle vous indiquant qu’elle est verrouillée s’affiche, vous pouvez demander à votre administrateur ou administratrice Workfront de la déverrouiller pour tous les groupes de l’entreprise.

   Lorsqu’elle est déverrouillée, vous et d’autres administrateurs et administratrices de groupes pouvez la configurer séparément pour vos propres groupes. Vous pouvez également la verrouiller pour votre groupe et tous les sous-groupes situés sous votre groupe.

   * [Paramètres par défaut de la nouvelle tâche](#new-task-defaults)
   * [Événements](#issues)
   * [Suppression](#deletion)

   <!--* <span class="preview">[Move](#move)</span>-->

   * [Dates effectives](#actual-dates)
   * [Accès](#access)

### Paramètres par défaut de la nouvelle tâche {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Date de début pour les nouvelles tâches</td> 
      <td> <p>Détermine la date de début par défaut des nouvelles tâches pour les personnes gestionnaires de projet. La date de début des nouvelles tâches peut être la date de début prévue du projet ou le jour de création de la tâche.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Type de durée </p> </td> 
      <td> <p>Détermine la relation entre le nombre de ressources (et leur pourcentage d’affectation) et la durée ou l’effort total de la tâche. Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Durée des tâches et types de durée : index des articles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de revenus</td> 
      <td> <p>Calcule les estimations de revenus prévus et réels d’une tâche. Lorsque le <strong>Type de revenu</strong> est défini sur <strong>Non facturable</strong>, les heures prévues et les heures effectives enregistrées ne génèrent pas d’estimation de revenu pour la tâche et le travail sur la tâche ne contribue pas au revenu au niveau du projet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de coût</td> 
      <td> <p>Calcule les estimations de coût prévu et réel d’une tâche. Lorsqu’il est défini sur <strong>Aucun coût</strong>, les heures prévues et les heures effectives enregistrées ne génèrent pas d’estimation de coût prévu ou réel pour la tâche et le travail sur la tâche ne contribue pas aux coûts au niveau du projet.</p> </td> 
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
      <td> <p>Lorsqu’une personne convertit un problème en projet ou tâche, le problème d’origine et le projet converti ou la tâche convertie deviennent des objets de résolution. Cette configuration vous permet de mettre en corrélation la résolution du problème d’origine avec la résolution de son objet résolvable. Pour plus d’informations sur les objets de résolution, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets de résolution et des objets résolvables</a>.</p> <p>Pour que cette configuration soit effective, l’option <strong>Conserver le problème d’origine et lier sa résolution à la tâche</strong> doit être sélectionnée.</p> 
       <ul> 
        <li>Lorsque ce paramètre est activé, vous pouvez créer des statuts personnalisés avec la même clé pour les problèmes et les projets ou les tâches. Lorsque le projet ou la tâche (en tant qu’objet résolvable) prend le statut personnalisé, la modification se répercute également sur le statut du problème. La clé de statut doit être la même pour les statuts du problème et du projet ou de la tâche.</li> 
        <li>Lorsque ce paramètre est désactivé, les statuts d’objet de résolution sont automatiquement définis sur le statut par défaut, au lieu des statuts personnalisés. Pour plus d’informations sur les statuts par défaut, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accéder à la liste des statuts de problème du système</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lors de la conversion d’un problème en tâche</td> 
      <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion d’un problème en tâche :</p> 
       <ul> 
        <li><strong>Conserver le problème d’origine et lier sa résolution à la tâche</strong> : lorsque vous convertissez le problème, il reste visible en tant que problème jusqu’à ce que la tâche soit terminée. Le statut du problème passe automatiquement à Fermé lorsque la tâche est terminée.</li> 
        <li><strong>Autoriser l’interlocuteur principal ou l’interlocutrice principale à accéder à la tâche</strong> : accorde à l’interlocuteur principal ou l’interlocutrice principale (le créateur ou la créatrice du problème) l’accès à la tâche pour l’examiner, apporter des modifications et rester informé de sa progression.</li> 
        <li> <p><strong>Autoriser la modification de ces paramètres lors de la conversion</strong> : permet à l’utilisateur ou l’utilisatrice qui convertit le problème de modifier ces options lors de la conversion d’un problème en tâche.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsqu’un problème est converti en projet</td> 
      <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion d’un problème en projet :</p> 
       <ul> 
        <li><strong>Conserver le problème d’origine et lier sa résolution au projet</strong> : lorsque vous convertissez le problème, il reste visible en tant que problème jusqu’à ce que le projet soit terminé. Le statut du problème passe automatiquement à Fermé lorsque le projet est terminé.</li> 
        <li><strong>Autoriser l’interlocuteur principal ou l’interlocutrice principale à accéder au projet</strong> : accorde à l’interlocuteur principal ou l’interlocutrice principale (le créateur ou la créatrice du problème) l’accès au projet pour examiner le projet, apporter des modifications et rester informé de sa progression.</li> 
        <li><strong>Autoriser la modification de ces paramètres lors de la conversion</strong> : permet à l’utilisateur ou l’utilisatrice qui convertit le problème de modifier les options répertoriées lors de la conversion d’un problème en projet.</li> 
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
        <p><b>Conseil</b> : ce paramètre s’applique également à la suppression de projets comportant des tâches ou des problèmes avec des heures enregistrées. Ce paramètre ne s’applique pas à la suppression de projets dont les heures sont enregistrées directement pour le projet. </p> 
        <p>Tenez compte des points suivants :</p> 
        <ul> 
         <li> <p>Lorsqu’elle est sélectionnée, vous recevez un avertissement informatif quand vous supprimez une tâche ou un problème. L’avertissement vous rappelle que si la tâche ou le problème comporte des heures enregistrées, elles seront déplacées vers le projet ou supprimées. Vous pouvez définir si les heures sont supprimées ou déplacées vers le projet dans la zone Préférences de feuilles de temps et d’heures de la configuration. Une fois que vous confirmez avoir pris connaissance de l’avertissement, la tâche ou le problème est supprimé. Pour plus d’informations sur la configuration des préférences de feuilles de temps et d’heures, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurer les préférences de feuilles de temps et d’heures</a>. </p> <p>Conseil : <span>lorsque vous supprimez un projet comportant des tâches et des problèmes ayant des heures enregistrées, les heures enregistrées sont supprimées ou conservées en fonction des paramètres de la zone Préférences de feuilles de temps et d’heures de la configuration</span>. </p> </li> 
         <li><span>Lorsque vous désactivez cette option, vous recevez un avertissement d’interdiction lorsque vous supprimez une tâche ou un problème avec des heures enregistrées, ou lorsque vous supprimez un projet avec des heures enregistrées pour ses tâches ou problèmes</span><span>.</span> L’avertissement indique que l’administrateur ou l’administratrice n’autorise pas la suppression de tâches ou de problèmes avec des heures enregistrées. Les tâches, problèmes<span> ou projets avec des heures enregistrées pour des tâches et des problèmes</span> ne peuvent pas être supprimés. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


<!-- *****also replace the & with "and" in the Deletion section

<div class="preview">

### Move

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Allow users to move tasks and issues with logged hours</td> 
      <td> <p> Lets you determine whether you allow the move of tasks or issues where hours are logged. This option is selected by default.</p> 
       <p>Consider the following:</p> 
        <ul> 
         <li> When it is selected, you can move tasks and issues that have time logged. The hours also move with the tasks or issues. </li>
      <li>When you deselect this option, you receive a prohibitive warning when you move a task or issue with logged hours. The warning specifies that the administrator does not allow for tasks or issues with logged hours to be moved. The tasks or issues that have hours logged cannot be moved. </li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

</div>

-->

### Dates effectives {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lorsqu’une tâche ou un problème passe de « Nouveau » à « En cours », définissez la date de début effectif sur</td> 
      <td> <p>Sélectionnez l’une des options suivantes pour savoir quand la date de début effectif est enregistrée dans Workfront lorsqu’une tâche ou un problème passe de <strong>Nouveau</strong> à <strong>En cours</strong> :</p> 
       <ul> 
        <li><strong>Maintenant :</strong> la date de début effectif est définie sur la date actuelle.</li> 
        <li><strong>Date de début prévue :</strong> la date de début effectif est définie sur la date de début prévue de la tâche ou du problème.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une fois qu’une tâche ou un problème est terminé, définissez la date d’achèvement effectif sur</td> 
      <td> <p>Sélectionnez l’une des options suivantes lorsque la date d’achèvement effectif est enregistrée dans Workfront lorsqu’une tâche ou un problème est terminé :</p> 
       <ul> 
        <li><strong>Maintenant :</strong> la date d’achèvement effectif est définie sur la date actuelle.</li> 
        <li> <p><strong>Date d’achèvement prévue :</strong> la date d’achèvement effectif est définie sur la date d’achèvement prévue de la tâche ou du problème.</p> </li> 
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
        <li><strong>Lui donner ... l’accès à une tâche</strong> : définit l’autorisation par défaut dont dispose une personne sur la tâche à laquelle elle est affectée. Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</li> 
        <li> <p><strong>Lui accorder également ... l’accès au projet</strong> : définit l’autorisation par défaut dont dispose une personne sur le projet auquel une tâche lui est affectée. Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences de projet à l’échelle du système</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsqu’une personne est affectée à un problème</td> 
      <td> 
       <ul> 
        <li><strong>Lui donner ... l’accès à une tâche</strong> : définit l’autorisation par défaut dont dispose une personne sur la tâche à laquelle elle est affectée. Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</li> 
        <li> <p><strong>Lui accorder également ... l’accès au projet</strong> : définit l’autorisation par défaut dont dispose une personne sur le projet auquel une tâche lui est affectée. Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences de projet à l’échelle du système</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsqu’une personne soumet une demande</td> 
      <td> 
       <ul> 
        <li><strong>Lui donner ... l’accès au problème</strong> : définit l’autorisation par défaut dont dispose un utilisateur ou une utilisatrice sur une demande qu’il ou elle a soumise. Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème</a>.</li> 
        <li> <p><strong>Les personnes appartenant à la même entreprise hériteront d’autorisations identiques pour toutes les demandes</strong> : permet aux utilisateurs et aux utilisatrices d’afficher les demandes soumises par d’autres utilisateurs et utilisatrices de la même société qu’eux. Ils disposent des mêmes autorisations sur ces demandes que sur les demandes qu’ils ont soumises.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
