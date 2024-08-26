---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configuration des préférences de tâche et de problème à l’échelle du système
description: Vous pouvez configurer des préférences à l’échelle du système pour les tâches et les problèmes. Ces préférences ont un impact sur la façon dont vos utilisateurs et utilisatrices créent des tâches et des problèmes dans Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '2074'
ht-degree: 99%

---

# Configurer les préférences de tâche et de problème à l’échelle du système

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez configurer les préférences à l’échelle du système pour les tâches et les problèmes. Ces préférences ont un impact sur la façon dont vos utilisateurs et utilisatrices créent des tâches et des problèmes dans [!DNL Workfront].

Par défaut, les préférences de tâche et de problème sont verrouillées et les administrateurs et administratrices de groupes ne peuvent pas les modifier au niveau du groupe, sauf si vous les déverrouillez pour tous les groupes du système. Pour plus d’informations, voir la section [Verrouiller les préférences de tâche et de problème pour les groupes](#lock-task-and-issue-preferences-for-groups) de cet article.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   ou
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer les préférences de tâche et de problème pour toutes les personnes dans [!DNL Workfront]

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Tâches et problèmes].**

1. Sur la page qui s’affiche, continuez avec l’une des 5 sections énumérées ci-dessous pour configurer les paramètres pour [!UICONTROL Paramètres par défaut de la nouvelle tâche], [!UICONTROL Problèmes], [!UICONTROL Suppression], [!UICONTROL Dates effectives] et [!UICONTROL Accès] :

   * [[!UICONTROL Paramètres par défaut de la nouvelle tâche]](#new-task-defaults)
   * [[!UICONTROL Événements]](#issues)
   * [[!UICONTROL Suppression]](#deletion)
   * [[!UICONTROL Dates effectives]](#actual-dates)
   * [[!UICONTROL Délégation]](#delegation)

   <!--
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Travailler sur ce projet</a> </li>
  --&gt;

* [[!UICONTROL Accès]](#access)

### [!UICONTROL Paramètres par défaut de la nouvelle tâche] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Start Date]</td> 
    <td> <p>Détermine la date de début par défaut des nouvelles tâches pour les personnes gestionnaires de projet. La date de début des nouvelles tâches peut être la date de début prévisionnelle du projet ou le jour de création de la tâche.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Duration Type] </p> </td> 
    <td> <p>Détermine la relation entre le nombre de ressources (et leur pourcentage d’affectation) et la durée ou l’effort total de la tâche. Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Durée de tâche et types de durée</a>.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Revenue Type]</td> 
    <td> <p>Calcule les estimations de revenus prévisionnels et réels d’une tâche. Lorsque l’option <strong>[!UICONTROL Revenue Type]</strong> est définie sur <strong>[!UICONTROL Not Billable]</strong>, les heures prévisionnelles et les heures effectives enregistrées ne génèrent pas d’estimation de revenus pour la tâche, et le travail sur la tâche ne contribue pas aux revenus du projet.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cost Type]</td> 
    <td> <p>Calcule les estimations de coût prévisionnel et réel d’une tâche. Lorsqu’elle est définie sur <strong>[!UICONTROL No Cost]</strong>, les heures prévisionnelles et les heures effectives enregistrées ne génèrent pas d’estimation de coût prévisionnel ou réel pour la tâche, et le travail sur la tâche ne contribue pas aux coûts du projet.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Problèmes {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object changes]</td> 
    <td> <p>Lorsqu’une personne convertit un problème en projet ou tâche, le problème d’origine et le projet converti ou la tâche convertie deviennent des objets de résolution. Cette configuration vous permet de mettre en corrélation la résolution du problème d’origine avec la résolution de son objet résolvable. Pour plus d’informations sur les objets de résolution, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets de résolution et des objets résolvables</a>.</p> <p>Pour que cette configuration soit effective, l’option <strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong> doit être sélectionnée.</p> 
      <ul> 
      <li>Lorsque ce paramètre est activé, vous pouvez créer des statuts personnalisés avec la même clé pour les problèmes et les projets ou les tâches. Lorsque le projet ou la tâche (en tant qu’objet résolvable) prend le statut personnalisé, la modification se répercute également sur le statut du problème. La clé de statut doit être la même pour les statuts du problème et du projet ou de la tâche.</li> 
      <li>Lorsque ce paramètre est désactivé, les statuts d’objet de résolution sont automatiquement définis sur le statut par défaut, au lieu des statuts personnalisés. Pour plus d’informations sur les statuts par défaut, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accéder à la liste des statuts de problème du système</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader" [!UICONTROL>Lors de la conversion d’un problème en tâche]</td> 
    <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion d’un problème en tâche :</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the task] : lors de la conversion d’un problème, il reste visible en tant que problème jusqu’à ce que la tâche soit terminée. </strong> Le statut du problème passe automatiquement à [!UICONTROL Closed] lorsque la tâche est terminée. Lorsque cette option est désélectionnée, le problème est supprimé.</p> <p><b>NOTE</b> :  <p>Les utilisateurs et les utilisatrices qui n’ont pas l’accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème pendant la conversion, quel que soit le statut de ce paramètre. Pour plus d’informations sur l’accès et les autorisations relatives aux problèmes, consultez ce qui suit :</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the task]</strong> : permet au contact principal (personne à l’origine de la création du problème) d’accéder à l’affichage de la tâche pour la passer en revue, de rester au fait de sa progression et de faire des commentaires dans la section des mises à jour de la tâche.</li> 
      <li> <p><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong> : permet à l’utilisateur ou à l’utilisatrice qui convertit le problème de modifier ces options pendant la conversion du problème en tâche.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When converting an issue to a project]</td> 
    <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion d’un problème en projet :</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the project] : lors de la conversion d’un problème, il reste visible en tant que problème jusqu’à ce que le projet soit terminé. </strong> Le statut du problème passe automatiquement à [!UICONTROL Closed] lorsque le projet est terminé. Lorsque cette option est désélectionnée, le problème est supprimé. </p> <p><b>NOTE</b> :  <p>Les utilisateurs et les utilisatrices qui n’ont pas l’accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème pendant la conversion, quel que soit le statut de ce paramètre. Pour plus d’informations sur l’accès et les autorisations relatives aux problèmes, consultez ce qui suit :</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the project]</strong> : permet au contact principal (personne à l’origine de la création du problème) d’accéder à l’affichage du projet pour le passer en revue, de rester au fait de sa progression et de faire des commentaires dans la section des mises à jour du projet.</li> 
      <li><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong> : permet à l’utilisateur ou à l’utilisatrice qui convertit le problème de modifier les options répertoriées pendant la conversion du problème en projet.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Suppression] {#deletion}

**[!UICONTROL Autoriser les utilisateurs et utilisatrices à supprimer les tâches et les problèmes comportant des heures consignées : vous permet de déterminer si vous autorisez la suppression des tâches ou des problèmes pour lesquels des heures ont été consignées.]** Cette option est sélectionnée par défaut.

>[!TIP]
>
>Ce paramètre s’applique également à la suppression de projets pour lesquels des tâches ou des problèmes comportent des heures consignées. Ce paramètre ne s’applique pas à la suppression de projets dont les heures sont consignées directement pour le projet.

* Lorsqu’elle est sélectionnée, un avertissement informatif s’affiche lorsque vous supprimez une tâche ou un problème. L’avertissement vous rappelle que si la tâche ou le problème comporte des heures consignées, elles seront déplacées vers le projet ou supprimées. Vous pouvez déterminer si les heures sont supprimées ou déplacées vers le projet dans la zone Préférences des feuilles de temps et des heures de la Configuration.  Une fois que vous confirmez avoir pris connaissance de l’avertissement, la tâche ou le problème est supprimé. Pour plus d’informations sur la configuration des préférences des feuilles de temps et des heures, voir [Configurer les préférences des feuilles de temps et des heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >Lorsque vous supprimez un projet comportant des tâches et des problèmes pour lesquels des heures ont été consignées, ces heures sont soit supprimées, soit conservées en fonction des paramètres définis dans la zone Préférences des feuilles de temps et des heures de la Configuration.  Un message d’avertissement ne s’affiche pas lors de la suppression d’un projet.

* Lorsque vous désélectionnez cette option, un avertissement d’interdiction s’affiche lorsque vous supprimez une tâche ou un problème comportant des heures consignées, ou lorsque vous supprimez un projet comportant des heures consignées pour ses tâches ou ses problèmes. L’avertissement spécifie que l’administrateur ou l’administratrice n’autorise pas la suppression de tâches ou de problèmes pour lesquels des heures ont été consignées. Les tâches, les problèmes ou les projets pour lesquels des heures ont été consignées ne peuvent pas être supprimés.

### [!UICONTROL Dates effectives] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue goes from "New" to "In Progress," set the Actual Start Date to]</td> 
    <td> <p>Sélectionnez l’une des options suivantes pour enregistrer la date de début effective dans [!DNL Workfront] lorsqu’une tâche ou un problème passe de <strong>[!UICONTROL New]</strong> à <strong>[!UICONTROL In Progress]</strong> :</p> 
      <ul> 
      <li><strong>[!UICONTROL Now] :</strong> la date de début effective est définie sur la date actuelle.</li> 
      <li><strong>[!UICONTROL The Planned Start Date] :</strong> la date de début effective est définie sur la date de début prévisionnelle de la tâche ou du problème.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue is completed, set the Actual Completion Date to]</td> 
    <td> <p>Sélectionnez l’une des options suivantes pour enregistrer la date d’achèvement effective dans [!DNL Workfront] lorsqu’une tâche ou un problème se termine :</p> 
      <ul> 
      <li><strong>[!UICONTROL Now] :</strong> la date d’achèvement effective est définie sur la date actuelle.</li> 
      <li> <p><strong>[!UICONTROL The Planned Completion Date] :</strong> la date d’achèvement effective est définie sur la date d’achèvement prévisionnelle de la tâche ou du problème.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Délégation

Activer le paramètre **[!UICONTROL Autoriser les utilisateurs et utilisatrices à déléguer leurs tâches et problèmes]** permet à toutes les personnes de déléguer temporairement leur travail à d’autres.

Lorsque ce paramètre est activé, les utilisateurs et les utilisatrices peuvent voir les éléments suivants :

* Le lien Déléguer dans leur zone Accueil.  Les utilisateurs et les utilisatrices peuvent y déléguer des affectations d’approbations, de tâches et de problèmes.
* Indication qu’une tâche ou un problème fait l’objet d’une délégation à un autre utilisateur ou une autre utilisatrice dans la zone [!UICONTROL Affectations et délégations] dans l’en-tête de la tâche ou du problème.

  Si vous désactivez le paramètre [!UICONTROL Autoriser les utilisateurs et utilisatrices à déléguer leurs tâches et problèmes], les délégations actuellement planifiées s’arrêteront et les personnes déléguées recevront une notification par e-mail indiquant que la délégation a été arrêtée.

Pour plus d’informations sur la délégation de travail à d’autres personnes, voir les articles suivants :

* [Vue d’ensemble de la délégation de travail](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Gérer la délégation des tâches et des problèmes](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Accès] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to a task]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task] : définit l’autorisation par défaut dont dispose une personne sur la tâche qui lui est affectée. </strong> Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project] : définit l’autorisation par défaut dont dispose une personne sur le projet pour lequel une tâche lui est affectée. </strong> Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences de projet à l’échelle du système</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to an issue]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task] : définit l’autorisation par défaut dont dispose une personne sur la tâche qui lui est affectée. </strong> Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project] : définit l’autorisation par défaut dont dispose une personne sur le projet pour lequel une tâche lui est affectée. </strong> Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences de projet à l’échelle du système</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone submits a request]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to the issue] : définit l’autorisation par défaut d’une personne sur une demande qu’elle soumet. </strong> Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème</a>.</li> 
      <li> <p><strong>[!UICONTROL People from the same company will inherit the same permissions for all requests]</strong> : permet aux utilisateurs et aux utilisatrices de voir les demandes soumises par d’autres utilisateurs et utilisatrices de la même entreprise. Ils disposent des mêmes autorisations sur ces demandes que sur les demandes qu’ils ont soumises.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Verrouiller les préférences de tâche et de problème pour les groupes {#lock-task-and-issue-preferences-for-groups}

Si les groupes de votre organisation ont besoin de préférences de tâche ou de problème configurées différemment pour leurs propres workflows, vous pouvez déverrouiller les préférences pour tous les groupes de l’organisation afin de pouvoir appliquer une configuration spécifique. Lorsque les préférences sont déverrouillées et que l’administrateur ou l’administratrice de groupes les modifie, les tâches ou les problèmes associés au groupe sont affectés par les paramètres au niveau du groupe et non au niveau du système.

Pour plus d’informations sur la manière dont un administrateur ou une administratrice de groupes configure les préférences de tâche et de problème pour un groupe, voir [Configurer les préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Une fois qu’un administrateur ou qu’une administratrice  a déverrouillé une préférence au niveau du système, tout membre de l’administration du groupe peut la configurer, puis la verrouiller pour s’assurer que tous les membres de son groupe et des sous-groupes inférieurs utilisent la même configuration. [!DNL Workfront] Cette fonction est similaire à la capacité qu’a un administrateur ou une administratrice  de configurer et de verrouiller une préférence pour toutes les personnes utilisant le système. [!DNL Workfront] Pour plus d’informations, voir [Configurer les préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Verrouiller ou déverrouiller une préférence de projet, de tâche ou de problème pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Pour verrouiller ou déverrouiller une préférence de tâche ou de problème afin que les groupes puissent la configurer :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Tâches et problèmes]**.

1. Effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs et les administratrices de groupes inférieurs au vôtre puissent configurer une préférence pour leurs groupes, déverrouillez-la ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que votre groupe et tous les groupes inférieurs utilisent votre configuration d’une préférence, assurez-vous qu’elle est verrouillée (par défaut).

     >[!IMPORTANT]
     >
     >Nous vous recommandons de communiquer avec l’ensemble des personnes qui administrent et utilisent le système afin de vous assurer que tous les besoins sont pris en compte lors de la configuration d’une préférence verrouillée. Lorsque vous la verrouillez, votre configuration est héritée par tous les groupes du système. De plus, si la préférence a été déverrouillée pour une période de temps donnée, votre configuration remplace celles que les administrateurs et administratrices de groupes ont pu effectuer.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
