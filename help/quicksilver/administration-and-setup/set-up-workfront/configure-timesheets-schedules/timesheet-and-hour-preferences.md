---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurer les préférences des feuilles de temps et des heures
description: En tant qu’administrateur ou administratrice  [!DNL Adobe Workfront] , vous pouvez spécifier des préférences pour les feuilles de temps et les heures dans  [!DNL Workfront]  afin de définir les éléments que les feuilles de temps peuvent préremplir et les éléments pour lesquels les personnes peuvent consigner des heures.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1411'
ht-degree: 95%

---

# Configurer les préférences des feuilles de temps et des heures

<!--Audited: 06/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez spécifier des préférences pour les feuilles de temps et les heures dans [!DNL Workfront] afin de définir les éléments que les feuilles de temps peuvent préremplir et les éléments pour lesquels les personnes peuvent consigner des heures.

>[!IMPORTANT]
>
>Outre les éléments qui préremplissent une feuille de temps selon les conditions décrites dans cet article, les éléments suivants s’affichent également, par défaut, sur les feuilles de temps :
>
>* Éléments pour lesquels vous avez consigné des heures pendant la période de la feuille de temps
>* Éléments épinglés dans la feuille de temps
>* Éléments que vous recherchez et ajoutez manuellement à la feuille de temps. Par défaut, les éléments ajoutés manuellement sont épinglés.
>
>Pour plus d’informations, voir [Enregistrer les heures](../../../timesheets/create-and-manage-timesheets/log-time.md) et [Vue d’ensemble de la feuille de temps](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).

Toutes les modifications que vous apportez aux feuilles de temps ont un impact sur toutes les feuilles de temps créées ultérieurement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Définir les préférences des feuilles de temps et des heures

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Feuille de temps et heures]** > **[!UICONTROL Préférences]**.

   La page Préférences des feuilles de temps et des heures s’affiche.

1. (Facultatif) Dans la zone de recherche **Préférences système des feuilles de temps et des heures**, commencez à saisir le nom d’un groupe, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   ![Zone Rechercher un groupe](assets/search-for-group-box-in-timesheets-preferences-page.png)

   La page Préférences de la feuille de temps et des heures se met à jour avec les préférences du groupe que vous avez sélectionné. Les préférences au niveau du système doivent être déverrouillées pour pouvoir modifier les préférences au niveau du groupe. Pour plus d’informations, voir la section [Déverrouiller les préférences de feuille de temps et d’heures pour les groupes](#unlock-timesheet-and-hour-preferences-for-groups) dans cet article.

1. Dans la section **[!UICONTROL Préférences générales]**, configurez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Log time for future dates]</td> 
      <td> <p>Permet aux utilisateurs et utilisatrices de consigner le temps pour des dates futures dans l’ensemble du système pour les éléments suivants :</p> 
       <ul> 
        <li>Tous les projets, tâches et problèmes auxquels ils ont accès pour consigner des heures.</li> 
        <li>Leurs feuilles de temps comme temps général.</li> 
       </ul> <p>Cette fonction est utile lorsque les utilisateurs et utilisatrices prévoient de s’absenter du bureau et souhaitent consigner ce temps à l’avance.</p> <p><b>REMARQUE</b> :</p> 
       <p>Vous ne pouvez pas empêcher les personnes de consigner des heures sur des tâches ou des problèmes qui sont fermés ou annulés. Vous pouvez uniquement les empêcher de consigner du temps sur des projets terminés ou morts. Nous vous recommandons d’utiliser des filtres dans les listes de tâches et de problèmes afin de masquer les tâches terminées ou annulées aux utilisateurs et utilisatrices.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Assign Job Roles to hour entries manually]</td> 
      <td> <p>Permettez aux utilisateurs et utilisatrices de sélectionner manuellement toute fonction attribuée à leur profil d’utilisateur ou d’utilisatrice, ou à l’objet.</p> <p><b>IMPORTANT</b> :  
        <ul> 
         <li>Si vous désactivez ce paramètre après avoir affecté des fonctions aux entrées d’heures, les personnes doivent ajuster les heures enregistrées sous différents rôles dans l’onglet [!UICONTROL Hours] du projet, de la tâche ou du problème.</li> 
         <li>Si aucune fonction n’est attribuée à la personne dans son profil et qu’une tâche lui est attribuée en tant que [!UICONTROL Task Owner] dans la boîte de dialogue [!UICONTROL Advanced Assignments], cette fonction s’affiche lorsque la personne enregistre les heures de la tâche.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict timesheet editing to owners and administrators]</td> 
      <td> <p>Restreignez la modification aux propriétaires de la feuille de temps et aux administrateurs et administratrices [!DNL Workfront]. Lorsque cette option est désactivée, les feuilles de temps peuvent également être modifiées par les personnes suivantes :</p> 
       <ul> 
        <li> <p>Les personnes ayant un accès administratif aux feuilles de temps et aux heures dans leur niveau d’accès.</p> </li> 
        <li> <p>Les personnes approbatrices de la feuille de temps si l’option « Peut modifier les heures » est activée sur la feuille de temps.</p> </li> 
        <li> <p>La personne responsable de la personne propriétaire de la feuille de temps.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict hour editing to owners and administrators]</td> 
      <td>Restreindre la modification à l’utilisateur ou à l’utilisatrice qui consigne les heures et aux administrateurs ou aux administratrices [!DNL Workfront]. Ce paramètre s’applique à l’onglet [!UICONTROL Hours] d’un projet ou à un rapport sur les heures.</td> 
     </tr> 
    </tbody> 
   </table>

1. Dans la section **[!UICONTROL L’endroit où les utilisateurs et utilisatrices peuvent enregistrer les heures]**, configurez l’une des options suivantes :

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Directly on projects]</td>
        <td>Permet aux utilisateurs et aux utilisatrices d’enregistrer les heures du projet (à la fois dans l’onglet [!UICONTROL Updates] et dans la feuille de temps). Si les utilisateurs et les utilisatrices n’enregistrent pas les heures au niveau du projet, ces options doivent rester décochées.</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are complete]</td>
        <td>Permet aux personnes de consigner les heures sur un projet qui a été marqué comme terminé. Si cette option est désactivée, les utilisateurs et les utilisatrices ne peuvent pas enregistrer les heures pour le travail effectué sur les projets dont le statut est [!UICONTROL Complete].</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are dead]</td>
        <td>Lorsque cette option est activée, les utilisateurs et les utilisatrices peuvent enregistrer les heures sur des projets ayant le statut [!UICONTROL Dead].</td>
    </tr>
   </table>

1. Dans la section **[!UICONTROL Renseigner les feuilles de temps automatiquement]**, configurez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Work that is within] &lt;number of weeks&gt; [!UICONTROL of the timesheet's work range]</td> 
      <td> <p>Définit le nombre de semaines avant et après la période de la feuille de temps qui contient les dates des tâches et des problèmes assignés à la personne.</p> 
      <p>Le paramètre par défaut est de 1 semaine et vous pouvez étendre cette période jusqu’à 4 semaines.</p> 
      <p>Cela signifie que la feuille de temps est remplie automatiqument avec des tâches et des problèmes dont les dates se situent entre quatre semaines avant la période de la feuille de temps et quatre semaines après la période de la feuille de temps, si vous sélectionnez 4 semaines pour votre plage. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have been completed]</td> 
      <td>Si plusieurs ressources sont généralement affectées à une seule tâche, nous recommandons ce paramètre. Cela signifie que lorsqu’une ressource consigne des heures sur la tâche et la marque comme terminée, les autres ressources affectées à la tâche peuvent toujours trouver la tâche ou le problème dans leur feuille de temps, afin de consigner leurs heures.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have Planned Dates in timesheet's date range]</td> 
      <td> <p>Lorsque cette option est sélectionnée, la feuille de temps inclut les tâches et les problèmes dont la date de début ou d’achèvement prévue se situe dans la période de la feuille de temps.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tasks that have Projected Dates in timesheet's date range]</td> 
      <td> <p>Lorsque cette option est sélectionnée, la feuille de temps inclut les tâches dont la date de début ou de fin prévisionnelle s’inscrit dans la période du projet, même si la date prévue du problème ou de la tâche se situe en dehors de la période de la feuille de temps.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans la section **[!UICONTROL Projets, tâches et problèmes supprimés]**, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> Lors de la suppression de projets</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Keep logged time already added to timesheets as general time]</strong> : si ce projet est restauré ultérieurement, le temps reste sur la feuille de temps)</li> 
        <li><strong>[!UICONTROL Delete any logged time]</strong> : si ce projet est restauré ultérieurement, le temps déjà consigné sera restauré sur le projet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lors de la suppression de tâches ou de problèmes</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Move any logged time to the project]</strong> contenant la tâche ou le problème : en cas de restauration ultérieure de la tâche ou du problème, le temps reste dans le projet.<br></li> 
        <li> <p><strong>[!UICONTROL Delete any logged time]</strong> : en cas de restauration ultérieure de la tâche ou du problème, le temps consigné sera restauré sur la tâche ou le problème.</p> <p>Pour plus d’informations sur ces options, consultez la section <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configure affect] sur les heures lorsqu’un objet est supprimé et restauré</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Déverrouiller les préférences de feuille de temps et d’heure pour les groupes

Les groupes de votre entreprise peuvent avoir besoin de feuilles de temps ou de préférences d’heure configurées différemment pour leurs workflows uniques. Vous pouvez déverrouiller les préférences de tous les groupes de l’organisation afin qu’ils puissent les configurer eux-mêmes.

Lorsqu’une préférence est déverrouillée et qu’un administrateur ou qu’une administratrice de groupe la modifie, elle affecte les propriétaires de feuilles de temps si le groupe est leur groupe d’accueil.

Pour plus d’informations sur la façon dont un administrateur ou une administratrice de groupe configure les préférences de feuille de temps et d’heure pour un groupe, consultez la section [Configurer les préférences de feuille de temps et d’heure pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Une fois qu’un administrateur ou qu’une administratrice [!DNL Workfront] a déverrouillé une préférence au niveau du système, tout membre de l’administration du groupe peut la configurer, puis la verrouiller pour s’assurer que tous les membres de son groupe et des sous-groupes inférieurs utilisent la même configuration. Cette fonction est similaire à la capacité qu’a un administrateur ou une administratrice [!DNL Workfront] de configurer et de verrouiller une préférence pour toutes les personnes utilisant le système. Pour plus d’informations, consultez la section [Verrouiller ou déverrouiller une feuille de temps et une préférence d’heure de groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Pour déverrouiller une préférence de projet afin que les groupes puissent la configurer :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Feuilles de temps et heures]**, puis cliquez sur **[!UICONTROL Préférences]**.

1. Effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs de groupes puissent configurer une préférence pour leurs groupes, cliquez sur le bouton bascule **déverrouiller** ![Déverrouiller](assets/unlock-toggle-button.png) pour le déverrouiller .
   * Si vous souhaitez que tous les groupes utilisent votre configuration pour une préférence, assurez-vous que le bouton (bascule) est verrouillé ![bascule des préférences verrouillées](assets/locked-preference-toggle.png) (valeur par défaut).

     >[!IMPORTANT]
     >
     >Nous vous recommandons de communiquer avec les administrateurs et administratrices et les utilisateurs et utilisatrices des groupes dans l’ensemble du système afin de vous assurer que tous les besoins sont pris en compte dans la manière dont vous configurez une préférence verrouillée.
     >
     >Lorsque vous la verrouillez, votre configuration est héritée par tous les groupes du système. De plus, si la préférence a été déverrouillée pour une période de temps donnée, votre configuration remplace celles que les administrateurs et administratrices de groupe ont pu effectuer.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
