---
user-type: administrator
product-area: system-administration;user-management
keywords: group,preferences,task,groups,issue,unlock
navigation-topic: create-and-manage-groups
title: Configuration des préférences de feuille de temps et d’heure pour un groupe
description: Au niveau du système, un administrateur Adobe Workfront peut déverrouiller les sections timesheet and hour preferences General Preferences et Pre-Renseignate timesheets with. Cela permet aux administrateurs de groupes de configurer les options de ces sections indépendamment pour leurs propres groupes.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: 3b0a82381d1c33d897b123a597df21ba54cc2565
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 6%

---

# Configuration des préférences de feuille de temps et d’heure pour un groupe

{{highlighted-preview}}

Un administrateur Adobe Workfront peut déverrouiller les sections suivantes des préférences de feuille de temps et d’heure au niveau du système afin que les administrateurs de groupe puissent les configurer indépendamment pour leurs propres groupes :

* Préférences générales
* <span class="preview">L’endroit où les utilisateurs et utilisatrices peuvent enregistrer les heures</span>
* Préremplir les feuilles de temps

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

Les sections suivantes de la page des préférences Frise chronologique et Heures ne peuvent être configurées qu’au niveau du système et ne peuvent pas être déverrouillées pour les groupes :

* Projets, tâches et problèmes supprimés

Pour plus d’informations sur la façon dont un administrateur Workfront déverrouille une feuille de temps et des préférences d’heure, consultez la section . [Déverrouiller les préférences de feuille de temps et d’heure pour les groupes ;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) dans l’article [Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>Une configuration au niveau du groupe est également possible pour les préférences du projet, ainsi que pour les préférences de tâche et de problème. Pour plus d’informations, voir [Configuration des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Préférences pour la feuille de temps et l’heure du groupe

Tenez compte des informations suivantes sur la configuration d’une feuille de temps ou d’une préférence d’heure déverrouillée pour un groupe :

* Si vous êtes administrateur de groupe et que vous configurez une préférence de feuille de temps ou d’heure pour votre groupe, cela affecte les personnes qui utilisent le groupe comme groupe d’accueil.
* En règle générale, une préférence déverrouillée reste déverrouillée indéfiniment. Si l’administrateur Workfront le reverrouille, le paramètre système prend à nouveau effet et les paramètres de la préférence accordée par les administrateurs du groupe sont perdus.
* Une feuille de temps hérite des préférences de feuille de temps et d’heure configurées pour le groupe d’accueil du propriétaire de la feuille de temps.

   <!--
  Add example here?
  -->

* Une fois qu’un administrateur Workfront a déverrouillé une préférence au niveau du système et que vous l’avez configurée pour votre groupe, vous pouvez la verrouiller pour vous assurer que tous les membres des groupes situés sous le vôtre utilisent la même configuration. Cela est parallèle à la possibilité qu’un administrateur de Workfront a de configurer et de verrouiller une préférence pour tous les utilisateurs du système. Pour plus d’informations, voir [Verrouillage ou déverrouillage d’une feuille de temps et d’une préférence d’heure de groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configuration d’une feuille de temps ou d’une préférence d’heure déverrouillée pour un groupe

>[!TIP]
>
>Si vous êtes administrateur de Workfront, vous pouvez ignorer les étapes 1 à 4 en accédant à Configuration > Frise chronologique et heures > Préférences, puis en recherchant le nom du groupe dans la zone située en haut de la page.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe dont vous souhaitez configurer les préférences de feuille de temps ou d’heure.
1. Dans le panneau de gauche, cliquez sur **Fiches horaires et heures**.

1. Sur la page qui s’affiche, dans la variable **Préférences générales** , configurez l’une des options suivantes :

   >[!TIP]
   >
   >Si vous passez la souris sur une préférence et qu’une info-bulle s’affiche pour vous indiquer qu’elle est verrouillée, vous pouvez demander à votre administrateur Workfront de la déverrouiller pour tous les groupes de l’organisation.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Enregistrer le temps pour les dates futures</td> 
      <td> <p>Permet aux utilisateurs de se connecter à l’heure des dates futures dans l’ensemble du système dans :</p> 
       <ul> 
       <li>Tous les projets, tâches et problèmes pour lesquels ils ont accès à la durée du journal, quel que soit le groupe du projet.</li> 
       <li>Leur feuille de temps comme heure générale</li>
       </ul> 
       <p>Cela s’avère utile lorsque les utilisateurs prévoient de quitter le bureau et qu’ils souhaitent enregistrer ce temps au préalable.</p> 
       <p><b>REMARQUE</b>: Vous ne pouvez pas empêcher les utilisateurs de se connecter à des tâches ou des problèmes qui sont fermés ou annulés. Vous pouvez uniquement empêcher les utilisateurs de se connecter à des projets complets ou inactifs. Nous vous recommandons d’utiliser des filtres dans les listes de tâches et de problèmes pour exclure de la visibilité pour les utilisateurs ceux qui ont été terminés ou annulés.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajouter des dépenses à partir d'une feuille de présence</td> 
      <td> <p>Permet aux utilisateurs d’enregistrer le temps et les dépenses dans la feuille de temps.</p> 
      <p>Lorsque cette préférence est activée pour un groupe et que le groupe est défini comme groupe d’accueil pour certains utilisateurs, une icône de dépense s’affiche en regard des projets et tâches de la feuille de temps de ces utilisateurs. Les utilisateurs peuvent cliquer sur cette icône pour ajouter ou modifier des dépenses pour le projet ou la tâche.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affectez manuellement des fonctions à des saisies d'heures</td> 
      <td> <p>Permet aux utilisateurs de sélectionner manuellement n’importe quel rôle de tâche attribué dans leur profil utilisateur ou affecté à l’objet.</p> <p><b>IMPORTANT</b>:  
        <ul> 
         <li>Si vous désactivez ce paramètre après avoir affecté des rôles de tâche aux entrées d’heure, les utilisateurs doivent ajuster les heures consignées sous différents rôles dans l’onglet Heures du projet, de la tâche ou du problème.</li> 
         <li>Si un rôle de tâche n’est pas attribué à l’utilisateur dans son profil et qu’une tâche est affectée en tant que propriétaire de la tâche dans la boîte de dialogue Affectations avancées , ce rôle de tâche s’affiche lorsque l’utilisateur consigne l’heure sur la tâche.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limiter la modification de feuilles de temps aux propriétaires et aux administrateurs</td> 
      <td> <p>Restreindre la modification aux propriétaires de feuilles de temps, quel que soit le groupe du projet et les administrateurs Workfront. Lorsque cette option est désactivée, les feuilles de temps peuvent également être modifiées en :</p> 
       <ul> 
        <li> <p>Utilisateurs disposant d’un accès administratif aux feuilles de temps et aux heures dans leur niveau d’accès</p> </li> 
        <li> <p>Approbateurs de la feuille de temps si l’option "Modifications des heures" est activée sur la feuille de temps</p> </li> 
        <li> <p>Le gestionnaire du propriétaire de la feuille de temps</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limitation de la modification des heures aux propriétaires et aux administrateurs</td> 
      <td>Restreindre la modification à l’utilisateur qui saisit les heures et les administrateurs Workfront. Ce paramètre s’applique à l’onglet Heures dans un projet ou dans un rapport Heures .</td> 
     </tr> 
    </tbody> 
   </table>

1. <span class="preview">Dans le **Où les utilisateurs peuvent consigner l’heure** , configurez l’une des options suivantes :</span>

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><span class="preview">Enregistrer le temps directement sur les projets</span></td> 
      <td><span class="preview">Permet aux utilisateurs de se connecter au projet (à la fois dans l’onglet Mises à jour et dans la feuille de temps). Si vous souhaitez empêcher vos utilisateurs d’enregistrer le temps au niveau du projet, laissez cette option décochée.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview">Enregistrer le temps sur les projets déjà terminés</span></td>
      <td><span class="preview">Permet aux utilisateurs d’enregistrer du temps sur un projet marqué comme terminé. Si cette option est désactivée, les utilisateurs ne peuvent pas enregistrer le temps de travail qu’ils ont terminé sur les projets dont l’état est Terminé.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview">Enregistrer le temps sur les projets inactifs</span></td> 
      <td><span class="preview">Lorsque cette option est activée, les utilisateurs peuvent ouvrir une session d’heures sur des projets dont l’état est Mort.</span></td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Cette préférence est appliquée en fonction de la configuration des préférences du groupe d’accueil de l’utilisateur. Si ces paramètres sont activés dans les préférences du groupe d’accueil de l’utilisateur, celui-ci pourra consigner directement le temps passé sur les projets, y compris les projets terminés ou morts, que les préférences du groupe du projet le permettent ou non.

1. Dans le **Préremplir les feuilles de temps** , configurez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Travail dans &lt;number of="" weeks=""&gt; de la plage de travail de la feuille de temps</td> 
      <td> <p>Définit le nombre de semaines avant et après la période de la feuille de temps qui contient les dates des tâches et les problèmes affectés à l’utilisateur. Le paramètre par défaut est de 1 semaine et vous pouvez l’étendre à 4 semaines. Cela signifie que la feuille de temps est prérenseignée avec des tâches et des problèmes dont les dates se situent entre quatre semaines avant la période de la feuille de temps, jusqu’à quatre semaines après la période de la feuille de temps, si vous sélectionnez 4 semaines pour la période. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tâches et Événements qui sont terminés</td> 
      <td>Si plusieurs ressources sont généralement affectées à une seule tâche, nous vous recommandons ce paramètre. Cela signifie que lorsqu’une ressource enregistre le temps par rapport à la tâche et la marque comme terminée, les autres ressources affectées à la tâche peuvent toujours trouver la tâche ou le problème dans leur feuille de temps, pour enregistrer leurs heures.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tâches et Événements ayant des dates prévues dans la plage de dates de la feuille de temps</td> 
      <td> <p>Lorsqu’elle est sélectionnée, la feuille de temps inclut des tâches et des problèmes dont la date de début planifiée ou la date de fin est comprise dans la plage de dates de la feuille de temps.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tâches ayant des dates prévues dans l'intervalle de dates de la feuille de temps</td> 
      <td> <p>Lorsqu’elle est sélectionnée, la feuille de temps inclut des tâches dont la date de début prévue ou la date de fin correspond à la période du projet, même si la date planifiée de l’émission ou de la tâche ne figure pas dans la plage de dates de la feuille de temps.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
