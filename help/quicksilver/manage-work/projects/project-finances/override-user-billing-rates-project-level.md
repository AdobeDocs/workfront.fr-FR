---
content-type: overview
product-area: projects
navigation-topic: financials
title: Remplacer les taux de facturation de l’utilisateur au niveau du projet
description: Cet article décrit comment remplacer les taux de facturation des utilisateurs système pour un projet.
author: Lisa
feature: Work Management
source-git-commit: 8f6f14d4b36a9eee499111b1a37912f641c9f2ba
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 23%

---

# Remplacer les taux de facturation des utilisateurs au niveau du projet

{{highlighted-preview-article-level}}

En tant que chef de projet, vous pouvez spécifier le taux de facturation d’un utilisateur pour un projet spécifique. Ce taux de facturation au niveau du projet remplace le taux de facturation au niveau du système pour cet utilisateur. Workfront utilise le taux de facturation au niveau du projet de l’utilisateur pour calculer le revenu, au lieu d’utiliser le taux de facturation au niveau du système.

Cet article décrit comment remplacer les taux de facturation des utilisateurs système pour un projet.

Pour obtenir des informations générales sur le remplacement des taux de facturation pour les projets et le calcul du revenu du projet, voir [Présentation du remplacement des taux de facturation et du calcul du revenu sur un projet](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Pour plus d&#39;informations sur le calcul du produit pour le projet, voir [Présentation de la hiérarchie des produits et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) et la section [Calculs du produit pour les tâches en fonction des affectations d&#39;utilisateurs et de rôles](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) de l&#39;article [Présentation de la facturation et du produit](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets et aux données financières</p>
       <p><p>Vous devez également disposer de l’un des éléments suivants :</p> 
        <ul> 
          <li> <p>Niveau d’accès de l’administrateur système. </li> 
          <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Gérer les autorisations du projet qui inclut Modifier les données financières </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remplacer les taux de facturation de l’utilisateur au niveau du projet

Lorsque vous remplacez le taux de facturation d’un utilisateur pour un projet, vous pouvez affecter des dates de validité et chaque période comporte un taux différent. Si vous n&#39;affectez pas de dates de validité, le remplacement du taux de facturation que vous saisissez est utilisé pour toute la durée du projet afin de calculer le produit.

Pour remplacer un taux de facturation de l’utilisateur pour un projet :

1. Accédez au projet dont vous souhaitez remplacer les taux de facturation.
1. Cliquez sur **Taux** dans le panneau de gauche. Vous devrez peut-être d’abord cliquer sur **Afficher plus**.
1. Cliquez sur l’onglet **Facturation** s’il n’est pas déjà sélectionné.
1. Cliquez sur **Ajouter un taux de facturation** > **Nouveau taux de facturation de l’utilisateur**.

   La boîte Taux de facturation du nouvel utilisateur s’ouvre.

1. Dans le champ **Utilisateur**, sélectionnez l’utilisateur pour lequel vous souhaitez modifier le taux de facturation.
1. Sélectionnez la **Devise** pour le remplacement du taux de facturation.
1. Dans le champ **Taux de facturation**, saisissez le premier remplacement du taux de facturation.
1. (Facultatif) Cliquez sur **Ajouter un taux effectif à la date** pour ajouter d’autres remplacements de taux de facturation.
1. (Sous condition) Si vous ajoutez plusieurs remplacements de taux de facturation, spécifiez les informations suivantes pour chaque ligne :

   * **Taux de facturation** : valeur du taux de facturation au cours de la période spécifiée.
   * **Date de début** : date à laquelle le remplacement du taux de facturation commence.
   * **Date de fin** : date de fin de la redéfinition (override) du taux de facturation.

   ![Nouvelle zone Taux de facturation de l’utilisateur affichant les dates d’effet](assets/new-user-billing-rate-on-project2.png)

   Workfront applique le taux utilisateur de remplacement aux heures qui se produisent pendant ces périodes lors du calcul du chiffre d’affaires du projet.

   Workfront vous permet de laisser des espaces entre les délais de remplacement, mais vous recevrez un avertissement pour confirmer que c’est intentionnel.

   Il n&#39;est pas nécessaire de spécifier une date de début pour le premier taux de remplacement ni une date de fin pour le dernier taux de remplacement.

   Si vous saisissez un seul remplacement de taux de facturation, ce taux s’applique pour toute la durée du projet. Si vous ajoutez plusieurs remplacements effectifs par la date, Workfront suppose que le premier remplacement s’applique à toutes les heures précédant sa date de fin et que le dernier remplacement s’applique à toutes les heures suivant sa date de début.

   Workfront suppose que le premier taux de remplacement est appliqué pour toutes les heures dont la date est antérieure à la date de fin du premier remplacement et que le dernier est appliqué pour toutes les heures dont la date est plus récente que la date de début du dernier remplacement.

   Si une heure est enregistrée avant la date de début prévue du projet, le tout premier taux de facturation est utilisé.

   Si une heure est consignée après la date d’achèvement prévue du projet, le tout dernier taux de facturation est utilisé.

1. Cliquez sur **Enregistrer**.
