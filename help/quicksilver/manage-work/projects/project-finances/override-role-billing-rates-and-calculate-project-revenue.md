---
product-area: projects
navigation-topic: financials
title: Vue d’ensemble du remplacement des taux de facturation des fonctions et du calcul des revenus sur un projet
description: Vous pouvez utiliser les taux de facturation pour calculer les recettes de vos projets lorsque vous les multipliez par les heures passées sur le projet. Pour plus d’informations sur les taux de facturation et les recettes, consultez l’article Présentation de la facturation et des recettes.
author: Alina, Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '3860'
ht-degree: 1%

---

# Vue d’ensemble du remplacement des taux de facturation des fonctions et du calcul des revenus sur un projet

{{highlighted-preview}}

Vous pouvez utiliser les taux de facturation pour calculer les recettes de vos projets lorsque vous les multipliez par les heures passées sur le projet. Pour plus d’informations sur les taux de facturation et les recettes, consultez l’article [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
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
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Présentation des taux de facturation des rôles des tâches et des types de recettes horaires des rôles

En tant qu’administrateur Adobe Workfront, vous pouvez associer des taux de facturation à des utilisateurs et à des rôles de tâche.\
Pour plus d’informations sur la création d’utilisateurs et leur association aux taux de facturation, consultez l’article [Ajout d’utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Pour plus d’informations sur la création de rôles de tâche et leur association aux taux de facturation, consultez l’article [Créer et gérer des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Les taux de facturation associés aux utilisateurs ne peuvent pas être remplacés.

Les taux de facturation associés aux rôles de tâche peuvent être remplacés au niveau de l’entreprise ou du projet.

Pour calculer les recettes sur les projets en fonction des taux de facturation des rôles de tâche, le **Type de revenu** des tâches sur les projets doit être l’un des suivants :

* Rôle par heure
* Rôle par heure avec limite
* Horaire du rôle plus fixe

Pour plus d’informations sur **le type de chiffre d’affaires** et les taux de facturation, voir [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Hiérarchie des remplacements de taux de facturation lors du calcul des recettes

Un rôle de tâche peut être associé à un taux de facturation de la manière suivante :

* En tant qu’administrateur Workfront, vous pouvez définir le taux de facturation au niveau du système associé à un rôle de tâche lorsque vous créez ce rôle de tâche.\
  Pour plus d’informations sur la création de rôles de tâche, voir [Création et gestion de rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* En tant qu’administrateur Workfront, vous pouvez définir le taux de facturation au niveau de l’entreprise pour le même rôle de tâche lorsque vous créez une société.\
  Lorsque Workfront calcule les recettes pour les projets associés à cette entreprise, le taux de facturation de l’entreprise est utilisé lorsque le rôle est affecté à des tâches, au lieu du taux de facturation au niveau du système pour ce rôle de tâche.\
  Les taux de rôles d’emploi modifiés au niveau de l’entreprise auront un impact sur tous les projets associés à cette entreprise.

  >[!NOTE]
  >
  >Si vous devez mettre à jour le taux de facturation de l’entreprise, celui du projet ne sera pas mis à jour automatiquement. Vous devez supprimer la société du projet, mettre à jour le taux de la société, puis rattacher à nouveau la société au projet, avant que le nouveau taux de la société ne prenne effet sur le projet. Pour plus d’informations sur l’association d’une entreprise à un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

  Pour plus d’informations sur la création de taux de facturation des rôles de tâche spécifiques à une entreprise, voir [Création et modification d’entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* En tant qu’administrateur Workfront, vous pouvez activer une option lors de la modification d’un projet pour appliquer des modifications aux taux de facturation au niveau de l’entreprise au projet lorsque les utilisateurs recalculent manuellement les finances du projet.\
  Pour plus d’informations, voir [Remplacement des taux de facturation au niveau du projet par des taux de facturation au niveau de l’entreprise](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* En tant qu’administrateur Workfront, vous pouvez définir des cartes de taux avec plusieurs taux de facturation par rôle, en fonction de l’emplacement et de la date. Lorsqu’une carte de taux est jointe à un projet, tous les rôles (par emplacement, si des emplacements sont utilisés) et leurs taux de facturation associés sont ajoutés à la section des taux de facturation du projet. Le fait de joindre une carte de taux remplace les taux de facturation existants sur le projet.

  Pour plus d’informations, voir [Gérer les cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) et [Joindre une carte de taux à un projet](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* En tant que chef de projet, vous pouvez définir le taux de facturation du même rôle de tâche au niveau du projet.\
  Les taux de rôle des tâches modifiés sur le projet n’auront une incidence que sur ce projet.

  Pour plus d’informations sur le remplacement des taux de rôle pour le projet, voir [Remplacement des taux de facturation des rôles au niveau du projet](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Si un rôle de tâche est associé à un taux de facturation au niveau du système, de la société et du projet, Workfront calcule les recettes des tâches à l’aide du taux de facturation du rôle de tâche au niveau du projet, lorsqu’il utilise les taux de rôle de tâche. Les recettes de toutes les tâches sont cumulées aux recettes du projet.

## Remplacer les taux de facturation des fonctions au niveau d’un projet

En tant que chef de projet, vous pouvez spécifier le taux de facturation d’un rôle de tâche sur un projet spécifique. Ce taux de facturation au niveau du projet remplace le taux de facturation au niveau du système pour ce rôle de tâche. Workfront utilise le taux de facturation au niveau du projet du rôle de tâche pour calculer les recettes, au lieu d’utiliser le taux de facturation au niveau du système.

<span class="preview">Vous pouvez également joindre une carte de taux au projet, qui importera les taux de facturation du rôle de tâche de la carte de taux dans le projet.</span>

Pour plus d’informations sur la façon de remplacer les taux de facturation des rôles de tâche au niveau du projet, voir [Remplacer les taux de facturation des rôles de tâche au niveau du projet](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Pour plus d’informations sur le rôle de tâche utilisé pour calculer les recettes du projet, voir la section &quot;Calcul des recettes pour les tâches en fonction des affectations d’utilisateurs et de rôles&quot; dans [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Pour plus d&#39;informations sur l&#39;association d&#39;une carte de taux à un projet, voir [Joindre une carte de taux à un projet](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>Dans le cas des Recettes réelles, les taux de facturation appliqués aux heures ajoutées à un enregistrement de facturation marqué comme Facturé ne doivent pas être affectés par les remplacements de taux de facturation qui surviennent après la facturation de l’enregistrement de facturation.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Présentation de la section Taux de facturation d’un projet

Après avoir spécifié les taux de facturation de remplacement pour les rôles de tâche associés au projet, vous pouvez voir tous les rôles de tâche et leurs remplacements dans l’onglet **Taux de facturation** du projet.

Notez les informations suivantes dans la liste de **Taux de facturation** :

* [Regroupement de rôles de tâche](#job-role-grouping)
* [Valeur du taux de facturation du projet](#project-billing-rate-value)
* [ Valeur du taux de facturation par défaut ](#default-billing-rate-value)
* [ Valeur du taux de facturation de la société ](#company-billing-rate-value)
* [Valeurs et délais de taux de facturation multiples](#multiple-billing-rate-values-and-timeframes)

### Regroupement des rôles de tâche {#job-role-grouping}

Les taux de facturation sont regroupés dans la zone **Taux de facturation** en fonction de leurs rôles de travail respectifs. <span class="preview">Si une carte de taux est jointe au projet, les rôles de tâche sont également regroupés par carte de taux. Si des emplacements sont appliqués aux rôles de tâche, le nom de l’emplacement est inclus dans le nom du rôle de tâche. Vous pouvez avoir le même rôle de tâche répertorié pour plusieurs emplacements.</span>

### Valeur du taux de facturation du projet {#project-billing-rate-value}

Dans la ligne de regroupement correspondant à un rôle de tâche, remarquez le taux de facturation de ce rôle de tâche au niveau du projet dans la colonne **Taux de facturation du projet** . Si le rôle de tâche comporte plusieurs taux de remplacement, le taux de remplacement correspondant à la date actuelle est affiché dans la ligne de regroupement de la colonne **Taux de facturation du projet** .

### Valeur du taux de facturation par défaut {#default-billing-rate-value}

Dans la ligne de regroupement d’un rôle de tâche, remarquez le taux de facturation de ce rôle de tâche au niveau du système dans la colonne **Taux de facturation par défaut** .

>[!NOTE]
>
>S’il existe des taux de facturation de projet pour un rôle de tâche, le **taux de facturation par défaut** n’est jamais appliqué au calcul des recettes pour le projet. Seuls les **taux de facturation du projet** sont appliqués pour calculer les recettes.

### Valeur du taux de facturation de la société {#company-billing-rate-value}

Dans la ligne de regroupement d’un rôle de tâche, remarquez le taux de facturation de ce rôle de tâche au niveau de l’entreprise dans la colonne **Taux de facturation de l’entreprise** . Cela signifie qu’une société est associée à ce projet et que ce rôle de travail a un taux de facturation différent pour cette société. Le taux de facturation de l’entreprise s’affiche, même s’il est identique au taux du projet.

>[!NOTE]
>
><span class="preview">Lorsqu’une carte de taux est jointe au projet, les **taux de facturation de l’entreprise** ne sont pas importés dans les taux de facturation. Les calculs sont basés sur les taux des cartes de taux ou les taux de la société pour les rôles de tâche.</span>
>
>S’il existe des taux de facturation de projet pour un rôle de tâche, le **taux de facturation de l’entreprise** n’est jamais appliqué au calcul des recettes du projet. Seuls les **taux de facturation du projet** sont appliqués pour calculer les recettes.

### Valeurs et délais de taux de facturation multiples {#multiple-billing-rate-values-and-timeframes}

Si vous disposez de plusieurs taux de facturation de remplacement pour un rôle de tâche spécifique, ils sont répertoriés sous le regroupement correspondant à ce rôle de tâche. Grâce à la modification en ligne, vous pouvez modifier les taux de remplacement et les **Début** **Date** et **Date de fin** des taux de facturation de remplacement sur cet onglet.

>[!NOTE]
>
>Vous ne pouvez pas spécifier une **Date de début** pour le premier taux de remplacement et vous ne pouvez pas spécifier une **Date de fin** pour le dernier taux de remplacement. Workfront suppose que le premier taux de remplacement est appliqué pour toutes les heures dont la date est antérieure à la **Date de fin** du premier remplacement et que le dernier est appliqué pour toutes les heures dont la date est plus récente que la **Date de début** du dernier remplacement.\
>Si une heure est enregistrée avant la date de début planifiée du projet, le premier taux de facturation est utilisé.\
>Si une heure est enregistrée après la date d’achèvement planifiée du projet, le dernier taux de facturation est utilisé.

## Calculer les recettes prévues

* [ Calculer les recettes prévues en fonction d’un remplacement de taux de facturation unique ](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [ Calculer les recettes prévues en fonction de plusieurs remplacements de taux de facturation](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Répartition des heures planifiées sur la durée d’une tâche](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcul des recettes planifiées sur la base d’un remplacement unique du taux de facturation {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Tenez compte de ce qui suit lors du calcul des Recettes prévues en fonction d’un remplacement de taux de facturation unique :

* Lorsque le **Type de recette** d’une tâche est **Heure de rôle**, Workfront multiplie les Heures planifiées d’une tâche par le taux de facturation du rôle de tâche associé à la tâche pour calculer les Recettes planifiées de la tâche.

* Lorsque le taux de facturation du rôle de tâche a été remplacé au niveau du projet, Workfront utilise le taux de remplacement du projet pour calculer les recettes planifiées.
* Lorsqu’une tâche comporte plusieurs affectations, les Recettes prévues sont calculées en multipliant le taux de facturation du rôle de chaque affectation et de l’affectation Heure planifiée correspondante.

>[!NOTE]
>
>Les Heures planifiées par affectation ne sont pas identiques aux Heures planifiées de la tâche, dans le cas de plusieurs affectations.

Pour plus d’informations sur le rôle de tâche utilisé pour calculer les recettes planifiées, voir la section &quot;Présentation des calculs de recettes pour les tâches basées sur les affectations d’utilisateurs et de rôles&quot; de l’article [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcul des recettes prévues en fonction de plusieurs remplacements de taux de facturation {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Tenez compte de ce qui suit lors du calcul des Recettes prévues en fonction de plusieurs remplacements de taux de facturation :

* Lorsque le **Type de recette** d’une tâche est **Heure de rôle**, Workfront multiplie les Heures planifiées d’une tâche par le taux de facturation du rôle de tâche associé à la tâche pour calculer les Recettes planifiées de la tâche.

  Pour plus d’informations sur le rôle de tâche utilisé pour calculer les recettes planifiées, voir la section &quot;Présentation des calculs de recettes pour les tâches basées sur les affectations d’utilisateurs et de rôles&quot; de l’article [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Dans le cas de remplacements multiples de taux de facturation, le taux par lequel les Heures planifiées sont multipliées change pendant la durée d’une tâche. Par défaut, Workfront répartit les Heures planifiées uniformément sur la durée d’une tâche, allouant un nombre égal d’heures pour chaque jour de la tâche. Lors du calcul de **Recettes planifiées** pour une tâche, Workfront multiplie l’Heure planifiée par jour par le taux de facturation de cette journée. Dans le cas de plusieurs taux de facturation, ce taux peut être différent chaque jour.

  Par exemple, vous avez une tâche avec un rôle Horaire **Type de revenu**. La tâche a une durée de 5 jours et une valeur Heures planifiées de 40 heures. Les heures planifiées par jour sont de 8 heures. Attribuez un rôle de tâche Gestionnaire de projets à la tâche et remplacez le taux de facturation de ce rôle de tâche pour les trois derniers jours de la tâche. Vous aurez donc un taux de facturation de l’ordre 1 pour les deux premiers jours et un taux de facturation de l’ordre 2 pour les trois jours restants de la tâche pour ce rôle de tâche.

  La formule qui calcule le **Chiffre d’affaires planifié** de cette tâche est la suivante :

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Pour plus d’informations sur la recherche du montant Heures planifiées par jour dans Workfront, consultez la section [Répartition des heures planifiées sur la durée d’une tâche](#distribution-of-planned-hours-across-the-duration-of-a-task) de cet article.

>[!NOTE]
>
>Si la tâche comporte plusieurs personnes désignées, le nombre d’heures planifiées est d’abord distribué à chaque personne désignée, puis à chaque jour pendant la durée de la tâche. Dans ce cas, les Recettes prévues calculeront en prenant en compte le nombre d’heures quotidiennes pour chaque responsable et le taux de facturation de chaque rôle de tâche qui pourrait changer pendant la durée de la tâche, en cas de taux de facturation multiples.

### Répartition des heures planifiées sur la durée d’une tâche {#distribution-of-planned-hours-across-the-duration-of-a-task}

Tenez compte de ce qui suit lorsque vous comprenez la répartition des heures planifiées sur la durée d’une tâche :

* Par défaut, Workfront répartit les heures planifiées uniformément sur la durée d’une tâche, allouant un nombre égal d’heures planifiées pour chaque jour de la tâche, en fonction de la disponibilité du planning du projet.

  Pour plus d’informations sur la compréhension de la répartition des heures planifiées sur la durée d’une tâche, voir la section &quot;Compréhension de la répartition des heures planifiées sur la durée d’une tâche&quot; dans l’article [Présentation des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >Les Heures planifiées par jour sont l’allocation des Heures planifiées pour chaque jour pendant la durée de la tâche. Si la tâche a une affectation, ce nombre représente également les Heures planifiées par jour et par affectation. Si la tâche comporte plusieurs affectations, les Heures planifiées par jour et par affectation sont différentes des Heures planifiées par jour pour la tâche. Il n’existe aucune représentation visuelle dans Workfront pour les heures planifiées par jour et par affectation, pour les tâches avec plusieurs affectations.
  >
  >
  >Les Heures planifiées par jour sont multipliées par le taux de facturation du rôle de tâche affecté à la tâche pour cette journée afin de calculer les Recettes planifiées par jour pour cette tâche. Une somme de tous les revenus planifiés quotidiens calculés de cette manière est égale aux revenus prévus pour cette tâche.

## Calculer les recettes réelles

* [Calculer les recettes réelles en fonction d’un remplacement de taux de facturation unique](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcul des recettes réelles en fonction de plusieurs remplacements de taux de facturation](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcul des recettes réelles en fonction d’un remplacement unique du taux de facturation {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Tenez compte de ce qui suit lors du calcul des Recettes réelles en fonction d’un remplacement de taux de facturation unique :

* Lorsque le **Type de recette** d’une tâche est **Heure de rôle**, Workfront multiplie les **Heures réelles** d’une tâche par le taux de facturation du rôle de tâche associé à la tâche pour calculer le **Recettes réelles** de la tâche. Les heures réelles sont les heures consignées directement dans la tâche.

  Pour plus d’informations sur le rôle de tâche utilisé pour calculer les **Recettes réelles**, consultez la section &quot;Comprendre les calculs de recettes pour les tâches basées sur les affectations d’utilisateurs et de rôles&quot; de l’article [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Si le taux de facturation du rôle de tâche a été remplacé au niveau du projet, Workfront utilise le taux de remplacement du projet pour calculer les recettes réelles. Lorsque vous remplacez le taux de facturation du rôle de tâche sur le projet, le **revenu réel** du projet est recalculé automatiquement à l’aide du nouveau taux ajusté.

  Pour plus d’informations sur le remplacement des taux de rôle pour le projet, voir [Remplacement des taux de facturation des rôles au niveau du projet](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Si vous souhaitez conserver les heures que vous avez déjà connectées au projet avant de remplacer le taux de facturation d’origine facturé au taux d’origine, vous devez les inclure dans un **enregistrement de facturation**, et vous devez marquer l’**enregistrement de facturation** comme **facturation**. Sinon, le **Recettes réelles** des heures enregistrées avant le remplacement du taux de facturation du projet sera recalculé à l’aide du nouveau taux lorsque les finances des projets seront recalculées.\
>Pour plus d’informations sur l’inclusion d’heures dans un enregistrement de facturation et le marquage sur **Facturé**, consultez l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcul des recettes réelles en fonction de plusieurs remplacements de taux de facturation {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Tenez compte de ce qui suit lors du calcul des Recettes réelles en fonction de plusieurs remplacements de taux de facturation :

* Lorsque le **Type de recette** d’une tâche est **Heure du rôle**, Workfront multiplie les **Heures réelles** de la tâche par le taux de facturation des rôles de tâche affectés à la tâche pour calculer le **Recettes réelles** de la tâche. Les heures réelles sont les heures consignées directement dans la tâche.

* Dans le cas de plusieurs remplacements de taux de facturation, le taux par lequel les **Heures réelles** sont multipliés pour calculer les **Recettes réelles** peut changer pendant la durée d’une tâche. Workfront utilise le taux de facturation du rôle de tâche dont la période correspond à la **Date d’entrée** des heures consignées pour la tâche afin de calculer les **Recettes réelles.**

  Par exemple, une tâche a le **Type de chiffre d’affaires** de **Rôle Heure** et est affectée au rôle de tâche du gestionnaire de projet. Remplacez le taux de facturation de ce rôle de tâche par le taux 1 pour les dates comprises entre le 19 et le 25 juin. À compter du 26 juin, remplacez le taux de facturation par le taux 2. Consignez 2 heures pour le 20 juin et 3 heures pour le 28 juin.

  Workfront calcule le **revenu réel** pour cette tâche à l’aide de la formule suivante :

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Pour plus d’informations sur le rôle de tâche utilisé pour calculer les **Recettes réelles**, consultez la section &quot;Comprendre les calculs de recettes pour les tâches basées sur les affectations d’utilisateurs et de rôles&quot; de l’article [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Incidence des fuseaux horaires lors du calcul des recettes sur la base de plusieurs taux de facturation

Les utilisateurs peuvent afficher différentes heures planifiées par jour par rapport aux autres utilisateurs, si des différences de fuseau horaire se produisent entre eux et d’autres entités dans Workfront. Les scénarios suivants peuvent fausser les informations Heures planifiées par jour pour un utilisateur par rapport à ce qu’un autre utilisateur voit :

* Les ordinateurs des deux utilisateurs peuvent être paramétrés pour deux fuseaux horaires différents.
* Les deux profils utilisateur dans Workfront peuvent être définis sur deux fuseaux horaires différents.
* Le fuseau horaire associé au profil utilisateur peut être différent du fuseau horaire système dans Workfront.
* Le fuseau horaire associé au profil utilisateur peut être différent du fuseau horaire du planning du projet.

Dans ce cas, le nombre d’heures planifiées par jour peut différer entre deux utilisateurs qui ne partagent pas les mêmes paramètres pour les fuseaux horaires. Ils verront également différents chiffres des recettes prévues lors de l’utilisation de plusieurs remplacements de taux de facturation sur un projet.

* [Calcul des recettes planifiées pour les utilisateurs dans différents fuseaux horaires](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcul des recettes réelles pour les utilisateurs dans différents fuseaux horaires](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcul des recettes planifiées pour les utilisateurs dans différents fuseaux horaires {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Si des utilisateurs de fuseaux horaires différents travaillent sur les mêmes projets, nous vous recommandons de ne pas modifier les remplacements de taux de facturation pour vos projets au cours de la semaine. Cela peut entraîner l’affichage d’un montant de recettes planifiées erroné pour votre projet, en raison des différences horaires entre les fuseaux horaires dans la planification des utilisateurs et le fuseau horaire du système Workfront . La plupart des plannings permettent aux week-ends d’être exclus des calculs des heures planifiées. Si un changement se produit dans le remplacement du taux de facturation d’un rôle de tâche, il est préférable qu’il se produise au cours d’un week-end plutôt qu’au milieu d’une semaine où il pourrait coïncider avec le milieu de la durée d’une tâche.

Tenez compte de ce qui suit lors du calcul des recettes planifiées pour les utilisateurs de différents fuseaux horaires :

* Pour les tâches dont le **Type de chiffre d’affaires** est de **Rôle Heure** et qui sont affectées à des rôles de tâche, le **Chiffre d’affaires planifié** est calculé en multipliant les **Heures planifiées** d’une tâche par le taux de facturation du rôle de tâche.

* Les **heures planifiées** sont réparties uniformément sur la **durée** de la tâche.

* La **durée** est la période entre le **Début planifié** **Date** et la **Date d’achèvement planifiée** de la tâche. Étant donné que les **Date de début planifiée** et **Date d’achèvement planifiée** des tâches peuvent varier en fonction des fuseaux horaires des utilisateurs qui visualisent la tâche, le nombre d’heures planifiées par jour peut différer pour deux utilisateurs dans deux fuseaux horaires différents.

* Le montant des heures planifiées par jour ne modifie pas les recettes planifiées d’un projet si le taux de facturation du rôle de tâche n’est pas modifié ou s’il n’y a qu’un seul remplacement de taux de facturation. Dans ce cas, même si deux utilisateurs de deux fuseaux horaires différents voient des heures planifiées par jour différentes, les recettes planifiées globales du projet sont identiques entre les deux utilisateurs.

  Cependant, dans le cas de plusieurs remplacements de taux de facturation, le **chiffre d’affaires planifié** global du projet peut sembler différent pour deux utilisateurs dans deux fuseaux horaires différents, car il dépend du nombre d’heures planifiées par jour (qui peut être différent pour les deux utilisateurs) et du remplacement de taux de facturation (qui peut être différent pour le même jour, lorsque chaque utilisateur examine la tâche dans son propre fuseau horaire).

* Le montant exact de **Recettes prévues** est celui que voit l’utilisateur qui a le même fuseau horaire que le Fuseau horaire de votre instance Workfront. Votre administrateur Workfront définit le fuseau horaire Workfront dans la zone Informations client système.\
  Pour plus d’informations sur la définition du fuseau horaire pour votre système, consultez l’article [Configuration des informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcul des recettes réelles pour les utilisateurs dans différents fuseaux horaires {#calculate-actual-revenue-for-users-in-different-time-zones}

Tenez compte de ce qui suit lors du calcul des recettes réelles pour les utilisateurs de différents fuseaux horaires :

* Lorsque le **Type de recette** d’une tâche est **Heure du rôle**, Workfront multiplie les **Heures réelles** de la tâche par le taux de facturation des rôles de tâche affectés à la tâche pour calculer le **Recettes réelles**. Les heures réelles sont les heures consignées directement dans la tâche.

* En cas de remplacement de plusieurs taux de facturation, Workfront utilise le taux de facturation du rôle de tâche dont la période correspond à la **Date d’entrée** des heures consignées pour la tâche afin de calculer le **Chiffre d’affaires réel**.

* Puisqu’il n’y a pas d’horodatage sur la **Date d’entrée** des heures consignées et qu’il n’y a pas d’horodatage sur les plages de dates de plusieurs remplacements de taux de facturation, les calculs de **Recettes réelles** ne sont pas affectés par le fuseau horaire associé aux utilisateurs.

Pour plus d’informations sur le rôle de tâche utilisé pour calculer les **Recettes réelles**, consultez la section &quot;Comprendre les calculs de recettes pour les tâches basées sur les affectations d’utilisateurs et de rôles&quot; de l’article [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Recalculer les finances du projet

Les finances sont calculées sur un projet à mesure que les modifications surviennent dans les heures consignées pour ce dernier.

Si les taux sont modifiés pendant la durée de vie d’un projet, vous pouvez recalculer manuellement les coûts et les revenus du projet, à l’aide de l’option Recalculer le financement d’un projet. En outre, certaines actions déclenchent un recalcul automatique.

Pour plus d’informations sur le nouveau calcul des finances de projet, consultez l’article [Recalculer les finances de projet](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Ajout d’un nouveau taux de facturation à l’aide de l’API

Pour ajouter un nouveau taux de facturation pour un rôle de tâche à l’aide de l’API, vous effectuez une action *setRatesForRole* pour l’objet **Rate** à l’aide de la *méthode PUT*.
L’action et les champs de date de l’objet **Rate** sont disponibles dans l’API version 8.0.
Si plusieurs taux de facturation sont déjà définis pour un rôle de tâche sur un projet et que vous souhaitez ajouter un nouveau taux de facturation pour celui-ci avec une nouvelle plage de dates, vous devez inclure le taux existant et le taux à ajouter dans le même appel API. Cette opération est similaire à la mise à jour des collections sur les objets.

L’appel API suivant est un exemple où **attachableID** est l’ **ID de projet** du projet dans lequel vous ajoutez le taux et **RoleID** est l’ **ID de rôle de tâche** pour lequel vous ajoutez le nouveau taux de facturation.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Pour plus d’informations sur l’utilisation de l’API Workfront, reportez-vous à l’article [Principes de base des API](https://experience.workfront.com/s/article/API-Basics-638808549).
