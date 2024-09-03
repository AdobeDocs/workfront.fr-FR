---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Vue d’ensemble des contraintes de tâches
description: Les contraintes de tâches déterminent quand une tâche doit commencer et se terminer dans un projet.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 100%

---

# Vue d’ensemble des contraintes de tâches

<!-- Audited: 12/2023 -->

Les contraintes de tâches déterminent quand une tâche doit commencer et se terminer dans un projet.

## Vue d’ensemble des contraintes de tâches

Lorsque vous élaborez votre plan de projet, vous prenez des décisions sur la séquence et la période de vos tâches dans le projet. Les tâches peuvent fonctionner indépendamment de toute séquence de tâches, mais elles peuvent avoir un impact sur la chronologie du projet. Les contraintes de tâches permettent au gestionnaire ou à la gestionnaire de projet de planifier le moment où certaines tâches peuvent commencer ou se terminer dans le cadre d’un projet.

En fonction de la contrainte utilisée, vous devrez peut-être spécifier une date de début prévue, une date d’achèvement prévue, ou les deux, pour la tâche.

Les types de contraintes qui requièrent des dates définies ont un impact sur les relations antérieures.

>[!TIP]
>
>Envisagez d’utiliser un type de contrainte qui ne nécessite pas de dates spécifiques si vous utilisez des relations antérieures entre les tâches.

Le tableau suivant présente chaque contrainte et son abréviation. Les abréviations sont utilisées dans les listes de tâches et lors de la création de fichiers d’import Kickstart. Cliquez sur le titre lié à chaque contrainte de tâche pour obtenir plus d’informations sur ce type de contrainte.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Nom de la contrainte</strong> </p> </th> 
   <th> <p><strong>Abréviation</strong> </p> </th> 
   <th> <p><strong>Description</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : dès que possible</a>. </p> </td> 
   <td scope="col"> <p>ATôP</p> </td>
   <td scope="col"> <p>Placez l’heure de début de la tâche aussi près que possible du début du projet.</p> 
   <p>Il s’agit de la contrainte par défaut si le projet utilise un Mode horaire à partir de la date de début et si la date de début par défaut du système pour une nouvelle tâche est définie sur Basée sur la date prévue du projet. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : le plus tard possible</a>. </p> </td> 
   <td scope="col"> <p>ATaP</p> </td> 
   <td scope="col"> <p>Place la date d’achèvement de la tâche aussi près que possible de la fin du projet.</p> 
   <p>Il s’agit de la contrainte par défaut lorsque le projet utilise un mode horaire à partir de la date d’achèvement et que la valeur par défaut du système ou du groupe pour la date de début d’une tâche est basée sur la date prévue du projet. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : première heure disponible</a>. </p> </td> 
   <td scope="col"> <p>PHD</p> </td> 
 <td scope="col"> <p>Planifie une tâche pour qu’elle commence à la première heure disponible après avoir pris en compte les relations antérieures.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : dernière heure disponible</a>. </p> </td> 
   <td scope="col"> <p>DHD</p> </td> 
   <td scope="col"> <p>Planifie une tâche pour qu’elle commence au dernier moment disponible après avoir pris en compte les relations antérieures et ultérieures dans le projet.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : commencer au plus tôt le</a>. </p> </td> 
   <td scope="col"> <p>CPTô</p> </td> 
   <td scope="col"> <p>Planifie le démarrage d’une tâche après la date spécifiée.</p> 
   <p>Il s’agit de la contrainte par défaut si le mode horaire du projet est à partir de la date de début et si la date de début par défaut du système ou du groupe pour une nouvelle tâche est fixée à aujourd’hui.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : commencer au plus tard le</a>. </p> </td> 
   <td scope="col"> <p>CPTr</p> </td> 
   <td scope="col"> <p>Planifie le démarrage d’une tâche avant la date spécifiée.</p> 
   <p>Il s’agit de la contrainte par défaut si le mode horaire du projet est à partir de la date d’achèvement et si la date par défaut du système ou du groupe pour la date de début d’une tâche est définie sur aujourd’hui. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : Finir Au Plus Tôt</a>. </p> </td> 
   <td scope="col"> <p>FPTô</p> </td>
   <td scope="col"> <p>Planifie une tâche pour qu’elle se termine après la date spécifiée.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : terminer au plus tard le</a>. </p> </td> 
   <td scope="col"> <p>FPTr</p> </td> 
   <td scope="col"> <p>Planifie une tâche pour qu’elle se termine avant la date spécifiée.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : Doit commencer le</a>. </p> </td> 
   <td scope="col"> <p>FC</p> </td> 
   <td scope="col"> <p>Planifie le démarrage d’une tâche à une date précise.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : doit se terminer le</a>. </p> </td> 
   <td scope="col"> <p>FF</p> </td> 
   <td scope="col"> <p>Planifie la fin d’une tâche à une date spécifique.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches : dates fixes</a> </p> </td> 
   <td> <p>FIXE</p> </td> 
   <td> <p>Planifie le début et la fin d’une tâche à des dates précises.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vue d’ensemble des contraintes par défaut

Lorsque vous créez de nouvelles tâches, Workfront sélectionne automatiquement une contrainte de tâche.

Workfront utilise deux variables pour décider quelle contrainte de tâche est sélectionnée par défaut pour une nouvelle tâche :

* Le champ **Projet prévu à partir du** du projet.

  Pour plus d’informations sur le champ Projet prévu à partir du, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* La préférence **Date de début** configurée par votre administrateur ou administratrice Workfront ou de groupe dans la zone **Tâches et problèmes** de la **Configuration**.

  Pour plus d’informations sur les préférences relatives aux tâches et aux problèmes, voir la section [Paramètres par défaut des nouvelles tâches](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) dans [Configurer les préférences des tâches et des problèmes au niveau du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Le tableau suivant montre la contrainte de tâche par défaut lorsque vous choisissez différentes variables pour votre projet et vos nouvelles tâches :

| Projet prévu à partir du | Date de début de la tâche | Contrainte de tâche par défaut |
|---|---|---|
| Date de début | En fonction de la date prévue de projet | Aussi Tôt Que Possible |
| Date de début | Aujourd’hui | Commencer Au Plus Tôt |
| Date d&#39;achèvement | En fonction de la date prévue de projet | Aussi Tard Que Possible |
| Date d&#39;achèvement | Aujourd’hui | Commencer Au Plus Tard |
