---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Présentation du type de durée : simple'
description: Le type de durée simple est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
TQID: https://experienceleague.adobe.com/-pBdowTzvPA4ubjZsZnaELWkVfmrd48nowdJJm0hhXk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 326
ht-degree: 46%

---

# Vue d’ensemble du type de durée : simple

<!-- Audited: 5/2025 -->

Le type de durée simple est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour plus d&#39;informations sur les types de durée dans Workfront, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Vue d’ensemble du type de durée simple

Votre administrateur Workfront ou de groupe peut définir le type de durée par défaut de votre système ou de votre groupe sur Simple. Dans ce cas, toutes les nouvelles tâches seront créées avec ce type de durée.

Pour plus d’informations sur la modification de votre tâche et les préférences de problème dans le cadre de vos préférences de projet à l’échelle du système ou du groupe, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Voici ce qui se produit lorsqu’une tâche est de type Durée simple :

* Les personnes responsables des projets peuvent modifier la durée et le nombre d’heures prévues d’une tâche lors de la modification de la façon dont ces heures doivent être réparties entre les personnes cessionnaires.

  Pour plus d’informations, voir [Mettre à jour le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Lorsque vous créez une tâche pour la première fois et que vous lui affectez le type de durée Simple mais que vous ne spécifiez pas de durée, Workfront calcule la durée de la tâche en fonction du nombre d&#39;heures prévues que vous spécifiez pour la tâche. Si vous modifiez manuellement la durée d&#39;une tâche de durée simple, Workfront cesse de faire correspondre les heures prévues à la durée, car il suppose que vous souhaitez les définir manuellement.
  >
  >Workfront calcule la durée des tâches dont la durée n’a pas été modifiée manuellement à l’aide de la formule suivante :
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Votre administrateur ou administratrice Workfront définit la variable `Typical hours per work day` dans la zone Préférences du projet de la configuration de votre instance.

* Le pourcentage de répartition est masqué, mais les heures de répartition peuvent être modifiées.
* Pour tous les nouveaux clientes et clients, le type de durée à l’échelle du système est défini sur simple.

## Remplacer le type de durée d’une tâche sur simple

Pour plus d’informations sur la modification du type de durée d’une tâche, voir [Mettre à jour le type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
