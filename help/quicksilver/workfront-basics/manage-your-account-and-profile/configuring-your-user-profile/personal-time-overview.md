---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurer les congés
description: Dans Adobe Workfront, il est important d’indiquer les congés approuvés, car ils ont une incidence sur votre planning et sur les dates d’achèvement prévues des tâches qui vous ont été affectées.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 75%

---

# Configurer les congés

<!-- Audited: 12/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment, and is being released in a phased rollout to Production.</span>-->

[!DNL Adobe Workfront] n’est pas conçu pour reproduire ou remplacer les systèmes existants de votre organisation pour la gestion, l’accumulation ou le suivi des congés personnels.

Cependant, il est important d’indiquer les congés approuvés, car ils ont une incidence sur votre planning et sur les [!UICONTROL dates d’achèvement prévues] des tâches qui vous ont été affectées.

Par exemple, si une tâche vous est affectée pour une durée de deux semaines et que vous prévoyez de prendre trois jours de congé pendant cette période, [!DNL Workfront] ajoute trois jours à la chronologie de la tâche pour tenir compte de ces congés.

Les outils de gestion des ressources utilisent également vos congés pour indiquer vos disponibilités de travail.

>[!NOTE]
>
>Pour éviter toute incohérence dans les dates auxquelles vous planifiez vos congés, nous vous recommandons de faire correspondre le fuseau horaire de votre profil d’utilisateur ou d’utilisatrice à celui de votre planning. Pour plus d’informations, consultez les articles suivants :
>
>* [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td> <p>Pour configurer vos congés personnels, vous devez disposer des éléments suivants :</p>
        <p>Standard (pour configurer vos congés personnels)</p>
        <p>Travail ou version ultérieure (pour configurer vos congés personnels)</p> </td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td><p>Pour apporter des modifications au calendrier des congés d’un autre utilisateur, vous devez être le responsable de cet utilisateur et disposer d’un accès Modifier l’utilisateur.</p>
   <p><strong>REMARQUE :</strong> si un responsable modifie le calendrier des congés personnels d’un autre utilisateur, toutes les entrées sont affichées dans le fuseau horaire de l’utilisateur et non dans celui du responsable.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer les congés dans [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Si votre organisation se trouve dans l’expérience unifiée Adobe, cliquez sur le menu du compte **Adobe** (image de votre profil) dans le coin supérieur droit de la zone de navigation supérieure, puis cliquez sur **Profil Workfront**.
>
>![profil workfront &#x200B;](assets/aue-profile.png)

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Congés]**.
1. Sélectionnez la date souhaitée pour vos congés.

   ![Calendrier des congés](assets/personal-time-off-calendar-0925.png)

   <!--Sample image in the Production environment:
   ![Personal time off calendar](assets/personal-time-off-calendar.png)-->

1. Sélectionnez **[!UICONTROL Toute la journée]**, si vous prenez une journée entière de congés.

   Si vous prenez moins d’une journée entière de congé, ne cochez pas la case et indiquez les heures de début et de fin de votre congé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Vos congés sont désormais visibles sur l’ensemble du système [!DNL Workfront] dans les outils de gestion des ressources tels que le planificateur de ressources et l’équilibreur de charge de travail. Si du travail vous est affecté pendant cette période, une info-bulle informe l’utilisateur ou l’utilisatrice que vous avez programmé des congés.
