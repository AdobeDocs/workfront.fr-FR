---
product-area: resource-management
navigation-topic: resource-planning
title: Ajuster les dates de budgétisation dans le planificateur de ressources
description: Si vous constatez des surallocations de vos ressources après les avoir budgétées dans le planificateur de ressources, vous pouvez explorer des scénarios d’hypothèses en déplaçant les heures, les équivalents temps complet ou les coûts budgétés vers une autre période. Sur la base des résultats de ces scénarios, vous pouvez alors ajuster les heures, les équivalents temps complet ou les coûts budgétés.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 97%

---

# Ajuster les dates de budget dans le planificateur de ressources

Si vous constatez des surallocations de vos ressources après les avoir budgétées dans le planificateur de ressources, vous pouvez explorer des scénarios d’hypothèses en déplaçant les heures, les équivalents temps complet ou les coûts budgétés vers une autre période. Sur la base des résultats de ces scénarios, vous pouvez alors ajuster les heures, les équivalents temps complet ou les coûts budgétés.

Des surallocations peuvent apparaître lorsque les heures, les équivalents temps complet ou les coûts budgétés de vos ressources sont supérieurs à leurs heures, équivalents temps complet ou coûts disponibles. Cela génère une valeur nette négative.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td>
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification à la gestion des ressources qui inclut l’accès en modification des priorités et des heures du budget dans le planificateur de ressources.</p> <p>Accès en modification aux données financières, aux projets et aux utilisateurs et utilisatrices</p></td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion des projets pour lesquels vous souhaitez budgéter les informations avec la possibilité de gérer les finances.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajuster les dates de budget

1. Allez dans le planificateur de ressources et sélectionnez **Par projet**.

   >[!NOTE]
   >
   >Vous ne pouvez utiliser l’option « Ajuster les dates budgétées » que lorsque vous affichez le planificateur de ressources par projet.

1. Pointez sur le nom d’un projet, puis cliquez sur le menu **Plus**.
1. Cliquez sur **Ajuster les dates de budget**.\
   La chronologie d’affectation du projet s’affiche.\
   Si un conflit de budget existe, la période pour laquelle les heures sont actuellement budgétées est surlignée en orange ; elle est en bleu en l’absence de conflit.

   ![Ajuster les dates de budget](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Faites glisser la période en surbrillance vers une autre période pour comprendre où il n’y a pas de conflit de budget pour le projet sélectionné. Lorsque vous trouvez une période où la valeur nette est positive, la période en surbrillance devient bleue.
1. Cliquez sur le « x » dans le coin supérieur droit de la chronologie d’affectation du projet pour la fermer.
1. Supprimez les heures budgétées de la chronologie existante du projet et ajoutez-les à la chronologie qui présente le plus de disponibilités.
1. Cliquer sur **Enregistrer**.
1. (Le cas échéant et facultatif) Si les délais sans conflit de budget sont en dehors de la chronologie du projet, cliquez sur le nom du projet pour y accéder.
1. (Le cas échéant et facultatif) Cliquez sur **Modifier le projet**, puis modifiez la **Date de début prévue** ou la **Date d’achèvement prévue** pour modifier la chronologie du projet sans conflit de budget.\
   Pour plus d’informations sur la modification de projets, consultez l’article [Modifier des projets](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Le cas échéant et facultatif) Cliquez sur **Enregistrer les modifications**.
1. Retournez au planificateur de ressources et saisissez à nouveau les heures, les équivalents temps complet ou les coûts budgétés dans la période sans conflit de budget.
1. Cliquer sur **Enregistrer**.
