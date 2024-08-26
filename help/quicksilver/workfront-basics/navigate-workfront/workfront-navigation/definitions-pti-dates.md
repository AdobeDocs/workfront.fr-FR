---
content-type: reference
navigation-topic: workfront-navigation
title: Vue d’ensemble des dates de projet, de tâche et de problèmes dans  [!DNL Workfront]
description: Cet article fournit des définitions des dates les plus courantes associées aux projets, aux tâches et aux problèmes dans  [!DNL Adobe Workfront].
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 6f1f669f7e2235637864a92a40aadbfb19b4310b
workflow-type: tm+mt
source-wordcount: '2301'
ht-degree: 51%

---

# Vue d’ensemble des dates du projet, de la tâche et du problème dans [!DNL Workfront]

<!-- Audited: 05/2024 -->

<!--consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc-->

<!-- there are dates below that need definition - ask Product-->

Cet article fournit des définitions des dates les plus courantes associées aux projets, aux tâches et aux problèmes dans . [!DNL Adobe Workfront] Les images incluses ici sont des exemples de l’affichage des dates dans Workfront et ne sont pas exhaustives. D’autres zones affichent les dates. Toutes les dates sont également visibles dans les rapports et les listes de projets, de tâches et de problèmes.

Pour plus d’informations sur les rapports et les listes, voir les articles suivants :

* [Commencer avec les listes dans  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [Prise en main des rapports](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

Pour plus d’informations sur les champs de projet, de tâche et de problème, consultez le [Glossaire de [!DNL Adobe Workfront] terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).


## [!UICONTROL Date de début effective]

La date de début effective est la date à laquelle un utilisateur ou une utilisatrice commence réellement à travailler sur un projet, une tâche ou un problème.  Le champ [!UICONTROL Date de début effective] est vide lors de la création du projet, de la tâche ou du problème.

Vous pouvez indiquer manuellement quand le travail a commencé sur une tâche ou un problème, ou la date de début effective se remplit automatiquement lorsque le statut de la tâche ou du problème passe de Nouveau à En cours ou Terminé.  La [!UICONTROL date de début effective] d’un projet coïncide avec la date de début de la première tâche du projet.

>[!TIP]
>
>La [!UICONTROL date de début effective] peut ne pas correspondre à la [!UICONTROL date de début prévue] d’un projet, d’une tâche ou d’un problème, car l’utilisateur ou l’utilisatrice peut commencer le travail plus tard ou plus tôt que la date prévue.

Pour plus d’informations, voir [Vue d’ensemble de la [!UICONTROL date de début effective]](../../../manage-work/projects/planning-a-project/project-actual-start-date.md) du projet.

>[!NOTE]
>
>La tâche Il faut commencer le ou les contraintes Dates fixes affectent la date de début prévue d’une tâche, et non la date de début effective.  Cette opération met à jour la date de début prévue à la date que vous avez spécifiée.  La [!UICONTROL date de début effective] est mise à jour indépendamment de la [!UICONTROL date de début prévue], comme décrit ci-dessus.

![](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL Date d’achèvement effective]

La [!UICONTROL date d’achèvement effective] est la date à laquelle un utilisateur ou une utilisatrice termine réellement un projet, une tâche ou un problème. La zone [!UICONTROL Date d’achèvement effective] est vide lors de la création du projet, de la tâche ou du problème.

Vous pouvez indiquer manuellement quand une tâche ou un problème se termine, ou la [!UICONTROL date d’achèvement effective] se remplit automatiquement lorsque l’une des situations suivantes se produit :

* Le statut du projet, de la tâche ou du problème passe à [!UICONTROL Terminé], [!UICONTROL Fermé], ou [!UICONTROL Résolu].
* Le pourcentage terminé de la tâche ou du projet est de 100 %.

La [!UICONTROL date d’achèvement effective] d’un projet correspond à la date à laquelle vous avez effectué la dernière tâche sur le projet.

>[!TIP]
>
>La [!UICONTROL date d’achèvement effective] peut ne pas correspondre à la [!UICONTROL date d’achèvement prévue].

Pour plus d’informations, voir [Vue d’ensemble de la [!UICONTROL date d’achèvement effective]](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md) du projet.

![](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## Date d&#39;achèvement du chemin d&#39;approbation

La date d’achèvement du chemin d’approbation est la date à laquelle l’approbation d’un projet, d’une tâche ou d’un problème a été accordée et que l’état de l’élément a été modifié.

La date d’achèvement du chemin d’approbation est visible dans les listes et rapports des projets, tâches et problèmes.

## Date de début du chemin d&#39;approbation

La date de début du chemin d’approbation est la date à laquelle le projet, la tâche ou le statut du problème a été remplacé par &quot;En attente d’approbation&quot; et la demande d’approbation de projet a été envoyée aux approbateurs.

La Date de début du chemin d’approbation est visible dans les listes et rapports des projets, tâches et problèmes.

<!--## Auto Closure Date -->

## Date d’achèvement budgétée

Il s’agit d’un champ obsolète pour les projets. Toute information que ce champ peut afficher dans une liste ou un rapport est liée à une fonctionnalité supprimée par Workfront. Ce champ ne peut pas être mis à jour.

Le champ est visible dans les listes et rapports du projet.

## Date de début budgétée

Il s’agit d’un champ obsolète pour les projets. Toutes les informations que ce champ peut afficher sont liées à une fonctionnalité que Workfront a supprimée. Ce champ ne peut pas être mis à jour.

Le champ est visible dans les listes et rapports du projet.

## [!UICONTROL Date d’engagement]

La date d’engagement est la date à laquelle une personne affectée à une tâche ou à un problème s’engage à terminer la tâche ou le problème.  Elle est différente de la [!UICONTROL date d’achèvement prévue], car il s’agit d’une estimation plus réaliste de la date d’achèvement donnée uniquement par la personne en charge du travail. Pour plus d’informations, voir Vue d’ensemble de la [[!UICONTROL date d’engagement]](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

>[!NOTE]
>
>La modification de la date d’engagement affecte la date d’achèvement prévisionnelle mais pas la date d’achèvement prévue d’une tâche ou d’un problème.  La ou le gestionnaire de projet peut utiliser les modifications apportées par une personne assignée à la [!UICONTROL date d’engagement] pour mettre à jour la [!UICONTROL date d’achèvement prévue] d’une tâche ou d’un problème.

<!--## Completion Pending Date-->

## Date de contrainte

Si vous utilisez une contrainte de tâche liée à une date spécifique, cette date spécifique devient la date de contrainte de la tâche.

Les contraintes de tâche suivantes mettent à jour le champ Date de contrainte :

* Il Faut Commencer Le
* Il Faut Finir Le
* Commencer Au Plus Tard
* Commencer Au Plus Tôt

>[!TIP]
>
>Une tâche avec une contrainte de dates fixes n’a pas de date de contrainte.
>

La Date de contrainte est visible dans une liste de tâches ou un rapport.

## Date d’entrée de l’événement converti

Date à laquelle le problème qui a été converti dans le projet ou la tâche a été créé.

La Date d’entrée du problème converti est visible dans les listes et rapports de projets et de tâches.

## Date d’échéance

Date à laquelle une tâche ou un problème doit être terminé. La date d’échéance d’une tâche ou d’une émission est la même que la date d’achèvement planifiée.

La tâche et le problème Échéance sont visibles dans les listes et rapports de tâches et de problèmes.

Pour plus d’informations, reportez-vous à la section [Date d’achèvement planifiée](#planned-completion-date) de cet article.

## Dû le

Date à laquelle le projet doit se terminer. La date d’échéance d’un projet est identique à la date d’achèvement prévue du projet.

La date d’échéance du projet est visible dans les listes et les rapports du projet.

Pour plus d’informations, reportez-vous à la section [Date d’achèvement planifiée](#planned-completion-date) de cet article.

## [!UICONTROL Date d’entrée]

[!UICONTROL Date d’entrée] est la date de création d’un projet, d’une tâche ou d’un problème dans [!DNL Workfront].

La date d’entrée n’a pas d’effet sur le calendrier des projets, des tâches ou des problèmes, mais elle est importante pour le suivi et la création de rapports.  [!DNL Workfront] génère automatiquement la [!UICONTROL date d’entrée] lors de la création de l’objet et vous ne pouvez pas la modifier manuellement.

![](assets/entry-date-in-task-details-highlighted-nwe.png)

## Échéance estimée

La tâche et la date d’échéance estimée du projet indiquent une date plus réaliste du moment où le projet ou la tâche doit se terminer.

Les dates estimées correspondent davantage à la réalité du projet et de la tâche, dans la mesure où elles prennent en compte ce qui influence l’achèvement réel du projet ou de la tâche. Les dates d’échéance estimées sont similaires aux dates d’achèvement prévues.

Pour plus d’informations, voir [Présentation des dates prévues et estimées](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

Les dates estimées du projet et de la tâche sont visibles dans les listes et rapports de projets et de tâches.

## Date de début estimée

La date de début estimée de la tâche et du projet indique une date plus réaliste de début du projet ou de la tâche.

Les dates estimées sont plus en phase avec la réalité du projet et de la tâche, car elles prennent en compte ce qui influence le début réel du projet ou de la tâche. Les dates de début estimées sont similaires aux dates de début projetées.

Pour plus d’informations, voir [Présentation des dates prévues et estimées](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

Les dates de début estimées du projet et de la tâche sont visibles dans les listes et rapports de projets et de tâches.

<!--## Exchange Rate Date-->

## Date de fin fixée

Le demandeur ou le propriétaire du projet identifie la date de fin fixe d’un projet lors de l’exécution de l’analyse de cas. Il s’agit de la date à laquelle il recommande que le projet soit terminé.

Il s’agit d’une estimation manuelle qui ne prend en compte aucune progression réelle des tâches sur le projet.

La date de fin fixe d’un projet est visible dans la section Analyse de cas du projet, ainsi que dans les listes et les rapports de projet.

![](assets/fixed-end-date-business-case-highlight.png)

## Date de début fixée

Le demandeur ou le propriétaire du projet identifie la date de début fixe d’un projet lors de l’exécution de l’analyse de cas. Il s’agit de la date à laquelle il est recommandé que le projet commence.

Il s’agit d’une estimation manuelle qui ne prend en compte aucune progression réelle des tâches sur le projet.

La date de début fixe d’un projet est visible dans la section Analyse de cas du projet, ainsi que dans les listes et les rapports de projet.

![](assets/fixed-start-date-business-case-highlight.png)

## Date de remise

Date à laquelle une tâche devient disponible pour le travail. Cela signifie que toutes les contraintes, validations et dépendances ont été réalisées et que les utilisateurs peuvent commencer à travailler sur la tâche.

La date de remise est un calcul qui ne peut pas être définie manuellement.

Pour plus d’informations sur la date de passation, voir [Présentation de la date de passation des tâches](/help/quicksilver/manage-work/tasks/task-information/handoff-task-date.md).

La Date de remise d’une tâche est visible dans les listes de tâches et les rapports.

## Dernière mise à jour financière

Date à laquelle l’une des informations financières sur un projet a été mise à jour. Cela inclut la mise à jour des champs financiers dans la section Finance ou Analyse de cas du projet.

La Date de la dernière mise à jour financière est visible dans les listes et les rapports de projet.

## Date de dernière mise à jour

Date de la dernière mise à jour du projet, de la tâche ou du problème. Une mise à jour est considérée comme toute modification qui déclenche l’enregistrement d’un projet, d’une tâche ou d’un problème. Cela inclut les modifications de l’état, de la condition, de la chronologie, des finances ou de tout autre champ.

La date de la dernière mise à jour est visible dans les listes et rapports des projets, des tâches et des problèmes.

## [!UICONTROL Date d’entrée des heures]

Lorsque vous consignez des heures pour des projets, des tâches et des problèmes afin d’indiquer le temps réel (en heures) que vous avez passé à travailler sur le projet, la tâche ou le problème, le temps que vous consignez devient les [!UICONTROL heures effectives] du projet, de la tâche ou du problème.

La date pour laquelle vous enregistrez l’heure est le champ [!UICONTROL Date d’entrée de l’heure] sur l’entrée d’heure.

La date d’entrée de l’heure est visible dans les listes d’heures et les rapports.

>[!TIP]
>
>La [!UICONTROL date d’entrée] d’une heure est différente de la [!UICONTROL date d’entrée] d’un autre objet Workfront, dans la mesure où il ne s’agit pas de la date de création du journal d’heure, mais plutôt de la date à laquelle vous souhaitez associer les heures.
>
>Par exemple, vous pouvez consigner les heures d’une tâche le 5 septembre, mais associer les heures au 1er septembre. La date d’entrée de l’heure est le 1er septembre.

Pour plus d’informations sur la façon de consigner l’heure dans Workfront, voir [Temps du journal](../../../timesheets/create-and-manage-timesheets/log-time.md).

>[!TIP]
>
>Nous recommandons de consigner le temps passé sur des tâches et des problèmes de travail, plutôt que sur des tâches ou des projets parent. Le temps consigné sur les tâches de travail est répercuté sur les tâches parent et le projet en tant qu’Heures effectives pour les tâches parent et le projet.  Le temps consigné sur les problèmes est répercuté sur le projet en tant qu’[!UICONTROL Heures effectives] pour le projet.

## [!UICONTROL Date d’achèvement prévue]

La [!UICONTROL date d’achèvement prévue] ou la [!UICONTROL date d’échéance] est la date à laquelle il est prévu qu’un projet, une tâche ou un problème soit terminé(e).

En fonction de la contrainte de tâche, il se peut que vous ne puissiez pas modifier la date d’achèvement prévue d’une tâche.  En fonction du [!UICONTROL mode de planification] du projet, il se peut que vous ne puissiez pas modifier la [!UICONTROL date d’achèvement prévue] d’un projet.

La [!UICONTROL date d’achèvement prévue] s’affiche comme la date d’échéance dans certaines zones de [!DNL Workfront].

Pour plus d’informations, consultez les articles suivants :

* [Vue d’ensemble de la [!UICONTROL date d’achèvement prévue] de la tâche](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Définir la [!UICONTROL date d’achèvement prévue] du projet](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Vue d’ensemble de la [!UICONTROL date d’achèvement prévue] du problème](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

![](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)

![](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)


## Alignement de date planifié

Il s’agit d’un indicateur automatique selon lequel Workfront attribue des projets, des tâches et des problèmes à afficher lorsqu’un élément sera terminé par rapport à sa date d’achèvement planifiée.

Voici les valeurs possibles pour l’indicateur d’alignement de la date planifiée :

* Sera terminé à la date d&#39;achèvement prévisionnelle
* Sera terminé avant la date d&#39;achèvement prévisionnelle
* Sera terminé après la date d&#39;achèvement prévisionnelle

L’alignement des dates prévues est visible dans les listes et rapports des projets, des tâches et des problèmes.

## [!UICONTROL Date de début prévue]

La [!UICONTROL date de début prévue] est la date à laquelle un projet, une tâche ou un problème doit commencer.

En fonction de la contrainte de tâche, il se peut que vous ne puissiez pas modifier la date de début prévue d’une tâche.  En fonction du [!UICONTROL mode de planification] du projet, il se peut que vous ne puissiez pas modifier la [!UICONTROL date de début prévue] d’un projet.

Pour plus d’informations, voir [Vue d’ensemble de la [!UICONTROL date de début prévue du projet]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

![](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL Date d’achèvement prévisionnelle]

La date d’achèvement prévisionnelle est un indicateur calculé en temps réel de la date d’achèvement du projet, de la tâche ou du problème.  Lorsque le projet, la tâche ou le problème est marqué comme étant terminé, la [!UICONTROL date d’achèvement prévisionnelle] devient la [!UICONTROL date d’achèvement effective].

Si tout se passe bien et comme prévu, la date d’achèvement prévisionnelle devrait correspondre à la date d’achèvement prévue.  Sinon, en raison des retards des tâches précédentes, la [!UICONTROL date d’achèvement prévisionnelle] peut être différente de la [!UICONTROL date d’achèvement prévue].

Pour plus d’informations, voir [Vue d’ensemble de la [!UICONTROL date d’achèvement prévisionnelle] pour les projets, les tâches et les problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

![](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL Date de début prévisionnelle]

La date de début prévisionnelle est une date en temps réel à laquelle le projet, la tâche ou le problème est lancé et qui tient compte de tous les retards.  Il s’agit d’une date de début plus précise pour le projet, la tâche ou le problème que la date de début prévue.  La [!UICONTROL date de début prévue] ne tient pas compte des retards ou des dates passées.

Lorsque vous planifiez un projet pour la première fois, la [!UICONTROL date de début prévue] et la [!UICONTROL date de début prévisionnelle] des tâches et du projet sont identiques. Comme des retards peuvent survenir ou que des tâches peuvent être achevées plus tôt, la [!UICONTROL date de début prévisionnelle] peut devenir différente de la [!UICONTROL date de début prévue].

Pour une tâche, une [!UICONTROL date de début prévisionnelle] peut également différer de sa [!UICONTROL date de début prévue] lorsque l’une de ses tâches antérieures est en retard sur le calendrier.

>[!TIP]
>
>Vous pouvez afficher la [!UICONTROL date de début prévisionnelle] d’un problème uniquement dans une liste ou un rapport.

Pour plus d’informations, voir [Vue d’ensemble de la [!UICONTROL date de début prévisionnelle]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md) du projet.

![](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

<!--## Rejection Date-->

## Date de marge

Les tâches peuvent parfois démarrer et se terminer tard sans affecter la date d’achèvement du projet.

La date du Slack affiche la date exacte à laquelle une tâche peut avoir une incidence définitive sur la date de fin du projet.

Pour plus d’informations sur la date du Slack d’une tâche, voir [Présentation de la date du Slack de la tâche](/help/quicksilver/manage-work/tasks/task-information/task-slack-date.md).

Les dates du Slack de tâches sont visibles dans les listes de tâches et les rapports.

## Démarré le

Date prévue pour le démarrage du projet. La date de début d’un projet est identique à la date de début prévue du projet.

Ce champ est visible dans les listes et les rapports de projet.

Pour plus d’informations, reportez-vous à la section [Date de début planifiée](#planned-start-date) de cet article.



