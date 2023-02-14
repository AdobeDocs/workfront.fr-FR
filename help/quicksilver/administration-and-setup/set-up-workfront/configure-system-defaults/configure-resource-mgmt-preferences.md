---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configuration des préférences de gestion des ressources
description: En tant que [!DNL Adobe Workfront] administrateur, vous pouvez configurer les préférences de gestion des ressources pour votre système. Ces préférences de gestion des ressources déterminent la manière dont la disponibilité ou la capacité de l’utilisateur et l’éditeur de texte enrichi sont calculés pour la variable [!DNL Workfront] outils de planification et de planification des ressources.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Configurer [!UICONTROL Gestion des ressources] préférences

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<!--drafted for Work time field: <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

En tant que [!DNL Adobe Workfront] administrateur que vous pouvez configurer [!UICONTROL Gestion des ressources] Préférences pour votre système. Ces préférences déterminent le mode de calcul de l’heure de l’utilisateur, de la disponibilité ou de la capacité de l’éditeur de texte enrichi pour la variable [!DNL Workfront] outils de planification et de planification des ressources.

## Exigences d’accès

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

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Niveau d’accès administrateur système</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>NOTE</b>:

Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

<!--drafted for Work time field: 

## Information taken into account when calculating user's capacity

When calculating a user's capacity, Workfront takes into account the following information:

* The number of scheduled hours, as defined in either the Schedule of the user or the Workfront system's [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (depending on which [!UICONTROL Schedule] is used, it can be the exceptions of the user's schedule, or those associated with the [!DNL Workfront] [!UICONTROL Default Schedule])
* User's time off
* The value of the Full Time Equivalent ([!UICONTROL FTE]) of the user or that of the [!DNL Workfront] system. The [!UICONTROL FTE] equals 1 when the user works full time, as defined in the schedule. 

<!-drafted for Work Time field  

* <span class="preview">The value of [!UICONTROL Work Time] for the user which refers to time that the user spends on project-related work. This does not include overhead time, like meetings and training. The [!UICONTROL Work Time] equals 1 when the user is available for work the entire time as indicated by the [!UICONTROL FTE] or the schedule, which means they don't spend any time in non-project-related work like meetings or trainings.</span>

-->

Pour plus d’informations sur la planification et la planification des ressources dans [!DNL Workfront], voir [Prise en main de la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

—>

## Configurer [!UICONTROL Gestion des ressources] préférences

>[!NOTE]
>
>Puisqu’il s’agit d’un paramètre global, cette sélection affecte tous les calculs pour l’ensemble du système, pour tous les utilisateurs, dans tous les outils de gestion des ressources et pour tous les groupes de ressources.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Cliquez sur **[!UICONTROL Gestion des ressources]**.
1. Sélectionnez l’une des méthodes suivantes pour calculer la disponibilité des utilisateurs dans [!DNL Workfront]:

   * **Planification par défaut**: [!DNL Workfront] utilise le planning par défaut du système et l’éditeur de texte enrichi de l’utilisateur pour calculer les heures disponibles de l’utilisateur dans les outils de gestion des ressources.

      Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Pour plus d’informations sur la valeur de l’utilisateur [!UICONTROL FTE], voir  [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcule les Heures disponibles d’un utilisateur à l’aide de la formule suivante lorsque l’administrateur de Workfront choisit La [!UICONTROL Planification par défaut]:

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > Par exemple, si la variable [!UICONTROL Planification par défaut] est de 40 heures par semaine et la variable [!UICONTROL FTE] dans le profil de l’utilisateur est 0,5, l’utilisateur peut travailler 20 heures par semaine.
      >Si l’utilisateur dispose d’une heure de congé un jour, ses Heures disponibles sont calculées comme suit :
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
   <!--drafted for Work Time field

      <div class="preview">
      
      In the Preview environment: 

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >For example, if the Default Schedule is 40 hours a week,  the FTE in the profile of the user is 0.5, the user has 1 hour of Time off one day, and the [!UICONTROL Work Time] in the profile of the user is 0.5, the user is available for actual project work for 9.5 hours a week.
      >
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>

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

   * **Planification de l’utilisateur**: [!DNL Workfront] utilise le planning de l’utilisateur ainsi que la variable [!UICONTROL Planification par défaut] du système pour calculer la valeur Disponible [!UICONTROL FTE] valeur de l’utilisateur dans les outils de gestion des ressources. Les Heures disponibles sont calculées uniquement selon le planning de l&#39;utilisateur. La valeur de la variable [!UICONTROL FTE] de l’utilisateur est ignoré. Il s’agit du paramètre par défaut.

      Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Pour plus d’informations sur la variable [!UICONTROL Planification], voir  [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Si l’utilisateur n’est pas associé à un planning, les Heures disponibles pour l’utilisateur sont calculées à l’aide de la variable [!UICONTROL Planification par défaut].

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      Le [!UICONTROL FTE] pour l’utilisateur est calculé par la formule suivante :

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Par exemple, si la variable [!UICONTROL Planification par défaut] est de 40 heures par semaine et le planning de l’utilisateur est de 30 heures par semaine, la variable [!UICONTROL FTE] de l’utilisateur est 0,70.
      >  
      >Si l’utilisateur dispose de 2 heures de pause un jour, son hebdomadaire disponible [!UICONTROL FTE] sera calculé comme suit :
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <!--drafted for Work Time field:

      <div class="preview">

      In the Preview environment: 
      
      The Available hours for the user is calculated by the following formula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```    

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week, the schedule of the user is 30 hours a week, and the user's [!UICONTROL Work Time] is 0.5 the [!UICONTROL FTE] of the user is 0.35.
      >
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      >
      >```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```
      (************ checking this second other with Dev/ Artur - not sure where Exceptions fit in **********)

      </div>
      -->
1. Cliquer sur **[!UICONTROL Enregistrer]**.
