---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interactions entre la date de validation et la date d’achèvement planifiée
description: Les dates de fin planifiée et de validation indiquent le moment où la tâche doit être terminée. Mais elles diffèrent en fonction de qui définit chaque date.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 1%

---

# Interactions entre la date de validation et la date d’achèvement planifiée

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Les dates de fin planifiée et de validation indiquent le moment où la tâche doit être terminée. Mais elles diffèrent en fonction de qui définit chaque date.

## Présentation de la date de validation et de la date d’achèvement planifiée

Les dates d’achèvement et de validation prévues existent pour les tâches et les problèmes.

Le tableau suivant contient des informations sur la différence entre les dates de validation et d’achèvement planifié :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Date d'engagement</td> 
   <td> <p>La date de validation est la date à laquelle la personne affectée à une tâche ou à une émission estime manuellement qu’elle aura terminé la tâche ou la publication.</p> <p>Pour plus d’informations sur les dates de validation, voir <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Présentation de la date de validation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Date d'achèvement prévue</td> 
   <td> <p>La date d’achèvement planifiée indique le moment où le propriétaire du projet s’attend à ce que la tâche ou le problème soit terminé. Il peut être soit défini manuellement par le propriétaire du projet, soit par toute personne disposant des autorisations Manage (Gérer) sur la tâche ou le problème, soit il peut être calculé automatiquement par Adobe Workfront.</p> <p>Pour plus d’informations sur les dates d’achèvement prévues, voir <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Présentation de la date d’achèvement planifiée de la tâche</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interactions entre la date de validation et la date d’achèvement planifiée

Lorsque le propriétaire du projet crée et affecte une tâche ou un problème, la tâche ou le problème aura les éléments suivants :

* Date d’achèvement prévue
* Pas de date d&#39;engagement

La personne désignée qui travaille sur la tâche ou le problème peut mettre à jour manuellement la date de validation ou la mettre automatiquement à jour en acceptant de travailler dessus. Il s’agit d’une manière visuelle d’indiquer au propriétaire du projet quand il serait réaliste pour lui d’effectuer la tâche ou le problème.

>[!TIP]
>
>Seul le cessionnaire peut mettre à jour la date de validation d’une tâche ou d’un problème.

La personne désignée qui modifie la date de validation ne modifie pas automatiquement la date d’achèvement planifiée. L’inverse est également vrai : la modification de la date d’achèvement planifiée ne modifie pas la date de validation.

Lorsque la date de validation est redéfinie sur une date postérieure à la date d’achèvement prévue, le propriétaire du projet est informé que cette modification s’est produite et qu’elle peut avoir une incidence sur la chronologie du projet, si le propriétaire du projet utilise l’expérience de commentaire héritée. Cette fonctionnalité n’est pas prise en charge dans la nouvelle expérience de commentaire. Pour plus d’informations, voir [Nouvelle expérience de commentaire](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

Si la date de validation proposée par la personne désignée est acceptable pour le propriétaire du projet, il doit mettre à jour manuellement la date d’achèvement planifiée de la tâche ou du problème. Pour plus d’informations, voir les articles suivants :

* [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [Mise à jour des dates de validation pour les tâches et les problèmes](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
