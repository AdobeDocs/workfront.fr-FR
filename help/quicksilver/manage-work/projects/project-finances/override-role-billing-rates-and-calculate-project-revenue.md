---
product-area: projects
navigation-topic: financials
title: Présentation du remplacement des taux de facturation et du calcul du revenu sur un projet
description: Vous pouvez utiliser les taux de facturation pour calculer le chiffre d’affaires de vos projets lorsque vous les multipliez par les heures consacrées au projet.
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: fda01f74912b5b9f28085e6dbc79ca3ba69e38fc
workflow-type: tm+mt
source-wordcount: '4653'
ht-degree: 77%

---

# Présentation du remplacement des taux de facturation et du calcul du revenu d’un projet

{{highlighted-preview}}

Vous pouvez utiliser les taux de facturation pour calculer les revenus de vos projets lorsque vous les multipliez par les heures passées sur le projet. Pour plus d’informations sur les taux de facturation et les revenus, consultez l’article [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Vue d&#39;ensemble des taux de facturation et des types de revenus de tâche

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez associer des taux de facturation à des personnes et à des fonctions.\
Pour plus d’informations sur la création d’utilisateurs et utilisatrices et leur association aux taux de facturation, consultez l’article [Ajouter des personnes](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Pour plus d’informations sur la création de fonctions et leur association aux taux de facturation, consultez l’article [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

<div class="preview">

### Présentation - Package Workflow Ultimate

Les taux de facturation associés aux utilisateurs et aux fonctions peuvent être remplacés au niveau du projet.

Pour calculer les revenus sur les projets suivant les taux de facturation des fonctions, le **Type de revenu** des tâches sur les projets doit être l’un des suivants :

* Rôle par heure
* Rôle par heure avec limite
* Rôle par heure plus fixe
* Utilisateur ou utilisatrice et rôle par heure
* Utilisateur et rôle par heure avec limitation
* Utilisateur ou utilisatrice et rôle par heure plus fixe

Pour calculer le revenu des projets en fonction des taux de facturation des utilisateurs, le type de revenu des tâches des projets doit être l&#39;un des suivants :

* Utilisateur, par heure
* Personne, par heure avec limite
* Utilisateur, par heure plus fixe
* Utilisateur ou utilisatrice et rôle par heure
* Utilisateur et rôle par heure avec limitation
* Utilisateur ou utilisatrice et rôle par heure plus fixe

Pour plus d’informations sur le **Type de revenu** et les taux de facturation, voir [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

</div>

### Présentation : tous les autres packages de Workfront et de workflow

Les taux de facturation associés aux personnes ne peuvent pas être remplacés.

Les taux de facturation associés aux fonctions peuvent être remplacés au niveau de l’entreprise ou du projet.

Pour calculer les revenus sur les projets suivant les taux de facturation des fonctions, le **Type de revenu** des tâches sur les projets doit être l’un des suivants :

* Rôle par heure
* Rôle par heure avec limite
* Rôle par heure plus fixe

Pour plus d’informations sur le **Type de revenu** et les taux de facturation, voir [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<div class="preview">

## Hiérarchie des remplacements de taux de facturation lors du calcul du chiffre d’affaires - Package Ultimate de workflow

>[!NOTE]
>
>Les types de revenus Utilisateur et Rôle par heure suivent une hiérarchie détaillée lors de la localisation du taux de facturation pour le calcul du revenu. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Une fonction peut être associée à un taux de facturation de la manière suivante :

* En tant qu’administrateur ou administratrice Workfront, vous pouvez définir le taux de facturation au niveau du système associé à une fonction lorsque vous créez cette fonction.\
  Pour plus d’informations sur la création de fonctions, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* En tant qu’administrateur Workfront, vous pouvez définir des cartes tarifaires avec plusieurs taux de facturation par rôle, en fonction des attributs et des dates d’entrée en vigueur. Lorsqu’une carte tarifaire est associée à un projet, tous les rôles, leurs attributs et leurs taux de facturation associés sont ajoutés à la section Taux de facturation du projet. Le fait de joindre une carte tarifaire remplace les taux de facturation existants sur le projet.

  Pour plus d’informations, voir [Gérer des cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md) et [Joindre une carte tarifaire à un projet](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

* En tant que personne gestionnaire de projet, vous pouvez définir le taux de facturation de la même fonction au niveau du projet.\
  Les taux de fonction modifiés sur le projet n’auront une incidence que sur ce projet.

  Pour plus d’informations sur le remplacement des taux de rôle pour le projet, voir [Remplacer les taux de facturation des fonctions au niveau du projet](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

</div>

## Hiérarchie des remplacements de taux de facturation lors du calcul du chiffre d’affaires - tous les autres packages Workfront et Workflow

Une fonction peut être associée à un taux de facturation de la manière suivante :

* En tant qu’administrateur ou administratrice Workfront, vous pouvez définir le taux de facturation au niveau du système associé à une fonction lorsque vous créez cette fonction.\
  Pour plus d’informations sur la création de fonctions, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* En tant qu’administrateur ou administratrice Workfront, vous pouvez définir le taux de facturation au niveau de l’entreprise pour la même fonction lorsque vous créez une entreprise.\
  Lorsque Workfront calcule les revenus pour les projets associés à cette entreprise, le taux de facturation de l’entreprise est utilisé lorsque le rôle est affecté à des tâches, au lieu du taux de facturation au niveau du système pour cette fonction.\
  Les taux de fonction modifiés au niveau de l’entreprise auront un impact sur tous les projets associés à cette entreprise.

  >[!NOTE]
  >
  >Si vous devez mettre à jour le taux de facturation de l’entreprise, celui du projet ne sera pas mis à jour automatiquement. Vous devez supprimer l’entreprise du projet, mettre à jour le taux de l’entreprise, puis rattacher à nouveau l’entreprise au projet, avant que le nouveau taux de l’entreprise ne prenne effet sur le projet. Pour plus d’informations sur l’association d’une entreprise à un projet, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

  Pour plus d’informations sur la création de taux de facturation des fonctions spécifiques à une entreprise, voir [Créer et modifer des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* En tant qu’administrateur ou administratrice Workfront, vous pouvez activer une option lors de la modification d’un projet pour appliquer des modifications aux taux de facturation au niveau de l’entreprise au projet lorsque les personnes recalculent manuellement les finances du projet.\
  Pour plus d’informations, voir [Remplacer les taux de facturation au niveau du projet par les taux de facturation au niveau de l’entreprise](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* En tant que personne gestionnaire de projet, vous pouvez définir le taux de facturation de la même fonction au niveau du projet.\
  Les taux de fonction modifiés sur le projet n’auront une incidence que sur ce projet.

  Pour plus d’informations sur le remplacement des taux de rôle pour le projet, voir [Remplacer les taux de facturation des fonctions au niveau du projet](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Si une fonction est associée à un taux de facturation au niveau du système, de l’entreprise et du projet, Workfront calcule les revenus des tâches à l’aide du taux de facturation de la fonction au niveau du projet, lorsqu’il utilise les taux de fonction. Les revenus de toutes les tâches sont cumulés aux revenus du projet.

## Remplacer les taux de facturation des fonctions au niveau du projet

En tant que personne gestionnaire de projet, vous pouvez spécifier le taux de facturation d’une fonction sur un projet spécifique. Ce taux de facturation au niveau du projet remplace le taux de facturation au niveau du système pour cette fonction. Workfront utilise le taux de facturation au niveau de la fonction pour calculer les revenus, au lieu d’utiliser le taux de facturation au niveau du système.

<span class="preview">Vous pouvez également joindre une carte tarifaire au projet, qui importera les taux de facturation des fonctions de la carte tarifaire dans le projet.</span>

Pour plus d’informations sur la façon de remplacer les taux de facturation des fonctions au niveau du projet, voir [Remplacer les taux de facturation des fonctions au niveau du projet](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Pour plus d’informations sur la fonction utilisée pour calculer le chiffre d’affaires du projet, reportez-vous à la section [&#x200B; Calculs du chiffre d’affaires pour les tâches en fonction des affectations d’utilisateurs et de rôles &#x200B;](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) dans [Présentation de la facturation et du chiffre d’affaires](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<span class="preview">Pour plus d’informations sur l’association d’une carte tarifaire à un projet, voir [Joindre une carte tarifaire à un projet](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>Pour les revenus réels, les taux de facturation des heures ajoutées à un enregistrement de facturation marqué comme « Facturé » ne doivent pas être affectés par les remplacements de taux de facturation intervenant après la facturation de cet enregistrement.

<div class="preview">

## Présentation de la section Taux de facturation d’un projet - Package Ultimate de workflow

Après avoir spécifié les taux de facturation de remplacement pour les fonctions associées au projet, vous pouvez voir toutes les fonctions et leurs remplacements dans l’onglet **Taux > Taux de facturation** du projet.

### Regroupements de taux

Les taux de facturation sont regroupés dans la zone **Taux de facturation** d’abord par leur source (carte tarifaire ou remplacement), puis par les types de ressources : fonction ou utilisateur.

Dans la ligne de regroupement correspondant à une fonction, remarquez le taux de facturation de cette fonction au niveau du projet dans la colonne **Valeur**. Si la fonction comporte des taux de remplacement effectifs par date, les taux sont affichés dans l&#39;ordre par date.

Lorsqu’il existe des taux de remplacement ou des taux de carte tarifaire pour une fonction, le taux par défaut du système pour la fonction n’est pas automatiquement appliqué lors du calcul du produit pour le projet. La hiérarchie est suivie pour déterminer le taux de facturation, en fonction du type de revenus. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

### Valeurs de taux de facturation multiples pour une fonction

Si vous disposez de plusieurs taux de facturation de remplacement pour une fonction spécifique, ils sont répertoriés sous le regroupement des fonctions. La modification en ligne vous permet de modifier les taux de remplacement et les **Date de début** et **Date de fin** des taux de remplacement dans cet onglet. Ou sélectionnez un taux et cliquez sur l’icône **Modifier** pour définir des taux de remplacement valides à une date.

>[!NOTE]
>
>Lorsque le champ **Date de début** ou **Date de fin** n&#39;est pas renseigné pour un taux effectif à la date, Workfront suppose que le premier taux de remplacement est appliqué pour toutes les heures dont la date est antérieure à la **Date de fin** du premier taux de remplacement et que le dernier taux de remplacement est appliqué pour toutes les heures dont la date est postérieure à la **Date de début** du dernier taux de remplacement.
>Si une heure est enregistrée avant la date de début prévue du projet, le premier taux de facturation est utilisé.\
>Si une heure est enregistrée après la date d’achèvement prévue du projet, le dernier taux de facturation est utilisé.

</div>

## Présentation de la section Taux de facturation d’un projet - Tous les autres packages Workfront et de workflow

Après avoir spécifié les taux de facturation de remplacement pour les fonctions associées au projet, vous pouvez voir tous les fonctions et leurs remplacements dans l’onglet **Taux de facturation** du projet.

Notez les informations suivantes dans la liste des **taux de facturation** :

* [Regroupement par fonction](#job-role-grouping)
* [Valeur du taux de facturation du projet](#project-billing-rate-value)
* [Valeur du taux de facturation par défaut](#default-billing-rate-value)
* [Valeur du taux de facturation de l’entreprise](#company-billing-rate-value)
* [Valeurs et délais de taux de facturation multiples](#multiple-billing-rate-values-and-timeframes)

### Regroupement par fonction {#job-role-grouping}

Les taux de facturation sont regroupés dans la zone **Taux de facturation** selon leurs fonctions respectives.

### Valeur du taux de facturation du projet {#project-billing-rate-value}

Dans la ligne de regroupement correspondant à une fonction, notez le taux de facturation de cette fonction au niveau du projet dans la colonne **Taux de facturation du projet**. Si la fonction comporte plusieurs taux de remplacement, celui qui correspond à la date actuelle est affiché dans la ligne de regroupement de la colonne **Taux de facturation du projet**.

### Valeur du taux de facturation par défaut {#default-billing-rate-value}

Dans la ligne de regroupement d’une fonction, notez le taux de facturation de cette fonction au niveau du système dans la colonne **Taux de facturation par défaut**.

>[!NOTE]
>
>S’il existe des taux de facturation de projet pour une fonction, le **taux de facturation par défaut** n’est jamais appliqué au calcul des revenus pour le projet. Seule les **taux de facturation du projet** sont appliquées au calcul des revenus.

### Valeur du taux de facturation de l’entreprise {#company-billing-rate-value}

Dans la ligne de regroupement d’une fonction, notez le taux de facturation de cette fonction au niveau de l’entreprise dans la colonne **Taux de facturation de l’entreprise**. Cela signifie qu’une entreprise est associée à ce projet et que cette fonction a un taux de facturation différent pour cette entreprise. Le taux de facturation de l’entreprise s’affiche, même s’il est identique au taux du projet.

>[!NOTE]
>
>S’il existe des taux de facturation de projet pour une fonction, le **taux de facturation de l’entreprise** n’est jamais appliqué au calcul des revenus du projet. Seuls les **taux de facturation du projet** sont appliqués au calcul des revenus.

### Valeurs et délais de taux de facturation multiples {#multiple-billing-rate-values-and-timeframes}

Si vous disposez de plusieurs taux de facturation de remplacement pour une fonction spécifique, ils sont répertoriés sous le regroupement correspondant à cette fonction. La modification en ligne vous permet de modifier les taux de remplacement et les **Date de début** **Date** et **Date de fin** des taux de facturation de remplacement dans cet onglet. Ou sélectionnez un taux et cliquez sur l’icône **Modifier** pour définir des taux de remplacement valides à une date.

>[!NOTE]
>
>Vous ne pouvez pas spécifier une **date de début** pour le premier taux de remplacement, et vous ne pouvez pas spécifier une **date de fin** pour le dernier taux de remplacement. Workfront suppose que le premier taux de remplacement est appliqué à toutes les heures dont la date est antérieure à la **date de fin** du premier taux de remplacement et que le dernier taux de remplacement est appliqué à toutes les heures dont la date est plus récente que la **date de début** du dernier remplacement.\
>Si une heure est enregistrée avant la date de début prévue du projet, le premier taux de facturation est utilisé.\
>Si une heure est enregistrée après la date d’achèvement prévue du projet, le dernier taux de facturation est utilisé.

## Calculer les revenus prévus

* [Calculer les revenus prévus en fonction d’un remplacement unique du taux de facturation](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calculer les revenus prévus en fonction de plusieurs remplacements de taux de facturation](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Répartition des heures prévues sur la durée d’une tâche](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calculer les revenus prévus en fonction d’un remplacement unique du taux de facturation {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Tenez compte des points suivants lors du calcul du revenu prévu sur la base d’un remplacement de taux de facturation unique :

* Lorsque le **Type de revenu** d’une tâche est **Rôle par heure**, Workfront multiplie le nombre d’heures prévues d’une tâche par le taux de facturation de la fonction associée à la tâche pour calculer ses revenus prévus.

* <span class="preview">Lorsque le **Type de revenus** d’une tâche est **Utilisateur et rôle par heure**, Workfront utilise une hiérarchie pour déterminer le taux de facturation de chaque tâche. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).</span>

* Lorsque le taux de facturation de la fonction a été remplacé au niveau du projet, Workfront utilise le taux de remplacement du projet pour calculer les revenus prévus.
* Lorsqu’une tâche comporte plusieurs affectations, les revenus prévus sont calculées en multipliant le taux de facturation de chaque fonction de l’affectation et de l’attribution du nombre d’heures prévues correspondante.

>[!NOTE]
>
>Dans le cas de plusieurs affectations, le nombre d’heures prévues par affectation n’est pas identique au nombre d’heures prévues de la tâche.

Pour plus d’informations sur la fonction utilisée pour calculer les revenus prévus, voir la section « Présentation des calculs de revenus pour les tâches basées sur les affectations d’utilisateurs et utilisatrices et de rôles » de l’article [Présentation de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calculer les revenus prévus en fonction de plusieurs remplacements de taux de facturation {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Tenez compte des points suivants lors du calcul du revenu prévu en fonction de plusieurs remplacements de taux de facturation :

* Lorsque le **Type de revenu** d’une tâche est **Rôle par heure**, Workfront multiplie le nombre d’heures prévues d’une tâche par le taux de facturation de la fonction associée à la tâche pour calculer ses revenus prévus.

  Pour plus d’informations sur la fonction utilisée pour calculer les revenus prévus, voir la section « Présentation des calculs de revenus pour les tâches basées sur les affectations d’utilisateurs et utilisatrices et de rôles » de l’article [Présentation de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<div class="preview">

* Lorsque le **Type de revenu** d’une tâche est **Utilisateur et rôle par heure** et qu’aucun utilisateur n’est affecté, Workfront multiplie les heures prévues d’une tâche par l’une de ces valeurs pour calculer le revenu prévu de la tâche :

   * Taux de remplacement manuel pour la fonction sur la tâche
   * Taux de fonctions du projet, qui peut provenir d’une carte tarifaire ou du niveau système.

  Pour plus d&#39;informations sur la fonction utilisée pour calculer le revenu prévu, voir [Présentation de la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) et la section [Calculs du revenu pour les tâches en fonction des affectations d&#39;utilisateurs et de rôles](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) de l&#39;article [Présentation de la facturation et du revenu](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

</div>

* Dans le cas de remplacements multiples de taux de facturation, le taux par lequel le nombre d’heures prévues est multiplié change pendant la durée d’une tâche. Par défaut, Workfront répartit le nombre d’heures prévues uniformément sur la durée d’une tâche, attribuant un nombre égal d’heures pour chaque jour de la tâche. Lors du calcul des **revenus prévus** d’une tâche, Workfront multiplie le nombre d’heures prévues par jour par le taux de facturation de ce jour. S’il existe plusieurs taux de facturation, ce taux peut être différent chaque jour.

  Par exemple, vous avez une tâche dont le **Type de revenu** est Rôle par heure. La tâche a une durée de 5 jours et une valeur du nombre d’heures prévues de 40 heures. Le nombre d’heures prévues par jour est de 8 heures. Attribuez une fonction Personne gestionnaire de projet à la tâche et remplacez le taux de facturation de cette fonction pour les trois derniers jours de la tâche. Vous aurez donc un taux de facturation 1 pour les deux premiers jours et un taux de facturation 2 pour les trois jours restants de la tâche pour cette fonction.

  La formule qui calcule les **revenus prévus** de cette tâche est la suivante :

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Pour plus d’informations sur le calcul du nombre d’heures prévues par jour dans Workfront, voir la section [Répartition du nombre d’heures prévues sur la durée d’une tâche](#distribution-of-planned-hours-across-the-duration-of-a-task) dans cet article.

>[!NOTE]
>
>Si la tâche comporte plusieurs personnes cessionnaires, le nombre d’heures planifiées est d’abord réparti entre chaque personne cessionnaire, puis entre chaque jour de la durée de la tâche. Dans ce cas, les revenus prévus seront calculés en prenant en compte le nombre d’heures quotidiennes pour chaque personne cessionnaire et le taux de facturation de chaque fonction qui pourrait changer pendant la durée de la tâche, s’il existe plusieurs taux de facturation.

### Répartition des heures prévues sur la durée d’une tâche {#distribution-of-planned-hours-across-the-duration-of-a-task}

Tenez compte de ce qui suit concernant la répartition du nombre d’heures prévues sur la durée d’une tâche :

* Par défaut, Workfront répartit le nombre d’heures prévues uniformément sur la durée d’une tâche, en attribuant un nombre égal d’heures prévues à chaque jour de la tâche, en fonction de la disponibilité du planning du projet.

  Pour plus d’informations sur la répartition du nombre d’heures prévues sur la durée d’une tâche, voir la section « Présentation de la répartition du nombre d’heures prévues sur la durée d’une tâche » dans l’article [Vue d’ensemble du nombre d’heures prévues](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >Le nombre d’heures prévues par jour correspond au nombre d’heures prévues attribué à chaque jour pendant la durée de la tâche. Si la tâche comporte une seule affectation, ce nombre représente également le nombre d’heures prévues par jour et par affectation. Si la tâche comporte plusieurs affectations, le nombre d’heures prévues par jour et par affectation est différent du nombre d’heures prévues par jour pour la tâche. Il n’existe aucune représentation visuelle dans Workfront pour le nombre d’heures prévues par jour et par affectation, pour les tâches avec plusieurs affectations.
  >
  >
  >Le nombre d’heures prévues par jour est multiplié par le taux de facturation de la fonction affectée à la tâche pour ce jour afin de calculer les revenus prévus par jour pour cette tâche. Une somme de tous les revenus prévus quotidiens calculés de cette manière est égale aux revenus prévus pour cette tâche.

## Calculer les revenus réels

Le taux de facturation du revenu réel est basé sur le propriétaire des heures consignées pour une tâche. Le « propriétaire » est la personne dont le temps est enregistré pour la tâche, même s’il n’est pas affecté à la tâche.

* [Calculer les revenus réels en fonction d’un remplacement unique de taux de facturation](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calculer les revenus réels en fonction de plusieurs remplacements de taux de facturation](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calculer les revenus réels en fonction d’un remplacement unique de taux de facturation {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Tenez compte des éléments suivants lorsque vous calculez les revenus réels en fonction d’un remplacement unique de taux de facturation :

* Lorsque le **Type de revenu** d’une tâche est **Rôle par heure**, Workfront multiplie les **Heures effectives** d’une tâche par le taux de facturation de la fonction associée à la tâche pour calculer les **Revenus réels** de la tâche. Les heures effectives sont les heures consignées directement pour la tâche.

  Pour plus d’informations sur la fonction utilisée pour calculer les **Revenus réels**, voir la section « Présentation du calcul des revenus pour les tâches basées sur les affectations d’utilisateurs et utilisatrices et de rôles » dans l’article [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* <span class="preview">Lorsque le **Type de revenus** d’une tâche est **Utilisateur et rôle par heure**, Workfront utilise une hiérarchie pour déterminer le taux de facturation de chaque tâche. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).</span>

* Si le taux de facturation de la fonction a été remplacé au niveau du projet, Workfront utilise le taux de remplacement du projet pour calculer les revenus réels. Lorsque vous remplacez le taux de facturation de la fonction sur le projet, les **Revenus réels** du projet sont recalculés automatiquement en utilisant le nouveau taux.

  Pour plus d’informations sur la modification des taux des fonctions pour un projet, voir [Remplacer les taux de facturation des fonctions au niveau du projet](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Si vous souhaitez que les heures que vous avez déjà enregistrées sur le projet avant d’annuler le taux de facturation initial soient facturées au taux initial, vous devez les inclure dans un **enregistrement de facturation**, et vous devez marquer l’**enregistrement de facturation** comme **Facturé**. Dans le cas contraire, les **Revenus réels** des heures enregistrées avant le remplacement du taux de facturation du projet seront recalculés en utilisant le nouveau taux lorsque les finances des projets seront recalculées.\
>Pour plus d’informations sur l’inclusion d’heures dans un enregistrement de facturation et le marquage de cet enregistrement comme **Facturé**, voir l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calculer les revenus réels en fonction de plusieurs remplacements de taux de facturation {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Tenez compte des éléments suivants lorsque vous calculez les revenus réels en fonction de plusieurs remplacements du taux de facturation :

* Lorsque le **Type de revenu** d’une tâche est **Rôle par heure**, Workfront multiplie les **Heures effectives** de la tâche avec le taux de facturation des fonctions affectées à la tâche pour calculer ses **Revenus réels**. Les heures effectives sont les heures consignées directement pour la tâche.

* <span class="preview">Lorsque le **Type de revenus** d’une tâche est **Utilisateur et rôle par heure**, Workfront utilise une hiérarchie pour déterminer le taux de facturation de chaque tâche. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).</span>

* S’il existe plusieurs remplacements du taux de facturation, le taux par lequel les **Heures effectives** sont multipliées pour calculer les **Revenus réels** peut changer pendant la durée d’une tâche. Workfront utilise le taux de facturation de la fonction dont la période correspond à la **Date d’entrée** des heures consignées pour la tâche afin de calculer les **Revenus réels**.

  Par exemple, une tâche qui possède le **Type de revenu** **Rôle par heure** est affectée à la fonction Personne gestionnaire de projet. Remplacez le taux de facturation de cette fonction par le taux 1 pour les dates comprises entre le 19 et le 25 juin. À partir du 26 juin, le taux de facturation sera remplacé par le taux 2. Enregistrez 2 heures pour le 20 juin et 3 heures pour le 28 juin.

  Workfront calcule les **Revenus réels** de cette tâche à l’aide de la formule suivante :

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Pour plus d’informations sur la fonction à utiliser pour calculer les **Revenus réels**, voir la section « Présentation des calculs de revenus pour les tâches basées sur les affectations d’utilisateurs et utilisatrices et de rôles » dans l’article [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Impact des fuseaux horaires lors du calcul du chiffre d’affaires en fonction de plusieurs taux de facturation

Les utilisateurs et utilisatrices peuvent voir des nombres d’heures prévues par jour différents de ceux d’autres personnes, si les fuseaux horaires diffèrent entre eux et d’autres entités de Workfront. Les scénarios suivants peuvent fausser les informations sur le nombre d’heures prévues par jour d’un utilisateur ou d’une utilisatrice par rapport à ce que voit une autre personne :

* Il se peut que les ordinateurs des deux personnes soient réglés sur deux fuseaux horaires différents.
* Les deux profils d’utilisateur ou d’utilisatrice dans Workfront peuvent être réglés sur deux fuseaux horaires différents.
* Le fuseau horaire associé au profil de la personne peut être différent du fuseau horaire du système dans Workfront.
* Le fuseau horaire associé au profil de la personne peut être différent du fuseau horaire du planning du projet.

Dans ces cas, le nombre d’heures prévues par jour peut être différent entre deux personness qui ne partagent pas les mêmes paramètres pour les fuseaux horaires. Elles verront également des chiffres différents pour les revenus prévus lorsqu’elles utilisent plusieurs taux de facturation pour un projet.

* [Calculer les revenus prévus pour les personnes dans différents fuseaux horaires](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calculer les revenus réels pour les personnes dans différents fuseaux horaires](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calculer le revenu prévu des utilisateurs dans différents fuseaux horaires {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Si des personnes situées dans des fuseaux horaires différents travaillent sur les mêmes projets, nous vous recommandons de ne pas modifier les taux de facturation pour vos projets pendant la semaine. Ce faisant, vous risquez d’afficher un montant erroné de revenus prévus pour votre projet, en raison des différences d’heures entre les fuseaux horaires du planning des personnes et le fuseau horaire du système Workfront. La plupart des plannings permettent d’exclure les week-ends du calcul du nombre d’heures prévues. Si une modification est apportée au taux de facturation d’une fonction, il est préférable qu’elle ait lieu pendant un week-end plutôt qu’au milieu de la semaine, où elle pourrait coïncider avec le milieu de la durée d’une tâche.

Tenez compte des points suivants lors du calcul du revenu prévu pour les utilisateurs de différents fuseaux horaires :

* Pour les tâches dont le **Type de revenu** est **Rôle par heure** ou <span class="preview">**Utilisateur et rôle par heure**</span> et qui sont affectées à des fonctions, le **Revenu prévu** est calculé en multipliant le **Heures prévues** d’une tâche par le taux de facturation de la fonction.

* Le **Nombre d’heures prévues** est réparti uniformément sur la **Durée** de la tâche.

* La **Durée** est la période de temps qui s’écoule entre la **Date de début prévue**&#x200B;**&#x200B;** et la **Date d’achèvement prévue** de la tâche. Comme la **Date de début prévue** et la **Date d’achèvement prévue** des tâches peuvent différer en fonction des fuseaux horaires des personnes qui visualisent la tâche, le nombre d’heures prévues par jour peut être différent pour deux personnes situées dans deux fuseaux horaires différents.

* Le nombre d’heures prévues par jour ne modifie pas les revenus prévus d’un projet si le taux de facturation de la fonction n’est pas modifié ou s’il n’y a qu’un seul remplacement du taux de facturation. Dans ce cas, même si deux personnes de deux fuseaux horaires différents voient des heures prévues par jour différentes, les revenus prévus globaux du projet sont identiques pour les deux personnes.

  Cependant, dans le cas de plusieurs remplacements de taux de facturation, les **Revenus prévus** globaux du projet peuvent sembler différents pour deux personnes dans deux fuseaux horaires différents, car ils dépendent du nombre d’heures prévues par jour (qui peut être différent pour les deux personnes) et du remplacement du taux de facturation (qui peut être différent pour le même jour, lorsque chaque personne examine la tâche dans son propre fuseau horaire).

* Le montant exact des **Revenus prévus** est celui vu par la personne qui a le même fuseau horaire que celui de votre instance Workfront. Votre administrateur ou administratrice Workfront définit le fuseau horaire Workfront dans la zone Infos client du système.\
  Pour plus d’informations sur la définition du fuseau horaire de votre système, voir l’article [Configurer les informations de base de votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calculer le revenu réel des utilisateurs dans différents fuseaux horaires {#calculate-actual-revenue-for-users-in-different-time-zones}

Tenez compte des points suivants lors du calcul du revenu réel des utilisateurs dans différents fuseaux horaires :

* Lorsque le **Type de revenu** d’une tâche est **Rôle par heure** ou <span class="preview">**Utilisateur et rôle par heure**</span>, Workfront multiplie les **Heures réelles** de la tâche par le taux de facturation des fonctions affectées à la tâche afin de calculer le **Revenu réel**. Les heures effectives sont les heures consignées directement pour la tâche.

* Dans le cas de plusieurs remplacements du taux de facturation, Workfront utilise le taux de facturation de la fonction dont la période correspond à la **Date d’entrée** des heures consignées pour la tâche afin de calculer les **Revenus réels**.

* Comme il n’y a pas de date et heure sur la **Date d’entrée** des heures consignées et qu’il n’y a pas de date et heure sur les plages de dates des remplacements multiples du taux de facturation, les calculs des **Revenus réels** ne sont pas affectés par le fuseau horaire associé aux personnes.

Pour plus d’informations sur la fonction utilisée pour calculer les **Revenus réels**, consultez la section « Comprendre les calculs de revenus pour les tâches basées sur les affectations de personnes et de rôles » dans l’article [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Recalculer les finances d’un projet

Les finances sont calculées sur un projet au fur et à mesure des changements dans les heures consignées pour le projet.

Si les taux sont modifiés pendant la durée de vie d’un projet, vous pouvez recalculer les coûts et les revenus du projet manuellement, en utilisant l’option Recalculer finances sur un projet. En outre, certaines actions déclenchent un nouveau calcul automatique.

Pour plus d’informations sur le recalcul des finances d’un projet, voir l’article [Recalculer les finances d’un projet](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Ajouter un nouveau taux de facturation à l’aide de l’API

Pour ajouter un nouveau taux de facturation pour une fonction à l’aide de l’API, vous effectuez une action *setRatesForRole* pour l’objet **Taux** à l’aide de la *méthode PUT*.
Les champs action et date de l’objet **Taux** sont disponibles dans la version 8.0 de l’API.
Si vous avez déjà défini plusieurs taux de facturation pour une fonction sur un projet et que vous souhaitez ajouter un nouveau taux de facturation avec une nouvelle plage de dates, vous devez inclure à la fois le taux existant et le taux à ajouter dans le même appel API. Cette méthode est similaire à celle utilisée pour mettre à jour les collections d’objets.

L’appel API suivant est un exemple où **attachableID** est l’**ID du projet** du projet pour lequel vous ajoutez le taux et **RoleID** est l’**ID de la fonction** pour laquelle vous ajoutez le nouveau taux de facturation.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         {« rateValue »:« 0.00 »,« startDate »:null,« endDate »:« 2017-06-11 »},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {« rateValue »:« 95.00 »,« startDate »:« 2017-06-21 »,« endDate »:null}</pre><pre>]</pre><pre>}</pre>Pour plus d’informations sur l’utilisation de l’API Workfront, voir l’article [Concepts de base de l’API](https://experience.workfront.com/s/article/API-Basics-638808549).
