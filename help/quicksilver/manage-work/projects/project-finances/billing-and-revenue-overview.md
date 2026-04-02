---
content-type: overview
product-area: projects
navigation-topic: financials
title: Vue d’ensemble de la facturation et des revenus
description: En tant que personne responsable de projet, vous pouvez utiliser les taux de facturation pour générer des revenus sur vos projets.
author: Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '4542'
ht-degree: 73%

---

# Vue d’ensemble de la facturation et des revenus

<!-- Audited: 1/2024 -->

{{highlighted-preview}}

En tant que personne responsable de projet, vous pouvez utiliser les taux de facturation pour générer des revenus sur vos projets.

Cet article décrit le suivi des revenus pour les projets. Les revenus sont calculés différemment dans le rapport d’utilisation. Pour plus d’informations sur le calcul des revenus dans le rapport d’utilisation, voir [Afficher les informations sur l’utilisation des ressources](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Vue d’ensemble des taux de facturation

Tenez compte des éléments suivants lorsque vous travaillez avec des taux de facturation :

* Vous avez besoin d’une licence Plan ou Standard avec un accès en modification aux données financières (en particulier aux taux de facturation) afin de gérer les taux de facturation.
Pour plus d’informations sur l’octroi de l’accès aux données financières, voir [Octroyer l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Les taux de facturation sont des montants de revenus par unité de travail associés à des fonctions ou à des utilisateurs et utilisatrices.

  En multipliant les taux par les heures de travail, vous générez des revenus pour vos projets.

* Après avoir établi vos taux de facturation, vous pouvez suivre les revenus en créant des enregistrements de facturation pour enregistrer ce qui a été facturé et ce qui ne l’a pas été.

  >[!TIP]
  >
  >Lorsque vous marquez un enregistrement de facturation comme étant facturé, il ne peut jamais être modifié. C’est important lorsque vos taux varient et que vous souhaitez verrouiller les informations relatives aux revenus et aux dépenses de votre projet. Le fait de les ajouter à un enregistrement de facturation et de les marquer comme facturées les empêche d’être mises à jour lorsque les taux sont actualisés dans votre système.

  Pour plus d’informations sur la création d’enregistrements de facturation, voir l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

* Vous pouvez créer des taux de facturation pour les utilisateurs et utilisatrices, les fonctions, ou vous pouvez avoir un taux de facturation unique pour un projet ou une tâche.

>[!IMPORTANT]
>
>Les taux qui calculent les revenus appartiennent à l’utilisateur ou à l’utilisatrice qui consigne le temps ou à sa fonction.

### Taux de facturation par carte tarifaire

{{ultimate-package}}

Lorsque vous avez accès à la modification des cartes tarifaires, vous pouvez définir des cartes tarifaires avec plusieurs taux de facturation par rôle, en fonction d’attributs tels que le lieu, le groupe ou l’agence. Les attributs peuvent être configurés jusqu’à cinq niveaux.

Une carte tarifaire doit être associée à un projet pour que ses taux soient appliqués. Lorsqu’un taux est verrouillé sur la carte tarifaire, il ne peut pas être remplacé au niveau du projet.

Les taux des cartes tarifaires font partie de la hiérarchie permettant de déterminer les taux, en fonction du type de revenus de la tâche.

Pour plus d’informations sur la création de cartes tarifaires, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Pour plus d&#39;informations sur la hiérarchie des taux, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

![Exemple de carte tarifaire](assets/sample-rate-card-march2026.png)

### Taux de facturation des utilisateurs et utilisatrices {#user-billing-rates}

En tant qu’administrateur ou administratrice des utilisateurs et utilisatrices, lorsque vous créez un utilisateur ou une utilisatrice, vous pouvez l’associer à des taux de facturation avec date d’entrée en vigueur en spécifiant des valeurs pour les champs Facturation à l’heure et les dates des taux.

Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir l’article [Ajouter des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

![Modifier les coûts et les taux de facturation des utilisateurs et utilisatrices](assets/edit-user-cost-billing-rate-1.png)

### Taux de facturation des fonctions {#job-role-billing-rates}

En tant qu’administrateur ou administratrice Adobe Workfront, lorsque vous créez une fonction, vous pouvez l’associer à des taux de facturation effectifs à la date en spécifiant les valeurs de taux et les dates.

Vous pouvez définir la valeur du taux de facturation d’une fonction à l’aide de la devise de base de votre système Workfront ou d’une autre devise. Les devises supplémentaires doivent également être définies dans les taux de change de votre système.

Pour plus d’informations sur la création de fonctions, consultez l’article [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

![Modifier les coûts et les taux de facturation des fonctions](assets/edit-job-role-multiple-billing-rates-new.png)

### Taux de facturation fixes pour les projets ou les tâches {#fixed-billing-rates-for-projects-or-tasks}

Outre les taux horaires pour les utilisateurs, les utilisatrices et les fonctions, vous pouvez également appliquer les taux de facturation fixes suivants :

* Montant fixe pour le type de revenu Fixe par heure
* Montant fixe pour le type de revenu Revenus fixes

Pour plus d’informations sur la manière dont les taux de facturation fixes sont utilisés pour calculer les revenus, voir [Vue d’ensemble des types de revenus des tâches](#overview-of-task-revenue-types).

<div class="preview">

### Remplacer les taux de facturation - Package Ultimate de workflow

>[!IMPORTANT]
>
>Vous pouvez remplacer les taux de facturation associés aux fonctions ou aux utilisateurs au niveau du projet. Vous ne pouvez pas remplacer les taux fixes.

Au niveau du projet, vous pouvez :

* Remplacer un taux de facturation pour une fonction (avec des attributs appliqués, tels que l’emplacement, le groupe ou l’agence).
* Remplacer un taux de facturation pour un utilisateur spécifique sur ce projet.

Les remplacements du taux de facturation ne sont pas génériques. Par exemple, vous ne remplaceriez pas « Designer » en tant que rôle. Au lieu de cela, vous pouvez remplacer « Designer - New York - Agence X » pour la période de validité de date appropriée. Les remplacements respectent la hiérarchie des taux de facturation ; le système les applique donc toujours par ordre de priorité.

</div>

### Remplacer les taux de facturation - tous les autres packages

>[!IMPORTANT]
>
>Vous pouvez remplacer les taux de facturation associés aux fonctions. Vous ne pouvez pas remplacer les taux de facturation des utilisateurs et utilisatrices ou les taux fixes.

Vous pouvez modifier les taux de facturation des fonctions pour les éléments suivants :

* Entreprise spécifique

  Pour plus d’informations sur la création de taux de facturation de fonctions spécifiques à une entreprise, voir [Créer et modifier des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Projet spécifique

  Pour plus d’informations sur la création de taux de facturation des fonctions spécifiques à un projet, consultez l’article [Présentation du remplacement des taux de facturation et du calcul du revenu sur un projet](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Suivre les montants des revenus

Workfront peut suivre automatiquement les revenus prévus lorsque des tâches sont créées en fonction du nombre d’heures prévues de ces tâches.

Il peut également suivre automatiquement les revenus réels lorsque les heures effectives sont consignées pour les tâches, les problèmes et le projet.

Le tableau suivant présente les types de revenus associés aux tâches, aux problèmes et aux projets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Revenus prévus</td> 
   <td> <p>Pour les tâches, il s’agit des revenus associés au nombre d’heures prévues. Les heures prévues pour toutes les tâches sont ajoutées aux heures prévues pour le projet, pour contribuer au calcul des heures prévues pour le projet. </p> <p>Pour plus d’informations sur les heures prévues dans Workfront, voir la section <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Vue d’ensemble des heures prévues</a>. </p> <ul><li><p>Workfront calcule les revenus prévus pour les tâches à l’aide de cette formule :</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><strong>NOTE</strong></br> Le taux horaire facturé dans la formule tient compte de toute modification du taux à la date d’entrée en vigueur.</p> </li><li><p>Workfront calcule les revenus prévus pour les projets à l’aide de la formule suivante :</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>NOTE</b>

<p>Les revenus prévus pour le projet, qui s’affichent dans la zone Détails du projet et dans les rapports de projet, diffèrent des revenus prévus qui s’affichent dans le rapport d’utilisation. </p></li></ul> <p>Les revenus prévus dans la zone Détails du projet reflètent les revenus de la tâche associés aux heures prévues pour la tâche ainsi que les revenus fixes du projet. Les revenus prévus dans le rapport d’utilisation affichent les revenus prévus associés uniquement aux heures prévues des affectations de tâches sur le projet. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Si le projet comporte une tâche de 10 heures, affectée à une personne externe au taux horaire de 20 $ et que le projet a des revenus fixes de 100 $, le rapport d’utilisation affiche 200 $ pour les revenus prévus (les revenus prévus associés aux heures de la tâche). La section Détails du projet affiche 300 $ (les revenus prévus de la tâche et les revenus fixes du projet). </p> 
     </div> </p> <p>Les revenus prévus pour la tâche sont calculés en utilisant les taux horaires de facturation des utilisateurs et utilisatrices ou des fonctions affectées aux tâches. Le type de revenu des tâches influence le taux (utilisateur, utilisatrice ou rôle) utilisé pour calculer les revenus prévus. Pour plus d’informations, voir les sections suivantes de cet article :</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Vue d’ensemble des types de revenus des tâches</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Calculer des revenus pour les tâches en fonction de l’affectation des utilisateurs et utilisatrices et des rôles</a> </p> </li> 
    </ul> <p>Pour plus d’informations sur le calcul des revenus planifiés dans le rapport d’utilisation, voir la section <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Afficher les informations sur l’utilisation des ressources</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Revenus réels*</td> 
   <td> <p>Revenus associés aux heures effectives des tâches, des problèmes et des projets. </p> <p>En général, Workfront calcule les revenus réels à l’aide de cette formule :</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><strong>NOTE</strong></br> Le taux horaire facturé dans la formule tient compte de toute modification du taux à la date d’entrée en vigueur.</p> <p>Pour plus d’informations sur le calcul des revenus réels dans le rapport d’utilisation, voir la section <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Afficher les informations sur l’utilisation des ressources</a>. </p> <p><b>CONSEIL</b>

Vous ne pouvez pas afficher les revenus réels au niveau du problème, mais les revenus associés aux heures effectives sur les problèmes contribuent aux revenus réels du projet. </p> </td>
</tr> 
 </tbody> 
</table>

* Pour les heures effectives, les taux de l’utilisateur ou de l’utilisatrice concernent toujours la personne qui consigne les heures ou les taux de ses fonctions. Pour savoir à quel moment Workfront utilise les taux de l’utilisateur ou de l’utilisatrice et à quel moment où il utilise les taux de ses fonctions, voir la section [Calculs de revenus](#revenue-calculations) dans cet article.

Par exemple, si une tâche ayant un Type de revenus horaires de l’utilisateur ou de l’utilisatrice est prévue pour une durée de 2 heures et que la personne qui y est affectée a un taux horaire de 30 $, les revenus prévus de la tâche sont de 60 $. Lorsque la tâche est terminée, si l’utilisateur ou l’utilisatrice ne consigne que 1,5 heure comme temps réel passé sur la tâche, le montant des revenus réels est de 45 $. Si une autre personne, non affectée à la tâche, consigne le temps, les revenus réels sont calculés sur la base de ses taux de facturation.

Vous pouvez enregistrer les revenus de la manière suivante :

* En définissant le type de revenu de vos tâches et en associant les utilisateurs et utilisatrices ou les rôles affectés aux éléments de travail à des taux de facturation. Cette opération calcule les revenus en fonction du nombre d’heures prévues ou effectives des éléments de travail. Vous pouvez fixer une limite au montant maximum facturé pour les tarifs horaires, ou non.\
  Pour plus d’informations sur la spécification du type de revenu d’une tâche, voir l’article [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* En facturant un taux de revenu fixe forfaitaire pour les tâches ou les projets.\
  Si vous disposez de tâches avec des revenus fixes, le montant des revenus fixes sera ajouté aux revenus prévus d’une tâche ou d’un projet, et les revenus prévus d’une tâche pourront être ajoutés à un enregistrement de facturation en tant que revenus fixes.
* En fixant un taux de revenu fixe forfaitaire pour la facturation d’un projet, puis en fixant les taux horaires pour les tâches du projet. Workfront ajoute les taux horaires des tâches au taux forfaitaire du projet.\
  Par exemple, un mécanicien utilisant Workfront peut saisir le coût des pièces comme revenu fixe pour le projet, puis facturer à l’heure le temps passé à réparer une voiture. Les revenus fixes des projets ou des tâches sont alors réalisés à l’achèvement de l’événement.

Vous pouvez également marquer vos tâches comme « non facturables », auquel cas aucun revenu prévu ni réel ne leur est associé.

## Vue d’ensemble des types de revenus des tâches {#overview-of-task-revenue-types}

Par défaut, le Type de revenus sur toutes les nouvelles tâches est défini en fonction des Préférences de tâche et d’événement spécifiées par votre administrateur Workfront ou de groupe.

Pour plus d’informations sur la définition des préférences de tâches et de problèmes pour votre instance Workfront, voir l’article [Configurer les préférences de tâches et de problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Le propriétaire du projet peut modifier le type de revenu des tâches et le revenu fixe des projets.

Pour plus d&#39;informations sur la définition du revenu fixe d&#39;un projet, consultez l&#39;article [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).
Pour plus d’informations sur la définition du type de revenus d’une tâche, consultez l’article [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

>[!NOTE]
>
><span class="preview">Vous devez disposer du package Workflow Ultimate pour que le type de revenu Utilisateur et Rôle par heure soit disponible.</span>

Vous pouvez appliquer les types de revenus suivants à vos tâches ou projets :

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
   <td> <p>Ce type peut être utilisé pour les projets et les tâches. </p> <p>Lorsqu’un modèle est joint à un projet, le revenu fixe du modèle est ajouté au revenu fixe du projet. Pour plus d’informations, voir <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Vue d’ensemble de l’attachement d’un modèle à un projet</a>. </p> <p>Pour les tâches, quelle que soit les affectations de la tâche, le revenu de la tâche est toujours calculé à l’aide du montant fixe spécifié dans la tâche. </p> <p>Les revenus fixes des tâches enfant sont répercutés sur les revenus de la tâche parent, puis sur les revenus du projet. Si un montant fixe est défini sur la tâche parent et/ou le projet, le montant est ajouté aux revenus prévus cumulés de toutes les tâches enfant.</p> <p>Le montant des revenus fixes sur les tâches peut être inclus dans un enregistrement de facturation sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisateur, par heure</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches. </p> <p>Le taux de facturation que vous avez défini pour une personne spécifique multiplié par le nombre d’heures prévues pour cette tâche devient le montant des revenus prévus de la tâche. Le taux de facturation que vous avez défini pour une personne spécifique multiplié par le nombre d’heures que la personne consigne pour la tâche est le montant des revenus réels de la tâche. <br>Par exemple, vous créez un utilisateur ou une utilisatrice et vous définissez 20 $ pour son champ Facturation par heure. Si la personne consigne 5 heures pour une tâche sur la feuille de temps, le montant de la facturation réelle de la tâche est de 100 $.</p>
   <p>Un profil d’utilisateur ou d’utilisatrice peut contenir plusieurs taux de facturation avec des dates d’entrée en vigueur. Par exemple, le premier taux de facturation de 20 $ se termine le 30 avril 2023 et le deuxième taux de facturation de 25 $ commence le 1er mai 2023. Si la personne consigne 2 heures le 28 avril et 3 heures le 2 mai pour une tâche, le montant de facturation réel de la tâche est de 40 $ + 75 $ = 115 $.</p>
   <p><b>CONSEIL</b>

Il s’agit du type de revenu par défaut lorsque vous créez une tâche.</p> </td>
</tr> 
  <tr> 
   <td> <p>Rôle par heure</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Ce type est similaire au taux par heure de l’utilisateur ou de l’utilisatrice mais il utilise les taux de la fonction plutôt que les taux de l’utilisateur ou de l’utilisatrice.</p> <p><strong>NOTE</strong><br> Une fonction peut également avoir plusieurs taux de facturation avec des dates d’entrée en vigueur.</p></td> 
  </tr> 
  <tr> 
   <td> <p><span class="preview">Utilisateur ou utilisatrice et rôle par heure</span></p> </td> 
   <td> <p><span class="preview">Ce type ne peut être utilisé que pour les tâches.</span></p> <p><span class="preview">Ce type examine les informations sur les utilisateurs et les rôles afin de déterminer le taux approprié.</span></p></td> 
  </tr>
  <tr> 
   <td> <p>Personne, par heure avec limite</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Les tâches sont facturées à l’heure comme pour Personne, par heure mais elles ont un montant limite maximum que vous pouvez spécifier. <br>Par exemple, si le taux de facturation d’une personne est de 25 $, mais que le montant limite de la tâche est de 20 $, et que la personne consigne une heure, le revenu réel de la tâche est de 20 $. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rôle, par heure avec limite</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Ce type est similaire à Personne, par heure avec limite, mais il utilise les taux de la fonction plutôt que les taux de l’utilisateur ou de l’utilisatrice. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="preview">Utilisateur et rôle par heure avec limitation</span></p> </td> 
   <td> <p><span class="preview">Ce type ne peut être utilisé que pour les tâches.</span></p> <p><span class="preview">Les tâches sont facturées toutes les heures comme dans Utilisateur et Rôle par heure, mais elles disposent d’un Montant limite maximal que vous pouvez spécifier.</span></p></td> 
  </tr>
  <tr> 
   <td> <p>Utilisateur, par heure plus fixe</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches. </p> <p>Les tâches sont facturées à l’heure comme pour Personne, par heure, mais elles sont assorties d’un montant fixe que vous pouvez ajouter au tarif de l’utilisateur ou de l’utilisatrice. Le montant fixe spécifié dans la tâche peut être inclus dans les enregistrements de facturation du projet. Le montant fixe n’est pas multiplié par les heures consacrées à la tâche. Seul le taux de facturation de l’utilisateur ou de l’utilisatrice le fait. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rôle par heure plus fixe</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches. </p> <p>Les tâches sont facturées à l’heure comme Rôle, par heure, mais elles sont assorties d’un montant fixe supplémentaire que vous pouvez ajouter au taux du rôle. Le montant fixe spécifié dans la tâche peut être inclus dans les enregistrements de facturation du projet. Le montant fixe n’est pas multiplié par les heures consacrées à la tâche. Seul le taux de facturation de la fonction le permet. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="preview">Utilisateur ou utilisatrice et rôle par heure plus fixe</span></p> </td> 
   <td> <p><span class="preview">Ce type ne peut être utilisé que pour les tâches.</span></p> <p><span class="preview">Les tâches sont facturées toutes les heures comme dans les rôles et les utilisateurs toutes les heures, mais vous pouvez ajouter un montant fixe supplémentaire au taux. Le montant fixe spécifié dans la tâche peut être inclus dans les enregistrements de facturation du projet. Le montant fixe n'est pas multiplié par les heures de la tâche.</span></p></td> 
  </tr>
  <tr> 
   <td> <p>Fixe par heure</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>La limite ou le montant fixe que vous avez défini pour la tâche, multiplié par le nombre d’heures saisies pour la tâche (indépendamment de la personne ou de sa fonction), constitue le montant de la facturation.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Non facturable</p> </td> 
   <td> <p>Ce type ne peut être utilisé que pour les tâches.</p> <p>Ce type de revenu n’a aucun effet sur les revenus. </p> <p>Si un objet parent dispose de ce paramètre, les tâches enfant ayant un type de facturation s’appliqueront toujours normalement.</p> <p>Lorsqu’une personne n’ayant pas accès aux données financières ou n’ayant pas d’autorisations financières sur un modèle crée un projet à partir de ce modèle, il s’agit du type de revenu par défaut pour les tâches du projet.</p> <p>Pour plus d’informations sur l’accès aux données financières, voir l’article <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Octroyer l’accès aux données financières</a>.<br>Pour plus d’informations sur les autorisations financières relatives aux objets, voir l’article <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Vue d’ensemble du partage des autorisations sur les objets</a>.<br>Pour plus d’informations sur la création de projets à partir de modèles, voir l’article <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Créer un projet à l’aide d’un modèle</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Vue d’ensemble des revenus pour les tâches parent

Si vous transformez une tâche autonome contenant des informations de facturation en une tâche parent, la nouvelle tâche parent conserve toutes les informations de facturation qui lui ont été précédemment appliquées, ainsi que les heures précédemment appliquées. Toutes les informations de facturation provenant des heures enregistrées dans les tâches enfant seront répercutées en tant que revenus réels dans la nouvelle tâche parent.

Les revenus prévus des tâches enfant sont également répercutés sur la tâche parent.

## Vue d’ensemble des revenus pour les problèmes

Les problèmes n’ont pas de montants pour les revenus prévus ou réels, mais ils peuvent avoir des coûts réels.

Si vous consignez des heures pour un problème et que vous utilisez un type d’heure marqué « Comptabiliser comme revenu », Workfront calcule un coût réel en fonction du taux de la personne qui consigne le temps. Ce nombre est ajouté au coût réel du projet. Les heures peuvent également être incluses dans un enregistrement de facturation.

Pour plus d’informations sur le suivi des coûts, voir l’article [Suivre les coûts](../../../manage-work/projects/project-finances/track-costs.md).

Pour plus d’informations sur les types d’heures, voir l’article [Gérer les types d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Calcul des revenus

* [Calcul des revenus pour les tâches en fonction de l’affectation des utilisateurs et utilisatrices et des rôles](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)
* [Calcul des revenus pour les projets](#revenue-calculations-for-projects)

### Calcul des revenus pour les tâches en fonction de l’affectation des utilisateurs et utilisatrices et des rôles {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Lors du calcul des revenus d’une tâche, tenez compte des points suivants :

* Si un utilisateur ou une utilisatrice ou une fonction indique un taux de 0,00 $, Workfront le lit comme un montant valable et le multiplie par le nombre d’heures relatives à la tâche pour calculer le revenu. Si vous souhaitez n’afficher aucun revenu pour vos tâches, assurez-vous que le champ du taux de facturation pour l’utilisateur ou l’utilisatrice ou la fonction est vide.
* Lorsque les taux de facturation des fonctions s’appliquent, Workfront utilise le taux de remplacement au niveau du projet, au lieu du taux de facturation pour ce rôle, défini au niveau du système, chaque fois qu’il existe un taux de remplacement sur le projet.
* Pour les revenus réels, si l’utilisateur ou l’utilisatrice ou la fonction présente plusieurs taux de facturation avec des dates d’entrée en vigueur, le revenu de la tâche correspond à la somme des revenus de chaque période au cours de laquelle l’utilisateur ou l’utilisatrice a consigné du temps. Les revenus prévus sont basés sur les heures prévues pour les périodes.
* En cas d’affectations multiples sur les tâches, les scénarios décrits ci-dessous s’appliquent à chaque personne cessionnaire.

Le système utilise une hiérarchie pour déterminer le taux utilisé dans les calculs de revenus en fonction des affectations de tâches.

Si votre équipe d’administration Workfront a activé le paramètre **Affecter manuellement des fonctions à des saisies d’heures** dans la zone Préférences de feuilles de temps et d’heures, et que la personne qui consigne le temps sur le projet sélectionne un rôle différent à associer à ces heures, les revenus réels de la tâche ou du projet sont toujours calculés en fonction du rôle associé à la saisie des heures. Pour plus d’informations sur l’activation de la consignation du temps pour une fonction spécifique, voir l’article [Configurer les préférences de feuilles de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

<div class="preview">

Pour le type de revenu Utilisateur et Rôle par heure , une fonction pour la facturation peut être définie au niveau du projet et de l’affectation. S&#39;il est défini au niveau du projet pour un utilisateur spécifique, ce rôle se propage automatiquement à toutes les affectations de cet utilisateur pendant la période de validité du contrat pour laquelle vous l&#39;avez appliqué. Vous pouvez toujours remplacer ce taux au niveau de l&#39;affectation, si nécessaire. Par exemple, la fonction principale d’une utilisatrice est Designer, mais vous définissez sa fonction pour la facturation d’un projet en tant que Senior Designer pour le mois d’août. Toutes les tâches qui leur sont assignées en août utiliseront automatiquement le taux de facturation de Senior Designer.

Cependant, pour une tâche particulière, vous pouvez remplacer le rôle uniquement pour cette affectation, afin de refléter le travail facturé. Ainsi, le système prend en charge à la fois la cohérence à l’échelle du projet et la flexibilité au niveau des affectations. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) et [Créer des affectations avancées](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

</div>

Les scénarios suivants existent lors du calcul des revenus des tâches sur la base du type de revenu et de la nature de l’affectation des tâches :

* **Le type de revenu de la tâche est Personne, par heure.**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Facturation par heure</td> 
     <td>Aucune affectation</td> 
     <td>Affectation de l’utilisateur ou de l’utilisatrice</td> 
     <td>Affectation de la fonction</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les revenus prévus</td> 
     <td>0,00 $</td> 
     <td> Si une personne affiche un taux de facturation dans son profil, c’est ce taux qui est utilisé pour calculer les revenus prévus. Dans le cas contraire, c’est le taux de facturation du système correspondant à sa fonction principale qui est utilisé. <br><p><b>NOTE</b> La personne peut être affectée à la tâche avec l’une de ses fonctions secondaires, mais c’est le taux de la fonction principale qui est utilisé ici.</p><p>Si le rôle de l’utilisateur ou l’utilisatrice a changé au cours de l’affectation, les taux corrects sont appliqués lorsque les finances du projet sont recalculées.</p></td> 
     <td>Le taux de facturation système de la fonction affectée à la tâche est utilisé pour calculer le revenu prévu. Les taux de facturation peuvent être modifiés au niveau du projet.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les revenus réels</td> 
     <td>Si l’utilisateur ou l’utilisatrice qui enregistre les heures a un taux de facturation dans son profil, ce taux est utilisé.
     <br>Dans le cas contraire, c’est le taux de facturation de leur fonction principale qui est utilisé. Si aucun taux de facturation n’est associé à l’utilisateur ou à l’utilisatrice ou à sa fonction principale, les revenus réels sont de 0,00 $. <br><p><b>NOTE</b>

  Seuls les taux associés à l’utilisateur ou à l’utilisatrice qui consigne les heures sont pris en compte pour le calcul, même si une autre personne est affectée à la tâche.</p></td>

  <td>Si l’utilisateur ou l’utilisatrice qui consigne les heures a un taux de facturation dans son profil, c’est ce taux qui est utilisé. <br>Dans le cas contraire, c’est le taux de facturation de leur fonction principale qui est utilisé. Si aucun taux de facturation n’est associé à l’utilisateur ou à l’utilisatrice ou à sa fonction principale, les revenus réels sont de 0,00 $. <br><p><b>NOTE</b>

  Seuls les taux associés à l’utilisateur ou à l’utilisatrice qui consigne les heures sont pris en compte pour le calcul, même si une autre personne est affectée à la tâche.</p></td>

  <td>Si l’utilisateur ou l’utilisatrice qui consigne les heures a un taux de facturation dans son profil, c’est ce taux qui est utilisé. Dans le cas contraire, c’est le taux de facturation de sa fonction principale qui est utilisé.<br><p><b>NOTE</b>

  Si la personne qui consigne ses heures n’est pas associée à un taux de facturation et qu’elle n’a pas de fonction ou de taux de facturation pour sa fonction, c’est le taux de la fonction associée à la tâche qui est utilisé. S’il n’existe aucun taux de facturation pour ce rôle, le chiffre d’affaires est de 0,00 $.</p></td>
  </tr> 
   </tbody> 
  </table>

* **Le type de revenu de la tâche est Rôle par heure.**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Facturation par heure</td> 
     <td>Aucune affectation</td> 
     <td>Affectation de l’utilisateur ou de l’utilisatrice</td> 
     <td>Affectation de la fonction</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les revenus prévus</td> 
     <td>0,00 $</td> 
     <td><p>Workfront examine la fonction que l’utilisateur ou l’utilisatrice remplit dans la tâche pour calculer les revenus prévus. <br>Si l’utilisateur ou l’utilisatrice n’a aucune fonction associée dans la tâche, les revenus sont de 0,00 $.</p> <p><strong>NOTE</strong><br> Si la fonction de l’utilisateur ou de l’utilisatrice a changé pendant l’affectation, les taux corrigés sont appliqués lorsque les finances du projet sont recalculées.</p> </td> 
     <td>Le taux de facturation de la fonction affectée à la tâche est utilisé pour calculer le revenu prévu. Les taux de facturation peuvent être modifiés au niveau du projet.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taux de facturation par heure pour les revenus réels</td> 
     <td>Workfront utilise le taux de facturation de la fonction principale de l’utilisateur ou de l’utilisatrice qui consigne les heures. <br>Si la journalisation de l'utilisateur n'est associée à aucune fonction ou si la fonction principale n'a aucun taux de facturation, le revenu réel est de 0,00 $. </td> 
     <td> Si la personne qui consigne les heures est affectée à la tâche, le taux de facturation de la fonction qui lui est associée sur la tâche est utilisé pour calculer les revenus réels. <br>Dans le cas contraire, c’est le taux de facturation de leur fonction principale qui est utilisé. Si l’utilisateur ou l’utilisatrice n’a pas de fonction principale ou si sa fonction principale n’a pas de taux de facturation, les revenus réels sont de 0,00 $. </td> 
     <td>Si l’une des fonctions de l’utilisateur ou de l’utilisatrice qui consigne les heures est affectée à la tâche, le taux de cette fonction est utilisé. Si la fonction affectée à la tâche n’est pas associée à l’utilisateur ou à l’utilisatrice qui consigne les heures, le taux de facturation de la fonction principale de l’utilisateur ou de l’utilisatrice est utilisé pour calculer les revenus réels. Si l’utilisateur ou l’utilisatrice n’a pas de fonction ou si aucun taux n’est associé à sa fonction principale, c’est le taux de la fonction affectée à la tâche qui est utilisé. </td> 
    </tr> 
   </tbody> 
  </table>

<div class="preview">

* **Le type de revenu de la tâche est Utilisateur et rôle par heure**

| Facturation par heure | Aucune affectation | Affectation de l’utilisateur ou de l’utilisatrice | Affectation de la fonction |
| --- | --- | --- | --- |
| Taux de facturation par heure pour les revenus prévus | 0,00 $ | Lorsqu’un utilisateur est affecté, le système recherche le taux dans un ordre spécifié, en commençant par un taux de facturation conservé. Vous trouverez ensuite un taux de carte tarifaire verrouillé, un taux saisi manuellement au niveau de l&#39;affectation, la fonction de facturation au niveau de l&#39;affectation, le remplacement du taux de facturation de l&#39;utilisateur au niveau du projet, la fonction de facturation au niveau du projet, le taux système de l&#39;utilisateur et le taux de la fonction principale de l&#39;utilisateur. <p> Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). | Lorsqu’une fonction est affectée, le système recherche d’abord un taux de facturation conservé, puis un taux de carte tarifaire verrouillé pour la fonction sur l’affectation. Elle recherche ensuite un taux de fonctions ajouté manuellement à l’affectation. Si ce taux n’est pas trouvé, il recherche un taux de fonction au niveau du projet, d’abord à partir d’une carte tarifaire, puis à partir du taux système. <p> Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). |
| Taux de facturation par heure pour les revenus réels | Seuls les taux associés à l’utilisateur ou à l’utilisatrice qui consigne les heures sont pris en compte pour le calcul, même si une autre personne est affectée à la tâche. <p> Le système recherche le taux dans un ordre spécifié, en commençant par un taux de facturation conservé. Vous trouverez ensuite un taux de carte tarifaire verrouillé, un taux de facturation de remplacement pour le projet, la fonction pour la facturation, le taux au niveau du système sur le profil utilisateur du propriétaire et le taux de facturation de la fonction principale du propriétaire. <p> Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). | Lorsqu’un utilisateur est affecté, le système recherche le taux dans un ordre spécifié, en commençant par un taux de facturation conservé. Vous trouverez ensuite un taux de carte tarifaire verrouillé, un taux saisi manuellement au niveau de l&#39;affectation, la fonction de facturation au niveau de l&#39;affectation, le remplacement du taux de facturation de l&#39;utilisateur au niveau du projet, la fonction de facturation au niveau du projet, le taux système de l&#39;utilisateur et le taux de la fonction principale de l&#39;utilisateur. <p> Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). | Lorsqu’une fonction est affectée, le système recherche d’abord un taux de facturation conservé, puis un taux de carte tarifaire verrouillé pour la fonction sur l’affectation. Elle recherche ensuite un taux de fonctions ajouté manuellement à l’affectation. Si ce taux n’est pas trouvé, il recherche un taux de fonction au niveau du projet, d’abord à partir d’une carte tarifaire, puis à partir du taux système. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). |

</div>

### Calcul des revenus pour les projets

Vous pouvez suivre les types de revenus suivants pour les projets :

* Les revenus prévus d’un projet sont calculés à l’aide de la formule suivante :

  `Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue`

  Pour plus d’informations sur le mode de calcul des revenus prévus des tâches, voir la section [Calculs des revenus des tâches basés sur les affectations d’utilisateurs et d’utilisatrices et de fonctions](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) de cet article.

* Les revenus réels d’un projet sont calculés à l’aide de la formule suivante :

  `Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)`

Pour plus d’informations sur la manière dont les revenus réels des tâches sont calculés, voir la section [Calculs des revenus des tâches basés sur les affectations d’utilisateurs et d’utilisatrices et de fonctions](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) de cet article.

Pour les revenus réels associés aux heures enregistrées directement sur le projet ou les problèmes, Workfront utilise le taux de facturation de l’utilisateur ou de l’utilisatrice qui consigne les heures sur le projet. Si l’utilisateur ou l’utilisatrice n’a pas de taux de facturation associé à son profil, Workfront utilise le taux de facturation de sa fonction principale. Si les deux taux sont nuls, les revenus réels associés aux heures consignées sur le projet ou les problèmes sont nuls.
