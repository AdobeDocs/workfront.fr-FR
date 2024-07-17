---
product-area: resource-management
navigation-topic: resource-planning
title: Régler des dates de budgétisation dans le planificateur de ressources
description: Si vous constatez une surallocation de vos ressources après les avoir budgétées dans le planificateur de ressources, vous pouvez explorer les scénarios de planification des ressources en déplaçant les heures budgétisées, l’éditeur de texte enrichi ou les coûts vers une autre période. En fonction des résultats de ces scénarios, vous pouvez ensuite ajuster vos heures, votre EPT ou votre coût budgété.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 19%

---

# Régler des dates de budgétisation dans le planificateur de ressources

Si vous constatez une surallocation de vos ressources après les avoir budgétées dans le planificateur de ressources, vous pouvez explorer les scénarios de planification des ressources en déplaçant les heures budgétisées, l’éditeur de texte enrichi ou les coûts vers une autre période. En fonction des résultats de ces scénarios, vous pouvez ensuite ajuster vos heures, votre EPT ou votre coût budgété.

Les suraffectations peuvent s’afficher lorsque les heures, l’éditeur de texte enrichi ou les coûts de vos ressources sont plus élevés que les heures, l’éditeur de texte enrichi ou les coûts disponibles. Cela génère une valeur nette négative.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à l’option Modifier les priorités et les heures du budget dans le planificateur de ressources</p> <p>Modifier l’accès aux données financières, aux projets et aux utilisateurs</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour les projets pour lesquels vous souhaitez budgétiser les informations avec la possibilité de Gérer les finances</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Ajuster les dates de budget

1. Accédez au planificateur de ressources et sélectionnez **Afficher par projet**.

   >[!NOTE]
   >
   >Vous ne pouvez utiliser l’option Ajuster les dates budgétées que lorsque vous affichez le planificateur de ressources par projet.

1. Passez la souris sur le nom d’un projet, puis cliquez sur le menu **Plus** .
1. Cliquez sur **Ajuster les dates de budget**.\
   La chronologie d’allocation de projet s’affiche.\
   La période où les heures sont actuellement budgétées est surlignée en orange en cas de conflit de budget et en bleu en cas d’absence de conflit.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Placez la période mise en surbrillance à une autre heure afin de comprendre où il n’y a aucun conflit de budget pour le projet sélectionné. Lorsque vous trouvez une période où la valeur Net est positive, la période mise en surbrillance passe en bleu.
1. Cliquez sur la croix (x) dans le coin supérieur droit de la chronologie d’allocation de projet pour la fermer.
1. Supprimez les heures budgétées de la chronologie existante du projet et ajoutez-les à la chronologie qui affiche la disponibilité la plus élevée.
1. Cliquer sur **Enregistrer**.
1. (Conditionnel et facultatif) Si les périodes sans conflit de budget ne sont pas dans la chronologie du projet, cliquez sur le nom du projet pour y accéder.
1. (Conditionnel et facultatif) Cliquez sur **Modifier le projet**, puis modifiez la **Date de début planifiée** ou la **Date d’achèvement planifiée** pour modifier la chronologie du projet pour la période sans conflit de budget.\
   Pour plus d’informations sur la modification des projets, consultez l’article [Modifier les projets](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Conditionnel et facultatif) Cliquez sur **Enregistrer les modifications**.
1. Revenez au planificateur de ressources et entrez à nouveau les heures, les ETP ou les coûts budgétés dans la période sans conflit de budget.
1. Cliquer sur **Enregistrer**.
