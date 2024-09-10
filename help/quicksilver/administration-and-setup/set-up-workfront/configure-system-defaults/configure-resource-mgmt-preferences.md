---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configuration des préférences de gestion des ressources
description: En tant que personne chargée de l’administration  [!DNL Adobe Workfront] , vous pouvez configurer les préférences de gestion des ressources pour votre système. Ces préférences de gestion des ressources déterminent la manière dont la disponibilité ou la capacité pour les utilisateurs et utilisatrices et l’éditeur de texte enrichi sont calculés pour les outils  [!DNL Workfront]  de planification des ressources.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 99%

---

# Configurer les préférences de [!UICONTROL Gestion des ressources]

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

En tant que personne chargée de l’administration [!DNL Adobe Workfront], vous pouvez configurer les préférences de [!UICONTROL Gestion des ressources] pour votre système. Ces préférences déterminent le mode de calcul de la disponibilité ou de la capacité des heures des utilisateurs et utilitrices ou de l’éditeur de texte enrichi pour les outils [!DNL Workfront] de planification des ressources.

## Conditions d’accès

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informations prises en compte lors du calcul de la capacité d’un utilisateur ou d’une utilisatrice

Lors du calcul de la capacité d’un utilisateur ou d’une utilisatrice, Workfront prend en compte les informations suivantes :

* Nombre d’heures planifiées, tel que défini dans le planning de l’utilisateur ou de l’utilisatrice dans le [!UICONTROL Planning par défaut] du système Workfront.
* [!UICONTROL Exceptions] [!UICONTROL d’horaire] (selon le [!UICONTROL Planning] utilisé, il peut s’agir des exceptions d’horaire de l’utilisateur ou de l’utilisatrice ou de celles associées au [!UICONTROL Planning par défaut] [!DNL Workfront]).
* Congés de l’utilisateur ou de l’utilisatrice
* Valeur de l’équivalent temps complet ([!UICONTROL Équivalent temps complet]) de l’utilisateur ou de l’utilisatrice ou du système [!DNL Workfront]. L’[!UICONTROL équivalent temps complet] est égal à 1 lorsque l’utilisateur ou l’utilisatrice travaille à temps complet, comme défini dans le planning.
* La valeur de [!UICONTROL Temps de travail] pour l’utilisateur ou l’utilisatrice qui fait référence au temps passé par l’utilisateur ou l’utilisatrice sur le travail lié au projet. Cela ne comprend pas la durée supplémentaire, comme les réunions et la formation. Le [!UICONTROL Temps de travail] est égal à 1 lorsque la personne est disponible pour le travail pendant toute la durée indiquée par l’[!UICONTROL équivalent temps complet] ou le planning, ce qui signifie qu’elle ne passe pas de temps sur des travaux non liés au projet comme des réunions ou des formations.


Pour plus d’informations sur le planning et la planification des ressources dans [!DNL Workfront], voir [Commencer avec la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configurer les préférence de [!UICONTROL Gestion des ressources]

>[!NOTE]
>
>Puisqu’il s’agit d’un paramètre global, cette sélection affecte tous les calculs pour l’ensemble du système, pour tous les utilisateurs et utilisatrices, dans tous les outils de gestion des ressources.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Gestion des ressources]**.
1. Sélectionnez l’une des méthodes suivantes pour calculer la disponibilité des utilisateurs et utilisatrices dans [!DNL Workfront] :

   * **Planning par défaut** : [!DNL Workfront] utilise le planning par défaut du système et l’éditeur de texte enrichi individuel de l’utilisateur ou de l’utilisatrice pour calculer les heures disponibles de l’utilisateur ou de l’utilisatrice dans les outils de gestion des ressources.

     Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Pour plus d’informations sur la localisation de la valeur de l’[!UICONTROL équivalent temps complet] de l’utilisateur ou de l’utilisatrice, voir [Modifier un profil d’utilisateur ou d’utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Workfront calcule les heures disponibles d’un utilisateur ou d’une utilisatrice à l’aide de la formule suivante lorsque l’administrateur ou l’administratrice Workfront choisit le [!UICONTROL Planning par défaut] :


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Par exemple, si le planning par défaut est de 40 heures par semaine, l’équivalent temps complet du profil de l’utilisateur ou de l’utilisatrice est de 0,5, l’utilisateur ou l’utilisatrice dispose d’une heure de congé d’un jour et le [!UICONTROL Temps de travail] dans le profil de l’utilisateur ou de l’utilisatrice est 0,5, l’utilisateur ou l’utilisatrice est disponible pour un travail réel sur le projet pendant 9,5 heures par semaine.
     >
     >Si l’utilisateur ou l’utilisatrice dispose d’une heure de congé un jour, ses heures disponibles sont calculées comme suit :
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



     <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **Planning de l’utilisateur ou de l’utilisatrice** : [!DNL Workfront] utilise le planning de l’utilisateur ou de l’utilisatrice ainsi que le [!UICONTROL Planning par défaut] du système pour calculer la valeur de l’[!UICONTROL équivalent temps complet] disponible de l’utilisateur ou de l’utilisatrice dans les outils de gestion des ressources. Les heures disponibles sont calculées uniquement selon le planning de l’utilisateur ou de l’utilisatrice. La valeur de l’[!UICONTROL équivalent temps complet] de l’utilisateur ou de l’utilisatrice est ignorée. Il s’agit du paramètre par défaut.

     Pour plus d’informations sur les plannings, voir [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Pour plus d’informations sur le [!UICONTROL Planning] de l’utilisateur ou de l’utilisatrice, voir [Modifier un profil d’utilisateur ou d’utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Si la personne n’est pas associé à un planning, les heures disponibles pour la personne sont calculées uniquement à l’aide du [!UICONTROL Planning par défaut].

     Les heures disponibles pour l’utilisateur ou l’utilisatrice sont calculées selon la formule suivante :


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     L’[!UICONTROL équivalent temps complet] pour l’utilisateur ou l’utilisatrice est calculé par la formule suivante :


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Par exemple, si le [!UICONTROL Planning par défaut] est de 40 heures par semaine, le planning de l’utilisateur ou de l’utilisatrice est de 30 heures par semaine et le [!UICONTROL Temps de travail] de l’utilisateur ou de l’utilisatrice est 0,5, l’[!UICONTROL équivalent temps complet] de l’utilisateur ou de l’utilisatrice est 0,35.
     >
     >Si l’utilisateur ou l’utilisatrice dispose de 2 heures de pause un jour, son [!UICONTROL équivalent temps complet] hebdomadaire disponible sera calculé comme suit :
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. Cliquer sur **[!UICONTROL Enregistrer]**.
