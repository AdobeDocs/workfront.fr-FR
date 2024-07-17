---
content-type: overview
product-area: projects
navigation-topic: financials
title: Vue d’ensemble de la facturation et du revenu
description: En tant que chef de projet, vous pouvez utiliser les taux de facturation pour capturer les recettes de vos projets.
author: Alina, Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: c485676fb5584e8438823e9ce0c28b551f6bab45
workflow-type: tm+mt
source-wordcount: '3691'
ht-degree: 1%

---

# Vue d’ensemble de la facturation et du revenu

<!-- Audited: 1/2024 -->

{{highlighted-preview}}

En tant que chef de projet, vous pouvez utiliser les taux de facturation pour capturer les recettes de vos projets.

Cet article décrit le suivi des recettes pour les projets. Les recettes sont calculées différemment dans le rapport d’utilisation. Pour plus d’informations sur les calculs des recettes dans le rapport d’utilisation, voir [Affichage des informations sur l’utilisation des ressources](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Présentation des taux de facturation

Tenez compte des points suivants lorsque vous utilisez des taux de facturation :

* Vous avez besoin d’une licence Plan ou Standard avec l’accès Modifier aux données financières pour gérer les taux de facturation.\
  Pour plus d’informations sur l’octroi de l’accès aux données financières, voir [Octroi de l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Les taux de facturation correspondent aux recettes par unité de travail associée aux rôles de travail ou aux utilisateurs.

  Le fait de multiplier les taux par les heures passées au travail génère des recettes pour vos projets.

* Après avoir établi vos taux de facturation, vous pouvez effectuer le suivi des recettes en créant des enregistrements de facturation afin d’enregistrer ce qui a été facturé ou n’a pas été facturé.

  >[!TIP]
  >
  >Lorsque vous marquez un enregistrement de facturation comme Facturé, il ne peut jamais être modifié. Ceci est important lorsque vos taux varient et que vous souhaitez verrouiller les informations de recettes et de dépenses sur votre projet. L’ajouter à un enregistrement de facturation et le marquer comme Facturé empêche sa mise à jour lors de la mise à jour des taux dans votre système.

  Pour plus d’informations sur la création d’enregistrements de facturation, consultez l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

* Vous pouvez créer des taux de facturation pour les utilisateurs, les rôles de tâche ou un taux de facturation unique pour un projet ou une tâche.

>[!IMPORTANT]
>
>Les taux qui calculent les recettes appartiennent à l’utilisateur qui consigne l’heure ou à son rôle de tâche.

* [Taux de facturation des utilisateurs](#user-billing-rates)
* [Taux de facturation des rôles de tâche](#job-role-billing-rates)
* [Taux de facturation fixes pour les projets ou les tâches](#fixed-billing-rates-for-projects-or-tasks)
* [Remplacer les taux de facturation](#override-billing-rates)

### Taux de facturation des utilisateurs {#user-billing-rates}

En tant qu’administrateur utilisateur, lorsque vous créez un utilisateur, vous pouvez l’associer à des taux de facturation à date effective en spécifiant les valeurs des champs Facturation par heure et les dates des taux.

Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir l’article [Ajouter des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

![Modifier les taux de facturation et de coût utilisateur](assets/edit-user-cost-billing-rate-1.png)

### Taux de facturation des rôles de tâche {#job-role-billing-rates}

En tant qu’administrateur Adobe Workfront, lorsque vous créez un rôle de tâche, vous pouvez l’associer aux taux de facturation en vigueur par date en spécifiant les valeurs des champs Facturation par heure et les dates des taux.

Vous pouvez définir la valeur d’un taux de facturation de rôle de tâche à l’aide de la devise de base de votre système Workfront ou à l’aide d’une autre devise personnalisée.

Pour plus d’informations sur la création de rôles de tâche et le remplacement de leur devise, consultez l’article [Créer et gérer des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

![Modifier les taux de facturation et le coût du rôle de tâche](assets/edit-job-role-multiple-billing-rates-new.png)

### Taux de facturation fixes pour les projets ou les tâches {#fixed-billing-rates-for-projects-or-tasks}

Outre les taux horaires d’utilisation et de rôle de tâche, vous pouvez également avoir les taux de facturation fixes suivants :

* Montant fixe pour le type de revenu horaire fixe
* Montant fixe pour le type de revenu fixe

Pour plus d’informations sur l’utilisation des taux de facturation fixes pour calculer les recettes, voir [Présentation des types de recettes de la tâche](#overview-of-task-revenue-types).

### Remplacer les taux de facturation {#override-billing-rates}

>[!IMPORTANT]
>
>Vous pouvez remplacer les taux de facturation associés aux rôles de tâche. Vous ne pouvez pas remplacer les taux de facturation des utilisateurs ou les taux fixes.

Vous pouvez remplacer les taux de facturation des rôles de tâche pour :

* Une société spécifique

  Pour plus d’informations sur la création de taux de facturation des rôles de tâche spécifiques à une entreprise, voir [Création et modification d’entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Un projet spécifique

  Pour plus d’informations sur la création de taux de facturation des rôles de tâche spécifiques à un projet, reportez-vous à l’article [Présentation du remplacement des taux de facturation des rôles de tâche et du calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Suivi des recettes

Workfront peut effectuer automatiquement le suivi des recettes planifiées lorsque des tâches sont créées en fonction des heures planifiées des tâches.

Il peut également effectuer automatiquement le suivi des recettes réelles lorsque les heures réelles sont consignées sur les tâches, les problèmes et le projet.

Le tableau suivant indique les types de recettes associés aux tâches, problèmes et projets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Revenus prévus</td> 
   <td> <p>Pour les tâches, il s’agit des recettes associées aux Heures planifiées des tâches. Les Heures planifiées de toutes les tâches sont cumulées aux Heures planifiées du projet pour contribuer au calcul des Heures planifiées du projet. </p> <p>Pour plus d’informations sur les heures planifiées dans Workfront, consultez la <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">présentation des heures planifiées</a>. </p> <ul><li><p>Workfront calcule les Recettes prévues pour les tâches à l’aide de cette formule :</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><strong>REMARQUE</strong></br> Le taux de facturation horaire dans la formule prend en compte toute modification du taux en vigueur à la date.</p> </li><li><p>Workfront calcule les recettes prévues pour les projets à l’aide de la formule suivante :</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>NOTE</b>

<p>Les recettes prévues du projet, qui s’affichent dans la zone Détails du projet et dans les rapports du projet, diffèrent des recettes prévues qui s’affichent dans le rapport Utilisation . </p></li></ul> <p>La zone Recettes planifiées dans les détails du projet reflète les recettes de la tâche associées aux heures planifiées de la tâche ainsi que les recettes fixes du projet. Le rapport Recettes planifiées du rapport Utilisation affiche les Recettes planifiées associées uniquement aux Heures planifiées des affectations de tâche du projet. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Si le projet comporte une tâche de 10 heures, affectée à un consultant avec un taux horaire de 20 $ et que le projet a un chiffre d’affaires fixe de 100 $, le rapport Utilisation affiche 200 $ pour les recettes planifiées (le chiffre d’affaires planifié associé aux heures de la tâche). La section Détails du projet affiche 300 $ (les recettes planifiées de la tâche et les recettes fixes du projet). </p> 
     </div> </p> <p>Tâche Les recettes planifiées sont calculées à l’aide des taux de facturation horaires des utilisateurs ou des rôles de tâche affectés aux tâches. Le type de chiffre d’affaires des tâches influence le taux (utilisateur ou rôle) utilisé pour le calcul des recettes planifiées. Pour plus d’informations, reportez-vous aux sections suivantes de cet article :</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Présentation des types de recettes de la tâche</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref"> Calculs de recettes pour les tâches en fonction des affectations d’utilisateur et de rôle</a> </p> </li> 
    </ul> <p>Pour plus d’informations sur les calculs des recettes planifiées dans le rapport Utilisation, voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Affichage des informations sur l’utilisation des ressources</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Recettes réelles*</td> 
   <td> <p>Recettes associées aux Heures réelles des tâches, des problèmes et des projets. </p> <p>En règle générale, Workfront calcule les recettes réelles à l’aide de cette formule :</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><strong>REMARQUE</strong></br> Le taux de facturation horaire dans la formule prend en compte toute modification du taux en vigueur à la date.</p> <p>Pour plus d’informations sur les calculs des recettes réelles dans le rapport d’utilisation, voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Affichage des informations sur l’utilisation des ressources</a>. </p> <p><b>CONSEIL</b>

Vous ne pouvez pas afficher les recettes réelles au niveau du problème, mais les recettes associées aux heures réelles sur les problèmes contribuent aux recettes réelles du projet. </p> </td>
</tr> 
 </tbody> 
</table>

*Pour les heures réelles, les taux de l’utilisateur se rapportent toujours à l’utilisateur qui consigne les heures ou aux taux de ses rôles de tâche. Pour plus d’informations sur le moment où Workfront utilise les taux de l’utilisateur et celui où il utilise les taux de ses rôles de tâche, consultez la section [Calculs de recettes](#revenue-calculations) de cet article.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Par exemple, si une tâche avec le type de revenu horaire de l’utilisateur est planifiée sur 2 heures et que l’utilisateur qui lui est affecté a un taux horaire de 30 $ de l’heure, le revenu planifié de la tâche est de 60 $. Lorsque la tâche est terminée, si l’utilisateur ne consigne que 1,5 heure comme temps réel passé à terminer la tâche, le montant des recettes réelles est de 45 $. Si un autre utilisateur qui n’est pas affecté à la tâche consigne l’heure, les Recettes réelles sont calculées en fonction des taux de facturation de cet utilisateur.

Vous pouvez enregistrer les recettes comme suit :

* En définissant le Type de revenu de vos tâches et en associant les utilisateurs ou les rôles affectés aux tâches aux taux de facturation. Cela calcule les recettes en fonction du montant des heures planifiées ou réelles sur les éléments de travail. Vous pouvez définir une limite sur le montant maximal facturé pour les taux horaires, ou non.\
  Pour plus d’informations sur la spécification du type de recette d’une tâche, voir l’article [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Facturation d’un taux de recettes fixe fixe fixe uniforme pour les tâches ou les projets.\
  Si vous avez des tâches avec des recettes fixes, le montant des recettes fixes sera ajouté en tant que recettes planifiées d’une tâche ou d’un projet, et les recettes planifiées d’une tâche pourront être ajoutées à un enregistrement de facturation en tant que recettes fixes.
* En définissant un taux de facturation fixe fixe pour un projet, puis en définissant des taux horaires pour les tâches du projet. Workfront ajoute les taux horaires des tâches au taux fixe du projet.\
  Par exemple, un mécanicien utilisant Workfront peut saisir un coût pour les pièces comme revenu fixe pour le projet, puis facturer toutes les heures le temps passé à réparer une voiture. Correction des recettes sur les projets ou les tâches qui sont alors réalisées à la fin de l’opération.

Vous pouvez également marquer vos tâches comme &quot;Non facturable&quot;, auquel cas aucune recette planifiée ou réelle n’est associée.

## Présentation des types de recettes de la tâche {#overview-of-task-revenue-types}

Par défaut, le Type de revenu de toutes les nouvelles tâches est défini en fonction des Préférences de tâche et de problème spécifiées par votre administrateur Workfront ou de groupe.\
Pour plus d’informations sur la définition de la tâche et des préférences de problème pour votre instance Workfront, consultez l’article [Configuration de la tâche à l’échelle du système et des préférences de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Le propriétaire du projet peut modifier le type de chiffre d’affaires des tâches et les recettes fixes des projets.\
Pour plus d’informations sur la spécification des recettes fixes d’un projet, consultez l’article [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).\
Pour plus d’informations sur la spécification du type de recette d’une tâche, voir l’article [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Vous pouvez appliquer les types de recettes suivants à vos tâches ou projets :

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Type de revenu</strong> </p> </th> 
   <th> <p><strong>Description</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Revenus fixes</p> </td> 
   <td> <p>Ce type peut être utilisé avec des projets et des tâches. </p> <p>Lors de l’association d’un modèle à un projet, les recettes fixes du modèle sont ajoutées aux recettes fixes du projet. Pour plus d’informations, voir <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Présentation de l’association d’un modèle à un projet</a>. </p> <p>Pour les tâches, quelles que soient les affectations de tâche, les recettes de la tâche sont toujours calculées à l’aide du montant fixe spécifié pour la tâche. </p> <p>Les tâches Recettes fixes provenant des enfants sont cumulées aux Recettes de la tâche parent, puis aux recettes du projet. Si un montant fixe est défini sur la tâche parent et/ou le projet, le montant est ajouté aux recettes planifiées cumulées à partir de n’importe quelle tâche enfant.</p> <p>Le montant des recettes fixes sur les tâches peut être inclus dans un enregistrement de facturation sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur, par heure</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches. </p> <p>Le taux de facturation que vous définissez pour un utilisateur spécifique multiplié par le nombre d’ Heures planifiées pour cette tâche devient le montant des Recettes planifiées de la tâche. Le taux de facturation que vous définissez pour un utilisateur spécifique multiplié par le nombre d’heures que l’utilisateur consigne par rapport à la tâche est le montant des recettes réelles de la tâche. <br>Par exemple, lorsque vous créez un utilisateur et que vous définissez 20 € pour son champ Facturation par heure , puis que l’utilisateur envoie 5 heures pour une tâche sur la feuille de temps, le montant de facturation réel de la tâche est de 100 €.</p>
   <p>Un profil utilisateur peut contenir plusieurs taux de facturation avec des dates d’entrée en vigueur. Par exemple, le premier taux de facturation utilisateur de 20 € s’achève le 30 avril 2023 et le second, de 25 €, commence le 1er mai 2023. Si l’utilisateur envoie 2 heures le 28 avril et 3 heures le 2 mai pour une tâche, alors le montant de facturation réel de la tâche est de 40 $ + 75 $ = 115 $.</p>
   <p><b>CONSEIL</b>

Il s’agit du type de recette par défaut lorsque vous créez une tâche.</p> </td>
</tr> 
  <tr> 
   <td> <p>Rôle par heure</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Ce type est similaire à Heure de l’utilisateur , mais utilise des taux de rôle de tâche plutôt que des taux d’utilisation.</p> <p><strong>REMARQUE</strong><br>Un rôle de tâche peut également avoir plusieurs taux de facturation avec des dates d’entrée en vigueur.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Heure de l’utilisateur avec limite</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Les tâches sont facturées toutes les heures comme dans l’option Heure de l’utilisateur, mais vous pouvez spécifier un montant de limite maximal. <br>Par exemple, si le taux de facturation d’un utilisateur est de 25 $, mais que le montant limite de la tâche est de 20 $ et que l’utilisateur consigne une heure, le chiffre d’affaires réel de la tâche est de 20 $. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rôle Horaire avec limite</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Ce type est similaire à Heure de l’utilisateur avec casquette , mais utilise des taux de rôle de tâche plutôt que des taux d’utilisation. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur, par heure plus fixe</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches. </p> <p>Les tâches sont facturées toutes les heures comme dans l’option Heure de l’utilisateur, mais disposent d’un montant fixe que vous pouvez ajouter au taux de l’utilisateur. Le montant fixe spécifié pour la tâche peut être inclus dans les enregistrements de facturation du projet. Le montant fixe n’est pas multiplié par les heures de la tâche. Seul le taux de facturation de l’utilisateur le fait. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rôle par heure plus fixe</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches. </p> <p>Les tâches sont facturées toutes les heures comme dans l’heure du rôle, mais vous disposez d’un montant fixe supplémentaire que vous pouvez ajouter au taux de rôle. Le montant fixe spécifié pour la tâche peut être inclus dans les enregistrements de facturation du projet. Le montant fixe n’est pas multiplié par les heures de la tâche. Seul le taux de facturation des rôles de tâche le fait. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fixe par heure</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Le plafond ou montant fixe que vous définissez pour la tâche multiplié par le nombre d’heures renseigné par rapport à la tâche (indépendamment de l’utilisateur ou de son rôle de tâche) est le montant de facturation.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Non facturable</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Ce type de revenu n’a aucun effet sur les recettes. </p> <p>Si un objet parent possède ce paramètre, les tâches enfants avec un type de facturation continueront de s’appliquer normalement.</p> <p>Lorsqu’un utilisateur n’ayant pas accès aux données financières ou qu’il n’a pas d’autorisations financières sur un modèle crée un projet à partir de ce modèle, il s’agit du type de recettes par défaut pour les tâches du projet.</p> <p>Pour plus d'informations sur l'accès aux données financières, consultez l'article <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l'accès aux données financières</a>.<br>Pour plus d’informations sur les autorisations financières sur les objets, consultez l’article <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Présentation des autorisations de partage sur les objets</a>.<br>Pour plus d’informations sur la création de projets à partir de modèles, reportez-vous à l’article <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Création d’un projet à l’aide d’un modèle</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Présentation des recettes pour les tâches parentes

Si vous changez une tâche autonome avec des informations de facturation sur celle-ci en un parent, la nouvelle tâche parente conserve les informations de facturation qui lui ont été précédemment appliquées, ainsi que les heures précédemment appliquées. Toutes les informations de facturation provenant des heures enregistrées dans les tâches enfants seront cumulées comme Recettes réelles à la nouvelle tâche parente.

Les recettes planifiées des tâches enfants sont également cumulées à la tâche parent.

## Présentation des recettes pour les problèmes

Les problèmes ne comportent pas de montants de recettes planifiées ou réelles, mais ils peuvent avoir un coût réel.

Si vous enregistrez les heures pour un problème et que vous utilisez un type d’heure marqué &quot;Compter comme recettes&quot;, Workfront calcule alors un montant de coût réel en fonction du taux de l’utilisateur qui se connecte au moment. Ce nombre est ajouté au coût réel du projet. Les heures peuvent également être incluses dans un enregistrement de facturation.

Pour plus d&#39;informations sur le suivi des coûts, consultez l&#39;article [Tracker les coûts](../../../manage-work/projects/project-finances/track-costs.md).

Pour plus d’informations sur les types d’heures, consultez l’article [Gérer les types d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Calculs de recettes

* [Calcul des recettes pour les tâches basées sur les affectations d’utilisateur et de rôle](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Calcul des recettes pour les tâches basées sur les affectations d’utilisateur et de rôle {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Pour calculer les recettes d’une tâche, tenez compte des points suivants :

* Si un utilisateur ou un rôle de tâche affiche un taux de 0,00 $, Workfront le lit comme un montant valide et multipliera ce montant par le nombre d’heures de la tâche pour calculer le chiffre d’affaires. Si vous souhaitez n’afficher aucune recette pour vos tâches, assurez-vous que le champ correspondant au taux de facturation de votre utilisateur ou rôle de tâche est vide.
* Lorsque les taux de facturation des rôles de tâche s’appliquent, Workfront utilise le taux de remplacement au niveau du projet, au lieu du taux de facturation pour ce rôle défini au niveau du système chaque fois qu’un taux de remplacement se produit sur le projet.
* Dans le cas des recettes réelles, si le rôle de l’utilisateur ou de la tâche comporte plusieurs taux de facturation avec des dates de validité, les recettes de la tâche sont la somme des recettes de chaque période au cours de laquelle l’utilisateur a consigné l’heure. Les recettes planifiées sont basées sur les heures planifiées des périodes.
* Dans le cas de plusieurs personnes désignées sur les tâches, les scénarios décrits ci-dessous s’appliquent à chaque personne désignée.

Il existe une hiérarchie dont le taux est utilisé dans les calculs des recettes en fonction des affectations de tâche.

Si votre administrateur Workfront a activé manuellement le paramètre **Attribuer les rôles de tâche aux entrées d’heure** dans la zone Préférences de la feuille de temps et des heures, et que l’heure de connexion de l’utilisateur sur le projet sélectionne un rôle différent à associer à cette heure, le revenu réel de la tâche ou du projet calcule toujours en fonction du rôle associé à l’entrée d’heure. Pour plus d’informations sur l’activation de la durée de journalisation pour un rôle de tâche spécifique, consultez l’article [Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Les scénarios suivants existent lors du calcul des recettes de la tâche en fonction du type de recettes et de la nature de l’affectation de la tâche :

* **Le type de revenu de la tâche est User Hourly**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure</td> 
     <td>Aucune affectation</td> 
     <td>Affectation d’utilisateur</td> 
     <td>Affectation de rôle de tâche</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les recettes prévues</td> 
     <td>0,00 $</td> 
     <td> Si un utilisateur a un taux de facturation dans son profil, ce taux est utilisé pour calculer les recettes prévues. Dans le cas contraire, le taux de facturation système de leur rôle de tâche principale est utilisé. <br><p><b>REMARQUE</b> L’utilisateur peut être affecté à la tâche avec l’un de ses rôles de tâche secondaires, mais le taux du rôle de tâche principal est utilisé ici à la place.</p><p>Si le rôle de l’utilisateur a changé au cours de l’affectation, les taux corrects sont appliqués lorsque les finances du projet sont recalculées.</p></td> 
     <td><p><span class="preview">Si une carte de taux est jointe au projet, les recettes planifiées sont calculées en fonction du rôle de tâche figurant dans la carte de taux.</span></p> <p><span class="preview">Les taux de facturation peuvent être remplacés au niveau du projet.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les recettes réelles</td> 
     <td>Si le profil de l’utilisateur qui consigne les heures comporte un taux de facturation, ce taux est utilisé. 
     <br><span class="preview">Lorsque l’heure est consignée pour un utilisateur ou un rôle ayant une affectation spécifique à un emplacement dans les affectations avancées, le taux de l’emplacement est utilisé.</span>
     <br>Dans le cas contraire, le taux de facturation de leur rôle de tâche principale est utilisé. Si aucun taux de facturation n’est associé à l’utilisateur ou à son rôle principal, le chiffre d’affaires réel est de 0,00 $. <br><p><b>NOTE</b>

  Seuls les taux associés à l&#39;utilisateur qui enregistre le temps sont pris en compte pour le calcul, même lorsqu&#39;un autre utilisateur est affecté à la tâche.</p></td>
  <td>Si le profil de l’utilisateur qui consigne les heures comporte un taux de facturation, ce taux est utilisé. <br><span class="preview">Lorsque l’heure est consignée pour un utilisateur ou un rôle ayant une affectation spécifique à un emplacement dans les affectations avancées, le taux de l’emplacement est utilisé.</span><br>Dans le cas contraire, le taux de facturation de leur rôle de tâche principale est utilisé. Si aucun taux de facturation n’est associé à l’utilisateur ou à son rôle principal, le chiffre d’affaires réel est de 0,00 $. <br><p><b>NOTE</b>

  Seuls les taux associés à l&#39;utilisateur qui enregistre le temps sont pris en compte pour le calcul, même lorsqu&#39;un autre utilisateur est affecté à la tâche.</p></td>
  <td>Si le profil de l’utilisateur qui consigne les heures comporte un taux de facturation, ce taux est utilisé. Dans le cas contraire, le taux de facturation de leur rôle de tâche principale est utilisé.<br><p><b>NOTE</b>

  Si le temps de journalisation de l’utilisateur n’est associé à aucun taux de facturation et qu’il n’y a pas de rôle de tâche ni de taux de facturation pour son rôle de tâche, le taux du rôle de tâche associé à la tâche est utilisé. S’il n’y a pas de taux de facturation pour ce rôle, les recettes sont de 0,00 $</p></td>
  </tr> 
   </tbody> 
  </table>

* **Le type de revenu de la tâche est Rôle Heure**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure</td> 
     <td>Aucune affectation</td> 
     <td>Affectation d’utilisateur</td> 
     <td>Affectation de rôle de tâche</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les recettes prévues</td> 
     <td>0,00 $</td> 
     <td><p>Workfront examine le rôle de la tâche que l’utilisateur remplit pour calculer les recettes planifiées. <br>Si l’utilisateur n’est associé à aucun rôle dans la tâche, le chiffre d’affaires est de 0,00 $.</p> <p><strong>REMARQUE</strong><br>Si le rôle de l’utilisateur a changé au cours de l’affectation, les taux corrects sont appliqués lorsque les finances du projet sont recalculées.</p> </td> 
     <td><p><span class="preview">Si une carte de taux est jointe au projet, les recettes planifiées sont calculées en fonction du rôle de tâche figurant dans la carte de taux.</span></p> <p><span class="preview">Les taux de facturation peuvent être remplacés au niveau du projet.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les recettes réelles</td> 
     <td>Workfront utilise le taux de facturation du rôle de tâche principal de l’utilisateur consignant l’heure. <br><span class="preview">Lorsque l’heure est consignée pour un utilisateur ou un rôle ayant une affectation spécifique à un emplacement dans les affectations avancées, le taux de l’emplacement est utilisé.</span> <br>Si l’utilisateur qui consigne l’heure n’a aucun rôle de tâche associé ou si le rôle de tâche principal n’a pas de taux de facturation, le chiffre d’affaires réel est de 0,00 $. </td> 
     <td> Si l’utilisateur qui consigne l’heure est affecté à la tâche, le taux de facturation du rôle de tâche associé à l’utilisateur sur la tâche est utilisé pour calculer les Recettes réelles. <br><span class="preview">Lorsque l’heure est consignée pour un utilisateur ou un rôle ayant une affectation spécifique à un emplacement dans les affectations avancées, le taux de l’emplacement est utilisé.</span> <br>Dans le cas contraire, le taux de facturation de leur rôle de tâche principal est utilisé. Si l’utilisateur n’a pas de rôle de tâche principal ou si son rôle de tâche principal n’a pas de taux de facturation, le chiffre d’affaires réel est de 0,00 $. </td> 
     <td>Si l’un des rôles de tâche de l’utilisateur qui enregistre la durée est affecté à la tâche, ce taux de rôle de tâche est utilisé. Si le rôle de tâche attribué à la tâche n’est pas associé à l’utilisateur qui enregistre l’heure, le taux de facturation du rôle principal de l’utilisateur est utilisé pour calculer les Recettes réelles. Si l’utilisateur n’a pas de rôle de tâche ou qu’aucun taux n’est associé à son rôle de tâche principal, le taux du rôle de tâche affecté à la tâche est utilisé. </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### Calcul des recettes pour les projets

Vous pouvez effectuer le suivi des types de recettes suivants pour les projets :

* Les recettes planifiées d’un projet sont calculées selon la formule suivante :

  `Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue`

  Pour plus d’informations sur le mode de calcul des recettes planifiées d’une tâche, voir la section [Calculs de recettes pour les tâches basées sur les affectations d’utilisateurs et de rôles](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) de cet article.

* Les recettes réelles d’un projet sont calculées à l’aide de la formule suivante :

  `Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)`

Pour plus d’informations sur le mode de calcul des recettes réelles de la tâche, reportez-vous à la section [Calculs de recettes pour les tâches basées sur les affectations d’utilisateurs et de rôles](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) de cet article.

Pour les recettes réelles associées aux heures enregistrées directement dans le projet ou aux problèmes, Workfront utilise le taux de facturation de l’utilisateur qui consigne l’heure sur le projet. Si aucun taux de facturation n’est associé à son profil, Workfront utilise le taux de facturation de son rôle de tâche de Principal. Si les deux taux sont nuls, le chiffre d’affaires réel associé aux heures enregistrées sur le projet ou aux problèmes est nul.
