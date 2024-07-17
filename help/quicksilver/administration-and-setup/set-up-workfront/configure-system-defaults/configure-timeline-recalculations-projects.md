---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configuration de nouveaux calculs de chronologie pour les projets
description: Recalculer les chronologies permet aux gestionnaires de voir comment les forces en dehors du projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévues pour le projet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 13%

---

# Configuration de nouveaux calculs de chronologie pour les projets

Recalculer les chronologies permet aux gestionnaires de voir comment les forces en dehors du projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévues pour le projet.

En tant qu&#39;administrateur [!DNL Adobe Workfront], vous pouvez recalculer manuellement les chronologies pour tous les projets du système. Les propriétaires de projet peuvent également recalculer manuellement les échéances des projets individuels. Pour plus d’informations, voir [Recalculer les chronologies de projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Cet article décrit comment, en tant qu&#39;administrateur [!DNL Workfront], vous pouvez déterminer comment et à quel moment [!DNL Workfront] calcule automatiquement les chronologies de projet en configurant les préférences du projet dans la zone [!UICONTROL Configuration].

## Conditions d’accès

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
   <td> <p>Niveau d’accès administrateur système</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer des recalculs automatiques

En tant qu&#39;administrateur [!DNL Adobe Workfront], vous pouvez configurer lorsque [!DNL Workfront] recalcule automatiquement les chronologies du projet. [!DNL Workfront] peut recalculer les calendriers du projet chaque nuit ou lorsque la portée du projet change, ou les deux.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit ou sur l’icône [!UICONTROL **Menu principal**] ![](assets/lines-main-menu.png) dans le coin supérieur gauche de [!DNL Workfront], le cas échéant, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets].**

1. Dans la section **[!UICONTROL Chronologies]** , activez ou désactivez l’un des paramètres ci-dessous, ou les deux. Par défaut, les deux paramètres sont activés.

   * **Chaque nuit :** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcule les chronologies une fois toutes les 24 heures, la nuit, uniquement pour les projets dont l’état est [!UICONTROL Actuel] et qui ont été mis à jour au cours des trois derniers mois. Selon la charge du système et d&#39;autres facteurs, le temps de recalcul peut être retardé de plus de 24 heures.

     Dans ce cas, [!DNL Workfront] recalcule la chronologie de tous les projets dont le [!UICONTROL type de mise à jour] est [!UICONTROL Automatique] ou [!UICONTROL Automatique et Changement].

   * **Lorsque la portée d’un projet change** : pour plus d’informations sur ce qui constitue un changement de portée d’un projet, voir [Recalculer les chronologies du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     Dans ce cas, [!DNL Workfront] recalcule la chronologie de tous les projets dont le type de mise à jour est [!UICONTROL Automatique et On Change] ou [!UICONTROL On Change Only].
Pour plus d’informations sur les types de mise à jour de projet, consultez la [présentation du type de mise à jour de projet](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   La chronologie de tous les projets du système est recalculée automatiquement en fonction du type de mise à jour de chaque projet.

## Recalculer les chronologies pour l’instance [!DNL Workfront] entière

Vous pouvez exécuter le diagnostic [!UICONTROL Recalculate Timeline] pour recalculer manuellement toutes les chronologies dans le système [!DNL Workfront]. Cela permet à tous les chefs de projet de voir immédiatement l’influence des modifications externes sur les dates prévues et prévues. Pour plus d’informations, voir [Utiliser les diagnostics pour déclencher des processus automatisés](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
