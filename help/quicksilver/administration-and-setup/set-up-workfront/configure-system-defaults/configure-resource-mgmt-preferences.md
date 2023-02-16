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
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Configurer [!UICONTROL Gestion des ressources] préférences

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu .</span>

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

## Informations prises en compte lors du calcul de la capacité d’un utilisateur

Lors du calcul de la capacité d’un utilisateur, Workfront prend en compte les informations suivantes :

* Le nombre d’heures planifiées, tel que défini dans la Planification de l’utilisateur ou dans le [!UICONTROL Planification par défaut]
* [!UICONTROL Planification] [!UICONTROL Exceptions] (selon le [!UICONTROL Planification] est utilisée, il peut s’agir des exceptions du planning de l’utilisateur ou de celles associées à la variable [!DNL Workfront] [!UICONTROL Planification par défaut])
* Délai d’interruption de l’utilisateur
* Valeur de l’équivalent temps plein ([!UICONTROL FTE]) de l’utilisateur ou de celle de la fonction [!DNL Workfront] système. Le [!UICONTROL FTE] est égal à 1 lorsque l’utilisateur travaille à temps plein, comme défini dans le planning.
* <span class="preview">La valeur de [!UICONTROL Temps de travail] pour l’utilisateur qui fait référence au temps passé par l’utilisateur sur le travail lié au projet. Cela ne comprend pas les temps de travail, comme les réunions et la formation. Le [!UICONTROL Temps de travail] est égal à 1 lorsque l’utilisateur est disponible pour le travail pendant toute la durée indiquée par la variable [!UICONTROL FTE] ou le planning, ce qui signifie qu&#39;ils ne passent pas de temps sur des travaux non liés au projet comme des réunions ou des formations.</span>

Pour plus d’informations sur la planification et la planification des ressources dans [!DNL Workfront], voir [Prise en main de la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configurer [!UICONTROL Gestion des ressources] préférences

>[!NOTE]
>
>Puisqu’il s’agit d’un paramètre global, cette sélection affecte tous les calculs pour l’ensemble du système, pour tous les utilisateurs, dans tous les outils de gestion des ressources.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Cliquez sur **[!UICONTROL Gestion des ressources]**.
1. Sélectionnez l’une des méthodes suivantes pour calculer la disponibilité des utilisateurs dans [!DNL Workfront]:

   * **Planification par défaut**: [!DNL Workfront] utilise le planning par défaut du système et l’éditeur de texte enrichi de l’utilisateur pour calculer les heures disponibles de l’utilisateur dans les outils de gestion des ressources.

      Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Pour plus d’informations sur la localisation de la valeur de la variable [!UICONTROL FTE], voir  [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcule les Heures disponibles d’un utilisateur à l’aide de la formule suivante lorsque l’administrateur de Workfront choisit La [!UICONTROL Planification par défaut]:


      Dans l’environnement de production :

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

      <div class="preview">

      Dans l’environnement Aperçu :

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >Par exemple, si la planification par défaut est de 40 heures par semaine, l’éditeur de texte enrichi du profil de l’utilisateur est de 0,5, l’utilisateur dispose d’une heure de congé d’un jour et la variable [!UICONTROL Temps de travail] dans le profil de l’utilisateur est 0,5, l’utilisateur est disponible pour un travail réel de projet pendant 9,5 heures par semaine.
      >
      >Si l’utilisateur dispose d’une heure de congé un jour, ses Heures disponibles sont calculées comme suit :
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>


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

      Dans l’environnement de production :


      Les heures disponibles pour l&#39;utilisateur sont calculées selon la formule suivante :

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```

      Le [!UICONTROL FTE] pour l’utilisateur est calculé par la formule suivante :

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
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

      <div class="preview">

      Dans l’environnement Aperçu :

      Les heures disponibles pour l&#39;utilisateur sont calculées selon la formule suivante :

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      Le [!UICONTROL FTE] pour l’utilisateur est calculé par la formule suivante :

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Par exemple, si la variable [!UICONTROL Planification par défaut] est de 40 heures par semaine, le planning de l’utilisateur est de 30 heures par semaine et le [!UICONTROL Temps de travail] est 0,5 ; [!UICONTROL FTE] de l’utilisateur est 0,35.
      >
      >Si l’utilisateur dispose de 2 heures de pause un jour, son hebdomadaire disponible [!UICONTROL FTE] sera calculé comme suit :
      >
      >
      ```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```

      </div>

1. Cliquer sur **[!UICONTROL Enregistrer]**.
