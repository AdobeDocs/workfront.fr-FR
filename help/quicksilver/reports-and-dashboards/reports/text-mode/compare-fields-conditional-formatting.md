---
product-area: reporting
navigation-topic: text-mode-reporting
title: Comparer des champs dans la mise en forme conditionnelle
description: Vous pouvez utiliser la mise en forme conditionnelle pour comparer 2 champs différents dans une vue et les mettre en surbrillance lorsque certains critères sont satisfaits entre les champs.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 22%

---

# Comparer des champs dans la mise en forme conditionnelle

Vous pouvez utiliser la mise en forme conditionnelle pour comparer 2 champs différents dans une vue et les mettre en surbrillance lorsque certains critères sont satisfaits entre les champs.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux Rapports, tableaux de bord et calendriers pour modifier la vue dans un rapport</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier l’affichage dans un rapport</p> <p>Autorisations de gestion d’une vue</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Exemple : Comparaison de la date de début réelle et de la date de début planifiée

Par exemple, si la Date de début réelle d’une tâche est postérieure à la Date de début planifiée, vous pouvez mettre en surbrillance la colonne Date de début planifiée à l’aide d’une mise en forme conditionnelle.

Pour comparer la date de début planifiée et la date de début réelle de la tâche à l’aide d’une mise en forme conditionnelle :

1. Accédez à une vue de tâche ou à un rapport.
1. (Conditionnel) Si vous utilisez un rapport, dans l’onglet **Colonnes (vues)**, cliquez sur l’en-tête de la colonne que vous souhaitez formater de manière conditionnelle pour la sélectionner.\
   Par exemple, sélectionnez la colonne **Date de début réelle** si vous souhaitez y ajouter la mise en forme conditionnelle en comparant les champs Date de début planifiée et Date de début réelle.

1. Cliquez sur **Options avancées**, puis sur Ajouter une **règle pour cette colonne**.

1. Renseignez les critères de comparaison à l’aide des valeurs existantes du créateur et spécifiez votre mise en forme conditionnelle.\
   Par exemple, nous voulons mettre en surbrillance les tâches dont la Date de début réelle est supérieure ou supérieure à la Date de début planifiée. Sélectionnez le modificateur Supérieur à et sélectionnez une date réelle dans le champ de date.\
     ![](assets/cond-format-1-350x84.png)

1. (Facultatif) Sélectionnez **Appliquer à la ligne entière** si vous souhaitez appliquer la mise en forme à la ligne entière.
1. Cliquez sur **Ajouter une règle**, puis **Terminé**.

1. Sélectionnez la colonne **Date de début réelle**, puis cliquez sur **Passer en mode texte**.

1. **Cliquez pour modifier le mode texte** , puis ajoutez la ligne de texte suivante :

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   Dans notre exemple : 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Si vous comparez un champ natif Workfront, utilisez la syntaxe de casse mixte pour le nom du champ. Si vous comparez un champ personnalisé, utilisez **DE:Nom réel du champ** pour le champ de nom que vous comparez au premier champ.\
   >Par exemple, si vous comparez la **Date de début réelle** à un champ personnalisé intitulé **Date de remise**, ajoutez l’instruction suivante dans votre code de mode texte :
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Assurez-vous que la ligne de code `righttext` correspond à l’instruction de la ligne de code `rightmethod`.

   ![](assets/cond-format-2-350x171.png)

1. Cliquer sur **Enregistrer**.
1. Cliquez sur **Enregistrer + Fermer**.

   La colonne met en surbrillance les champs qui répondent à vos critères.
