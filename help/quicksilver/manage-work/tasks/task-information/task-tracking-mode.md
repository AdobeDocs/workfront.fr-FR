---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Présentation du mode de suivi des tâches
description: Vous pouvez ajuster le paramètre Mode de tracking d’une tâche lors de la création ou de la modification d’une tâche afin de contrôler comment et à quel moment les indicateurs Etat de progression d’une tâche s’affichent. Adobe Workfront affiche des indicateurs d’état de progression lorsque vous configurez certains paramètres pour le suivi de la progression des tâches.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: d2836549ee3c615201ce5f3454258e9af31efa42
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Présentation du mode de suivi des tâches

<!-- Audited: 01/2024 -->

Vous pouvez ajuster le paramètre Mode de tracking d’une tâche lors de la création ou de la modification d’une tâche afin de contrôler comment et à quel moment les indicateurs Etat de progression d’une tâche s’affichent. Adobe Workfront affiche des indicateurs d’état de progression lorsque vous configurez certains paramètres pour le suivi de la progression des tâches.

Pour plus d’informations sur l’état de progression des tâches, voir [Présentation de l’état de progression de la tâche](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Options du mode de suivi {#tracking-mode-options}

En tant que propriétaire de tâche ou chef de projet, vous pouvez sélectionner la manière dont Workfront indique l’état d’avancement de chaque tâche. Pour plus d’informations sur la façon de définir le mode de suivi sur vos tâches, voir [Définir le mode de suivi pour les tâches](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Vous pouvez sélectionner l’une des options suivantes :

* [L’utilisateur doit mettre à jour](#user-must-update)
* [Heure d’activation de l’hypothèse](#assume-on-time)
* [Ignorer les avertissements tardifs](#ignore-late-warnings)
* [Fin automatique](#auto-complete)
* [Tâche antérieure](#predecessor)

### Utilisateur doit mettre à jour {#user-must-update}

Lorsque cette option est sélectionnée, Workfront utilise les heures Pourcentage d’achèvement et Heures réelles consignées de la tâche pour déterminer l’état d’avancement de la tâche. Il s’agit de l’option par défaut.

### Supposer à l&#39;heure {#assume-on-time}

Workfront suppose qu’une tâche sera terminée à temps, quel que soit l’état d’achèvement actuel. Si la tâche ne se termine pas à temps (à la date de fin planifiée), Workfront utilise automatiquement une date de fin planifiée du jour de travail suivant. Vous devez toujours indiquer le moment où la tâche est terminée. Utilisez cette option lorsque les utilisateurs ne mettront pas régulièrement à jour leurs tâches.

### Ignorer avertissements de retard {#ignore-late-warnings}

L’état de progression d’une tâche est Activé à temps jusqu’à ce qu’elle devienne En retard. Par exemple, si vous planifiez une tâche pour une durée de 10 jours et que le jour où elle doit être terminée, la tâche affiche un pourcentage d’achèvement de 60 %, Workfront met à jour la date d’achèvement prévue en ajoutant quatre jours et l’état de progression de la tâche devient en retard.

### Conclusion automatique {#auto-complete}

Workfront suppose que les tâches seront terminées comme prévu et les marque comme étant terminées à leur date d’échéance ou d’achèvement prévu. En attendant, Workfront utilise Pourcentage d’achèvement et Heures réelles consignées pour déterminer l’état de progression. Cependant, quel que soit l’état de progression avant la date d’achèvement planifiée, Workfront marque toujours la tâche terminée.

Les exceptions suivantes existent :

* Si la tâche comporte des prédécesseurs incomplets, elle ne sera pas terminée automatiquement tant que tous ses prédécesseurs ne seront pas terminés. Les prédécesseurs doivent être appliqués.
* Si la tâche présente une contrainte de date fixe, elle se termine toujours à la date d’achèvement planifiée, que ses prédécesseurs soient terminés ou non.

>[!IMPORTANT]
>
>Lorsque vous sélectionnez l’option de fin automatique des tâches, la tâche est terminée lorsque l’heure du projet est recalculée. Si le type de mise à jour du projet est défini sur Automatique ou Automatique et Sur modification, la chronologie du projet est calculée quotidiennement. Pour plus d’informations sur les recalculs de la chronologie sur les projets, voir [Recalculer les calendriers du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>L’heure de la date de fin réelle est minuit du jour où la chronologie est automatiquement calculée. L’heure utilisée pour générer cet horodatage est le fuseau horaire de votre système tel que défini par votre administrateur Workfront dans la section Informations sur le client de la configuration. Pour plus d’informations sur la définition du fuseau horaire de votre système, voir [Configuration des informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Tâche antérieure {#predecessor}

Workfront estime la date d’achèvement prévue d’une tâche en fonction de sa relation précédente. L’état d’avancement d’une tâche est déterminé en fonction de cette estimation. Par exemple, la tâche B a une durée d’un jour et est planifiée deux jours après son prédécesseur, la tâche A, qui doit prendre cinq jours. Un utilisateur met ensuite la tâche B à jour pour la terminer à 50 %, mais le prédécesseur, la tâche A, n’a pas encore commencé. Workfront programme la tâche B dépendante pour qu’elle soit terminée six jours après la date de début de la tâche précédente, ce qui permet 5 jours pour la tâche A et 1 jour pour la tâche B.
