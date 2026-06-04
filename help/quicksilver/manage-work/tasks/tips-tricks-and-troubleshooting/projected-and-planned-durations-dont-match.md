---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: La durée prévisionnelle ne correspond pas à la durée prévue
description: 'Cet article décrit la résolution de problèmes dans Adobe Workfront en cas de réception du message suivant : ''La durée prévue d''une tâche/d''un événement est passée à 0 et ne correspond pas à la durée prévue.'''
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
TQID: https://experienceleague.adobe.com/cdGUhn51Xeqie8iW75phQTQKMvdO2ub-HSjcCjcHLec
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 234
ht-degree: 83%

---

# La durée prévisionnelle ne correspond pas à la durée prévue.

## Problème

Vous recevez le message d’erreur suivant : « La durée prévisionnelle d’une tâche / d’un problème est passée à 0 et ne correspond pas à la durée prévue ».

## Cause

Cela est dû au fait que la date de début prévisionnelle correspond à la date d’achèvement prévisionnelle.

## Solution

De nombreux facteurs peuvent faire correspondre les dates de début et d’achèvement prévisionnelles. Ce problème est en grande partie lié à l’affectation du temps sur la tâche ou le problème en question.

La plupart du temps, en fonction du type de durée de la tâche et de sa contrainte de tâche, la date d’achèvement prévisionnelle de l’affectation doit souvent être prolongée. Cependant, dans certains cas, en fonction de la configuration du type de durée et de la contrainte de tâche, cette valeur peut-être nulle.

Ci-dessous, vous trouverez une liste des éléments essentiels à examiner dans ces situations, accompagnée de liens vers des articles complémentaires :

* Date d’achèvement prévisionnelle : [vue d’ensemble de la date d’achèvement prévisionnelle pour les projets, tâches et problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* Contrainte de tâche : [vue d’ensemble de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* Type de durée : [vue d’ensemble de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

Si la date d’achèvement prévisionnelle, la contrainte de tâche ou le type de durée fonctionnent comme prévu, contactez le service d’assistance pour un diagnostic plus approfondi.
