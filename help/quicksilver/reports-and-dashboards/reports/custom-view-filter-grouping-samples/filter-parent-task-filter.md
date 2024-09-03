---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Filtre : afficher les tâches parents »'
description: Vous pouvez appliquer les filtres de tâches ci-dessous pour afficher les tâches opérationnelles. Les tâches opérationnelles sont des tâches qui peuvent être accomplies de manière indépendante et qui ne sont pas des tâches parents d’autres tâches. Dans un exemple, un filtre identifie les tâches enfants qui pourraient être elles-mêmes des parents. Dans ce cas, il ne s’agit pas de tâches opérationnelles.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 100%

---

# Filtre : afficher les tâches parents

Vous pouvez appliquer les filtres de tâches ci-dessous pour afficher les tâches opérationnelles. Les tâches opérationnelles sont des tâches qui peuvent être accomplies de manière indépendante et qui ne sont pas des tâches parents d’autres tâches. Dans un exemple, un filtre identifie les tâches enfants qui pourraient être elles-mêmes des parents. Dans ce cas, il ne s’agit pas de tâches opérationnelles.

>[!TIP]
>
>* Si vous envisagez d’ajouter plus d’un filtre à un rapport, nous vous recommandons d’ajouter tous vos filtres à l’aide de l’interface du créateur de rapports, puis de cliquer sur Passer en mode texte une fois que toutes les autres règles de filtrage ont été ajoutées. Ensuite, vous pouvez ajouter le code pour le filtre de la tâche parent comme indiqué ci-dessus. 
>* Nous vous recommandons également d’ajouter un regroupement pour le nom du projet afin de faciliter la lecture du rapport. Pour plus d’informations sur l’ajout de regroupements à vos rapports, consultez l’article [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher les tâches sans enfants (elles peuvent avoir un parent)

Vous pouvez appliquer le filtre suivant à un rapport de tâche pour afficher les tâches sans enfants.Elles peuvent avoir leurs propres parents et être les enfants d’autres tâches.

1. Dans le **menu principal** ![](assets/main-menu-icon.png), cliquez sur **Rapports.**

1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **Rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans la ligne **Saisissez le nom du champ...**, saisissez **Nombre d’enfants**.

1. Sélectionnez **Égal (sensible à la casse)** pour votre modificateur, puis saisissez **0** pour le nombre d’enfants.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Ou

   Cliquez sur **Passer en mode texte**, et dans la fenêtre d’édition de texte, copiez et collez le texte suivant : 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Cliquez sur **Enregistrer + Fermer**.

   Cela permet d’obtenir un rapport pour toutes les tâches qui sont des tâches opérationnelles dans votre système. Certaines de ces tâches peuvent avoir un parent, mais elles ne sont pas elles-mêmes des tâches parents.

## Afficher les tâches avec des parents (elles peuvent avoir des enfants)

Vous pouvez appliquer le filtre suivant à un rapport de tâche pour afficher les tâches avec des parents, ce qui signifie qu’il s’agit de tâches enfants. Toutefois, ces tâches peuvent également avoir des enfants, car le filtre n’exclut pas leurs enfants. Les tâches enfants qui sont également des parents d’autres tâches ne sont pas considérées comme des tâches opérationnelles.

1. Dans le **menu principal** ![](assets/main-menu-icon.png) , cliquez sur **Rapports.
1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **Rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans la ligne **Saisissez un nom de champ...**, saisissez **Identifiant parent**.
1. Sélectionnez **N’est pas vide** pour votre modificateur.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Ou

   Cliquez sur **Passer en mode texte**, et dans la fenêtre d’édition de texte, copiez et collez le texte suivant : 

   `parentID_Mod=notblank`

1. Cliquez sur **Enregistrer + Fermer**.

   Cela permet d’obtenir un rapport pour toutes les tâches de votre système qui ont des parents et qui sont des tâches enfants de ces mêmes parents. Certaines de ces tâches peuvent également être elles-mêmes parents.

## Afficher les tâches sans enfants ni parents (tâches indépendantes)

Vous pouvez appliquer le filtre suivant à un rapport de tâches pour afficher les tâches opérationnelles indépendantes.Ces tâches n’ont ni parents ni enfants.

1. Dans le **Menu principal** ![](assets/main-menu-icon.png), cliquez sur **Rapports.**
1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **Rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre** et dans la ligne **Saisissez un nom de champ...**, saisissez **Nombre d’enfants**, sélectionnez **Égal (sensible à la casse)** pour votre modificateur, puis saisissez **0** pour le nombre d’enfants.
1. Cliquez sur **Ajouter une autre règle de filtre** et dans la ligne **Saisissez un nom de champ...**, saisissez **Identifiant parent**, puis sélectionnez **Est vide**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Ou

   Au lieu des étapes 6 et 7, cliquez sur **Passer en mode texte** et dans la fenêtre d’édition de texte, copiez et collez le texte suivant : 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Cliquez sur **Enregistrer + Fermer**.

   Cela permet d’obtenir un rapport sur toutes les tâches de votre système qui n’ont ni parents ni enfants. Il s’agit de tâches opérationnelles indépendantes.
