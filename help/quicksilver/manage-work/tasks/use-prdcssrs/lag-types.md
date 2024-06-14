---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Vue d’ensemble des types de décalage
description: La durée correspond au temps qui doit s’écouler après la fin d’un prédécesseur appliqué jusqu’à ce que la tâche dépendante puisse commencer (Durée positive), ou au temps pendant lequel une tâche dépendante peut commencer avant le début du prédécesseur (Durée négative).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 3%

---

# Vue d’ensemble des types de décalage

<!-- Audited: 01/2024 -->

La durée correspond au temps qui doit s’écouler après la fin planifiée d’un prédécesseur jusqu’à ce que la tâche dépendante puisse commencer (Durée positive), ou au temps pendant lequel une tâche dépendante peut commencer avant le début du prédécesseur (Durée négative).

Les dates Prévues, Prévues et Estimées des tâches qui lui succèdent sont calculées en tenant compte des dates de retard et de planification, de projection et de début estimé (fin) des tâches précédentes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : formule </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour les tâches et le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Définition des types de balise et de balise sur les tâches

Vous pouvez indiquer des types de retard sur les tâches lorsque vous définissez leurs relations de prédécesseur.

### Définition des types de balises dans la section Prédécesseurs d’une tâche {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Accédez à une tâche pour laquelle vous souhaitez définir le prédécesseur et le Type de log.
1. Cliquez sur **Prédécesseurs** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis **Prédécesseurs**.
1. Cliquez sur **Ajouter un prédécesseur**.
1. (Facultatif) Si vous souhaitez ajouter un prédécesseur de plusieurs projets, remplacez la variable **Projet parent** par un autre projet.
1. Commencez à saisir le nom de la tâche de prédécesseur, puis sélectionnez-la lorsqu’elle apparaît dans la liste.
1. Sélectionnez la variable **Type de dépendance**.

   Pour plus d’informations sur les types de dépendance de prédécesseur, voir [Présentation des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Spécifiez un **Étiquette** quantité utilisant une valeur numérique. Vous pouvez indiquer des nombres négatifs pour indiquer un décalage négatif.
1. Sélectionnez l’une des options suivantes pour identifier le type de retard que vous souhaitez indiquer pour votre prédécesseur :

   * **Days**
   * **Jours calendaires**
   * **Pourcentage**
   * **Jour de la semaine**
   * **Jour de la semaine (non nul)**

     Pour plus d’informations sur ces types de balises et sur leur mode de calcul, consultez la section . [Types de balise](#lag-types) dans cet article.

1. Cliquer sur **Enregistrer**.

### Définition des types de balises dans une liste de tâches  {#indicate-lag-types-in-a-task-list}

1. Dans la liste des tâches, sélectionnez l’option **Standard** vue.

1. Cliquez dans le **Prédécesseurs** correspondant à la tâche pour laquelle vous souhaitez spécifier un prédécesseur et un montant de retard.
1. Renseignez les champs suivants sans espaces :

   * le nombre de tâches à indiquer comme prédécesseur de la tâche sélectionnée.
   * abréviation du type de dépendance à indiquer entre les tâches

     Pour plus d’informations sur les abréviations des types de dépendance, voir [Présentation des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * soit un **+** pour un décalage positif ou une **-** pour un décalage négatif

   * la quantité de retard ;
   * abréviation du type de balise que vous souhaitez utiliser

     Pour plus d’informations sur les abréviations des types de balises, voir la section . [Types de balise](#lag-types) dans cet article.

   Par exemple, pour indiquer qu’une tâche a un prédécesseur et un décalage positif de 2 jours, vous devez saisir `1fs+2d` dans la colonne Prédécesseurs .

1. Appuyez sur Entrée du clavier pour enregistrer les modifications apportées à votre tâche.

## Types de balise {#lag-types}

Un exemple de tâche qui nécessiterait un temps de retard peut être de scier des arbres dans du bois. Si le bois fraîchement coupé doit sécher pendant un certain temps avant de pouvoir être coupé, il y aurait un temps de retard entre couper les arbres et les scier dans du bois.

Le tableau suivant illustre les types de balises et indique comment indiquer la durée de chacune d’elles :

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
   <td> <p>Jours (j ou de)</p> </td> 
   <td> <p>Le délai entre deux tâches liées par une dépendance est mesuré en jours de travail. Il s’agit du type de balise par défaut. </p> <p>Par exemple, s’il existe une dépendance de départ avec un décalage de 2 jours ouvrés et que la tâche du prédécesseur se termine le vendredi, la tâche dépendante commence le mercredi. Les jours du week-end ne comptent pas dans le décalage. </p> <p>Remarque : La limite de délai maximale pour les jours est de 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Jours calendaires (c ou ce)</p> </td> 
   <td> <p>Le délai entre deux tâches est mesuré en jours calendaires, notamment les jours fériés et les week-ends. </p> <p>Remarque : bien que ce type de délai comptabilise les jours non ouvrés dans le délai, une tâche dépendante ne peut jamais commencer un jour non ouvré. Si ce type de décalage permet au début de la tâche dépendante d'un jour non ouvré, la Date de début planifiée de la tâche dépendante est planifiée le jour ouvré suivant. </p> <p>Par exemple, s’il existe une dépendance de début de fin avec un décalage de 2 jours calendaires et que la tâche précédente se termine le jeudi, la tâche dépendante commence le lundi au lieu d’un dimanche. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Pourcentage (p ou pe)</p> </td> 
   <td> <p>Le délai est exprimé sous la forme d’un pourcentage du temps estimé pour terminer la tâche précédente. </p> <p>Par exemple, s’il existe une dépendance arrivée-début avec un décalage de 20 % par rapport à une tâche de prédécesseur de 10 jours, le système calcule le nombre de jours représentant 20 % de la durée de la tâche du prédécesseur et l’utilise comme décalage. Dans ce cas, cela prendrait 2 jours après la fin de la tâche. </p>

<p><b>NOTE</b></p> La limite de retard maximale pour le pourcentage est de 2 000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Jour de la semaine (w ou we) </p> </td> 
   <td> <p>Le délai entre deux tâches est mesuré en indiquant les jours de la semaine pour lesquels la date de fin planifiée du prédécesseur contient la date de fin planifiée.</p> <p>Pour ce type de balise, chaque jour de la semaine est associé à un nombre :</p> 
    <ul> 
     <li>Dimanche=1</li> 
     <li>Lundi=2</li> 
     <li>Mardi=3</li> 
     <li>Mercredi=4</li> 
     <li>Jeudi=5</li> 
     <li>Vendredi=6</li> 
     <li>samedi=7</li> 
    </ul> <p>Si vous souhaitez indiquer que la Date de début planifiée du successeur doit être un mardi de la semaine en cours et que le mardi est antérieur à la Date de fin planifiée du prédécesseur, vous devez coder votre successeur avec la formule suivante : </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>NOTE</b></p>

Si la Date de début du successeur est calculée pour correspondre à un certain mardi et ce jour passé pour la semaine en cours, la Date de début planifiée de la tâche successeur est le même jour (mardi) de la semaine suivante, si disponible. </p> <p>Si vous souhaitez indiquer que le retard doit tomber un samedi de la semaine en cours et que le samedi se situe après la date d’achèvement prévue du prédécesseur, vous devez coder votre successeur avec la formule suivante :</p> <p><code>4fs+7w</code> </p> <p>Si le samedi est un jour sans travail, le lendemain disponible après le samedi (pour indiquer un décalage positif) est sélectionné comme Date de début planifiée du successeur. </p>

<p>Cela ne s’applique pas aux exceptions de planification. Si une date est également une exception de planning et que la Date de début du successeur est calculée pour correspondre à ce jour, le système tente alors de trouver la date disponible la plus proche, qui est le jour de la semaine spécifié dans l'expression du prédécesseur.</p>

<p>Par exemple, si la Date de début est calculée pour correspondre à un certain mardi et que ce jour est une exception de planification et que le décalage du prédécesseur est positif, il choisira le mardi suivant (s’il s’agit également d’un jour ouvré) comme Date de début du successeur. Si le décalage est négatif, le système choisit le mardi précédent comme Date de début.</p>

<p>Pour indiquer les semaines passées ou futures, vous pouvez ajouter un nombre devant le numéro du jour pour le type de décalage. </p> <p>Par exemple, pour indiquer le lundi de 10 semaines auparavant, vous pouvez utiliser ce code pour indiquer le prédécesseur de votre successeur :</p> <p><code>4fs-102w</code> </p> <p>10 indique il y a 10 semaines et 2 est le numéro attribué à lundi. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Jour de la semaine non nul (k ou ke)</p> </td> 
   <td> <p>Le délai entre deux tâches est mesuré de la même manière que le type de décalage Jour de la semaine , sauf si l’heure du prédécesseur se termine le même jour de la semaine spécifié. Le délai est ensuite calculé sur la semaine adjacente (+/-). </p> <p>Dans ce cas, le délai ne peut jamais être de 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Balise négative

Vous pouvez utiliser une balise négative pour indiquer la nécessité ou la capacité de la tâche de commencer avant la fin de la tâche précédente.

Tenez compte des règles suivantes lorsque vous utilisez des indicateurs négatifs :

* Le journal négatif ne peut pas forcer les dates de Début/Fin d’une tâche à être avant ou après les dates de Début/Fin planifiées du projet. Ces dates sont spécifiées dans le champ Planifier à partir du du projet.

  Dans ce cas, tenez compte des points suivants :

   * Planifiez le projet à partir de la date d’achèvement.
   * La dernière tâche du projet doit utiliser la contrainte Doit se terminer sur la tâche . Il est recommandé de donner à la tâche une durée suffisante pour tenir compte de toutes les tâches du projet. Les autres tâches fonctionnent bien avec la contrainte Dès que possible .

* L’utilisation d’une relation de prédécesseur Finish-Start avec des tâches peut générer un message d’erreur.

  Dans ce cas, tenez compte des points suivants :

   * Définissez une relation de prédécesseur Finish-Finish entre les tâches.
   * La Durée de la tâche qui lui succède doit être égale ou supérieure au nombre prévu de jours de retard entre les tâches.
