---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Vue d’ensemble des contraintes de tâches
description: Les contraintes de tâche déterminent à quel moment une tâche doit commencer et se terminer sur un projet.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 8%

---

# Vue d’ensemble des contraintes de tâches

<!-- Audited: 12/2023 -->

Les contraintes de tâche déterminent à quel moment une tâche doit commencer et se terminer sur un projet.

## Présentation des contraintes de tâche

Lorsque vous créez le plan de votre projet, vous prenez des décisions sur la séquence et la période de vos tâches sur le projet. Les tâches peuvent fonctionner indépendamment de n’importe quelle séquence de tâches, mais elles peuvent avoir un impact sur la chronologie du projet. Les contraintes de tâche permettent à un chef de projet de planifier le moment où certaines tâches peuvent démarrer ou se terminer sur un projet.

Selon la contrainte que vous utilisez, vous devrez peut-être spécifier une date de début planifiée, une date de fin planifiée ou les deux pour la tâche.

Les types de contraintes qui nécessitent des dates définies ont un impact sur les relations de prédécesseur.

>[!TIP]
>
>Envisagez d’utiliser un type de contrainte qui ne nécessite pas de dates spécifiques si vous utilisez des relations de prédécesseur entre les tâches.

Le tableau suivant affiche chaque contrainte et son abréviation. Les abréviations sont utilisées dans les listes de tâches et lors de la création de fichiers d&#39;import de démarrage rapide. Cliquez sur le titre associé de chaque contrainte de tâche pour plus d’informations sur ce type de contrainte.

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
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Présentation de la contrainte de tâche : Dès que possible</a> </p> </td> 
   <td scope="col"> <p>ATôP</p> </td>
   <td scope="col"> <p>Place l’heure de début de la tâche aussi près que possible du début du projet.</p> 
   <p>Il s’agit de la contrainte par défaut si le projet utilise un mode de planification à partir de la date de début et si la date de début par défaut du système d’une nouvelle tâche est définie sur Basé sur la date planifiée du projet. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Présentation de la contrainte de tâche : aussi tard que possible </a> </p> </td> 
   <td scope="col"> <p>ATaP</p> </td> 
   <td scope="col"> <p>Place le délai d’achèvement de la tâche aussi près que possible de la fin du projet.</p> 
   <p>Il s’agit de la contrainte par défaut lorsque le mode de planification du projet est à partir de la date de fin et que la valeur par défaut du système ou du groupe pour la date de début d’une tâche est définie sur Basé sur la date planifiée du projet. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Présentation de la contrainte de tâche : Temps disponible le plus tôt</a> </p> </td> 
   <td scope="col"> <p>PHD</p> </td> 
 <td scope="col"> <p>Planifie une tâche pour qu’elle commence le plus tôt possible après avoir pris en compte les relations de prédécesseur.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Présentation de la contrainte de tâche : heure disponible la plus récente</a> </p> </td> 
   <td scope="col"> <p>DHD</p> </td> 
   <td scope="col"> <p>Planifie une tâche pour qu’elle commence au moment le plus récent disponible après avoir pris en compte les relations entre le prédécesseur et le successeur dans le projet.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Présentation de la contrainte de tâche : ne pas commencer avant</a> </p> </td> 
   <td scope="col"> <p>CPTô</p> </td> 
   <td scope="col"> <p>Planifie une tâche à démarrer après la date que vous spécifiez.</p> 
   <p>Il s’agit de la contrainte par défaut si le mode de planification du projet est défini sur Date de début et si la date de début par défaut du système ou du groupe d’une nouvelle tâche est définie sur Aujourd’hui.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Présentation de la contrainte de tâche : ne pas commencer plus tard que</a> </p> </td> 
   <td scope="col"> <p>CPTr</p> </td> 
   <td scope="col"> <p>Planifie une tâche à démarrer avant la date que vous spécifiez.</p> 
   <p>Il s’agit de la contrainte par défaut si le mode de planification du projet est à partir de la date de fin et si la valeur par défaut du système ou du groupe pour la date de début d’une tâche est définie sur Aujourd’hui. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Présentation de la contrainte de tâche : ne pas terminer avant </a> </p> </td> 
   <td scope="col"> <p>FPTô</p> </td>
   <td scope="col"> <p>Planifie une tâche à terminer après la date que vous spécifiez.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Présentation de la contrainte de tâche : Terminer au plus tard </a> </p> </td> 
   <td scope="col"> <p>FPTr</p> </td> 
   <td scope="col"> <p>Planifie une tâche à terminer avant la date que vous spécifiez.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Présentation de la contrainte de tâche : Doit démarrer le </a> </p> </td> 
   <td scope="col"> <p>FC</p> </td> 
   <td scope="col"> <p>Planifie une tâche pour qu’elle commence exactement à une date spécifique.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Présentation de la contrainte de tâche : Doit Se Terminer Sur</a> </p> </td> 
   <td scope="col"> <p>FF</p> </td> 
   <td scope="col"> <p>Planifie une tâche pour qu’elle se termine à une date spécifique.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Présentation de la contrainte de tâche : Dates fixes</a> </p> </td> 
   <td> <p>FIXE</p> </td> 
   <td> <p>Planifie une tâche pour qu’elle commence et se termine à des dates spécifiques.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Présentation des contraintes par défaut

Lorsque vous créez des tâches, une contrainte de tâche est automatiquement sélectionnée par Workfront.

Workfront utilise deux variables pour décider quelle contrainte de tâche est sélectionnée par défaut pour une nouvelle tâche :

* Le champ **Planification du projet à partir de** sur le projet.

  Pour plus d’informations sur le champ Planifier le projet à partir de , voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* La préférence **Date de début** configurée par votre administrateur Workfront ou de groupe dans la zone **Tâches et problèmes** de **Configuration**.

  Pour plus d’informations sur les préférences Tâches et problèmes, consultez la section [Nouvelles valeurs par défaut de la tâche](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) dans [ Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Le tableau suivant affiche la contrainte de tâche par défaut lors du choix de différentes variables pour votre projet et vos nouvelles tâches :

| Planification du projet à partir de | Date de début de tâche | Valeur par défaut de la contrainte de tâche |
|---|---|---|
| Date de début | En fonction de la date prévue de projet | Aussi Tôt Que Possible |
| Date de début | Aujourd’hui | Commencer Au Plus Tôt |
| Date d&#39;achèvement | En fonction de la date prévue de projet | Le plus tard possible |
| Date d&#39;achèvement | Aujourd’hui | Commencer Au Plus Tard |
