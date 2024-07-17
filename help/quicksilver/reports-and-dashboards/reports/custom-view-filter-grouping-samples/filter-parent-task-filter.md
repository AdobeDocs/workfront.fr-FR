---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : afficher les tâches parentes'
description: Vous pouvez appliquer les filtres de tâches ci-dessous pour afficher les tâches en cours. Les tâches de travail sont des tâches qui peuvent être exploitées indépendamment et qui ne sont pas des tâches parents d’autres tâches. Dans un exemple, un filtre identifie les tâches des enfants qui peuvent être des parents eux-mêmes. Dans ce cas, il ne s’agit pas de tâches opérationnelles.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 16%

---

# Filtre : afficher les tâches parent

Vous pouvez appliquer les filtres de tâches ci-dessous pour afficher les tâches en cours. Les tâches de travail sont des tâches qui peuvent être exploitées indépendamment et qui ne sont pas des tâches parents d’autres tâches. Dans un exemple, un filtre identifie les tâches des enfants qui peuvent être des parents eux-mêmes. Dans ce cas, il ne s’agit pas de tâches opérationnelles.

>[!TIP]
>
>* Si vous envisagez d’ajouter plusieurs filtres à un rapport, nous vous recommandons d’ajouter tous les filtres à l’aide de l’interface du Créateur de rapports, puis de cliquer sur Passer en mode Texte après l’ajout de toutes les autres règles de filtrage. Vous pouvez ensuite ajouter le code pour le filtre de tâche parent comme indiqué ci-dessus. 
>* Nous vous recommandons également d’ajouter un regroupement pour le nom du projet afin de faciliter la lecture du rapport. Pour plus d’informations sur l’ajout de groupes à vos rapports, consultez l’article [Présentation des groupes dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

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
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher les tâches sans enfants (ils peuvent avoir un parent)

Vous pouvez appliquer le filtre suivant à un rapport de tâches pour afficher les tâches sans enfant. Ils pourraient avoir leurs propres parents et être des enfants d&#39;autres tâches.

1. Dans le **menu principal** ![](assets/main-menu-icon.png), cliquez sur **Rapports.**

1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans la ligne **Commencer à saisir le nom du champ ...**, commencez à saisir **Nombre d&#39;enfants**.

1. Sélectionnez **Egal (sensible à la casse)** pour votre modificateur, puis entrez **0** pour le nombre d&#39;enfants.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Ou

   Cliquez sur **Passer en mode Texte**, puis, dans la fenêtre d’édition de texte, copiez et collez le texte suivant : 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Cliquez sur **Enregistrer + Fermer**.

   Cette opération extrait un rapport pour toutes les tâches qui fonctionnent sur votre système. Certaines de ces tâches peuvent avoir un parent, mais il ne s’agit pas de tâches parentes elles-mêmes.

## Afficher les tâches avec les parents (ils peuvent avoir des enfants)

Vous pouvez appliquer le filtre suivant à un rapport de tâches pour afficher les tâches avec les parents, ce qui signifie qu’il s’agit de tâches enfants. Cependant, ces tâches peuvent également comporter des enfants, car le filtre n’exclut pas leurs enfants. Les tâches pour enfants qui sont également des parents pour d’autres tâches ne sont pas considérées comme des tâches de travail.

1. Dans le **menu principal** ![](assets/main-menu-icon.png), cliquez sur **Rapports.
1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans la ligne **Commencer à saisir le nom du champ ...**, commencez à saisir **Parent ID**.
1. Sélectionnez **N’est pas vierge** pour votre modificateur.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Ou

   Cliquez sur **Passer en mode Texte**, puis, dans la fenêtre d’édition de texte, copiez et collez le texte suivant : 

   `parentID_Mod=notblank`

1. Cliquez sur **Enregistrer + Fermer**.

   Cette opération extrait un rapport pour toutes les tâches de votre système qui ont des parents et sont des tâches enfants de ces parents. Certaines de ces tâches peuvent être un parent lui-même.

## Afficher les tâches sans enfants et sans parents (tâches autonomes)

Vous pouvez appliquer le filtre suivant à un rapport de tâche pour afficher les tâches de travail autonomes. Ces tâches n&#39;ont pas de parent et elles n&#39;ont pas d&#39;enfants à elles.

1. Dans le **menu principal** ![](assets/main-menu-icon.png), cliquez sur **Rapports.**
1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez un **rapport de tâche**.
1. Cliquez sur **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre** et, dans la ligne **Déclencher la saisie du nom du champ...**, commencez à saisir **Nombre d’enfants**, sélectionnez **Égal (sensible à la casse)** pour votre modificateur, puis saisissez **0** pour le nombre d’enfants.
1. Cliquez sur **Ajouter une autre règle de filtre** et, dans la ligne **Commencer à saisir le nom du champ...**, commencez à saisir **ID parent**, puis sélectionnez **Est vierge**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Ou

   Au lieu des étapes 6 à 7, cliquez sur **Passer en mode Texte** et dans la fenêtre de modification de texte, copiez et collez le texte suivant : 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Cliquez sur **Enregistrer + Fermer**.

   Cette opération extrait un rapport pour toutes les tâches de votre système qui n’ont ni parents ni enfants. Il s’agit de tâches de travail autonomes.
