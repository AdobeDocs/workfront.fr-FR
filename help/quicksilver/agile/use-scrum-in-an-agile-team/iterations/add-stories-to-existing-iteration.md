---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Ajouter des histoires à une itération existante
description: Vous pouvez ajouter des histoires à une itération de plusieurs façons.
author: Jenny
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 81%

---

# Ajouter des histoires à une itération existante

Vous pouvez ajouter des histoires à une itération de l’une des manières suivantes :

* À partir de la liste d’attente après la création de l’itération, comme décrit dans la section [Déplacer des histoires de la liste d’attente vers une itération ou [!UICONTROL Kanban] panorama](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) dans [Gérer la liste d’attente Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Dans la page [!UICONTROL Détails] de la tâche ou du problème individuel.
* À partir d’une tâche ou d’une liste de problèmes
* À partir d’un rapport
* À partir d’un tableau de bord

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Travail ou supérieur</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Gérer l’accès au projet sur lequel porte l’histoire </td> 
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprendre l’impact de l’ajout d’histoires sur les dates des tâches

Par défaut, lorsque vous ajoutez une tâche existante à une itération, les [!UICONTROL Date de début prévue] et [!UICONTROL Date d’achèvement prévue] de la tâche sont définies comme suit :

### [!UICONTROL Date de début prévue] de la tâche

* La tâche utilise la date de début de l’itération lorsque :

   * Le projet n’a pas de [!UICONTROL Date de début prévue] définie.
   * La [!UICONTROL Date de début prévue] du projet est *antérieure* ou *égale* à la date de début de l’itération.

* La tâche utilise la [!UICONTROL Date de début prévue] du projet lorsque :

   * La [!UICONTROL Date de début prévue] du projet est *postérieure* à la date de début de l’itération.

### [!UICONTROL Date d’achèvement prévue] de la tâche

* La tâche utilise la date de fin de l’itération lorsque :

   * Le projet n’a pas de [!UICONTROL Date d’achèvement prévue] définie.
   * La [!UICONTROL Date de début prévue] du projet est *antérieure ou égale* à la date de début de l’itération ou la [!UICONTROL Date d’achèvement prévue] du projet est *antérieure ou égale* à la date de fin de l’itération.

* La tâche utilise la [!UICONTROL Date d’achèvement prévue] du projet lorsque :

   * La [!UICONTROL Date de début prévue] du projet est *postérieure* à la date de début de l’itération et la [!UICONTROL Date d’achèvement prévue] du projet est *postérieure* à la date de fin de l’itération.

Vous pouvez configurer des équipes Scrum individuelles de manière à utiliser les dates du projet par défaut plutôt que les dates d’itération. Pour plus d’informations, consultez la section [Configurer l’application des dates lors de l’ajout d’éléments de travail à une itération](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) de l’article [Configurer Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Ajouter une histoire à une itération existante

Vous pouvez ajouter une tâche ou un problème à n’importe quelle itération si vous disposez de la gestion de l’accès au projet. Gardez les éléments suivants à l’esprit lorsque vous déplacez une tâche ou un problème vers une itération :

* Si vous ajoutez plusieurs équipes, la tâche ou le problème ne peut s’afficher que sur l’itération d’une équipe. Il s’agit de l’itération choisie à l’étape 3 ci-dessous.
* Si la tâche ou le problème est assigné à une équipe agile et déplacé vers l’itération d’une autre équipe, l’affectation de l’équipe ne change pas.
* Si la tâche ou le problème n’est pas assigné à une équipe, la tâche ou le problème est assigné à l’équipe propriétaire de l’itération.
* Vous ne pouvez pas ajouter de tâches parents à l’itération. Si vous ajoutez des tâches enfants, la tâche parent apparaît sur le panorama Scrum sous la forme d’un couloir.

>[!IMPORTANT]
>
>Une fois que la tâche est déplacée vers l’itération, vous ne pouvez pas mettre à jour le [!UICONTROL Type de durée] ou la [!UICONTROL Contrainte de tâche]. Le [!UICONTROL Type de durée] est défini sur [!UICONTROL Simple] et la [!UICONTROL Contrainte de tâche] est définie sur [!UICONTROL Dates fixes] afin que la chronologie de la tâche reste cohérente avec la chronologie de l’itération.

1. Ouvrez la tâche ou l’événement à ajouter à une itération.
Ou
Accédez au projet, rapport ou tableau de bord contenant la tâche ou l’événement à ajouter à une itération. Sélectionnez ensuite une ou plusieurs tâches ou un ou plusieurs événements.

1. Cliquez sur **[!UICONTROL Plus]** ![Icône Plus](assets/more-icon.png) > **[!UICONTROL Ajouter à l’itération]**.
Vous ne pouvez pas attribuer des tâches ou des problèmes affectés à des équipes non agiles.

1. Dans la zone **[!UICONTROL Ajouter à]**, commencez à saisir le nom de l’itération, puis sélectionnez-la lorsqu’elle apparaît dans la liste.

   >[!NOTE]
   >
   >Vous pouvez déplacer une histoire d’une itération existante vers une nouvelle itération.

1. Cliquez sur **[!UICONTROL Ajouter]**.
