---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configuration des préférences de gestion des ressources
description: En tant qu'administrateur  [!DNL Adobe Workfront] , vous pouvez configurer les préférences de gestion des ressources pour votre système. Ces préférences de gestion des ressources déterminent le mode de calcul de la disponibilité ou de la capacité de l’utilisateur et de l’éditeur de texte enrichi pour les outils de planification et de planification de la ressource  [!DNL Workfront] .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 10%

---

# Configuration des préférences de [!UICONTROL gestion des ressources]

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

En tant qu&#39;administrateur [!DNL Adobe Workfront], vous pouvez configurer les préférences de [!UICONTROL gestion des ressources] pour votre système. Ces préférences déterminent le mode de calcul de l’heure de l’utilisateur ou de la disponibilité ou de la capacité de l’éditeur de texte enrichi pour les outils de planification et de planification des ressources [!DNL Workfront].

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

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Niveau d’accès administrateur système</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>.</p> <p><b>NOTE</b> :

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

+++

## Informations prises en compte lors du calcul de la capacité d’un utilisateur

Lors du calcul de la capacité d’un utilisateur, Workfront prend en compte les informations suivantes :

* Le nombre d’heures planifiées, tel que défini dans la Planification de l’utilisateur ou dans la [!UICONTROL Planification par défaut] du système Workfront
* [!UICONTROL Planning] [!UICONTROL Exceptions] (selon la [!UICONTROL Planification] utilisée, il peut s’agir des exceptions de la planification de l’utilisateur, ou de celles associées à la [!DNL Workfront] [!UICONTROL Planification par défaut])
* Intervalle de l’utilisateur
* La valeur de l’équivalent temps plein ([!UICONTROL FTE]) de l’utilisateur ou de celui du système [!DNL Workfront]. L’ [!UICONTROL éditeur de texte enrichi ] est égal à 1 lorsque l’utilisateur travaille à temps plein, comme défini dans le planning.
* La valeur de [!UICONTROL Work Time] pour l’utilisateur qui fait référence au temps que l’utilisateur passe sur le travail lié au projet. Cela ne comprend pas les temps de travail, comme les réunions et la formation. Le [!UICONTROL temps de travail] est égal à 1 lorsque l’utilisateur est disponible pour le travail pendant toute la durée indiquée par l’ [!UICONTROL EPT] ou l’horaire, ce qui signifie qu’il ne passe pas de temps sur des travaux non liés à un projet comme des réunions ou des formations.


Pour plus d’informations sur la planification et la planification des ressources dans [!DNL Workfront], voir [Prise en main de la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configuration des préférences de [!UICONTROL gestion des ressources]

>[!NOTE]
>
>Puisqu’il s’agit d’un paramètre global, cette sélection affecte tous les calculs pour l’ensemble du système, pour tous les utilisateurs, dans tous les outils de gestion des ressources.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Resource Management]**.
1. Sélectionnez l’une des méthodes suivantes pour calculer la disponibilité des utilisateurs dans [!DNL Workfront] :

   * **La planification par défaut** : [!DNL Workfront] utilise la planification par défaut du système et l’éditeur de texte enrichi individuel de l’utilisateur pour calculer les heures disponibles de l’utilisateur dans les outils de gestion des ressources.

     Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Pour plus d’informations sur la localisation de la valeur de l’ [!UICONTROL ETR] de l’utilisateur, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Workfront calcule les Heures disponibles d’un utilisateur à l’aide de la formule suivante lorsque l’administrateur Workfront choisit le [!UICONTROL Planning par défaut] :


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Par exemple, si la planification par défaut est de 40 heures par semaine, l’éditeur de texte enrichi du profil de l’utilisateur est de 0,5, l’utilisateur dispose d’une heure de congé par jour et que le [!UICONTROL temps de travail] du profil de l’utilisateur est de 0,5, l’utilisateur peut travailler sur le projet pendant 9,5 heures par semaine.
     >
     >Si l’utilisateur dispose d’une heure de congé un jour, ses Heures disponibles sont calculées comme suit :
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

   * **The User&#39;s Schedule** : [!DNL Workfront] utilise la planification de l’utilisateur ainsi que la [!UICONTROL planification par défaut] du système pour calculer la valeur [!UICONTROL FTE] disponible de l’utilisateur dans les outils de gestion des ressources. Les Heures disponibles sont calculées uniquement selon le planning de l&#39;utilisateur. La valeur de l’ [!UICONTROL FTE] de l’utilisateur est ignorée. Il s’agit du paramètre par défaut.

     Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Pour plus d’informations sur la [!UICONTROL planification] d’un utilisateur, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Si l’utilisateur n’est pas associé à une planification, les Heures disponibles pour l’utilisateur sont calculées à l’aide uniquement de la [!UICONTROL Planification par défaut].

     Les heures disponibles pour l&#39;utilisateur sont calculées selon la formule suivante :


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     Le [!UICONTROL FTE] disponible pour l’utilisateur est calculé à l’aide de la formule suivante :


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Par exemple, si la [!UICONTROL planification par défaut] est de 40 heures par semaine, la planification de l’utilisateur est de 30 heures par semaine et le [!UICONTROL temps de travail] de l’utilisateur est de 0,5, l’ [!UICONTROL ETR] de l’utilisateur est de 0,35.
     >
     >Si l’utilisateur dispose de 2 heures de temps libre un jour, son [!UICONTROL FTE] hebdomadaire disponible sera calculé comme suit :
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
