---
content-type: overview
product-area: projects
keywords: récurrent,revenant,récurrent
navigation-topic: manage-tasks
title: Aperçu des tâches récurrentes
description: Vue d’ensemble des tâches récurrentes
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
TQID: https://experienceleague.adobe.com/O5PP-k5GFVPeJoKRHiJbOv1r-05X7sAnmAR4wBLmijk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 679
ht-degree: 99%

---

# Vue d’ensemble des tâches récurrentes

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Vous pouvez créer des tâches récurrentes pour les activités que vous devez répéter dans le cadre d’un seul projet.

Cet article présente des informations et des considérations sur la création et la modification de tâches récurrentes.

Pour plus d’informations sur la création de tâches récurrentes dans Adobe Workfront, voir [Créer des tâches récurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Vue d’ensemble et considérations relatives aux tâches récurrentes

Vous pouvez choisir de créer des tâches récurrentes pour indiquer le travail répétable pendant la durée de vie d’un projet.

Par exemple, lors d’un projet informatique, les logiciels doivent probablement être sauvegardés à intervalles réguliers. La création d’une tâche récurrente pour cette activité réduit le temps nécessaire à la configuration de plusieurs tâches individuelles.

Tenez compte des points suivants lors de la création de tâches récurrentes dans Workfront :

* Vous ne pouvez pas ajouter de tâches récurrentes à un modèle.
* Vous ne pouvez pas ajouter une fréquence de périodicité à une tâche existante.
* Les tâches récurrentes apparaissent en tant que sous-tâches ou tâches enfants pour l’occurrence principale qui apparaît en tant que tâche parente.
* Vous ne pouvez pas joindre d’approbation à une tâche récurrente parent.
* Workfront transfère la plupart des champs que vous mettez à jour pour la périodicité parent lors de sa création vers les tâches enfants. Les champs suivants ne sont pas transférés vers les tâches enfants lors de leur création :

   * La contrainte de tâche des tâches enfants se transforme automatiquement en :

      * Doit Démarrer le pour les projets prévus à partir de la date de début.
      * Doit Être terminé le pour les projets prévus à partir de la date d’achèvement.

   * Les documents joints au parent ne sont pas transférés aux tâches enfants.

* Les modifications suivantes se produisent sur la tâche parent une fois que vous avez indiqué que la tâche est récurrente :

   * Le champ Durée est renommé Durée par occurrence pour la tâche parent. Il reste Durée pour les tâches enfants.
   * Le statut est Désactivé sur la tâche parent et automatiquement défini sur Nouveau pour les tâches enfants. La tâche parent se termine automatiquement et le statut est mis à jour sur Terminé lorsque toutes les tâches enfants sont terminées.
   * Les seuls types de durée disponibles pour les tâches récurrentes sont les suivants :

      * Simple
      * Piloté par l&#39;effort
* La durée et les heures prévues indiquées pour une nouvelle tâche récurrente sont la durée et les heures prévues de chaque occurrence. La durée de la tâche parent est le temps écoulé entre la date de début prévue de la tâche la plus ancienne et la date d’achèvement prévue e de la tâche la plus récente. Les heures prévues de la tâche parent sont le total de toutes les heures prévues de toutes les occurrences.

## Considérations relatives à la modification des tâches récurrentes

Certaines modifications que vous apportez à une tâche parent récurrente peuvent ne pas être mises à jour sur toutes les occurrences existantes. Les tâches enfants qui affichent la progression ou qui ont été mises à jour individuellement ne sont pas mises à jour lorsque vous mettez à jour le parent. Workfront considère qu’une tâche affiche la progression dans les situations suivantes :

* Le statut est mis à jour et la tâche n’est plus sur Nouveau.
* Le pourcentage terminé de la tâche est supérieur à zéro.
* La tâche a des relations de tâche antérieure

Le tableau suivant indique si les modifications apportées au déclencheur parent sont mises à jour sur les tâches enfants qui n’ont pas été modifiées individuellement ou affichent la progression :

| Champs mis à jour sur la tâche parent | Met à jour le transfert vers les tâches enfants non modifiées ou les tâches enfants sans progression enregistrés |
|---|---|
| Fréquence de périodicité* | ✔ |
| Affectations | ✔ |
| Nom | ✔ |
| Description | ✔ |
| Priorité | ✔ |
| Durée | ✔ |
| Heures prévues | ✔ |
| Type de coût | ✔ |
| Type de revenus | ✔ |
| Nivellement des ressources | ✔ |
| Délai de nivellement | ✔ |
| Contrainte de tâche | Ne met pas à jour les tâches enfants |
| Ajouter ou supprimer des formulaires personnalisés | Ne met pas à jour les tâches enfants |
| Type de durée | Ne met pas à jour les tâches enfants |
| Informations sur les formulaires personnalisés | Ne met pas à jour les tâches enfants |

{style="table-layout:auto"}

&#42; Les scénarios suivants existent lorsque vous mettez à jour la Fréquence de périodicité d’une tâche parent :

* Si vous modifiez la Fréquence de périodicité sur une tâche parent existante, les sous-tâches existantes sont supprimées et remplacées par de nouvelles sous-tâches qui suivent la nouvelle fréquence de périodicité si elles n’affichent aucune progression et si vous ne les avez pas mises à jour manuellement.
* Si vous modifiez la Fréquence de périodicité sur une tâche parent existante, les sous-tâches qui affichent la progression ne sont pas supprimées. À ce stade, ces tâches sont considérées comme distinctes de la périodicité.

&#42;&#42; Les affectations effectuées sur la tâche parent sont appliquées à toutes les sous-tâches de la périodicité. Toute modification apportée à l’affectation sur la tâche parent remplace toute affectation individuelle sur la sous-tâche. Si la tâche affiche la progression, l’affectation ne change pas.


