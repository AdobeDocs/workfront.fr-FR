---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Aperçu du mode de suivi des tâches
description: Vous pouvez régler le paramètre Mode de suivi d’une tâche lors de la création ou de la modification d’une tâche afin de contrôler comment et à quel moment les indicateurs Statut de la progression d’une tâche s’affichent. Adobe Workfront affiche des indicateurs de statut de la progression lorsque vous configurez certains paramètres pour le suivi de la progression des tâches.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 99%

---

# Vue d’ensemble du mode de suivi des tâches

<!-- Audited: 01/2024 -->

Vous pouvez régler le paramètre Mode de suivi d’une tâche lors de la création ou de la modification d’une tâche afin de contrôler comment et à quel moment les indicateurs Statut de la progression d’une tâche s’affichent. Adobe Workfront affiche des indicateurs de statut de la progression lorsque vous configurez certains paramètres pour le suivi de la progression des tâches.

Pour plus d’informations sur le statut de la progression des tâches, consultez [Vue d’ensemble du statut de la progression de tâche](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click <strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the <strong>Settings</strong> section, use the <strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Options de Mode de suivi {#tracking-mode-options}

En tant que propriétaire de la tâche, ou chef ou cheffe de projet, vous pouvez sélectionner la manière dont Workfront indique le statut de la progression de chaque tâche. Pour plus d’informations sur la façon de définir le mode de suivi sur vos tâches, consultez [Définir le mode de suivi pour les tâches](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Vous pouvez sélectionner l’une des options suivantes :

* [L’utilisateur doit mettre à jour](#user-must-update)
* [Supposer à l’heure](#assume-on-time)
* [Ignorer avertissements de retard](#ignore-late-warnings)
* [Conclusion automatique](#auto-complete)
* [Tâche antérieure](#predecessor)

### Utilisateur doit mettre à jour {#user-must-update}

Lorsque cette option est sélectionnée, Workfront utilise le Pourcentage terminé et les Heures effectives de la tâche consignés pour déterminer le statut de la progression de la tâche. Il s’agit de l’option par défaut.

### Supposer à l’heure {#assume-on-time}

Workfront suppose qu’une tâche sera terminée à temps, quel que soit le statut d’achèvement actuel. Si la tâche n’est pas terminée à temps (à la Date d’achèvement prévue), Workfront suppose automatiquement une Date d’achèvement prévue le jour ouvrable suivant. Vous devez toujours indiquer le moment où la tâche est terminée. Utilisez cette option lorsque les utilisateurs et les utilisatrices ne mettront pas à jour régulièrement leurs tâches.

### Ignorer avertissements de retard {#ignore-late-warnings}

Le statut de la progression d’une tâche est À l’heure jusqu’à ce qu’elle devienne En retard. Par exemple, si vous planifiez une tâche pour une durée de 10 jours et que, le jour auquel elle doit être terminée, la tâche affiche un pourcentage terminé de 60 %, Workfront met à jour la date d’achèvement projetée en ajoutant quatre jours et le statut de la progression de la tâche devient En retard.

### Conclusion automatique {#auto-complete}

Workfront suppose que les tâches seront terminées comme prévu et les signale comme étant terminées à leur date d’échéance ou d’achèvement prévue. En attendant, Workfront utilise le Pourcentage terminé et les Heures effectives consignés pour déterminer le statut de la progression. Cependant, quel que soit le statut de la progression avant la date d’achèvement planifiée, Workfront marque toujours la tâche comme étant terminée.

Les exceptions suivantes s’appliquent :

* Si la tâche comporte des tâches antérieures incomplètes, elle ne sera pas terminée automatiquement tant que toutes ses tâches antérieures ne seront pas terminées. Les tâches antérieures doivent être appliquées.
* Si la tâche présente une contrainte de date fixe, elle se termine toujours à la date d’achèvement prévue, que ses taches antérieures soient terminées ou non.

>[!IMPORTANT]
>
>Lorsque vous sélectionnez l’option de conclusion automatique des tâches, la tâche est terminée lorsque l’heure du projet est recalculée. Si le type de mise à jour du projet est défini sur Automatique ou Automatique et En cas de modification, la chronologie du projet est calculée quotidiennement. Pour plus d’informations sur les recalculs de la chronologie sur les projets, consultez [Recalculer la chronologie de projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>L’heure de la date d’achèvement réelle est minuit le jour où la chronologie est automatiquement calculée. L’heure utilisée pour générer cet horodatage est le fuseau horaire de votre système tel que défini par votre administrateur ou administratrice Workfront dans la section Informations sur le client de la configuration. Pour plus d’informations sur la définition du fuseau horaire de votre système, consultez [Configurer les informations de base de votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Tâche antérieure {#predecessor}

Workfront estime la date d’achèvement projetée d’une tâche en fonction de la relation avec sa tâche antérieure. Le statut de la progression d’une tâche est déterminé sur la base de cette estimation. Par exemple, la tâche B a une durée de 1 jour et est planifiée pour se terminer deux jours après sa tâche antérieure, la tâche A, qui doit prendre cinq jours. Un utilisateur ou une utilisatrice met ensuite la tâche B à jour comme étant terminée à 50 %, mais la tâche antérieure, la tâche A, n’a pas encore commencé. Workfront planifie la tâche B dépendante pour qu’elle soit terminée six jours après la date de début de la tâche de prédécesseur, ce qui laisse 5 jours pour la tâche A et 1 jour pour la tâche B.
