---
title: Modifier les regroupements existants
description: Modifier les regroupements existants
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 88%

---

# Modifier les regroupements existants

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

Vous pouvez personnaliser un regroupement que vous avez créé à l’origine ou qui a été partagé avec vous. Vous pouvez ensuite l’enregistrer en tant que nouveau regroupement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Contributeur ou version ultérieure</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Requête ou supérieure</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Editer l'accès aux Rapports, Tableaux de bord, Calendriers pour modifier un groupement dans un rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de gestion relatives à un rapport pour modifier un regroupement dans un rapport</p> <p>Autorisations de gestion relatives à un regroupement</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez créer un regroupement avant de pouvoir le modifier.

Pour plus d’informations sur la création d’un regroupement, voir la section [Créer des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Étapes pratiques

1. Accédez à une liste d’objets contenant le regroupement que vous souhaitez personnaliser.
1. Cliquez sur l’icône **Regroupement**.
1. Sélectionnez le groupe que vous souhaitez personnaliser, puis cliquez sur l&#39;icône **Modifier** ![Icône Modifier](assets/edit-icon.png).

   ![Sélectionnez l’icône de modification.](assets/customizegrouping-nwe-standard-350x291.png)

   Le créateur d’interface pour la personnalisation du regroupement s’ouvre.

1. Dans la section **Prévisualisation du regroupement**, cliquez sur **Ajouter un regroupement** pour définir le mode d’organisation des informations dans le rapport. Vous trouverez ci-dessous un aperçu de ce à quoi ressemble un regroupement dans le rapport.

1. Commencez à saisir le nom du champ qui représente la manière dont vous souhaitez organiser les informations dans le rapport, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif et le cas échéant) Lors de l’affichage d’une liste mise à jour, sélectionnez **Réduire ce regroupement par défaut** si vous souhaitez que les résultats du regroupement s’affichent de manière réduite plutôt que développée. Ce paramètre est désactivé par défaut et les résultats du regroupement s’affichent toujours dans la liste développée.

   Pour plus d’informations sur les listes mises à jour et héritées, voir la section « Différence entre les listes mises à jour et héritées » de l’article [Prise en main des listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Lorsque vous ajustez manuellement les regroupements lors de l’affichage d’une liste, Workfront mémorise vos préférences manuelles jusqu’à ce que vous vous déconnectiez. Lorsque vous vous reconnectez, la liste s’affiche en fonction de ce paramètre.
   >* Les résultats d’un regroupement s’affichent toujours de façon développée après que l’on y a accédé à partir d’un élément de graphique ou d’une liste héritée. Dans ce genre de cas, ce paramètre est ignoré.

1. Répétez les étapes 4, 5 et 6 pour définir des regroupements supplémentaires.\
   Vous pouvez définir jusqu’à trois regroupements pour organiser les informations. Vous pouvez organiser vos informations encore davantage en utilisant jusqu’à quatre regroupements grâce à un rapport de matrice. Pour plus d’informations sur les rapports de matrice, voir la section [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Cliquez sur **Enregistrer le groupement** pour remplacer le groupement actuel par vos modifications.
