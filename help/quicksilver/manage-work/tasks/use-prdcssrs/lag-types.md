---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Vue d’ensemble des types de décalage
description: Le décalage correspond au temps qui doit s’écouler après la fin d’une tâche antérieure imposée jusqu’à ce que la tâche dépendante puisse commencer (décalage positif), ou au temps pendant lequel une tâche dépendante peut commencer avant le début de la tâche antérieure (décalage négatif).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 100%

---

# Vue d’ensemble des types de décalage

<!-- Audited: 01/2024 -->

Le décalage correspond au temps qui doit s’écouler après la fin prévue d’une tâche antérieure jusqu’à ce que la tâche dépendante puisse commencer (décalage positif), ou au temps pendant lequel une tâche dépendante peut commencer avant le début de la tâche antérieure (décalage négatif).

Les dates Prévues, Prévisionnelles et Estimées des tâches ultérieures sont calculées en tenant compte des dates de décalage, prévues, prévisionnelles et de début (fin) estimées des tâches antérieures.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : formule </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Types de décalage {#lag-types}

Un exemple de tâche qui nécessiterait un temps de décalage peut être de scier des arbres en planches. Si le bois fraîchement coupé doit sécher pendant un certain temps avant de pouvoir être coupé, il y aurait un temps de décalage entre couper les arbres et les scier en planches.

Le tableau suivant illustre les types de décalage et comment indiquer la durée de chacun d’eux :

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Valeur</strong> </p> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Jours (d ou de)</p> </td> 
   <td> <p>Le délai entre deux tâches liées par une dépendance est mesuré en jours ouvrés. Il s’agit du type de décalage par défaut. </p> <p>Par exemple, s’il existe une dépendance finir-commencer avec un décalage de 2 jours ouvrés et que la tâche antérieure se termine le vendredi, la tâche dépendante commence le mercredi. Les jours du week-end ne comptent pas dans le décalage. </p> <p>Note : la limite de décalage maximale pour les jours est de 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Jours calendaires (c ou ce)</p> </td> 
   <td> <p>Le délai entre deux tâches est mesuré en jours calendaires, notamment les jours fériés et les week-ends. </p> <p>Note : bien que ce type de décalage comptabilise les jours non ouvrés dans le décalage, une tâche dépendante ne peut jamais commencer un jour non ouvré. Si ce type de décalage fait commencer la tâche dépendante un jour non ouvré, la date de début planifiée de la tâche dépendante est planifiée le jour ouvré suivant. </p> <p>Par exemple, s’il existe une dépendance finir-commencer avec un décalage de 2 jours calendaires et que la tâche antérieure se termine le jeudi, la tâche dépendante commence le lundi au lieu d’un dimanche. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Pourcentage (p ou pe)</p> </td> 
   <td> <p>Le délai est exprimé sous la forme d’un pourcentage du temps estimé pour terminer la tâche antérieure. </p> <p>Par exemple, s’il existe une dépendance finir-commencer avec un décalage de 20 % par rapport à une tâche antérieure de 10 jours, le système calcule le nombre de jours représentant 20 % de la durée de la tâche antérieure et l’utilise comme décalage. Dans ce cas, elle serait de 2 jours après l’achèvement de la tâche. </p>

<p><b>NOTE</b></p> La limite de décalage maximale pour le pourcentage est de 2 000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Jour de la semaine (w ou we) </p> </td> 
   <td> <p>Le délai entre deux tâches est mesuré en indiquant les jours de la semaine pour la semaine qui contient la date d’achèvement prévue du prédécesseur.</p> <p>Pour ce type de décalage, chaque jour de la semaine est associé à un chiffre :</p> 
    <ul> 
     <li>Dimanche=1</li> 
     <li>Lundi=2</li> 
     <li>Mardi=3</li> 
     <li>Mercredi=4</li> 
     <li>Jeudi=5</li> 
     <li>Vendredi=6</li> 
     <li>Samedi=7</li> 
    </ul> <p>Si vous souhaitez indiquer que la date de début planifiée du successeur doit être un mardi de la semaine en cours et que le mardi est antérieur à la date d’achèvement prévue du prédécesseur, vous devez coder votre successeur avec la formule suivante : </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>NOTE</b></p>

Si la date de début du successeur est calculée pour correspondre à un certain mardi et ce jour est passé pour la semaine en cours, la date de début planifiée de la tâche successeuse est le même jour (mardi) de la semaine suivante, si disponible. </p> <p>Si vous souhaitez indiquer que le décalage doit tomber un samedi de la semaine en cours et que le samedi se situe après la date d’achèvement prévue du prédécesseur, vous devez coder votre successeur avec la formule suivante :</p> <p><code>4fs+7w</code> </p> <p>Si le samedi est un jour non ouvré, le lendemain disponible après le samedi (pour indiquer un décalage positif) est sélectionné comme date de début planifiée du successeur. </p>

<p>Cela ne s’applique pas aux exceptions de planification. Si une date est également une exception de planning et que la date de début du successeur est calculée pour correspondre à ce jour, le système tente alors de trouver la date disponible la plus proche, qui est le jour de la semaine spécifié dans l’expression du prédécesseur.</p>

<p>Par exemple, si la date de début est calculée pour correspondre à un certain mardi et que ce jour est une exception de planning et que le décalage du prédécesseur est positif, il choisira le mardi suivant (s’il s’agit également d’un jour ouvré) comme date de début du successeur. Si le décalage est négatif, le système choisit le mardi précédent comme date de début.</p>

<p>Pour indiquer les semaines passées ou futures, vous pouvez ajouter un numéro devant le chiffre du jour pour le type de décalage. </p> <p>Par exemple, pour indiquer le lundi de 10 semaines auparavant, vous pouvez utiliser ce code pour indiquer le prédécesseur de votre successeur :</p> <p><code>4fs-102w</code> </p> <p>10 indique il y a 10 semaines et 2 est le numéro attribué au lundi. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Jour de la semaine non nul (k ou ke)</p> </td> 
   <td> <p>Le délai entre deux tâches est mesuré de la même manière que le type de décalage Jour de la semaine , sauf si l’heure du prédécesseur se termine le même jour de la semaine spécifié. Le délai est ensuite calculé sur la semaine adjacente (+/-). </p> <p>Dans ce cas, le délai ne peut jamais être de 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Décalage négatif

Vous pouvez utiliser un décalage négatif pour indiquer la nécessité ou la capacité de la tâche à commencer avant la fin de la tâche antérieure.

Tenez compte des règles suivantes lorsque vous utilisez des décalages négatifs :

* Le décalage négatif ne peut pas forcer les dates de Début/Fin d’une tâche à être avant ou après les dates de Début/Fin prévues du projet. Ces dates sont spécifiées dans le champ Planifier à partir de du projet.

  Dans ce cas, tenez compte des points suivants :

   * Planifiez le projet à partir de la date d’achèvement.
   * La dernière tâche du projet doit utiliser la contrainte de tâche Doit se terminer le. Il est recommandé de donner à la tâche une durée suffisante pour tenir compte de toutes les tâches du projet. Les autres tâches fonctionnent bien avec la contrainte Aussi tôt que possible.

* L’utilisation d’une relation d’antériorité Terminer-Démarrer pour les tâches peut générer un message d’erreur.

  Dans ce cas, tenez compte des points suivants :

   * Définissez une relation d’antériorité Terminer-Démarrer entre les tâches.
   * La Durée de la tâche ultérieure qui doit être égale ou supérieure au nombre prévu de jours de décalage entre les tâches.

## Indiquer un décalage et des types de décalage sur des tâches

Vous pouvez indiquer des types de décalage sur les tâches lorsque vous définissez leurs relations antérieures.

### Indiquer des types de décalage dans la section antérieure d’une tâche {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Accédez à une tâche pour laquelle vous souhaitez définir la tâche antérieure et le type de décalage.
1. Cliquez sur **Tâches antérieures** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Tâches antérieures**.
1. Cliquez sur **Ajouter une tâche antérieure**.
1. (Facultatif) Si vous souhaitez ajouter une tâche antérieure de plusieurs projets, remplacez le nom du **projet parent** par un autre projet.
1. Commencez à saisir le nom de la tâche antérieure, puis sélectionnez-la lorsqu’elle apparaît dans la liste.
1. Sélectionnez le **type de dépendance**.

   Pour plus d’informations sur les types de dépendance des tâches antérieures, voir [Vue d’ensemble des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Spécifiez une durée de **décalage** à l’aide d’une valeur numérique. Vous pouvez indiquer des nombres négatifs pour indiquer un décalage négatif.
1. Sélectionnez l’une des options suivantes pour identifier le type de décalage que vous souhaitez indiquer pour votre tâche antérieure :

   * **Jours**
   * **Jours civils**
   * **Pourcentage**
   * **Jour de la semaine**
   * **Jour de la semaine (différent de zéro)**

     Pour plus d’informations sur ces types de décalage et sur leur mode de calcul, consultez la section [Types de décalage](#lag-types) dans cet article.

1. Cliquer sur **Enregistrer**.

### Indiquer des types de décalage dans une liste de tâches  {#indicate-lag-types-in-a-task-list}

1. Dans la liste des tâches, sélectionnez la vue **Standard**.

1. Cliquez dans la colonne **Tâches antérieures** correspondant à la tâche pour laquelle vous souhaitez spécifier une tâche antérieure et une durée de décalage.
1. Saisissez les informations suivantes sans espaces :

   * le numéro de la tâche à indiquer comme antérieure à la tâche sélectionnée.
   * l’abréviation du type de dépendance à indiquer entre les tâches.

     Pour plus d’informations sur les abréviations des types de dépendance, voir [Vue d’ensemble des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * soit un **+** pour un décalage positif soit un **-** pour un décalage négatif.

   * la durée du décalage.
   * l’abréviation du type de décalage que vous souhaitez utiliser.

     Pour plus d’informations sur les abréviations des types de décalage, voir la section [Types de décalage](#lag-types) dans cet article.

   Par exemple, pour indiquer qu’une tâche a une tâche antérieure et un décalage positif de 2 jours, vous devez saisir `1fs+2d` dans la colonne Tâches antérieures.

1. Appuyez sur la touche Entrée de votre clavier pour enregistrer les modifications apportées à votre tâche.