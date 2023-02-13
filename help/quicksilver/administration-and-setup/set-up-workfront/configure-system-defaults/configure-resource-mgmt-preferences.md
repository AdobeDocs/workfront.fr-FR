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
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---

# Configurer [!UICONTROL Gestion des ressources] préférences

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

En tant que [!DNL Adobe Workfront] administrateur que vous pouvez configurer [!UICONTROL Gestion des ressources] Préférences pour votre système. Ces préférences déterminent la manière dont la disponibilité ou la capacité de l’utilisateur et l’éditeur de texte enrichi sont calculés pour la variable [!DNL Workfront] outils de planification et de planification des ressources.

Pour plus d’informations sur la planification et la planification des ressources dans [!DNL Workfront], voir [Prise en main de la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Exigences d’accès

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
   <td> <p>Niveau d’accès administrateur système</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer [!UICONTROL Gestion des ressources] préférences

>[!NOTE]
>
>Puisqu’il s’agit d’un paramètre global, cette sélection affecte tous les calculs pour l’ensemble du système, pour tous les utilisateurs, dans tous les outils de gestion des ressources et pour tous les groupes de ressources.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Cliquez sur **[!UICONTROL Gestion des ressources]**.
1. Sélectionnez l’une des méthodes suivantes pour calculer la disponibilité des utilisateurs dans [!DNL Workfront]:

   * **Planification par défaut**: [!DNL Workfront] utilise la planification par défaut du système et l’éditeur de texte enrichi de l’utilisateur pour calculer les heures disponibles de l’utilisateur dans les outils de gestion des ressources.\

      Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Pour plus d’informations sur la valeur de l’éditeur de texte enrichi de l’utilisateur, voir  [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcule les Heures disponibles d’un utilisateur à l’aide de la formule suivante lorsque l’administrateur de Workfront choisit la Planification par défaut :

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **Exemple:**\
      Par exemple, si la planification par défaut est de 40 heures par semaine et que l’éditeur de texte enrichi du profil de l’utilisateur est de 0,5, l’utilisateur peut travailler 20 heures par semaine.

      Si l’utilisateur dispose d’une heure de congé un jour, ses Heures disponibles sont calculées comme suit :

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

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

   * **Planification de l’utilisateur**: [!DNL Workfront] utilise la planification de l’utilisateur ainsi que la planification par défaut du système pour calculer la valeur de l’éditeur de texte enrichi disponible de l’utilisateur dans les outils de gestion des ressources. Les Heures disponibles sont calculées uniquement selon le planning de l&#39;utilisateur. La valeur de l’éditeur de texte enrichi de l’utilisateur est ignorée. Il s’agit du paramètre par défaut.

      >[!NOTE]
      >
      >Si l’utilisateur n’est pas associé à une planification, les Heures disponibles pour l’utilisateur sont calculées à l’aide de la Planification par défaut.

      L’éditeur de texte enrichi disponible pour l’utilisateur est calculé à l’aide de la formule suivante :

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **Exemple :** Par exemple, si la planification par défaut est de 40 heures par semaine et que la planification de l’utilisateur est de 30 heures par semaine, l’éditeur de texte enrichi de l’utilisateur est de 0,75.

      Si l’utilisateur dispose de 2 heures de temps libre un jour, son éditeur de texte enrichi hebdomadaire sera calculé comme suit :

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. Cliquer sur **[!UICONTROL Enregistrer]**.
