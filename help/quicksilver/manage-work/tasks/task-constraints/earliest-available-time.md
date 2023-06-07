---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Présentation de la contrainte de tâche : Heure disponible la plus proche"'
description: La première heure disponible est une contrainte de tâche qui planifie qu’une tâche commence au moment le plus tôt possible après avoir pris en compte les relations de prédécesseur.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Présentation de la contrainte de tâche : Heure disponible la plus tôt

La première heure disponible est une contrainte de tâche qui planifie qu’une tâche commence au moment le plus tôt possible après avoir pris en compte les relations de prédécesseur.

Pour plus d’informations sur la mise à jour de la contrainte de tâche sur une tâche, voir [Mettre à jour la contrainte de tâche d’une tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## Différence entre le plus tôt temps disponible et le plus tôt possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

La contrainte Heure disponible la plus ancienne diffère de la contrainte Dès que possible lorsque tous les critères suivants existent :

* Le projet est planifié à partir de la fin
* Les tâches du projet ont une relation de prédécesseur
* La tâche précédente présente une contrainte de tâche flexible.

Dans ce cas :

* **Heure disponible la plus récente :** L’utilisation de la contrainte de la première heure disponible sur la tâche qui lui succède donne la priorité à la contrainte flexible du prédécesseur.

   **EXEMPLE**

   La tâche A est un prédécesseur de la tâche B. La tâche B a la contrainte Temps disponible la plus ancienne et la tâche A la contrainte Aussi tardive que possible. Dans ce cas, la tâche B est planifiée aussi près que possible de la fin du projet.

   ![Contrainte horaire disponible la plus ancienne lorsque les dates de la tâche sont proches de la date d’achèvement du projet](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Dès Que Possible :** Dans ce scénario, l’utilisation de la contrainte Dès que possible sur la tâche qui lui succède donne la priorité à la tâche qui lui succède.

   **EXEMPLE**

   La tâche A est un prédécesseur de la tâche B. La tâche B a la contrainte Dès que possible et la tâche A la contrainte Aussi tard que possible. Dans ce cas, la tâche B est planifiée aussi près que possible du début du projet.

   ![Dès que possible contrainte lorsque les dates de la tâche sont proches de la date de début du projet](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
