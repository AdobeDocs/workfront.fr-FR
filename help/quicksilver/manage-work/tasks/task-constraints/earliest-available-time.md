---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '« Vue d’ensemble de la contrainte de tâche : "Première Heure Disponible" »'
description: Le délai le plus court est une contrainte de tâche qui planifie une tâche pour qu’elle commence au plus tôt après avoir pris en compte les relations antérieures.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 100%

---

# Vue d’ensemble des contraintes de tâches : Première heure disponible

Le délai le plus court est une contrainte de tâche qui planifie une tâche pour qu’elle commence au plus tôt après avoir pris en compte les relations antérieures.

Pour plus d’informations sur la mise à jour de la contrainte de tâche, voir [Mettre à jour la contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## Différence entre Première heure disponible et Aussi tôt que possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

La contrainte Première heure disponible diffère de la contrainte Aussi tôt que possible lorsque tous les critères suivants sont remplis :

* Le projet est planifié à partir de la date d’achèvement.
* Les tâches du projet ont une relation antérieure.
* La tâche antérieure a une contrainte de tâche flexible.

Dans ce cas :

* **Première Heure Disponible :** l’utilisation de la contrainte « Première Heure Disponible » pour la tâche ultérieure donne la priorité à la contrainte flexible antérieure.

  **EXEMPLE**

  La tâche A est antérieure à la tâche B. La tâche B est soumise à la contrainte « Première Heure Disponible » et la tâche A est soumise à la contrainte « Aussi Tard Que Possible ». Dans ce cas, la tâche B est programmée le plus près possible de la fin du projet.

  ![Contrainte « Première Heure Disponible » lorsque les dates de la tâche sont proches de la date d’achèvement du projet.](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Aussi Tôt Que Possible :** dans ce scénario, l’utilisation de la contrainte « Aussi Tôt Que Possible » pour la tâche ultérieure donne la priorité à cette dernière.

  **EXEMPLE**

  La tâche A est antérieure à la tâche B. La tâche B a la contrainte « Aussi Tôt Que Possible » et la tâche A a la contrainte « Aussi Tard Que Possible ». Dans ce cas, la tâche B est programmée le plus près possible du début du projet.

  ![Contrainte « Aussi Tôt Que Possible » lorsque les dates de la tâche sont proches de la date de début du projet.](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
