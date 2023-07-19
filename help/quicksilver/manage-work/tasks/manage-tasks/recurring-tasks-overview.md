---
content-type: overview
product-area: projects
keywords: recurrent,reoccur,récurrent
navigation-topic: manage-tasks
title: Présentation des tâches récurrentes
description: Présentation des tâches récurrentes
author: Alina
feature: Work Management
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: f8d596121f90d4f0c57e65cc415d1df87c14730c
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 2%

---

# Présentation des tâches récurrentes

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Vous pouvez créer des tâches récurrentes pour les activités que vous devez répéter dans le cadre d’un seul projet.

Cet article présente des informations et des considérations sur la création et la modification de tâches récurrentes.

Pour plus d’informations sur la création de tâches récurrentes dans Adobe Workfront, voir [Créer des tâches récurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Tâches récurrentes - Aperçu et remarques

Vous pouvez choisir de créer des tâches récurrentes pour indiquer le travail répétable pendant la durée de vie d’un projet.

Par exemple, lors d’un projet informatique, les logiciels doivent probablement être sauvegardés à intervalles réguliers. La création d’une tâche récurrente pour cette activité réduit le temps nécessaire à la configuration de plusieurs tâches individuelles.

Tenez compte des points suivants lors de la création de tâches récurrentes dans Workfront :

* Vous ne pouvez pas ajouter de tâches récurrentes à un modèle.
* Vous ne pouvez pas ajouter une fréquence de périodicité à une tâche existante.
* Les tâches récurrentes apparaissent en tant que sous-tâches ou enfants pour l’occurrence principale qui apparaît en tant que tâche parente.
* Vous ne pouvez pas joindre de validation à une tâche récurrente parent.
* Workfront transfère la plupart des champs que vous mettez à jour pour la périodicité parent lors de sa création vers les tâches enfants. Les champs suivants ne sont pas transférés vers les tâches enfants lors de leur création :

   * La contrainte de tâche des tâches enfants se transforme automatiquement en :

      * Doit démarrer sur pour les projets planifiés à partir de la date de début.
      * Doit être terminé le pour les projets planifiés à partir de la date d’achèvement.

   * Les documents joints au parent ne sont pas transférés aux enfants.

* Les modifications suivantes se produisent sur la tâche parent une fois que vous avez indiqué que la tâche est récurrente :

   * Le champ Durée est renommé Durée par occurrence pour la tâche parent. Il reste Durée pour les tâches des enfants.
   * L’état est désactivé sur la tâche parent et automatiquement défini sur Nouveau sur les enfants. La tâche parente se termine automatiquement et l’état est mis à jour sur Terminé lorsque tous les enfants sont terminés.
   * Les seuls types de durée disponibles pour les tâches récurrentes sont les suivants :

      * Simple
      * Piloté par l&#39;effort
* La Durée et les Heures planifiées indiquées pour une nouvelle tâche récurrente sont la Durée et les Heures planifiées de chaque périodicité. La Durée de la tâche parent est l’heure entre la Date de début planifiée de la première tâche et la Date de fin planifiée de la dernière tâche. Les Heures planifiées de la tâche parent sont le total de toutes les Heures planifiées de toutes les récurrences.

## Observations relatives à la modification des tâches récurrentes

Certaines modifications que vous apportez à un parent de tâche récurrente peuvent ne pas être mises à jour sur toutes les récurrences existantes. Les tâches enfants qui affichent la progression ou qui ont été mises à jour individuellement ne sont pas mises à jour lorsque vous mettez à jour le parent. Workfront considère qu’une tâche affiche des progrès dans les situations suivantes :

* L’état est mis à jour et la tâche n’est plus nouvelle.
* Le pourcentage d’achèvement de la tâche est supérieur à zéro
* La tâche a des relations de prédécesseur

Le tableau suivant indique si les modifications apportées au déclencheur parent sont mises à jour sur les enfants qui n’ont pas été modifiés individuellement ou affichent la progression :

| Champs mis à jour sur la tâche parent | Mises à jour du transfert vers les enfants non modifiés ou les enfants sans progression enregistrés |
|---|---|
| Fréquence de récurrence* | ✔ |
| Affectations&#42;&#42; | ✔ |
| Nom | ✔ |
| Description | ✔ |
| Priorité | ✔ |
| Durée | ✔ |
| Heures prévues | ✔ |
| Type de coût | ✔ |
| Type de revenu | ✔ |
| Nivellement des ressources | ✔ |
| Délai de nivellement | ✔ |
| Contrainte de tâche | Ne met pas à jour les enfants |
| Ajout ou suppression d’une Forms personnalisée | Ne met pas à jour les enfants |
| Type de durée | Ne met pas à jour les enfants |
| Informations sur les formulaires personnalisés | Ne met pas à jour les enfants |

{style="table-layout:auto"}

&#42; Les scénarios suivants existent lorsque vous mettez à jour la Fréquence de périodicité d’une tâche parent :

* Si vous modifiez la Fréquence de périodicité sur une tâche parente existante, les sous-tâches existantes sont supprimées et remplacées par de nouvelles sous-tâches qui suivent la nouvelle fréquence de périodicité si elles n’affichent aucune progression et si vous ne les avez pas mises à jour manuellement.
* Si vous modifiez la Fréquence de périodicité sur une tâche parente existante, les sous-tâches qui affichent la progression ne sont pas supprimées. Ces tâches sont considérées comme distinctes de la périodicité actuelle.

&#42;&#42; Les affectations effectuées sur la tâche parent sont appliquées à toutes les sous-tâches de la périodicité. Toute modification apportée à l’affectation sur la tâche parente remplace toute affectation individuelle sur la sous-tâche. Si la tâche affiche la progression, l’affectation ne change pas.

 
