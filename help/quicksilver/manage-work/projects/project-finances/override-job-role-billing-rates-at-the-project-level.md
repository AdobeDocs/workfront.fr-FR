---
product-area: projects
navigation-topic: financials
title: Remplacer les taux de facturation des fonctions au niveau du projet
description: En tant que personne gestionnaire de projet, vous pouvez spécifier le taux de facturation d’une fonction sur un projet spécifique. Ce taux de facturation au niveau du projet remplace le taux de facturation au niveau du système pour cette fonction. Workfront utilise le taux de facturation au niveau de la fonction pour calculer les revenus, au lieu d’utiliser le taux de facturation au niveau du système.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 41%

---

# Remplacer les taux de facturation des fonctions au niveau du projet

{{highlighted-preview}}

En tant que personne gestionnaire de projet, vous pouvez spécifier le taux de facturation d’une fonction sur un projet spécifique. Ce taux de facturation au niveau du projet remplace le taux de facturation au niveau du système pour cette fonction. Workfront utilise le taux de facturation au niveau de la fonction pour calculer les revenus, au lieu d’utiliser le taux de facturation au niveau du système.

Cet article décrit comment vous pouvez remplacer les taux de facturation des fonctions au niveau du système pour un projet.

Pour obtenir des informations générales sur le remplacement des taux de facturation des fonctions pour les projets et le calcul du revenu du projet, voir [Présentation du remplacement des taux de facturation et du calcul du revenu sur un projet](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Pour plus d&#39;informations sur la fonction utilisée pour calculer le produit pour le projet, voir [Présentation de la hiérarchie des produits et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) et la section [Calculs du produit pour les tâches en fonction des affectations d&#39;utilisateurs et de rôles](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) de l&#39;article [Présentation de la facturation et du produit](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>Pour les revenus réels, les taux de facturation des heures ajoutées à un enregistrement de facturation marqué comme « Facturé » ne doivent pas être affectés par les remplacements de taux de facturation intervenant après la facturation de cet enregistrement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Pour remplacer le taux de facturation d’une fonction pour un projet : tout Workfront ou package de workflow</p>
        <p>Pour appliquer des attributs à la fonction : Workflow Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets et aux données financières</p> <p>Accès administratif aux fonctions</p></td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Gérer les autorisations du projet qui inclut Modifier les données financières </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remplacer les taux de facturation des fonctions au niveau du projet

Lorsque vous remplacez le taux de facturation d&#39;un projet, vous pouvez affecter des dates de validité et chaque période a un taux différent. Si vous n&#39;affectez pas de dates de validité, le remplacement du taux de facturation que vous saisissez est utilisé pour toute la durée du projet afin de calculer le produit.

Vous pouvez ajouter de nouveaux taux de facturation à un modèle de projet, lesquels deviennent des taux de facturation du projet lorsque vous créez le projet à partir de ce modèle. Pour plus d’informations sur la modification de modèles, voir [Modifier des modèles de projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>Vous ne pouvez pas remplacer les taux de facturation des utilisateurs pour un projet à moins que vous ne disposiez du package Workflow Ultimate.

Pour remplacer un taux de facturation dans un projet, procédez comme suit :

1. Accédez au projet dont vous souhaitez remplacer les taux de facturation.
1. Cliquez sur **Taux de facturation** dans le panneau de gauche.

   Ou

   <span class="preview">Cliquez sur **Taux** dans le panneau de gauche, puis cliquez sur l’onglet **Facturation** s’il n’est pas déjà sélectionné.</span>

1. Cliquez sur **Ajouter un taux de facturation** > **Nouveau taux de facturation**.

   Ou

   <span class="preview">Cliquez sur **Ajouter un taux de facturation > Nouveau taux de facturation de la fonction**.</span>

   La zone « Nouveau taux de facturation » apparaît.

1. Sélectionnez dans le champ **Fonction** la fonction dont vous souhaitez modifier le taux de facturation.

1. <span class="preview">(Facultatif) Sélectionnez des attributs pour le taux de facturation, tels que l’agence ou l’emplacement.</span>

   <span class="preview">L&#39;administrateur système définit les attributs de taux dans la zone Configuration.</span>

1. Sélectionnez la **Devise** pour le remplacement du taux de facturation.
1. Dans le champ **Taux de facturation**, saisissez le remplacement du taux de facturation, puis cliquez sur **Enregistrer** pour remplacer le taux de facturation une fois

   Ou

   Cliquez sur **Ajouter un taux** pour remplacer d’autres taux de facturation.

1. (Conditionnel) Pour les remplacements du taux de facturation effectif à une date donnée, saisissez les informations suivantes pour chaque ligne :

   * **Taux de facturation** : valeur du taux de facturation du début du projet à la première date du premier remplacement.
   * **Date de début** : date à laquelle le remplacement du taux de facturation commence.
   * **Date de fin** : date de fin de la redéfinition (override) du taux de facturation.

   ![Taux de facturation avec dates de remplacement](assets/new-job-role-billing-rate-on-project2.png)

   Workfront applique le taux de remplacement de la fonction aux heures qui se produisent pendant ces périodes lors du calcul du chiffre d’affaires du projet.

   Workfront vous permet de laisser des espaces entre les délais de remplacement, mais vous recevrez un avertissement pour confirmer que c’est intentionnel.

   Il n&#39;est pas nécessaire de spécifier une date de début pour le premier taux de remplacement ni une date de fin pour le dernier taux de remplacement.

   Si vous saisissez un seul remplacement de taux de facturation, ce taux s’applique pour toute la durée du projet. Si vous ajoutez plusieurs remplacements effectifs par la date, Workfront suppose que le premier remplacement s’applique à toutes les heures précédant sa date de fin et que le dernier remplacement s’applique à toutes les heures suivant sa date de début.

   Workfront suppose que le premier taux de remplacement est appliqué pour toutes les heures dont la date est antérieure à la date de fin du premier remplacement et que le dernier est appliqué pour toutes les heures dont la date est plus récente que la date de début du dernier remplacement.

   Si une heure est enregistrée avant la date de début prévue du projet, le tout premier taux de facturation est utilisé.

   Si une heure est consignée après la date d’achèvement prévue du projet, le tout dernier taux de facturation est utilisé.

1. Cliquez sur **Enregistrer**.
