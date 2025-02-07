---
user-type: administrator
product-area: system-administration;user-management
keywords: groupe,préférences,tâche,groupes,problème,déverrouillage
navigation-topic: create-and-manage-groups
title: Configuration des préférences de feuille de temps et d'heures pour un groupe
description: Au niveau du système, l’équipe d’administration Adobe Workfront peut déverrouiller les sections de préférences de feuilles de temps et d’heures Préférences générales et Préremplir les feuilles de temps avec... Cela permet aux administrateurs et administratrices de groupes de configurer les options de ces sections séparément pour leurs propres groupes.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 97%

---

# Configurer les préférences de feuilles de temps et d’heures pour un groupe

Un administrateur ou une administratrice Adobe Workfront peut déverrouiller les sections suivantes des préférences de feuilles de temps et d’heures au niveau du système, afin que les administrateurs et administratrices de groupes puissent les configurer séparément pour leurs propres groupes :

* Préférences générales
* L’endroit où les utilisateurs et utilisatrices peuvent enregistrer les heures
* Préremplir les feuilles de temps

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Les sections suivantes de la page Préférences de feuilles de temps et d’heures sont configurables uniquement au niveau du système et ne peuvent pas être déverrouillées pour les groupes :

* Projets, tâches et problèmes supprimés

Pour plus d’informations sur la manière dont un administrateur ou une administratrice Workfront déverrouille une préférence de feuilles de temps et d’heures, consultez la section [Déverrouiller les préférences de feuilles de temps et d’heures pour les groupes](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) dans l’article [Configurer les préférences de feuilles de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>La configuration au niveau du groupe est également possible pour les préférences de projets et pour les préférences de tâches et de problèmes. Pour plus d’informations, consultez la section [Configurer les préférences de projets pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Configurer les préférences de tâches et de problèmes pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

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

## Préférences de feuilles de temps et d’heures pour les groupes

Tenez compte des informations suivantes concernant la configuration d’une préférence de feuilles de temps ou d’heures non verrouillée pour un groupe :

* Si vous êtes administrateur ou administratrice de groupes et que vous configurez une préférence de feuilles de temps ou d’heures pour votre groupe, cela affecte les personnes qui utilisent ce groupe comme groupe principal.
* En règle générale, une préférence déverrouillée reste déverrouillée indéfiniment. Si l’administrateur ou l’administratrice Workfront la verrouille à nouveau, le paramètre système prend à nouveau effet et les paramètres de la préférence définie par les administrateurs et administratrices de groupes sont perdus.
* Une feuille de temps hérite des préférences de feuilles de temps et d’heures configurées pour le groupe principal de la personne propriétaire de la feuille de temps.

  <!--
  Add example here?
  -->

* Une fois qu’un administrateur ou une administratrice Workfront a déverrouillé une préférence au niveau du système et que vous l’avez configurée pour votre groupe, vous pouvez la verrouiller pour vous assurer que toutes les personnes membres des groupes situés sous le vôtre utilisent la même configuration. Ceci vient en parallèle de la capacité qu’a un administrateur ou une administratrice Workfront de configurer et de verrouiller une préférence pour tous les utilisateurs et utilisatrices du système. Pour plus d’informations, consultez la section [Verrouiller ou déverrouiller une préférence de feuilles de temps et d’heures pour les groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurer une préférence de feuilles de temps ou d’heures non verrouillée pour un groupe

>[!TIP]
>
>Si vous êtes administrateur ou administratrice de Workfront, ignorez les étapes 1 à 4 en accédant à Configuration > Feuille de temps et heures > Préférences, puis en recherchant le nom du groupe dans la zone située en haut de la page.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez configurer les préférences de feuilles de temps ou d’heures.
1. Dans le panneau de gauche, cliquez sur **Feuilles de temps et heures**.

1. Sur la page qui s’affiche, dans la section **Préférences générales**, configurez l’une des options suivantes :

   >[!TIP]
   >
   >Si vous passez la souris sur une préférence et qu’une info-bulle s’affiche pour vous indiquer qu’elle est verrouillée, vous pouvez demander à votre administrateur ou à votre administratrice Workfront de la déverrouiller pour tous les groupes de l’organisation.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Consigner le temps pour les dates futures</td> 
      <td> <p>Permet aux utilisateurs et utilisatrices de consigner le temps pour des dates futures dans l’ensemble du système pour les éléments suivants :</p> 
       <ul> 
       <li>Tous les projets, tâches et problèmes pour lesquels ils ont accès pour consigner le temps, quel que soit le groupe du projet.</li> 
       <li>Leurs feuilles de temps comme temps général.</li>
       </ul> 
       <p>Cette fonction est utile lorsque les utilisateurs et utilisatrices prévoient de s’absenter du bureau et souhaitent consigner ce temps à l’avance.</p> 
       <p><b>NOTE</b> : vous ne pouvez pas empêcher les utilisateurs et utilisatrices de consigner du temps sur des tâches et des problèmes qui sont fermés ou annulés. Vous pouvez uniquement les empêcher de consigner du temps sur des projets terminés ou morts. Nous vous recommandons d’utiliser des filtres dans les listes de tâches et de problèmes afin de masquer les tâches terminées ou annulées aux utilisateurs et utilisatrices.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajouter des dépenses à partir d’une feuille de temps</td> 
      <td> <p>Permet aux personnes d’enregistrer à la fois les heures et les dépenses dans la feuille de temps.</p> 
      <p>Lorsque cette préférence est activée pour un groupe et que ce dernier est défini comme groupe principal pour certaines personnes, une icône de dépense s’affiche à côté des projets et des tâches sur les feuilles de temps de ces personnes. Les personnes peuvent cliquer sur cette icône pour ajouter ou modifier des dépenses pour le projet ou la tâche.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attribuer manuellement des fonctions aux entrées d’heures</td> 
      <td> <p>Permettez aux utilisateurs et utilisatrices de sélectionner manuellement toute fonction attribuée à leur profil d’utilisateur ou d’utilisatrice, ou à l’objet.</p> <p><b>IMPORTANT</b> :  
        <ul> 
         <li>Si vous désactivez ce paramètre après avoir attribué des fonctions aux entrées d’heures, les personnes doivent ajuster les heures consignées sous différents rôles dans l’onglet Heures du projet, de la tâche ou du problème.</li> 
         <li>Si la personne n’a pas de fonction attribuée dans son profil et qu’une tâche lui est attribuée en tant que propriétaire de la tâche dans la boîte de dialogue Affectations avancées, cette fonction apparaît lorsque la personne consigne des heures pour la tâche.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limiter la modification de feuilles de temps aux personnes propriétaires et aux administrateurs et administratices</td> 
      <td> <p>Limitez la modification aux personnes propriétaires des feuilles de temps, indépendamment du groupe du projet et des administrateurs et administratrices Workfront. Lorsque cette option est désactivée, les feuilles de temps peuvent également être modifiées par les personnes suivantes :</p> 
       <ul> 
        <li> <p>Les personnes ayant un accès administratif aux feuilles de temps et aux heures dans leur niveau d’accès.</p> </li> 
        <li> <p>Les personnes approbatrices de la feuille de temps si l’option « Peut modifier les heures » est activée sur la feuille de temps.</p> </li> 
        <li> <p>La personne responsable de la personne propriétaire de la feuille de temps.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limiter la modification des heures aux personnes propriétaires et aux administrateurs et administratrices.</td> 
      <td>Limitez la modification à la personne qui a saisi les heures et aux administrateurs et administratrices de Workfront. Ce paramètre s’applique à l’onglet Heures d’un projet ou d’un rapport d’heures.</td> 
     </tr> 
    </tbody> 
   </table>

1. Dans la section **L’endroit où les utilisateurs et utilisatrices peuvent enregistrer les heures**, configurez l’une des options suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Consigner les heures directement sur les projets</td> 
      <td>Permet aux personnes de consigner les heures sur le projet (à la fois sur l’onglet Mises à jour et sur la feuille de temps). Si vous souhaitez empêcher vos utilisateurs et utilisatrices de consigner des heures au niveau du projet, ne cochez pas cette option.</td>
     </tr>
     <tr>
      <td role="rowheader">Consigner les heures sur les projets déjà terminés</td>
      <td>Permet aux personnes de consigner les heures sur un projet qui a été marqué comme terminé. Si cette option est désactivée, les personnes ne peuvent pas consigner d’heures pour le travail qu’elles ont effectué sur des projets dont le statut est Terminé.</td>
     </tr>
     <tr>
      <td role="rowheader">Consigner les heures sur les projets obsolètes</td> 
      <td>Lorsque cette option est activée, les personnes peuvent enregistrer des heures sur des projets dont le statut est Immobilisé.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Cette préférence est appliquée en fonction de la configuration des préférences du groupe principal de la personne. Si ces paramètres sont activés dans les préférences du groupe principal de la personne, celle-ci pourra consigner directement les heures sur les projets, y compris les projets terminés ou obsolètess, que les préférences du groupe de projet l’y autorisent ou non.

1. Dans la section **Renseigner les feuilles de temps automatiquement**, configurez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Travail compris dans &lt;nombre de semaines&gt; dans la plage de travail de la feuille de temps</td> 
      <td> <p>Définit le nombre de semaines avant et après la période de la feuille de temps qui contient les dates des tâches et des problèmes assignés à la personne. Le paramètre par défaut est de 1 semaine et vous pouvez étendre cette période jusqu’à 4 semaines. Cela signifie que la feuille de temps est remplie automatiqument avec des tâches et des problèmes dont les dates se situent entre quatre semaines avant la période de la feuille de temps et quatre semaines après la période de la feuille de temps, si vous sélectionnez 4 semaines pour votre plage. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tâches et problèmes terminés</td> 
      <td>Si plusieurs ressources sont généralement affectées à une seule tâche, nous recommandons ce paramètre. Cela signifie que lorsqu’une ressource consigne des heures sur la tâche et la marque comme terminée, les autres ressources affectées à la tâche peuvent toujours trouver la tâche ou le problème dans leur feuille de temps, afin de consigner leurs heures.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tâches et problèmes ayant des dates prévues dans la période de la feuille de temps</td> 
      <td> <p>Lorsque cette option est sélectionnée, la feuille de temps inclut les tâches et les problèmes dont la date de début ou d’achèvement prévue se situe dans la période de la feuille de temps.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tâches ayant des dates prévisionnelles dans la période de la feuille de temps</td> 
      <td> <p>Lorsque cette option est sélectionnée, la feuille de temps inclut les tâches dont la date de début ou de fin prévisionnelle s’inscrit dans la période du projet, même si la date prévue du problème ou de la tâche se situe en dehors de la période de la feuille de temps.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
