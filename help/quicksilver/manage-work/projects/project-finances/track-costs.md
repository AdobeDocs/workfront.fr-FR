---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Suivre les coûts
description: Vous pouvez suivre les coûts des projets, des tâches et des problèmes dans Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: d431ae178a157522e2b5d8d963da7b0623510d28
workflow-type: tm+mt
source-wordcount: '2480'
ht-degree: 100%

---

# Suivre les coûts

<!-- Audited: 02/2024 -->

Vous pouvez suivre les coûts des projets, des tâches et des problèmes dans Adobe Workfront.

## Calculer les coûts dans Workfront

Pour assurer le suivi des coûts, vous devez associer des utilisateurs et utilisatrices et des fonctions à des taux de coûts horaires.

Les taux de coûts horaires sont des montants de coûts par unité de travail, associés à des fonctions ou à des utilisateurs et utilisatrices. En multipliant les taux par les heures consacrées au travail, vous obtenez les coûts de vos projets, tâches ou problèmes.

Les scénarios suivants sont possibles :

* Si le type de coût de vos tâches est le taux horaire de la personne, ce taux calcule les coûts de la tâche et du projet.

  Pour plus d’informations sur l’association de personnes à des taux de coûts, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Si le type de coût de vos tâches est Rôle horaire, le taux horaire de la fonction calcule les coûts de la tâche et du projet.

  Pour plus d’informations sur l’association de fonctions à des taux de coûts, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront ne calcule que le coût réel pour les problèmes, et les problèmes n’ont pas de type de coût. Pour plus d’informations, voir la section [Suivi des coûts pour les problèmes dans Workfront](#how-workfront-tracks-costs-for-issues) dans cet article.

>[!TIP]
>
>Vous ne pouvez pas remplacer les taux de coûts pour les projets. Lorsque vous avez établi le taux du coût horaire d’une personne ou d’une fonction, ce taux calcule tous les coûts dans le système.

## Indices de performances des coûts Workfront

Workfront calcule un certain nombre d’indices de performances en matière de coûts pour les projets, ce qui permet de suivre ces projets en termes de rentabilité.\
Pour plus d’informations sur le calcul des indices coûts-performances, voir :

* [Calculer l’indice Coûts Performances (ICP)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calculer l’indice de performances de la planification des coûts (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calculer l’indice de performances de planification (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Suivi des coûts des tâches et des projets dans Workfront

Les types de coûts sont calculés différemment pour les tâches et pour les projets.

### Suivi des coûts dans Workfront {#how-workfront-tracks-costs}

Vous pouvez suivre plusieurs types de coûts pour les tâches et les projets dans Workfront. Les coûts globaux sont calculés selon la formule suivante :

`Costs = Labor Costs + Expense Costs`

* Les **coûts de main-d’œuvre** sont associés aux heures passées sur les tâches et les projets et aux taux de coût horaire des ressources associées aux tâches. En règle générale, Workfront calcule les coûts de main-d’œuvre suivants :

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Coûts prévus de la main-d’œuvre</td> 
     <td> <p>Ils sont calculés à l’aide de la formule suivante :</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Coûts budgétés de la main-d’œuvre</td> 
     <td> <p>Ils sont calculés à l’aide de la formule suivante :</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Coûts réels de la main-d’œuvre</td> 
     <td> <p>Ils sont calculés à l’aide de la formule suivante :</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations, consultez la section [Calcul des coûts planifiés, budgétés et réels dans Workfront](#how-workfront-calculates-planned-budgeted-and-actual-costs) de cet article.

* Les **coûts des dépenses** sont associés aux dépenses des projets et des tâches.\
  Lorsque vous créez un projet, vous pouvez définir des dépenses prévues pour l’ensemble du projet. En outre, vous pouvez associer des dépenses à des tâches nouvelles ou existantes. Pour plus d’informations, voir [Gérer les dépenses des projets](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Les **coûts fixes** sont définis comme un montant fixe de coûts pour un projet. Ils font partie du coût prévu du projet, qui représente la somme d’argent dont vous avez besoin pour mener à bien le projet.

  >[!TIP]
  >
  >Lorsque vous attachez un modèle à un projet, le coût fixe du modèle est ajouté au coût fixe du projet. Pour plus d’informations, voir [Vue d’ensemble de l’attachement d’un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Calcul des coûts planifiés, budgétés et réels dans Workfront {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront calcule le coût prévu et le coût réel de chaque tâche individuelle d’un projet. Il utilise ces calculs sur les tâches individuelles pour établir le coût prévu et le coût réel du projet.

#### Coûts prévus {#planned-cost}

Le coût prévu d’un projet est le coût associé au travail prévu (heures prévues) sur le projet.

Le coût prévu d’un projet est calculé à l’aide de la formule suivante :

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Par exemple, vous avez les dépenses suivantes dans l’onglet Dépenses d’une tâche : une dépense de marketing de 100 $ et une dépense de marketing de 50 $. Dans l’onglet Finance, vous sélectionnez le type de coût horaire de l’utilisateur ou de l’utilisatrice. Un utilisateur ou une utilisatrice est affecté à la tâche et son taux horaire est de 15 $. L’utilisateur ou l’utilisatrice est affecté à cette tâche pour une durée de 5 heures. Dans l’onglet Dépenses du projet, vous avez un coût prévu de 100 $ pour une dépense appelée Conseils. Vous avez également un coût fixe de 200 $ pour le projet.

Le coût prévu du projet est calculé comme suit :

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

Le taux horaire de la formule tient compte de toute modification du taux à compter de la date d’entrée en vigueur.

#### Coût budgété {#budgeted-cost}

Le coût budgété d’un projet est le coût associé au travail budgété (heures budgétées) sur le projet.

Le coût budgété du projet est identique au coût prévu du projet si les deux conditions suivantes sont remplies :

* Le nombre d’heures prévues des tâches du projet correspond aux heures budgétées (dans le planificateur de ressources).
* Le type de facturation des tâches est Rôle horaire.

Le coût budgété du projet est calculé à l’aide de la formule ci-dessous si les conditions suivantes sont remplies :

* Le nombre d’heures prévues des tâches du projet ne correspond pas aux heures budgétées (dans le planificateur de ressources).
* Le type de facturation des tâches est Rôle horaire.

Lorsque les conditions ci-dessus sont remplies, Workfront calcule le coût budgété du projet à l’aide de la formule suivante :

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Coûts réels {#actual-cost}

Le coût réel d’un projet est le coût associé au travail réel (heures consignées) sur le projet.

Le coût réel est calculé à l’aide de la formule suivante :

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Par exemple, vous avez les dépenses suivantes dans l’onglet Dépenses d’une tâche : une dépense de marketing avec un coût réel de 110 $ et une dépense administrative avec un coût réel de 40 $. Vous sélectionnez le type de coût Rôle horaire et affectez la fonction de consultant à la tâche. Le taux de la fonction de consultant est de 15 $ par heure, et il y a 6 heures consignées sur la tâche pour la fonction de consultant. Une dépense de conseils est associée au projet (dans l’onglet Dépenses), avec un coût réel de 100 $, et un utilisateur ou une utilisatrice avec un taux de coût horaire de 20 $ dans son profil utilisateur/utilisatrice consigne 10 heures sur le projet. Vous avez également un coût fixe de 200 $ pour le projet.

Le coût réel du projet est calculé comme suit :

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

Le taux horaire de la formule tient compte de toute modification du taux à compter de la date d’entrée en vigueur.

>[!NOTE]
>
>Le coût réel des dépenses du projet est calculé comme suit :
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Ces coûts ne sont pas dupliqués dans le calcul du coût réel. Par exemple, si un coût fixe fait partie du coût réel du projet, il n’est pas ajouté séparément au coût réel.

>[!NOTE]
>
>Lors de la consignation des heures de travail sur un projet, les scénarios suivants se présentent lors du calcul du coût réel de main-d’œuvre pour le projet :
>
>* Par défaut, Workfront utilise le taux de coût horaire de l’utilisateur ou de l’utilisatrice pour calculer le coût réel de main-d’oeuvre.
>* Si l’utilisateur ou l’utilisatrice qui consigne l’heure n’est associé à aucun coût, Workfront utilise le taux de coût horaire du rôle principal de l’utilisateur ou de l’utilisatrice.
>* Si votre administrateur ou administratrice Workfront a activé le paramètre **Attribuer manuellement des fonctions à des saisies d’heures** dans la zone Préférences en matière d’heures et de feuilles de temps lors de la configuration, et que l’utilisateur ou l’utilisatrice qui consigne des heures sur le projet sélectionne un rôle différent à associer à ces heures, le coût réel du projet est calculé sur la base du rôle spécifié lors de la consignation des heures. Pour plus d’informations sur l’activation de la consignation des heures pour une fonction spécifique, voir l’article [Configurer les préférences en matière de feuilles de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### Calcul des types de coûts pour les tâches dans Workfront {#how-workfront-calculates-cost-types-for-tasks}

Les coûts prévus et réels des tâches et leurs coûts de main-d’œuvre sont déterminés par le type de coût de chaque tâche.

Vous pouvez configurer le type de coût pour des tâches individuelles au sein du projet. Chaque type de coût affecte les valeurs des coûts prévus et réels.

Pour plus d’informations sur la manière de modifier le type de coût d’une tâche, voir [Mettre à jour le type de coût d’une tâche](../../../manage-work/tasks/task-information/update-task-cost-type.md).

Le tableau suivant décrit les types de coûts de tâche disponibles dans Workfront :

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>Type de coût de tâche</strong> </p> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>Utilisateur, par heure</p> </td> 
   <td> <p>Il s’agit du type de coût par défaut lorsque vous créez une tâche.</p> <p>Le <strong>coût prévu</strong> est calculé à l’aide de la formule suivante : </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Le coût prévu de main-d’œuvre est calculé par :<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Note : <p>Considérez les impacts suivants de l’utilisation du type de coût horaire de l’utilisateur ou de l’utilisatrice et du calcul du coût prévu :</p> 
     <ul> 
      <li>Si vous attribuez plusieurs ressources à une tâche, Workfront ajuste les calculs du coût prévu en fonction du pourcentage de la tâche attribuée à chaque ressource.</li>
      <li>Pour les taux de coûts effectifs par date, le coût prévu de main-d’œuvre est la somme des coûts prévus de chaque période couverte dans la tâche.</li>
      <li>La valeur du champ Coût prévu peut être différente selon que vous affichez le coût prévu à partir de la tâche elle-même ou à partir du rapport d’utilisation.<br><strong>Lors de l’affichage du coût prévu à partir de la tâche elle-même :</strong> le champ Coût prévu prend en considération le champ Coût/heure défini au niveau de la fonction (lorsque le champ Coût/heure n’a pas été défini au niveau de l’utilisateur ou de l’utilisatrice).<br><strong>Lors de l’affichage du coût prévu dans le rapport d’utilisation du projet :</strong> le champ Coût prévu ne prend pas en compte le champ Coût/heure défini au niveau de la fonction. En revanche, si vous souhaitez que le rapport d’utilisation prenne en compte le champ Coût/heure défini au niveau de la fonction, vous devez définir le type de coût de la tâche sur Rôle horaire. </li> 
     </ul> </p> <p><strong>Le coût réel</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Le coût réel de main-d’œuvre est calculé selon la formule suivante :</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Par exemple, un utilisateur ou une utilisatrice a un coût horaire de 20 $ dans son profil. Lorsqu’il ou elle enregistre 5 heures pour une tâche, le coût réel de main-d’œuvre de la tâche est de 100 $. Si l’utilisateur ou l’utilisatrice n’est pas associé à un coût horaire, le coût réel est calculé sur la base du coût horaire de sa fonction principale. Si il ou elle n’a pas de fonction ou si le coût horaire de sa fonction n’est pas défini, le coût réel de la tâche est égal à zéro. </p> <p>Remarque : les coûts réels sont calculés sur la base du coût horaire de l’utilisateur ou de l’utilisatrice qui enregistre le temps, quelle que soit la personne affectée à la tâche. En outre, le taux horaire de facturation dans la formule tient compte de toute modification du taux à compter de la date d’entrée en vigueur.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rôle par heure</p> </td>
   <td> <p><strong>Le coût prévu</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Le coût prévu de main-d’œuvre de la tâche est calculé selon la formule suivante :</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Remarque : si vous affectez plusieurs ressources à une tâche, Workfront ajuste les calculs du nombre d’heures prévues en fonction du pourcentage de la tâche affectée à chaque ressource. En outre, le taux horaire de la formule tient compte de toute modification du taux à compter de la date d’entrée en vigueur.</p> <p><strong>Le coût réel</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Le coût réel de main-d’œuvre de la tâche est calculé selon la formule suivante :</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Par exemple, une tâche est assignée à une fonction ou à un utilisateur ou une utilisatrice ayant une fonction pour laquelle le coût horaire est de 20 $. Lorsqu’un utilisateur ou une utilisatrice enregistre 5 heures pour une tâche, le coût réel de main-d’œuvre de la tâche est de 100 $. Si l’utilisateur ou l’utilisatrice affecté à la tâche n’a pas de fonction associée à la tâche, le coût réel est calculé sur la base du coût horaire de sa fonction principale. Si il ou elle n’a pas de fonction ou si le coût horaire de sa fonction n’est pas défini, le coût réel de la tâche est égal à zéro. </p> <p>Remarque : les heures effectives d’une tâche de rôle horaire sont calculées par rapport aux fonctions des utilisateurs et utilisatrices associés à la tâche, et non par rapport aux fonctions associées à l’utilisateur ou utilisatrice qui enregistre le temps. En outre, le taux horaire de facturation dans la formule tient compte de toute modification du taux à compter de la date d’entrée en vigueur.</p> <p>Si votre administrateur ou administratrice Workfront a activé le paramètre <strong>Attribuer des fonctions à des entrées horaires manuellement</strong> dans la zone Préférences en matière des feuilles de temps et des heures dans Configuration, et que l’utilisateur ou l’utilisatrice qui enregistre les heures sur la tâche sélectionne une fonction différente à associer à ces heures, le coût réel d’une tâche de rôle par heure se calcule sur la base de la fonction spécifiée lors de l’enregistrement des heures. Pour plus d’informations sur l’activation de l’enregistrement des heures pour une fonction spécifique, voir l’article <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurer les préférences en matière de feuilles de temps et d’heures</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fixe par heure</p> </td> 
   <td> <p><strong>Le coût prévu</strong> est calculé selon la formule suivante :</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Le coût de main-d’œuvre de la tâche est calculé selon la formule suivante :</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Le coût réel</strong> est calculé selon la formule suivante : </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Le coût réel de main-d’œuvre de la tâche est calculé selon la formule suivante :</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Ce type de coût ne prend pas en compte les utilisateurs et utilisatrices individuels et les fonctions.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aucun coût</p> </td> 
   <td> <p>Ce type de coût n’affecte pas les coûts. Si une tâche parent a ce type de coût, les sous-tâches ayant un autre type de coût sont calculées en fonction de leur type de coût individuel, et le coût de la tâche parent est affecté en conséquence. </p> <p>Lorsqu’un utilisateur ou une utilisatrice n’ayant pas accès aux données financières ou n’ayant pas d’autorisations financières sur un modèle crée un projet à partir de ce modèle, il s’agit du type de coût par défaut pour les tâches du projet.</p> <p>Pour plus d’informations sur l’accès aux données financières, voir l’article <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l’accès aux données financières</a>.</p> <p>Pour plus d’informations sur les autorisations financières sur les objets, voir l’article <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Partager les autorisations financières sur un objet</a>.</p> <p>Pour plus d’informations sur la création de projets à partir de modèles, voir l’article <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Créer un projet à l’aide d’un modèle</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Suivi des coûts des problèmes dans Workfront {#how-workfront-tracks-costs-for-issues}

Les problèmes n’ont pas et n’affectent pas les types de coûts suivants sur un projet :

* Coûts prévus
* Coût budgété

Les problèmes peuvent toutefois avoir un **coût réel** qui influe également sur le coût réel du projet.

Le tableau suivant explique comment le coût réel est calculé pour les problèmes, en fonction du type d’affectation du problème :

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>Affectation des utilisateurs et utilisatrices</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Le coût réel</strong> est calculé selon la formule suivante :</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Le taux de coût horaire de l’utilisateur ou de l’utilisatrice qui enregistre l’heure est pris en compte ici, quelle que soit la personne affectée au problème. </p> <p>Si l’utilisateur ou l’utilisatrice qui enregistre l’heure n’a pas de taux de coût horaire dans son profil, le taux de coût horaire de sa fonction principale est utilisé pour le calcul du coût réel du problème.</p> <p>Si l’utilisateur ou l’utilisatrice qui enregistre l’heure ne dispose pas de rôle dans son profil ou de taux associé à celui-ci, les heures réelles sont calculées en utilisant le taux de coût horaire de la fonction principale de la personne principale affectée au problème. Si cette fonction n’a pas de taux défini, le coût réel du problème est égal à zéro. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affectation des rôles</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Le coût réel</strong> est calculé selon la formule suivante :</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>Le taux de coût horaire de l’utilisateur ou de l’utilisatrice qui enregistre l’heure de ce problème est pris en compte ici, quel que soit le rôle affecté à ce problème. </p> <p>Si l’utilisateur ou l’utilisatrice qui enregistre l’heure ne dispose pas d’un taux de coût horaire associé, le taux de coût horaire de sa fonction principale est utilisé pour calculer le coût réel du problème.</p><p>Si l’utilisateur ou l’utilisatrice qui enregistre l’heure n’a pas de rôle dans son profil ou ne dispose pas de taux associé à celui-ci, le coût réel du problème est zéro. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aucune affectation</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Le coût réel</strong> est calculé selon la formule suivante :</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Si l’utilisateur ou l’utilisatrice qui enregistre l’heure ne dispose pas de taux de coût horaire associé à son profil, le taux de coût horaire de sa fonction principale est utilisé pour calculer le coût réel du problème. </p> <p>Si l’utilisateur ou l’utilisatrice qui enregistre l’heure n’a pas de fonction associée à son profil ou si sa fonction principale n’a pas de taux de coût horaire défini, le coût réel du problème est égal à zéro. </p> </td> 
  </tr> 
 </tbody> 
</table>
