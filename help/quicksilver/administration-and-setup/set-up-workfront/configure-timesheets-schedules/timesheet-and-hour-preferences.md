---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configuration des préférences de feuille de temps et d’heure
description: Comme [!DNL Adobe Workfront] administrateur, vous pouvez spécifier des préférences pour les feuilles de temps et les heures dans [!DNL Workfront] afin de définir les éléments que les feuilles de temps peuvent préremplir et les éléments auxquels les utilisateurs peuvent se connecter.
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 66e6c96ca51a159f6e9a16178f06dd016217c7d8
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Configuration des préférences de feuille de temps et d’heure

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Comme [!DNL Adobe Workfront] administrateur, vous pouvez spécifier des préférences pour les feuilles de temps et les heures dans [!DNL Workfront] afin de définir les éléments que les feuilles de temps peuvent préremplir et les éléments auxquels les utilisateurs peuvent se connecter.

>[!IMPORTANT]
>
>Outre les éléments qui préremplissent une feuille de temps selon les conditions décrites dans cet article, les éléments suivants s’affichent également, par défaut, sur les feuilles de temps :
>
>* Éléments pour lesquels vous avez consigné l’heure pendant la période de la feuille de temps
>* Éléments épinglés dans la feuille de temps
>* Éléments que vous recherchez et ajoutez manuellement à la feuille de temps. Par défaut, les éléments ajoutés manuellement sont épinglés.
>
>Pour plus d’informations, voir [Temps de connexion](../../../timesheets/create-and-manage-timesheets/log-time.md) et [Présentation de la feuille de temps](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).



Toutes les modifications que vous apportez aux feuilles de temps ont un impact sur toutes les feuilles de temps créées ultérieurement.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>Actuel :[!UICONTROL Plan]</p>
   Ou
   <p>Nouveau : Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur.</p>  </td>
</tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Définition des préférences de feuille de temps et d’heure

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Frise chronologique et heures]** > **[!UICONTROL Préférences]**.

   La page Fiches horaires et préférences Heures s’affiche.

1. (Facultatif) Dans la variable **Préférences des Fiches horaires et heures système** , commencez à saisir le nom d’un groupe, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   ![](assets/search-for-group-box-in-timesheets-preferences-page.png)

   La page Préférences de la feuille de temps et des heures se met à jour avec les préférences du groupe que vous avez sélectionné. Les préférences au niveau du système doivent être déverrouillées pour pouvoir modifier les préférences au niveau du groupe. Pour plus d’informations, voir la section [Déverrouiller les préférences de feuille de temps et d’heure pour les groupes ;](#unlock-timesheet-and-hour-preferences-for-groups) dans cet article.

1. Dans le **[!UICONTROL Préférences générales]** , configurez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Durée du journal des dates futures]</td> 
      <td> <p>Permet aux utilisateurs de se connecter à l’heure des dates futures dans l’ensemble du système dans :</p> 
       <ul> 
        <li>Tous les projets, tâches et problèmes pour lesquels ils ont accès au temps de journalisation</li> 
        <li>Leur feuille de temps comme heure générale</li> 
       </ul> <p>Cela s’avère utile lorsque les utilisateurs prévoient de quitter le bureau et qu’ils souhaitent enregistrer ce temps au préalable.</p> <p><b>REMARQUE</b>:</p> 
       <p>Vous ne pouvez pas empêcher les utilisateurs de se connecter à des tâches ou des problèmes qui sont fermés ou annulés. Vous pouvez uniquement empêcher les utilisateurs de se connecter à des projets complets ou inactifs. Nous vous recommandons d’utiliser des filtres dans les listes de tâches et de problèmes pour exclure de la visibilité pour les utilisateurs ceux qui ont été terminés ou annulés.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Affecter manuellement des rôles de tâche aux entrées d’heure]</td> 
      <td> <p>Permet aux utilisateurs de sélectionner manuellement n’importe quel rôle de tâche attribué dans leur profil utilisateur ou affecté à l’objet.</p> <p><b>IMPORTANT</b>:  
        <ul> 
         <li>Si vous désactivez ce paramètre après avoir affecté des rôles de tâche aux entrées d’heure, les utilisateurs doivent ajuster les heures enregistrées sous différents rôles dans l’onglet [!UICONTROL Hours] du projet, de la tâche ou du problème.</li> 
         <li>Si un rôle de tâche n’est pas attribué à l’utilisateur dans son profil et qu’une tâche est affectée en tant que [!UICONTROL Propriétaire de la tâche] dans la boîte de dialogue [!UICONTROL Affectations avancées], ce rôle de tâche s’affiche lorsque l’utilisateur connecte l’heure de la tâche.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restreindre la modification de la feuille de temps aux propriétaires et aux administrateurs]</td> 
      <td> <p>Restreindre la modification aux propriétaires de la feuille de temps et [!DNL Workfront] administrateurs. Lorsque cette option est désactivée, les feuilles de temps peuvent également être modifiées en :</p> 
       <ul> 
        <li> <p>Utilisateurs disposant d’un accès administratif aux feuilles de temps et aux heures dans leur niveau d’accès</p> </li> 
        <li> <p>Approbateurs de la feuille de temps si l’option "Modifications des heures" est activée sur la feuille de temps</p> </li> 
        <li> <p>Le gestionnaire du propriétaire de la feuille de temps</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restreindre la modification d’heure aux propriétaires et administrateurs]</td> 
      <td>Restreindre la modification à l’utilisateur qui saisit les heures et [!DNL Workfront] administrateurs. Ce paramètre s’applique à l’onglet [!UICONTROL Hours] d’un projet ou d’un rapport Hours.</td> 
     </tr> 
    </tbody> 
   </table>

1. Dans le **[!UICONTROL Où les utilisateurs peuvent consigner l’heure]** , configurez l’une des options suivantes :

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Directement sur les projets]</td>
        <td>Permet aux utilisateurs de se connecter au projet (à la fois dans l’onglet [!UICONTROL Mises à jour] et dans la feuille de temps). Si les utilisateurs n’enregistrent pas de temps au niveau du projet, ces options doivent rester décochées.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Sur les projets terminés]</td>
        <td>Permet aux utilisateurs d’enregistrer du temps sur un projet marqué comme terminé. Si cette option est désactivée, les utilisateurs ne peuvent pas enregistrer le temps passé pour le travail qu’ils ont terminé sur les projets dont l’état est [!UICONTROL Terminé].</td>
    </tr>
    <tr>
        <td>[!UICONTROL Sur les projets morts]</td>
        <td>Lorsque cette option est activée, les utilisateurs peuvent ouvrir une session d’heures sur des projets avec le statut [!UICONTROL Morts] .</td>
    </tr>
   </table>

1. Dans le **[!UICONTROL Préremplissage des feuilles de temps]** , configurez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Travail compris dans] &lt;number of="" weeks=""&gt; [!UICONTROL de la plage de travail de la feuille de temps]</td> 
      <td> <p>Définit le nombre de semaines avant et après la période de la feuille de temps qui contient les dates des tâches et les problèmes affectés à l’utilisateur.</p> 
      <p>Le paramètre par défaut est de 1 semaine et vous pouvez l’étendre à 4 semaines.</p> 
      <p>Cela signifie que la feuille de temps est prérenseignée avec des tâches et des problèmes dont les dates se situent entre quatre semaines avant la période de la feuille de temps, jusqu’à quatre semaines après la période de la feuille de temps, si vous sélectionnez 4 semaines pour la période. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tâches et problèmes terminés]</td> 
      <td>Si plusieurs ressources sont généralement affectées à une seule tâche, nous vous recommandons ce paramètre. Cela signifie que lorsqu’une ressource enregistre le temps par rapport à la tâche et la marque comme terminée, les autres ressources affectées à la tâche peuvent toujours trouver la tâche ou le problème dans leur feuille de temps, pour enregistrer leurs heures.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tâches et problèmes ayant des dates planifiées dans la période de la feuille de temps]</td> 
      <td> <p>Lorsqu’elle est sélectionnée, la feuille de temps inclut des tâches et des problèmes dont la date de début planifiée ou la date de fin est comprise dans la plage de dates de la feuille de temps.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tâches dont les dates ont été projetées dans la période de la feuille de temps]</td> 
      <td> <p>Lorsqu’elle est sélectionnée, la feuille de temps inclut des tâches dont la date de début prévue ou la date de fin correspond à la période du projet, même si la date planifiée de l’émission ou de la tâche ne figure pas dans la plage de dates de la feuille de temps.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans le **[!UICONTROL Projets, tâches et problèmes supprimés]** , spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> Lors de la suppression de projets</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Conserver l’heure enregistrée déjà ajoutée aux feuilles de temps en tant qu’heure générale]</strong>: si ce projet est restauré à une date ultérieure, l’heure reste sur la feuille de temps.</li> 
        <li><strong>[!UICONTROL Supprimer toute heure enregistrée]</strong>: si ce projet est restauré par la suite, l’heure déjà enregistrée est restaurée dans le projet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lors de la suppression de tâches ou de problèmes</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Déplacer toute heure enregistrée vers le projet]</strong> où réside la tâche ou le problème : si cette tâche ou ce problème est restauré par la suite, le temps reste sur le projet.<br></li> 
        <li> <p><strong>[!UICONTROL Supprimer toute heure enregistrée]</strong>: si cette tâche ou ce problème est restauré par la suite, l’heure consignée est restaurée à la tâche ou au problème.</p> <p>Pour plus d’informations sur ces options, voir <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configurer l’effet] sur les heures lorsqu’un objet est supprimé et restauré</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Déverrouiller les préférences de feuille de temps et d’heure pour les groupes ;

Les groupes de votre entreprise peuvent avoir besoin de feuilles de temps ou de préférences d’heure configurées différemment pour leurs workflows uniques. Vous pouvez déverrouiller les préférences de tous les groupes de l’organisation afin qu’ils puissent les configurer eux-mêmes.

Lorsqu’une préférence est déverrouillée et qu’un administrateur de groupe la modifie, elle affecte les propriétaires de feuilles de temps si le groupe est leur groupe d’accueil.

Pour plus d’informations sur la façon dont un administrateur de groupe configure les préférences de feuille de temps et d’heure pour un groupe, voir [Configuration des préférences de feuille de temps et d’heure pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Après une [!DNL Workfront] l’administrateur déverrouille une préférence au niveau du système. tout administrateur de groupe peut la configurer, puis la verrouiller pour s’assurer que tous les membres de leur groupe et les sous-groupes ci-dessous utilisent la même configuration. Cela est parallèle à la capacité qu’a une [!DNL Workfront] l’administrateur doit configurer et verrouiller une préférence pour tous les utilisateurs du système. Pour plus d’informations, voir [Verrouillage ou déverrouillage d’une feuille de temps et d’une préférence d’heure de groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Pour déverrouiller une préférence de projet afin que les groupes puissent la configurer :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Fiches horaires et heures]**, puis cliquez sur **[!UICONTROL Préférences]**.

1. Effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs de groupes puissent configurer une préférence pour leurs groupes, cliquez sur le bouton **déverrouiller** basculer ![](assets/unlock-toggle-button.png) pour le déverrouiller.
   * Si vous souhaitez que tous les groupes utilisent votre configuration pour une préférence, assurez-vous qu’elle est verrouillée. ![](assets/locked-preference-toggle.png) (il s’agit de la valeur par défaut).

     >[!IMPORTANT]
     >
     >Nous vous recommandons de communiquer avec les administrateurs et les utilisateurs de groupes dans tout le système pour vous assurer que tous les besoins sont pris en compte dans la configuration d’une préférence verrouillée.
     >
     >Lorsque vous le verrouillez, votre configuration pour elle est héritée par tous les groupes du système. Et si la préférence a été déverrouillée pendant une période quelconque, votre configuration remplace celles que les administrateurs de groupe peuvent avoir faites.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
