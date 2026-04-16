---
content-type: overview
product-area: projects
navigation-topic: financials
title: Définir un rapport des heures supplémentaires
description: Vous pouvez définir un taux d'heures supplémentaires pour une tâche afin d'ajuster le calcul du revenu prévu pour les affectations de tâche.
author: Lisa
feature: Work Management
exl-id: 832d3aab-3e09-4d83-91a6-be0145ce3554
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 15%

---

# Définir un taux d’heures supplémentaires

Lorsqu&#39;un ratio d&#39;heures supplémentaires est ajouté à une tâche, il est appliqué à toutes les affectations de la tâche. Il multiplie toutes les heures prévues pour cette tâche et affecte les calculs du revenu prévu.

Le taux d&#39;heures supplémentaires ne peut pas varier pour les affectations au sein de la même tâche. Si différents multiplicateurs d&#39;heures supplémentaires sont requis, vous devez créer des sous-tâches distinctes sous une tâche parent.

>[!NOTE]
>
>Aucune validation n&#39;empêche l&#39;ajout du taux d&#39;heures supplémentaires à une tâche qui n&#39;en fait pas.

## Calcul des heures supplémentaires sur le revenu prévu

Le système détermine d’abord le taux de facturation à l’aide de la hiérarchie de taux de facturation standard. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Si le taux d&#39;heures supplémentaires existe sur la tâche, le calcul est :
Revenu prévu = Taux de facturation × Ratio des heures supplémentaires × Heures prévues

Si le ratio des heures supplémentaires est vide, le calcul est :
Revenu prévu = Taux de facturation × Heures prévues

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
   <td>Modifier l’accès aux données de tâches, de projets et financières</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td><p>Gérer les autorisations d’accès à une tâche qui inclut la modification des taux de facturation</p>
     <p>Autorisations de contribution ou de niveau supérieur pour un projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Le type de revenu de la tâche doit être Utilisateur et Rôle par heure. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Le champ **Taux heures sup.** doit être activé sur votre modèle de mise en page.

1. Dans le modèle de disposition, cliquez sur la flèche vers le bas sous **Personnaliser ce que voient les utilisateurs**, puis cliquez sur **Tâche**.
1. Dans la section **Détails**, sélectionnez le champ **Ratio des heures supplémentaires** dans la zone **Finances**.

   Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Définir le taux d&#39;heures supplémentaires sur une tâche

1. Accédez à la tâche que vous souhaitez modifier.

   Pour plus d&#39;informations, voir [Gérer les finances de la tâche dans la section Détails de la tâche](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Cliquez sur **Détails de la tâche** dans le panneau de gauche.
1. Dans la zone **Finances**, saisissez le multiplicateur des heures supplémentaires dans le champ **Ratio des heures supplémentaires**.
1. Cliquez sur **Enregistrer les modifications**.
