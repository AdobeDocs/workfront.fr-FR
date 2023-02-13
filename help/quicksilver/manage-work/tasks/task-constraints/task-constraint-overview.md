---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Présentation de la contrainte de tâche
description: Les contraintes de tâche déterminent à quel moment une tâche doit commencer et se terminer sur un projet.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 10%

---

# Présentation de la contrainte de tâche

Les contraintes de tâche déterminent à quel moment une tâche doit commencer et se terminer sur un projet.

## Présentation des contraintes de tâche

Lorsque vous créez le plan de votre projet, vous prenez des décisions sur la séquence et la période de vos tâches sur le projet. Les tâches peuvent fonctionner indépendamment de n’importe quelle séquence de tâches, mais elles peuvent avoir un impact sur la chronologie du projet. Les contraintes de tâche permettent à un chef de projet de planifier le moment où certaines tâches peuvent démarrer ou se terminer sur un projet.

Selon la contrainte que vous utilisez, vous devrez peut-être spécifier une date de début planifiée, une date de fin planifiée ou les deux pour la tâche.

Les types de contraintes qui nécessitent des dates définies ont un impact sur les relations de prédécesseur.

>[!TIP]
>
>Envisagez d’utiliser un type de contrainte qui ne nécessite pas de dates spécifiques si vous utilisez des relations de prédécesseur entre des tâches.

Le tableau suivant affiche chaque contrainte et son abréviation. Les abréviations sont utilisées dans les listes de tâches et lors de la création de fichiers d&#39;import de démarrage rapide. Cliquez sur le titre associé de chaque contrainte de tâche pour plus d’informations sur ce type de contrainte.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Nom de la contrainte</strong> </p> </th> 
   <th> <p><strong>Abréviation</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Présentation de la contrainte de tâche : Dès Que Possible</a> </p> </td> 
   <td scope="col"> <p>ATôP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Présentation de la contrainte de tâche : Aussi Tard que possible </a> </p> </td> 
   <td scope="col"> <p>ATaP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Présentation de la contrainte de tâche : Heure disponible la plus tôt</a> </p> </td> 
   <td scope="col"> <p>PHD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Présentation de la contrainte de tâche : Dernière heure disponible</a> </p> </td> 
   <td scope="col"> <p>DHD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Présentation de la contrainte de tâche : Ne Commencer Pas Au Plus Tôt</a> </p> </td> 
   <td scope="col"> <p>CPTô</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Présentation de la contrainte de tâche : Ne pas démarrer plus tard que</a> </p> </td> 
   <td scope="col"> <p>CPTr</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Présentation de la contrainte de tâche : Terminer au plus tôt</a> </p> </td> 
   <td scope="col"> <p>FPTô</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Présentation de la contrainte de tâche : Terminer au plus tard</a> </p> </td> 
   <td scope="col"> <p>FPTr</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Présentation de la contrainte de tâche : Doit démarrer le</a> </p> </td> 
   <td scope="col"> <p>FC</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Présentation de la contrainte de tâche : Doit Terminer le</a> </p> </td> 
   <td scope="col"> <p>FF</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Présentation de la contrainte de tâche : Dates fixes</a> </p> </td> 
   <td> <p>FIXE</p> </td> 
  </tr> 
 </tbody> 
</table>

## Présentation des contraintes par défaut

Lorsque vous créez des tâches, une contrainte de tâche est automatiquement sélectionnée par Workfront.

Workfront utilise deux variables pour décider quelle contrainte de tâche est sélectionnée par défaut pour une nouvelle tâche :

* Le **Planification du projet à partir de** sur le projet.

   Pour plus d’informations sur le champ Planifier le projet à partir de , voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* Le **Date de début** la préférence configurée par votre administrateur Workfront ou de groupe dans la variable **Tâches et problèmes** area of **Configuration**.

   Pour plus d’informations sur les préférences de tâches et de problèmes, voir la section &quot;Nouvelles valeurs par défaut de la tâche&quot; dans [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Le tableau suivant affiche la contrainte de tâche par défaut lors du choix de différentes variables pour votre projet et vos nouvelles tâches :

| Planification du projet à partir de | Date de début de la tâche | Valeur par défaut de la contrainte de tâche |
|---|---|---|
| Date de début | En fonction de la date prévue de projet | Aussi Tôt Que Possible |
| Date de début | Aujourd’hui | Commencer Au Plus Tôt |
| Date d&#39;achèvement | En fonction de la date prévue de projet | Aussi tard que possible |
| Date d&#39;achèvement | Aujourd’hui | Commencer Au Plus Tard |
