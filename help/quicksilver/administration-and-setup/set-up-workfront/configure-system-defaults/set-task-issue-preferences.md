---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configuration des préférences de tâche et de problème à l’échelle du système
description: Vous pouvez configurer des préférences à l’échelle du système pour les tâches et les problèmes. Ces préférences ont un impact sur la manière dont vos utilisateurs créent des tâches et des problèmes dans Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '2074'
ht-degree: 4%

---

# Configuration des préférences de tâche et de problème à l’échelle du système

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

En tant qu’administrateur [!DNL Adobe Workfront], vous pouvez configurer des préférences à l’échelle du système pour les tâches et les problèmes. Ces préférences ont un impact sur la manière dont vos utilisateurs créent des tâches et des problèmes dans [!DNL Workfront].

Par défaut, les préférences de tâche et de problème sont verrouillées et les administrateurs de groupe ne peuvent pas les modifier au niveau du groupe, sauf si vous les déverrouillez pour tous les groupes du système. Pour plus d’informations, reportez-vous à la section [Verrouiller la tâche et émettre des préférences pour les groupes](#lock-task-and-issue-preferences-for-groups) de cet article.


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

## Configuration des préférences de tâche et de problèmes pour tous les membres de [!DNL Workfront]

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]** >**[!UICONTROL Tâches et problèmes].**

1. Sur la page qui s’affiche, passez à l’une des 5 sections répertoriées ci-dessous pour configurer les paramètres pour les [!UICONTROL Nouvelles tâches par défaut], [!UICONTROL Problèmes], [!UICONTROL Suppression], [!UICONTROL Dates réelles] et [!UICONTROL Accès] :

   * [[!UICONTROL Nouvelles valeurs par défaut de tâche]](#new-task-defaults)
   * [[!UICONTROL Événements]](#issues)
   * [[!UICONTROL Suppression]](#deletion)
   * [[!UICONTROL Dates réelles]](#actual-dates)
   * [[!UICONTROL Délégation]](#delegation)

   <!--
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Travailler dessus</a> </li>
  --&gt;

* [[!UICONTROL Accès]](#access)

### [!UICONTROL Nouvelles valeurs par défaut de tâche] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Date de début]</td> 
    <td> <p>Détermine la date de début par défaut des nouvelles tâches pour les gestionnaires de projet. La date de début des nouvelles tâches peut être la date de début prévue du projet ou le jour de création de la tâche.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Duration Type] </p> </td> 
    <td> <p>Détermine la relation entre le nombre de ressources (et leur pourcentage d’allocation) et la durée ou l’effort total de la tâche. Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Durée de tâche et types de durée</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Revenue Type]</td> 
    <td> <p>Calcule les estimations de recettes prévues et réelles pour une tâche. Lorsque le <strong>[!UICONTROL Revenue Type]</strong> est défini sur <strong>[!UICONTROL Not Billable]</strong>, les heures planifiées et les heures réelles enregistrées ne génèrent pas d’estimation de recettes pour la tâche, et le travail sur la tâche ne contribue pas aux recettes au niveau du projet.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cost Type]</td> 
    <td> <p>Calcule les estimations de coûts prévues et réelles pour une tâche. Lorsqu’elle est définie sur <strong>[!UICONTROL Aucun coût]</strong>, les heures planifiées et les heures réelles enregistrées ne génèrent pas d’estimation de coût planifiée ou réelle de la tâche, et le travail sur la tâche ne contribue pas aux coûts au niveau du projet.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Problèmes {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Mettre automatiquement à jour l’état Problème résolvable lorsque l’état de l’objet de résolution change]</td> 
    <td> <p>Lorsqu’une personne convertit un problème en projet ou tâche, le problème d’origine et le projet ou la tâche converti deviennent des objets de résolution. Ce paramètre vous permet de mettre en corrélation la résolution du problème d’origine avec la résolution de son objet résolvable. Pour plus d’informations sur la résolution d’objets, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution d’objets résolvables </a>.</p> <p>Pour que ce paramètre ait un effet, l’option <strong>[!UICONTROL Conserver le problème d’origine et lier sa résolution à la tâche]</strong> doit être sélectionnée.</p> 
      <ul> 
      <li>Lorsque ce paramètre est activé, vous pouvez créer des états personnalisés avec la même clé pour les problèmes, les projets ou les tâches. Lorsque le projet ou la tâche (en tant qu’objet résolvable) devient un état personnalisé, la modification se répercute également sur l’état du problème. La clé d’état doit être la même pour le problème et les états du projet ou de la tâche.</li> 
      <li>Lorsque ce paramètre est désactivé, les statuts des objets de résolution sont automatiquement définis sur l’état par défaut, au lieu des statuts personnalisés. Pour plus d’informations sur les états par défaut, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accès à la liste des états des problèmes système</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader" [!UICONTROL>Lors de la conversion d’un problème en tâche]</td> 
    <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion, d’un problème à l’autre :</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Conserver le problème d’origine et lier sa résolution à la tâche]</strong> : lorsque vous convertissez le problème, il reste visible en tant que problème jusqu’à ce que la tâche soit terminée. Le statut du problème passe automatiquement à [!UICONTROL Fermé] une fois la tâche terminée. Si cette option est désélectionnée, le problème est supprimé.</p> <p><b>NOTE</b> :  <p>Les utilisateurs n’ayant pas accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème lorsqu’ils le convertissent, quel que soit l’état de ce paramètre. Pour plus d’informations sur l’accès et les autorisations pour les problèmes, voir :</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Autoriser les contacts de Principal à avoir accès à la tâche]</strong> : donne au contact principal (créateur du problème) l’accès à la tâche pour examiner la tâche, rester informé de son avancement et faire des commentaires sur la section Mises à jour de la tâche.</li> 
      <li> <p><strong>[!UICONTROL Autoriser la modification de ces paramètres lors de la conversion]</strong> : permet à l’utilisateur qui convertit le problème de modifier ces options lors de la conversion d’un problème en tâche.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Lors de la conversion d’un problème en projet]</td> 
    <td> <p>Les paramètres de cette section déterminent ce qui se passe pendant le processus de conversion d’un problème à l’autre :</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Conservez le problème d’origine et liez sa résolution au projet]</strong> : lorsque vous convertissez le problème, il reste visible en tant que problème jusqu’à la fin du projet. Le statut du problème passe automatiquement à [!UICONTROL Fermé] une fois le projet terminé. Si cette option est désélectionnée, le problème est supprimé. </p> <p><b>NOTE</b> :  <p>Les utilisateurs n’ayant pas accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème lorsqu’ils le convertissent, quel que soit l’état de ce paramètre. Pour plus d’informations sur l’accès et les autorisations pour les problèmes, voir :</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Autoriser les contacts de Principal à avoir accès au projet]</strong> : donne au contact principal (créateur du problème) l’accès au projet pour examiner le projet, rester informé de son avancement et faire des commentaires sur la section Mises à jour du projet.</li> 
      <li><strong>[!UICONTROL Autoriser la modification de ces paramètres lors de la conversion]</strong> : permet à l’utilisateur qui convertit le problème de modifier les options répertoriées lors de la conversion d’un problème en projet.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Suppression] {#deletion}

**[!UICONTROL Autoriser les utilisateurs à supprimer les tâches et problèmes avec les heures enregistrées]** : permet de déterminer si vous autorisez la suppression des tâches ou des problèmes où les heures sont consignées. Cette option est sélectionnée par défaut.

>[!TIP]
>
>Ce paramètre s’applique également à la suppression des projets comportant des tâches ou des problèmes avec les heures de connexion. Ce paramètre ne s’applique pas à la suppression de projets pour lesquels le temps est consigné directement pour le projet.

* Lorsqu’elle est sélectionnée, vous recevez un avertissement informatif lorsque vous supprimez une tâche ou un problème. L’avertissement vous rappelle que si la tâche ou le problème a des heures enregistrées, elles seront déplacées vers le projet ou supprimées. Vous pouvez définir si les heures sont supprimées ou déplacées vers le projet dans la zone [!UICONTROL Préférences de la feuille de temps et des heures] de la [!UICONTROL Configuration]. Une fois que vous avez confirmé l’affichage de l’avertissement, la tâche ou le problème est supprimé. Pour plus d’informations sur la configuration des préférences de la feuille de temps et des heures, voir [ Configuration des préférences de la feuille de temps et de l’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >Lorsque vous supprimez un projet avec des tâches et des problèmes ayant des heures enregistrées, les heures consignées sont soit supprimées, soit conservées selon les paramètres de la zone [!UICONTROL Préférences de la feuille de temps et des heures] de la [!UICONTROL configuration]. Le message d’avertissement ne s’affiche pas lors de la suppression d’un projet.

* Lorsque vous désactivez cette option, vous recevez un avertissement prohibitif lorsque vous supprimez une tâche ou un problème lié aux heures journalisées, ou lorsque vous supprimez un projet avec des heures journalisées pour ses tâches ou problèmes. L’avertissement indique que l’administrateur n’autorise pas la suppression de tâches ou de problèmes avec les heures enregistrées. Les tâches, problèmes ou projets dont les heures sont enregistrées pour les tâches et problèmes ne peuvent pas être supprimés.

### [!UICONTROL Dates réelles] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Lorsqu’une tâche ou un problème passe de "Nouveau" à "En cours", définissez la Date de début réelle sur]</td> 
    <td> <p>Sélectionnez l’une des options suivantes lorsque la date de début réelle est enregistrée dans [!DNL Workfront] lorsqu’une tâche ou un problème passe de <strong>[!UICONTROL Nouveau]</strong> à <strong>[!UICONTROL En cours]</strong> :</p> 
      <ul> 
      <li><strong>[!UICONTROL Maintenant] :</strong> La date de début réelle est définie sur la date actuelle.</li> 
      <li><strong>[!UICONTROL Date de début planifiée] :</strong> La date de début réelle est définie sur la date de début planifiée de la tâche ou du problème.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Lorsqu’une tâche ou un problème est terminé, définissez la Date de fin réelle sur]</td> 
    <td> <p>Sélectionnez l’une des options suivantes lorsque la date de fin réelle est enregistrée dans [!DNL Workfront] lorsqu’une tâche ou un problème est terminé :</p> 
      <ul> 
      <li><strong>[!UICONTROL Maintenant] :</strong> La date d’achèvement réelle est définie sur la date actuelle.</li> 
      <li> <p><strong>[!UICONTROL Date d’achèvement planifiée] :</strong> La date d’achèvement réelle est définie sur la date d’achèvement planifiée de la tâche ou du problème.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Délégation

L’activation du paramètre **[!UICONTROL Autoriser les utilisateurs à déléguer leurs tâches et problèmes]** permet à tous les utilisateurs d’ de déléguer temporairement leur travail à d’autres utilisateurs.

Lorsque ce paramètre est activé, les utilisateurs peuvent voir les éléments suivants :

* Le lien [!UICONTROL Déléguer] dans leur zone [!UICONTROL Accueil]. Ils peuvent déléguer des validations ou des affectations de tâche et d’émission à partir de là.
* Une indication qu’une tâche ou un problème est délégué à un autre utilisateur dans la zone [!UICONTROL Affectations et délégations] de l’en-tête de tâche ou de problème.

  Si vous désactivez le paramètre [!UICONTROL Autoriser les utilisateurs à déléguer leurs tâches et problèmes], les délégations actuellement planifiées s’arrêteront et les utilisateurs délégués recevront une notification par courrier électronique indiquant que la délégation a été arrêtée.

Pour plus d’informations sur la délégation de travail à d’autres personnes, consultez les articles suivants :

* [Présentation de la délégation de travail](../../../manage-work/delegate-work/delegate-work-overview.md)
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
    <td role="rowheader">[!UICONTROL Lorsqu’une personne est affectée à une tâche]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Donnez-leur ... accès à une tâche]</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour la tâche à laquelle il est affecté. Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Octroi de l’accès aux utilisateurs</a>.</li> 
      <li> <p><strong>[!UICONTROL Accorder également ... l’accès au projet]</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour le projet auquel une tâche lui est affectée. Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Lorsqu’une personne est affectée à un problème]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Donnez-leur ... accès à une tâche]</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour la tâche à laquelle il est affecté. Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Octroi de l’accès aux utilisateurs</a>.</li> 
      <li> <p><strong>[!UICONTROL Accorder également ... l’accès au projet]</strong> : définit l’autorisation par défaut dont dispose un utilisateur pour le projet auquel une tâche lui est affectée. Pour plus d’informations sur les autorisations de projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Lorsqu’une personne envoie une demande]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Donnez-leur ... accès au problème]</strong> : définit l’autorisation par défaut d’un utilisateur sur une demande qu’il a envoyée. Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème</a>.</li> 
      <li> <p><strong>[!UICONTROL Les personnes d’une même société hériteront des mêmes autorisations pour toutes les demandes]</strong> : permet aux utilisateurs d’afficher les demandes envoyées par d’autres utilisateurs de la même société qu’eux. Ils disposent des mêmes autorisations sur ces demandes que sur leurs propres demandes envoyées.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Verrouillage des préférences de tâche et d’émission pour les groupes {#lock-task-and-issue-preferences-for-groups}

Si les groupes de votre organisation ont besoin d’une tâche ou d’une préférence d’émission configurée différemment pour leurs workflows uniques, vous pouvez déverrouiller la préférence pour tous les groupes de l’organisation afin qu’ils puissent la configurer eux-mêmes. Lorsqu’une préférence est déverrouillée et que l’administrateur du groupe la modifie, les tâches ou les problèmes associés au groupe sont affectés par le paramètre de niveau groupe de la préférence plutôt que par le paramètre de niveau système.

Pour plus d’informations sur la façon dont un administrateur de groupe configure les préférences de tâche et de problème pour un groupe, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Une fois qu’un administrateur [!DNL Workfront] a déverrouillé une préférence au niveau du système, tout administrateur de groupe peut la configurer, puis la verrouiller pour s’assurer que tous les membres de leur groupe et les sous-groupes ci-dessous utilisent la même configuration. Cela est parallèle à la possibilité qu’un administrateur [!DNL Workfront] doit configurer et verrouiller une préférence pour tous les utilisateurs du système. Pour plus d’informations, voir [Configuration des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Verrouillage ou déverrouillage d’un projet, d’une tâche ou d’une préférence de problème pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Pour verrouiller ou déverrouiller une tâche ou une préférence d’émission afin que les groupes puissent la configurer :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Tâches et problèmes]**.

1. Effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs de groupes situés sous votre groupe puissent configurer une préférence pour leurs groupes, déverrouillez-la ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que votre groupe et tous les groupes sous-jacents utilisent votre configuration pour une préférence, assurez-vous qu’il est verrouillé (il s’agit de la valeur par défaut).

     >[!IMPORTANT]
     >
     >Nous vous recommandons de communiquer avec les administrateurs et les utilisateurs de groupes dans tout le système pour vous assurer que tous les besoins sont pris en compte dans la configuration d’une préférence verrouillée. Lorsque vous le verrouillez, votre configuration pour elle est héritée par tous les groupes du système. Et si la préférence a été déverrouillée pendant une période quelconque, votre configuration remplace celles que les administrateurs de groupe peuvent avoir faites.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
