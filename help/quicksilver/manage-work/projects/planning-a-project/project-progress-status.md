---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Aperçu de l'état d'avancement du projet
description: Adobe Workfront détermine le statut de progression d’un projet en examinant la progression du projet tout au long de sa chronologie. Vous pouvez configurer Workfront pour qu’il détermine la condition d’un projet en fonction de la valeur du statut de progression des tâches. Pour en savoir plus sur le statut de progression d’un projet, consultez cet article.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
TQID: https://experienceleague.adobe.com/V9eyzkoYIREb4zUuDxmyDhnQa54YQaYTv2woNTOhq24
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 375
ht-degree: 80%

---

# Vue d’ensemble du statut de la progression d’un projet

<!--Audited: 12/2023-->

Adobe Workfront détermine le statut de progression d’un projet en examinant la progression du projet tout au long de sa chronologie. Vous pouvez configurer Workfront pour qu’il détermine la condition d’un projet en fonction de la valeur du statut de progression des tâches. Pour plus d’informations sur la configuration de la condition du projet, voir l’article [Vue d’ensemble de la condition du projet et du type de condition](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Voici les statuts de progression des projets dans Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>À l’heure</td> 
   <td> Le statut de progression d’un projet est <strong>À l’heure</strong> si :<ul><li>Si les dates d'échéance prévisionnelle et estimée sont antérieures ou égales à la date d'achèvement prévue du projet <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>En danger</td> 
   <td> Le statut de progression d’un projet est <strong>En danger</strong> si <strong>tous</strong> les éléments suivants sont vrais :<ul><li>Les dates d’achèvement estimées et projetées se situent toutes deux dans le futur.</li><li> La date d'échéance estimée est postérieure à la fois à la date d'achèvement prévue et à la date d'achèvement prévisionnelle <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul> </td> 
  </tr> 
  <tr> 
   <td>En retard</td> 
   <td> Le statut de progression d’un projet est <strong>Retardé</strong> si <strong>tous</strong> les éléments suivants sont vrais :<ul><li>Les dates d’achèvement estimées et projetées se situent toutes deux dans le futur.</li><li> Les dates d’achèvement estimées et projetées sont toutes deux postérieures à la date d’achèvement prévue du projet.</li><li> La date d'échéance estimée n'est pas postérieure à la date d'achèvement prévisionnelle
   <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>En retard</td> 
   <td> 
     Le statut de progression d’un projet est <strong>En retard</strong> si <strong>l’un</strong> des éléments suivants est vrai :<ul><li>Le projet est achevé et la date d’achèvement réelle est postérieure à la date d’achèvement prévue. <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Le projet n’est pas achevé et la date d’achèvement prévue est dépassée. <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants :

* La date d’achèvement projetée du projet est déterminée par la tâche du chemin critique dont la date d’achèvement projetée est la plus tardive.
* La date d&#39;échéance estimée du projet est déterminée par la tâche sur le chemin critique avec la dernière date d&#39;échéance estimée.

Pour plus d’informations sur le chemin critique du projet, voir [Vue d’ensemble du chemin critique du projet](../../../manage-work/tasks/manage-tasks/critical-path.md).

Pour plus d’informations sur les dates d’achèvement projetées, voir [Vue d’ensemble de la date d’achèvement prévue pour les projets, les tâches et les problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
