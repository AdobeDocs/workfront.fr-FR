---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Suivi des coûts
description: Vous pouvez effectuer le suivi des coûts des projets, tâches et problèmes dans Adobe Workfront.
author: Alina, Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 1%

---

# Suivi des coûts

Vous pouvez effectuer le suivi des coûts des projets, tâches et problèmes dans Adobe Workfront.

## Comment Workfront calcule les coûts

Pour effectuer le suivi des coûts, vous devez associer les utilisateurs et les rôles de tâche aux taux de coût horaires.

Les taux de coût horaires sont des montants de coûts par unité de travail associée aux rôles de travail ou aux utilisateurs. Le fait de multiplier les taux par les heures passées au travail génère des coûts pour vos projets, tâches ou problèmes.

Les scénarios suivants existent :

* Si le type de coût de vos tâches est Heure de l’utilisateur, le taux horaire de l’utilisateur calcule les coûts de la tâche et du projet.

  Pour plus d’informations sur l’association des utilisateurs aux taux de coût, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Si le type de coût de vos tâches est Rôle horaire, le taux horaire du rôle calcule les coûts de la tâche et du projet.

  Pour plus d’informations sur l’association de rôles de tâche aux taux de coût, voir [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront calcule uniquement le coût réel pour les problèmes et les problèmes qui n’ont pas de type de coût. Pour plus d’informations, voir la section [Suivi des coûts par Workfront pour les problèmes](#how-workfront-tracks-costs-for-issues) dans cet article.

>[!TIP]
>
>Vous ne pouvez pas remplacer les taux de coût des projets. Une fois que vous avez défini le coût par heure sur un rôle d’utilisateur ou de tâche, ce taux calcule tous les coûts du système.

## Index de performances des coûts Workfront

Workfront calcule un certain nombre d’index de performances des coûts pour les projets, de sorte que les projets puissent faire l’objet d’un suivi en vue d’optimiser leur rentabilité.\
Pour plus d’informations sur le calcul des index de coûts-performances, voir :

* [Calculer l’indice de performance des coûts (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calcul de l’index de performance de la planification des coûts (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calcul de l’index de performance de planification (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Suivi des coûts par Workfront pour les tâches et les projets

* [Suivi des coûts par Workfront](#how-workfront-tracks-costs)
* [Comment Workfront calcule les coûts prévus, budgétaires et réels](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Méthode de calcul des types de coûts par Workfront pour les tâches](#how-workfront-calculates-cost-types-for-tasks)

### Suivi des coûts par Workfront  {#how-workfront-tracks-costs}

Vous pouvez effectuer le suivi de plusieurs types de coûts pour les tâches et les projets dans Workfront. Les coûts globaux sont calculés par la formule suivante :

`Costs = Labor Costs + Expense Costs`

* **Coûts du travail** sont associées aux heures sur les tâches et les projets et aux taux de coût par heure des ressources associées aux tâches. En règle générale, Workfront calcule les coûts de main-d’oeuvre suivants :

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Coûts du travail prévus</td> 
     <td> <p>Elles sont calculées à l'aide de la formule suivante :</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Coûts du travail budgétés</td> 
     <td> <p>Elles sont calculées à l'aide de la formule suivante :</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Coûts de main-d’oeuvre réels</td> 
     <td> <p>Elles sont calculées à l'aide de la formule suivante :</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations, voir [Comment Workfront calcule les coûts prévus, budgétaires et réels](#how-workfront-calculates-planned-budgeted-and-actual-costs) dans cet article.

* **Coûts de la dépense** sont associés aux dépenses sur les projets et les tâches.\
  Lorsque vous créez un projet, vous pouvez définir les dépenses prévues pour l’ensemble du projet. De plus, vous pouvez associer des dépenses à des tâches nouvelles ou existantes. Pour plus d’informations, voir [Gestion des dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Coûts fixes** sont définies comme un montant fixe de coût pour un projet. Il fait partie du coût planifié du projet, qui représente le montant d’argent dont vous avez besoin pour terminer le projet.

  >[!TIP]
  >
  >Lors de l’association d’un modèle à un projet, le coût fixe d’un modèle est ajouté au coût fixe du projet. Pour plus d’informations, voir [Présentation de l’association d’un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Comment Workfront calcule les coûts prévus, budgétaires et réels {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront calcule le coût planifié et le coût réel de chaque tâche d’un projet. Workfront utilise ces calculs pour les tâches individuelles afin de calculer le coût planifié et le coût réel du projet.

* [Coûts prévus](#planned-cost)
* [Coût budgété](#budgeted-cost)
* [Coûts réels](#actual-cost)

#### Coûts prévus {#planned-cost}

Le coût planifié d’un projet est le coût associé au travail planifié (heures planifiées) sur le projet.

Le Coût planifié d&#39;un projet est calculé selon la formule suivante :

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Par exemple, vous avez les dépenses suivantes dans l&#39;onglet Dépenses d&#39;une tâche : une dépense marketing de 100 € et une dépense administrative de 50 €. Dans l&#39;onglet Finance, sélectionnez le type de coût Heure de l&#39;utilisateur . Un utilisateur est affecté à la tâche et son taux horaire est de 15 $. L’utilisateur est chargé de travailler 5 heures sur cette tâche. Dans l&#39;onglet Dépenses du projet, vous avez un coût prévisionnel de 100 $ pour une dépense appelée Conseils. Vous avez également un coût fixe de 200 $ pour le projet.

Le coût planifié du projet est calculé comme suit :

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

Le taux horaire dans la formule prend en compte toute modification du taux en vigueur à la date.

#### Coût budgété {#budgeted-cost}

Le Coût budgété d&#39;un projet est le coût associé au travail budgété (Heures budgétisées) sur le projet.

Le coût budgété du projet est le même que le coût planifié du projet si les deux conditions suivantes sont remplies :

* Les heures planifiées des tâches du projet correspondent aux heures budgétisées (dans le planificateur de ressources)
* La tâche Type de facturation de la tâche est Rôle horaire.

Le coût budgété du projet est calculé à l&#39;aide de la formule ci-dessous si les conditions suivantes sont remplies :

* Les heures planifiées des tâches du projet ne correspondent pas aux heures budgétisées (dans le planificateur de ressources)
* Le type de facturation des tâches est Rôle Heure.

Lorsque les conditions ci-dessus sont remplies, Workfront calcule le coût budgété du projet à l’aide de la formule suivante :

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Coûts réels {#actual-cost}

Le coût réel d’un projet est le coût associé au travail réel (heures enregistrées) sur le projet.

Le coût réel est calculé à l&#39;aide de la formule suivante :

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Par exemple, vous avez les dépenses suivantes dans l&#39;onglet Dépenses d&#39;une tâche : une dépense marketing dont le coût réel est de 110 €, et une dépense administrative dont le coût réel est de 40 €. Vous sélectionnez le type de coût Heure du rôle et attribuez le rôle de tâche de consultant à la tâche. Le taux d’occupation du rôle de consultant est de 15 $ par heure et il y a 6 heures de connexion à la tâche pour le rôle de consultant. Une dépense de conseil est associée au projet (dans l&#39;onglet Dépenses ), avec un coût réel de 100 euros et un utilisateur avec un taux de coût par heure de 20 euros dans son profil utilisateur consigne 10 heures sur le projet. Vous avez également un coût fixe de 200 $ pour le projet.

Le coût réel du projet est calculé comme suit :

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

Le taux horaire dans la formule prend en compte toute modification du taux en vigueur à la date.

>[!NOTE]
>
>Le coût réel des dépenses du projet est calculé comme suit :
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Ces coûts ne sont pas dupliqués dans le calcul du coût réel. Par exemple, si un coût fixe fait partie du coût réel du projet, il n’est pas ajouté séparément au coût réel.

>[!NOTE]
>
>Lors de la connexion à un projet, les scénarios suivants existent lors du calcul du coût réel de la main-d’oeuvre pour le projet :
>
>* Par défaut, Workfront utilise le taux de coût par heure de l’utilisateur pour calculer le coût réel de la main-d’oeuvre.
>* Si l’utilisateur qui consigne l’heure n’est associé à aucun coût, Workfront utilise le taux de coût par heure du rôle de Principal de l’utilisateur.
>* Si votre administrateur Workfront a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** dans la zone Préférences Heures et Heures , et le temps de connexion de l’utilisateur sur le projet sélectionne un rôle différent à associer à ce moment, le coût réel du projet calcule en fonction du rôle spécifié lorsque les heures ont été enregistrées. Pour plus d’informations sur l’activation de la durée de journalisation pour un rôle de tâche spécifique, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### Méthode de calcul des types de coûts par Workfront pour les tâches {#how-workfront-calculates-cost-types-for-tasks}

Les coûts prévus et réels des tâches et leurs coûts de main-d’oeuvre sont déterminés par le type de coût de chaque tâche.

Vous pouvez configurer le type de coût pour des tâches individuelles dans le projet. Chaque type de coût affecte les valeurs Coût planifié et Coût réel .

Pour plus d’informations sur la modification du type de coût d’une tâche, voir [Mettre à jour le type de coût de tâche](../../../manage-work/tasks/task-information/update-task-cost-type.md).

Le tableau suivant décrit les types de coûts de tâche disponibles dans Workfront :

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Type de coût de tâche</strong> </p> </th> 
   <th> <p><strong>Description</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Utilisateur, par heure</p> </td> 
   <td> <p>Il s’agit du type de coût par défaut lorsque vous créez une tâche.</p> <p><strong>Coût planifié</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Lorsque le coût de la main-d’oeuvre planifiée est calculé comme suit :<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Note: <p>Tenez compte des impacts suivants de l’utilisation du type de coût horaire de l’utilisateur et du calcul du coût planifié :</p> 
     <ul> 
      <li>Si vous attribuez plusieurs ressources à une tâche, Workfront ajuste les calculs du coût planifié en fonction du pourcentage de la tâche affectée à chaque ressource.</li>
      <li>Pour les taux de coût en vigueur à la date, le coût du Travail planifié est la somme des coûts prévus pour chaque période couverte par la tâche.</li>
      <li>La valeur du champ Coût planifié peut différer selon que vous affichez le coût planifié à partir de la tâche elle-même ou du rapport Utilisation .<br><strong>Lors de l’affichage du coût planifié à partir de la tâche elle-même :</strong> Le champ Coût planifié prend en compte le champ Coût/heure défini au niveau Rôle de la tâche (lorsque le champ Coût/heure n’a pas été défini au niveau de l’utilisateur).<br><strong>Lors de l’affichage du coût planifié dans le rapport Utilisation du projet :</strong> Le champ Coût planifié ne prend pas en compte le champ Coût/heure défini au niveau Rôle de la tâche. Au lieu de cela, si vous souhaitez que le rapport Utilisation prenne en compte le champ Coût/heure défini au niveau Rôle de la tâche, vous devez définir le Type de coût de la tâche sur Horaire du rôle. </li> 
     </ul> </p> <p><strong>Coût réel</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Où le coût réel de la main-d’oeuvre est calculé par :</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Par exemple, un utilisateur a un taux de coût par heure de 20 € dans son profil. Lorsqu’il consigne 5 heures pour une tâche, le coût réel du travail est de 100 $ pour cette tâche. Si l’utilisateur n’est associé à aucun taux de coût par heure, le coût réel est calculé en fonction du taux de coût par heure de son rôle de tâche Principal. Si le taux de coût par heure de leur rôle professionnel n’est pas défini, alors le coût réel de la tâche est nul. </p> <p>Remarque : les coûts réels sont calculés en fonction du taux de coût par heure pour l’utilisateur qui consigne l’heure, indépendamment de qui est affecté à la tâche. En outre, le taux de facturation horaire dans la formule prend en compte toute modification du taux en vigueur à la date.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rôle par heure</p> </td>
   <td> <p><strong>Coût planifié</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Où le coût du travail planifié de la tâche est calculé comme suit :</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Remarque : si vous affectez plusieurs ressources à une tâche, Workfront ajuste les calculs pour les Heures planifiées en fonction du pourcentage de la tâche affectée à chaque ressource. En outre, le taux horaire dans la formule prend en compte toute modification du taux en vigueur à la date.</p> <p><strong>Coût réel</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Où le coût réel de la main-d’oeuvre de la tâche est calculé comme suit :</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Par exemple, une tâche est affectée à un rôle de tâche ou à un utilisateur avec un rôle de tâche pour lequel le taux de coût par heure est de 20 €. Lorsqu’un utilisateur consigne 5 heures pour une tâche, le coût réel du travail est de 100 $ pour cette tâche. Si l’utilisateur affecté à la tâche n’a pas de rôle de tâche associé à la tâche, le coût réel est calculé en fonction du taux Coût par heure de son rôle de tâche Principal. Si le taux de coût par heure de leur rôle professionnel n’est pas défini, alors le coût réel de la tâche est nul. </p> <p>Note:   <p> La tâche Heures réelles d’un rôle Heure est calculée en fonction des rôles de tâche des utilisateurs associés à la tâche, et non des rôles associés à l’utilisateur qui consigne l’heure. En outre, le taux de facturation horaire dans la formule prend en compte toute modification du taux en vigueur à la date.</p> <p>Si votre administrateur Workfront a activé la variable <strong>Affecter manuellement des rôles de tâche aux entrées d’heure</strong> dans la zone Préférences Heures et Heures , et le temps de connexion de l’utilisateur à la tâche sélectionne un autre rôle à associer à cette heure, la tâche Coût réel d’un rôle Heure calcule en fonction du rôle spécifié lorsque les heures ont été enregistrées. Pour plus d’informations sur l’activation de la durée de journalisation pour un rôle de tâche spécifique, voir l’article <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configuration des préférences de feuille de temps et d’heure</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fixe par heure</p> </td> 
   <td> <p><strong>Coût planifié</strong> est calculé selon la formule suivante :</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Où le coût de main-d’oeuvre de la tâche est calculé par :</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Coût réel</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Où le coût réel de la main-d’oeuvre de la tâche est calculé par :</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Ce type de coût ne prend pas en compte les utilisateurs individuels ni les rôles de tâche.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aucun coût</p> </td> 
   <td> <p>Ce type de coût n’a aucune incidence sur les coûts. Si une tâche parente possède ce type de coût, les sous-tâches avec un autre type de coût sont calculées en fonction de leurs types de coûts individuels, et le coût de la tâche parente est affecté en conséquence. </p> <p>Lorsqu’un utilisateur n’ayant pas accès aux données financières ou qu’un utilisateur ne disposant pas d’autorisations financières sur un modèle crée un projet à partir de ce modèle, il s’agit du type de coût par défaut pour les tâches du projet.</p> <p>Pour plus d’informations sur l’accès aux données financières, consultez l’article . <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l'accès aux données financières</a>.</p> <p>Pour plus d’informations sur les autorisations financières relatives aux objets, reportez-vous à l’article <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Partage des autorisations financières sur un objet</a>.</p> <p>Pour plus d’informations sur la création de projets à partir de modèles, reportez-vous à l’article <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Créer un projet à l’aide d’un modèle</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Suivi des coûts par Workfront pour les problèmes {#how-workfront-tracks-costs-for-issues}

Les problèmes n’ont pas et n’affectent pas les types de coûts suivants sur un projet :

* Coûts prévus
* Coût budgété

Les problèmes peuvent, toutefois, avoir une **Coût réel** qui affecte également le coût réel du projet.

Le tableau suivant explique comment le coût réel est calculé pour les problèmes, en fonction du type d’affectation sur le problème :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">Coût réel du problème</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attribution des utilisateurs</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Coût réel</strong> est calculé selon la formule suivante :</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Le taux de coût par heure de l’utilisateur qui consigne l’heure est pris en compte ici, indépendamment de qui est affecté au problème. </p> <p>Si le profil de l’utilisateur qui consigne l’heure n’a pas de taux Coût par heure, le taux Coût par heure de son rôle de tâche Principal calcule le coût réel du problème. Si l’utilisateur qui consigne l’heure n’a aucun rôle dans son profil ou aucun taux associé, les Heures réelles sont calculées à l’aide du taux Coût par heure du rôle de tâche par Principal de la personne désignée par Principal sur le problème. Si aucun taux n’est défini pour ce rôle, le coût réel de l’émission est nul. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attribution des rôles</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Coût réel</strong> est calculé selon la formule suivante :</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>Le taux de coût par heure de l’utilisateur consignant le temps passé sur le problème est pris en compte ici, quel que soit le rôle attribué au problème. </p> <p>Si l’utilisateur qui enregistre l’heure n’est pas associé à un taux de coût par heure, le taux de coût par heure de son rôle de Principal calcule le coût réel de l’émission.<br>Si l’utilisateur qui consigne l’heure n’a aucun rôle dans son profil ou qu’aucun taux ne lui est associé, le coût réel de l’émission est nul. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aucune affectation</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Coût réel</strong> est calculé selon la formule suivante :</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Si l’utilisateur qui consigne l’heure n’a pas de taux Coût par heure associé à son profil, le taux Coût par heure de son rôle de tâche Principal calcule le coût réel de l’émission. </p> <p>Si l’utilisateur qui consigne l’heure n’a aucun rôle de tâche associé à son profil ou si son rôle de tâche Principal n’a pas de taux de coût par heure défini, le coût réel de l’émission est nul. </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
