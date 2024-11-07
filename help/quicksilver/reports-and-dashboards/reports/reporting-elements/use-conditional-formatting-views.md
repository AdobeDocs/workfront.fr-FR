---
product-area: reporting
navigation-topic: reporting-elements
title: Utiliser une mise en forme conditionnelle dans les vues
description: À mesure que vous partagez vos rapports avec d’autres personnes dans Adobe Workfront, pensez à personnaliser l’affichage des rapports, à faciliter la lecture de certaines informations ou à simplement vous distinguer.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 97%

---

# Utiliser une mise en forme conditionnelle dans les vues

<!-- Audited: 11/2024 -->

À mesure que vous partagez vos rapports avec d’autres personnes dans Adobe Workfront, pensez à personnaliser l’affichage des rapports, à faciliter la lecture de certaines informations ou à simplement vous distinguer.

Vous pouvez personnaliser l&#39;onglet Détails de vos rapports en ajoutant une mise en forme spéciale ou conditionnelle à la vue de vos rapports.

Pour plus d’informations sur la création de rapports, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

En mettant en forme de manière conditionnelle les colonnes dans la vue du rapport, vous pouvez configurer des règles qui affectent la manière dont le rapport s’affiche. Lorsque ces conditions ou règles sont remplies, la mise en forme spéciale est appliquée.

Par exemple, si le pourcentage terminé d’une tâche est inférieur à 20 %, vous pouvez mettre le champ en surbrillance en affichant le pourcentage en gras, en rouge et dans une couleur d’arrière-plan jaune.

Avec une vue mise en forme de manière conditionnelle, vous pouvez :

* Modifier l’en-tête d’une colonne.
* Remplacer la valeur d’une colonne par du texte ou une image personnalisés.
* Mettre en forme l’affichage d’un champ en modifiant le type de police, la couleur, l’alignement ou la couleur de l’arrière-plan.

Les modifications que vous apportez dans la vue du rapport ne prennent effet que dans l&#39;onglet Détails du rapport. Ces modifications n’affectent pas les onglets Résumé, Matrice ou Graphique du rapport.

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
   <td> <p>Nouveau :</p> 
   <ul><li>Standard pour les vues de rapport</li>
  <li> Contribution ou supérieur pour les vues de liste</li></ul>
   <p>Actuel :</p>
   <ul>
    <li> Plan pour les vues de rapport </li>
    <li> Requête ou supérieur pour les vues de liste </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux Rapports, tableaux de bord et calendriers pour modifier une vue dans un rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour créer ou modifier une vue dans un rapport</p> <p>Gérer les autorisations pour une vue</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez créer un rapport pour pouvoir ajouter une mise en forme conditionnelle à sa vue.

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Créer une vue mise en forme de manière conditionnelle

{{step1-to-reports}}

1. Cliquez sur le nom d’un rapport dans lequel vous souhaitez créer une vue avec mise en forme conditionnelle.

   Ou

   Cliquez sur **Nouveau rapport**, puis sélectionnez un type d’objet pour créer un nouveau rapport.

1. (Le cas échéant) Si vous modifiez un rapport existant, cliquez sur **Actions de rapport**, puis cliquez sur **Modifier**.

1. Dans l’onglet **Colonnes (vue)**, cliquez pour sélectionner une colonne existante, ou cliquez sur **Ajouter une colonne** pour créer une colonne.
1. Dans le champ **Afficher dans cette colonne** dans le coin supérieur gauche de Report Builder, sélectionnez le champ à afficher dans la nouvelle colonne.
1. Cliquez sur **Options avancées**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Personnaliser le libellé de colonne</strong></td> 
      <td> <p>Indiquez un nom pour la colonne.</p> <p>Si vous modifiez une colonne existante, indiquez un nom pour la colonne existante.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Format du champ</strong></td> 
      <td>Choisissez le format d’affichage de la valeur dans la colonne. Selon le champ de colonne, vous pouvez ainsi définir le mode d’affichage des dates, des nombres ou des devises. Toutes les colonnes n’affichent pas cette option.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher cette colonne lorsque le graphique est visible sur un tableau de bord.</strong></td> 
      <td>Sélectionnez ce champ si vous souhaitez que la colonne s’affiche lorsque le rapport est placé sur un tableau de bord. La colonne s’affiche toujours lorsque vous consultez le rapport en dehors d’un tableau de bord.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Ajouter une règle à cette colonne**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. Dans la section **Lorsque :**, définissez une déclaration de condition pour la colonne.

   Par exemple : « Lorsque le pourcentage de tâche terminé est égal à (respect de la casse) 50. »
1. Dans la section **Afficher le champ comme suit :**, indiquez à quoi ressemble ce champ lorsque la condition définie ci-dessus est remplie.

   Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Couleur du texte</strong></td> 
      <td> <p>Sélectionnez la couleur d’affichage du texte à l’aide du sélecteur de couleurs.</p> <p><b>NOTE</b></p> <p> Si le champ contient un lien hypertexte, les sélections de couleur du texte ne sont pas appliquées à ce champ.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Format du texte</strong></td> 
      <td>Choisissez d’afficher le texte en gras ou en italique.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Alignement du texte</strong></td> 
      <td>Indiquez si le texte doit être aligné à droite, au centre ou à gauche dans la colonne.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contexte</strong></td> 
      <td>Sélectionnez la couleur de fond du texte à l’aide du sélecteur de couleurs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher l’icône</strong></td> 
      <td>Sélectionnez l’une des 16 icônes si vous souhaitez afficher une icône au lieu de la valeur réelle pour cette colonne.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher le texte</strong></td> 
      <td> <p>Sélectionnez cette option pour afficher un libellé personnalisé pour cette colonne, au lieu de sa valeur réelle. Indiquez le texte à afficher à la place de la valeur dans le champ fourni.</p> <p><b>IMPORTANT</b></p> <p>Sélectionner <strong>Afficher le texte</strong> désactive la possibilité de modifier en ligne le texte de cette colonne.<br>De plus, vous ne pouvez pas modifier la valeur d’une colonne Tâche antérieure, car elle contient une logique intégrée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Appliquer à toute la ligne</strong></td> 
      <td>Sélectionnez cette option pour appliquer des paramètres à la ligne entière plutôt que d’appliquer des paramètres uniquement à la colonne sélectionnée.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Ajouter une règle**.\
   Vous pouvez ajouter des règles supplémentaires à la même colonne ou ajouter des règles à d’autres colonnes.

   Les règles sont appliquées dans l’ordre dans lequel elles ont été créées. Elles sont combinées, mais elles ne se chevauchent pas, bien qu’une règle de colonne ait la priorité sur une règle de ligne sur la même cellule.

   **EXEMPLE 1**

   Vous pouvez d’abord créer une règle qui indique que lorsqu’un projet est dans le statut En cours de création, le texte est violet et en gras. Vous créez ensuite une deuxième règle qui indique que lorsque le nom d’une tâche n’est pas vide, le texte est rouge et en italique, et la couleur d’arrière-plan est verte. Dans cet exemple, les événements suivants se produisent :

   * Les tâches dont le statut du projet est En cours de création sont affichées en texte violet et en gras. Si le nom de la tâche n’est pas vide, les tâches ont également un arrière-plan vert.
   * Les tâches dont le statut du projet est autre qu’En cours de création (et que le nom de la tâche n’est pas vide) sont affichées dans un texte rouge et en italique avec un arrière-plan vert.

   **EXEMPLE 2**

   Créez une règle dans la colonne Date d’achèvement prévue du projet qui affecte la ligne entière, en faisant griser l’arrière-plan si le projet est annulé (par exemple, lorsque le statut du projet est Inactif). Créez ensuite une règle de colonne qui affiche l’arrière-plan en rouge lorsque la date d’achèvement prévue du projet est inférieure à aujourd’hui (ce qui signifie que le projet est en retard). Dans cet exemple, si un projet annulé a une date d’achèvement en retard, cette cellule apparaîtra en rouge même si les autres cellules de la ligne sont grises. Pour corriger cette mise en forme :

   * Modifiez la mise en forme de la date d’achèvement prévue et supprimez la règle de colonne stipulant un arrière-plan rouge pour les projets en retard.
   * Ajoutez une règle de colonne avec la même mise en forme que la règle de ligne (arrière-plan gris lorsque le statut du projet = Inactif).
   * Ajoutez à nouveau la règle de colonne stipulant un arrière-plan rouge pour les projets en retard.
   * Lorsque vous enregistrez les règles et la vue, l’arrière-plan rouge n’est pas appliqué à un projet annulé.

1. Cliquer sur **Enregistrer**.
1. Cliquez sur **Enregistrer + Fermer**.\
   Sur le rapport, les personnes voient des modifications apportées au format si les conditions spécifiées sont remplies.
