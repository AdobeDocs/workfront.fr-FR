---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Filtre : afficher les tâches parents »'
description: Vous pouvez appliquer les filtres de tâches ci-dessous pour afficher les tâches opérationnelles. Les tâches opérationnelles sont des tâches qui peuvent être accomplies de manière indépendante et qui ne sont pas des tâches parents d’autres tâches. Dans un exemple, un filtre identifie les tâches enfants qui pourraient être elles-mêmes des parents. Dans ce cas, il ne s’agit pas de tâches opérationnelles.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 66%

---

# Filtre : afficher les tâches parents

<!--Audited: 10/2024-->

Vous pouvez appliquer les filtres de tâches ci-dessous pour afficher les tâches opérationnelles. Les tâches opérationnelles sont des tâches qui peuvent être accomplies de manière indépendante et qui ne sont pas des tâches parents d’autres tâches. Dans un exemple, un filtre identifie les tâches enfants qui pourraient être elles-mêmes des parents. Dans ce cas, il ne s’agit pas de tâches opérationnelles.

>[!TIP]
>
>* Si vous envisagez d’ajouter plus d’un filtre à un rapport, nous vous recommandons d’ajouter tous vos filtres à l’aide de l’interface du créateur de rapports, puis de cliquer sur Passer en mode texte une fois que toutes les autres règles de filtrage ont été ajoutées. Ensuite, vous pouvez ajouter le code pour le filtre de la tâche parent comme indiqué ci-dessus. 
>* Nous vous recommandons également d’ajouter un regroupement pour le nom du projet afin de faciliter la lecture du rapport. Pour plus d’informations sur l’ajout de regroupements à vos rapports, consultez l’article [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher les tâches sans enfants (elles peuvent avoir un parent)

Vous pouvez appliquer le filtre suivant à un rapport de tâches pour afficher les tâches sans enfant. Ils pourraient avoir leurs propres parents et être des enfants d&#39;autres tâches.

1. Dans le **menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit ou dans le **menu principal** ![](assets/lines-main-menu.png) dans le coin supérieur gauche, si disponible, cliquez sur **Rapports**.

1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **Rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Sur la ligne **Commencer à saisir le nom du champ ...**, commencez à saisir **Nombre d’enfants**, puis cliquez sur **Tâche &quot; Nombre d’enfants** lorsqu’il s’affiche dans la liste.

1. Sélectionnez **Égal (sensible à la casse)** pour votre modificateur, puis saisissez **0** pour le nombre d’enfants.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Ou

   Cliquez sur **Basculer vers le mode Texte**. Dans la fenêtre d’édition de texte, copiez et collez le texte suivant :

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Cliquez sur **Enregistrer + Fermer**.

   Cela permet d’obtenir un rapport pour toutes les tâches qui sont des tâches opérationnelles dans votre système. Certaines de ces tâches peuvent avoir un parent, mais elles ne sont pas elles-mêmes des tâches parents.

## Afficher les tâches avec des parents (elles peuvent avoir des enfants)

Vous pouvez appliquer le filtre suivant à un rapport de tâche pour afficher les tâches avec des parents, ce qui signifie qu’il s’agit de tâches enfants. Toutefois, ces tâches peuvent également avoir des enfants, car le filtre n’exclut pas leurs enfants. Les tâches enfants qui sont également des parents d’autres tâches ne sont pas considérées comme des tâches opérationnelles.

1. Dans le **menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit ou dans le **menu principal** ![](assets/lines-main-menu.png) dans le coin supérieur gauche, si disponible, cliquez sur **Rapports**.

1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **Rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Sur la ligne **Commencer à saisir le nom du champ ...**, commencez à saisir **Parent ID**, puis sélectionnez **Tâche &quot; Parent ID** lorsqu’il s’affiche dans la liste.
1. Sélectionnez **N’est pas vide** pour votre modificateur.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Ou

   Cliquez sur **Passer en mode texte**, et dans la fenêtre d’édition de texte, copiez et collez le texte suivant : 

   `parentID_Mod=notblank`

1. Cliquez sur **Enregistrer + Fermer**.

   Cela permet d’obtenir un rapport pour toutes les tâches de votre système qui ont des parents et qui sont des tâches enfants de ces mêmes parents. Certaines de ces tâches peuvent également être elles-mêmes parents.

## Afficher les tâches sans enfants ni parents (tâches indépendantes)

Vous pouvez appliquer le filtre suivant à un rapport de tâche pour afficher les tâches de travail autonomes. Ces tâches n&#39;ont pas de parent et elles n&#39;ont pas d&#39;enfants à elles.

1. Dans le **menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit ou dans le **menu principal** ![](assets/lines-main-menu.png) dans le coin supérieur gauche, si disponible, cliquez sur **Rapports**.

1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **Rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans la ligne **Commencer à saisir le nom du champ ...**, commencez à saisir **Nombre d’enfants**, puis sélectionnez **Tâche &quot; Nombre d’enfants** dans la liste.
1. Sélectionnez **Égal (sensible à la casse)** pour votre modificateur, puis saisissez **0** pour le nombre d’enfants.
1. Cliquez sur **Ajouter une autre règle de filtre**.
1. Dans la ligne **Commencer à saisir le nom du champ ...**, commencez à saisir **Parent ID**, puis sélectionnez **Tâche &quot; Parent ID** dans la liste.
1. Sélectionnez **Est vierge** pour le modificateur.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Ou

   Au lieu des étapes 6 à 10 <!--ensure steps above stay accurate-->, cliquez sur **Passer en mode Texte** et dans la fenêtre de modification de texte, copiez et collez le texte suivant :

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Cliquez sur **Enregistrer + Fermer**.

   Cela permet d’obtenir un rapport sur toutes les tâches de votre système qui n’ont ni parents ni enfants. Il s’agit de tâches opérationnelles indépendantes.
