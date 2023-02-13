---
product-area: reporting
navigation-topic: text-mode-reporting
title: Comparaison de champs dans la mise en forme conditionnelle
description: Vous pouvez utiliser la mise en forme conditionnelle pour comparer 2 champs différents dans une vue et les mettre en surbrillance lorsque certains critères sont satisfaits entre les champs.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Comparaison de champs dans la mise en forme conditionnelle

Vous pouvez utiliser la mise en forme conditionnelle pour comparer 2 champs différents dans une vue et les mettre en surbrillance lorsque certains critères sont satisfaits entre les champs.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux Rapports, tableaux de bord et calendriers pour modifier la vue dans un rapport</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier l’affichage dans un rapport</p> <p>Gestion des autorisations pour un affichage</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Exemple : Comparaison de la date de début réelle et de la date de début planifiée

Par exemple, si la Date de début réelle d’une tâche est postérieure à la Date de début planifiée, vous pouvez mettre en surbrillance la colonne Date de début planifiée à l’aide d’une mise en forme conditionnelle.

Pour comparer la date de début planifiée et la date de début réelle de la tâche à l’aide d’une mise en forme conditionnelle :

1. Accédez à une vue de tâche ou à un rapport.
1. (Conditionnel) Si vous utilisez un rapport, dans la variable **Colonnes (affichage)** , cliquez sur l’en-tête de la colonne que vous souhaitez formater de manière conditionnelle pour la sélectionner.\
   Par exemple, sélectionnez la variable **Date de début réelle** si vous souhaitez y ajouter la mise en forme conditionnelle en comparant les champs Date de début planifiée et Date de début réelle .

1. Cliquez sur **Options avancées**, puis cliquez sur Ajouter un **Règle pour cette colonne**.

1. Renseignez les critères de comparaison à l’aide des valeurs existantes du créateur et spécifiez votre mise en forme conditionnelle.\
   Par exemple, nous voulons mettre en surbrillance les tâches dont la Date de début réelle est supérieure ou supérieure à la Date de début planifiée. Sélectionnez le modificateur Supérieur à et sélectionnez une date réelle dans le champ de date.\
     ![](assets/cond-format-1-350x84.png)

1. (Facultatif) Sélectionnez **Appliquer à l’ensemble de la ligne** si vous souhaitez appliquer la mise en forme à la ligne entière.
1. Cliquez sur **Ajouter une règle**, puis **Terminé**.

1. Sélectionnez la **Date de début réelle** , puis cliquez sur **Passer en mode Texte**.

1. **Cliquer pour modifier le texte** , puis ajoutez la ligne de texte suivante :

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   Dans notre exemple : 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Si vous comparez un champ natif Workfront, utilisez la syntaxe de casse mixte pour le nom du champ. Si vous comparez un champ personnalisé, utilisez **DE:Nom réel du champ** pour le champ nom que vous comparez au premier champ.\
   >Par exemple, si vous comparez la variable **Date de début réelle** avec un champ personnalisé libellé **Date de remise**, ajoutez l’instruction suivante dans votre code de mode texte :
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Assurez-vous que la variable `righttext` la ligne de code correspond à l’instruction dans la variable `rightmethod` ligne de code.

   ![](assets/cond-format-2-350x171.png)

1. Cliquer sur **Enregistrer**.
1. Cliquez sur **Enregistrer + Fermer**.

   La colonne met en surbrillance les champs qui répondent à vos critères.
