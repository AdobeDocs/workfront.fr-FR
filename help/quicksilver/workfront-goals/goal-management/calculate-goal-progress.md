---
product-previous: workfront-goals
navigation-topic: goal-management
title: Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront
description: La progression de l’objectif dépend d’indicateurs de progression tels que les activités, les résultats ou les objectifs enfant. La condition de l’objectif est déterminée par sa progression à l’heure actuelle.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 98%

---

# Vue d’ensemble de la progression et de la condition des objectifs dans les Objectifs Adobe Workfront

<!--Audited for P&P only: 4/2025-->

>[!IMPORTANT]
>
>Votre organisation doit disposer des éléments suivants pour utiliser les fonctionnalités décrites dans cet article :
>
>
>* Pour la nouvelle structure de forfait et de licence :
>
>   * Un forfait Ultimate
>    
>* Pour la structure de forfait et de licence actuelle :
>
>   * Un forfait Pro ou supérieur
>   * Une licence Objectifs Adobe Workfront en plus d’une licence Workfront.
>
> Contactez la personne chargée de la gestion de votre compte Workfront pour en savoir plus sur la licence Objectifs Workfront.
>
>Pour plus d’informations sur l’accès aux Objectifs Workfront, voir la section [Conditions requises pour utiliser les Objectifs Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront calcule automatiquement la progression de l’objectif en fonction de la progression de ses indicateurs de progression.

## Vue d’ensemble de la progression et du seuil de l’objectif

Une fois que vous avez activé un objectif, la solution Objectifs Workfront commence à calculer sa progression et sa condition et affiche les indicateurs suivants lorsque vous pointez sur le champ Progression :

| Indicateur | Description de l’indicateur |
|---|---|
| Pourcentage terminé réel | Pourcentage de réalisation de l’objectif à ce stade. Objectifs Workfront détermine cette valeur en calculant le pourcentage terminé de tous les indicateurs de progression associés à l’objectif. |
| Pourcentage terminé attendu | Pourcentage de l’objectif qui doit être terminé à ce stade pour que l’objectif soit achevé dans les temps. La solution Objectifs Workfront calcule cette valeur en tenant compte de la durée de l’objectif et du moment présent. Si l’objectif se termine dans les temps, il doit afficher cette valeur à l’heure actuelle. |
| Progression | Libellé qui indique si l’objectif est dans les temps, ou s’il est en difficulté et risque de ne pas aboutir. |

![En difficulté](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Pourcentage terminé réel](#actual-percent-complete)
* [Pourcentage terminé attendu](#expected-percent-complete)
* [Progression et condition](#progress)

### Pourcentage terminé réel {#actual-percent-complete}

La solution Objectifs Workfront calcule automatiquement le pourcentage terminé réel d’un objectif en fonction de la moyenne de pourcentage terminé des indicateurs de progression de l’objectif.

Les éléments suivants sont considérés comme des indicateurs de progression pour les objectifs :

* Résultats

  Pour plus d’informations sur l’ajout de résultats aux objectifs, voir [Ajouter des résultats aux objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Activités

  Pour plus d’informations sur l’ajout d’activités, y compris des projets, à des objectifs, voir [Ajouter des activités aux objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Objectifs enfant alignés

  Pour plus d’informations sur les objectifs parent et enfant, voir [Aligner des objectifs en les connectant dans les Objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  La solution Objectifs Workfront calcule le pourcentage terminé réel à l’aide de la formule suivante :

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Par exemple, si un objectif a un résultat achevé à 20 %, une barre de progression manuelle remplie à 30 %, un projet à 10 % et un objectif enfant à 40 %, le pourcentage terminé de l’objectif est de 25 %.

### Pourcentage terminé attendu {#expected-percent-complete}

La solution Objectifs Workfront calcule automatiquement le pourcentage terminé attendu d’un objectif en fonction du nombre total de jours sur sa durée ainsi que du nombre de jours écoulés depuis la date de début.

Objectifs Workfront calcule le pourcentage terminé attendu à l’aide de la formule suivante :

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Par exemple, si un objectif doit être achevé dans 90 jours, et qu’aujourd’hui est le 45e jour de cette durée, le pourcentage terminé attendu est de 50 %.

### Progression et condition {#progress}

La solution Objectifs Workfront calcule un pourcentage de progression et attribue un libellé de progression aux objectifs en fonction du pourcentage terminé prévu qui a été atteint à ce moment précis. La barre de pourcentage terminé de l’objectif change de couleur pour indiquer la progression de l’objectif.

La condition de l’objectif est également mise à jour en conséquence, afin d’indiquer si l’objectif est en passe d’être terminé à temps ou s’il est en retard.

La solution Objectifs Workfront calcule le pourcentage de progression d’un objectif à l’aide de la formule suivante :

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Par exemple, si le pourcentage terminé attendu est de 53 % à l’heure actuelle et que le pourcentage terminé réel est de 30 %, le pourcentage de progression de l’objectif est de 56 %. La solution Objectifs Workfront attribue à cet objectif la condition « En difficulté ».

Le graphique suivant illustre la relation entre les libellés de condition et le pourcentage de progression :

![Graphique des libellés de statut de progression](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

Le tableau ci-dessous répertorie les libellés de condition d’objectif et les pourcentages de progression d’objectif associés à chaque libellé.

>[!TIP]
>
>Les libellés de condition d’objectif correspondent au nom et à la couleur de la condition du projet Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Nom de la progression de l’objectif</b></td> 
   <td><b>Définition de la progression de l’objectif</b></td> 
   <td><b>Pourcentage de progression de l’objectif</b></td> 
   <td><b>Couleur de la barre de pourcentage terminé</b></td> 
   <td><b>Icône de l’indicateur de condition</b></td> 
  </tr> 
  <tr> 
   <td>Nouveau</td> 
   <td> <p>L’objectif vient d’être créé et n’enregistre pas encore la progression. La progression de l’objectif s’affiche comme Nouveau jusqu’à ce qu’une personne mette à jour sa progression pour la première fois. </p> <p>Pour plus d’informations sur la mise à jour de la progression de l’objectif, voir <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Mettre à jour la progression des objectifs dans Objectifs Adobe Workfront</a>.</p> </td> 
   <td>Aucun pourcentage</td> 
   <td>Aucune barre</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Dans les temps</span> </p> </td> 
   <td>La progression vers l’objectif avance comme prévu et il est très probable qu’il serat atteint dans les temps. </td> 
   <td>90 à 100 %</td> 
   <td>Vert</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>À risque</span> </p> </td> 
   <td>La progression vers l’objectif prend du retard, mais il peut encore être atteint dans les temps. </td> 
   <td>70 à 89,99 %</td> 
   <td>Jaune</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>En difficulté</span> </p> </td> 
   <td> <p>Il est très probable que l’objectif ne sera pas atteint à temps. </p> </td> 
   <td>0 à 69,99 %</td> 
   <td>Rouge</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>
