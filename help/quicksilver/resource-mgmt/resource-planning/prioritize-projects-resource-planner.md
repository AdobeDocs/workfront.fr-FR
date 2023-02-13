---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Définir la priorité des projets dans le planificateur de ressources
description: Les projets sont répertoriés par ordre de priorité dans le planificateur de ressources, le projet le plus important se trouvant en haut.
author: Alina
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 1%

---

# Définir la priorité des projets dans le planificateur de ressources

Les projets sont répertoriés par ordre de priorité dans le planificateur de ressources, le projet le plus important se trouvant en haut.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à l’option Modifier les priorités et les heures du budget dans le planificateur de ressources</p> <p>Modifier l’accès aux données financières, aux projets et aux utilisateurs</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations des projets pour lesquels vous souhaitez budgétiser les informations avec la possibilité de Gérer les finances</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Ordre par défaut des projets dans le planificateur de ressources

Par défaut, les projets sont répertoriés dans la vue Projet du planificateur de ressources en tenant compte des critères ci-dessous.

>[!IMPORTANT]
>
>Les projets sont répertoriés selon les trois critères ci-dessous uniquement la première fois que vous ouvrez le planificateur de ressources. Toutefois, cette priorité par défaut devient automatiquement votre priorité personnalisée et ne peut pas être rétablie à la priorité d’origine chaque fois que vous effectuez l’une des opérations suivantes :
>
>* Lorsque vous cliquez sur Enregistrer à tout moment.
>* Lorsque vous modifiez manuellement la priorité de planification du projet. Pour plus d’informations sur la modification manuelle de la priorité de planification du projet, voir la section [Modification manuelle de la priorité de planification des projets](#manually-change-the-project-planning-priority) dans cet article.
>
>Une fois que la priorité du projet devient votre priorité personnalisée, les modifications apportées aux informations du projet n’affectent plus l’ordre des projets utilisant ces critères. Ensuite, vous pouvez classer les projets par priorité uniquement manuellement.

Les critères par défaut d’origine pour la liste des projets dans la vue Projet sont les suivants, dans cet ordre :

1. Par la note d’alignement sur le projet.\
   Pour plus d’informations sur la note d’alignement du projet, voir [Application d’une fiche d’évaluation à un projet et génération d’une note d’alignement](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. Par date de début planifiée du projet (si le champ Alignement est nul ou est identique pour plusieurs projets).
1. Par ordre alphabétique (si le champ Alignement est nul ou est identique et que la date de début planifiée est identique pour plusieurs projets).

Tenez compte des points suivants lorsque vous travaillez avec les priorités de projet dans le planificateur de ressources :

* Vous pouvez personnaliser manuellement la priorité du projet uniquement lorsque vous appliquez la vue Projet. Cela modifie également l’ordre des projets dans le planificateur de ressources.
* Lorsque vous appliquez les vues de rôle ou d’utilisateur dans le planificateur de ressources, les projets apparaissent dans le même ordre de priorité que celui défini dans la vue Projet.
* L’ordre des projets dans le planificateur de ressources vous est propre. D’autres utilisateurs peuvent afficher les mêmes projets dans le planificateur de ressources, mais dans un ordre différent. Vous ne pouvez pas générer de rapports sur le champ Priorité de planification du projet . Cette option est visible uniquement dans le planificateur de ressources et sert d’indicateur pour hiérarchiser vos projets.

Les projets associés à un portfolio peuvent avoir une priorité au niveau du portfolio. Vous pouvez activer l’affichage de la priorité de portefeuille d’un projet dans le planificateur de ressources, en plus de la priorité du planificateur de ressources. Vous pouvez également classer les projets en fonction de leur priorité de portefeuille.

## Modification manuelle de la priorité de planification des projets {#manually-change-the-project-planning-priority}

Pour réorganiser les projets dans le planificateur de ressources, vous devez disposer des autorisations Modifier de la gestion des ressources et Gérer les ressources.

En donnant une nouvelle priorité aux projets, vous pouvez les classer par ordre d’importance.

Pour modifier la priorité de planification du projet :

1. Accédez au **Resource Planner**.

1. Cliquez dans le champ à gauche du nom du projet qui contient un numéro, saisissez un numéro pour modifier la Priorité de planification, puis appuyez sur Entrée.\
   ![](assets/mceclip4.png)\
   Ou\
   Passez la souris sur le nom du projet, cliquez sur l’indicateur situé à gauche du nom du projet, puis faites-le glisser et déposez-le à l’endroit approprié pour modifier la priorité.

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   Lorsque vous sélectionnez des nombres pour classer les projets par priorité, sélectionnez des nombres plus faibles pour les priorités plus élevées (plus importantes) et des nombres plus élevés pour les priorités moins importantes (moins importantes). Lorsque vous définissez le numéro de priorité d’un projet sur un numéro inférieur (priorité supérieure), tous les autres projets du planificateur de ressources se déplacent vers le bas de la liste (deviennent moins importants).\
   Lorsque vous définissez le numéro de priorité d’un projet sur un numéro supérieur (priorité inférieure), tous les autres projets du planificateur de ressources sont déplacés vers le haut de la liste (plus important).

1. Cliquer sur **Enregistrer**.\
   L’ordre des projets change en fonction de vos sélections et cela devient votre priorité de projet personnalisée dans le planificateur de ressources. D’autres utilisateurs ne peuvent pas voir votre ordre de priorité pour les projets dans le planificateur de ressources, bien qu’ils puissent peut-être afficher les mêmes projets dans leurs planificateurs de ressources.

## Classer les projets en fonction de leur priorité Portfolio dans le planificateur de ressources

>[!IMPORTANT]
>
>Votre entreprise doit disposer d’un plan d’entreprise ou d’un plan Workfront supérieur pour hiérarchiser les projets dans Portfolio Optimizer.
>
>Pour plus d’informations sur les plans Workfront, voir [Nos plans](https://www.workfront.com/plans).
>
>Pour plus d’informations sur la priorité des projets dans Portfolio Optimizer, voir [Hiérarchisation des projets dans Portfolio Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Ouvrez le **Resource Planner** dans le **Vue du projet**.
1. Cliquez sur le bouton **Paramètres** icône .
1. Activez la variable **Afficher les priorités de Portfolio** pour afficher les priorités du projet en fonction du Portfolio auquel elles sont affectées. La priorité des projets selon leur portefeuille s’affiche en regard de la priorité du planificateur de ressources. Ce paramètre est désactivé par défaut.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   Les priorités de portefeuille des projets s’affichent uniquement dans la vue Projet du planificateur de ressources.

1. Cliquez sur **Commande** pour classer les projets en fonction des priorités du portefeuille.

   Si vous avez des projets qui appartiennent à plusieurs portefeuilles, vous pouvez voir plusieurs projets ayant la même priorité de portefeuille dans le planificateur de ressources. Dans ce cas, les projets ayant la même priorité de portefeuille sont répertoriés selon les critères suivants, dans cet ordre :

   1. Score d&#39;alignement
   1. Date de début prévue
   1. Nom du projet

   ![](assets/rp-portfolio-priority-ordered-350x198.png)

1. Cliquer sur **Enregistrer**.

## Effet de la modification de la priorité de planification du projet sur les heures disponibles de l’utilisateur

La priorité de planification des projets affecte les heures disponibles des utilisateurs. Les utilisateurs associés au projet dont la priorité est la plus élevée affichent la disponibilité complète de la colonne Heures disponibles (AVL) pour ce projet, en fonction de leurs plannings.

Les mêmes utilisateurs associés au deuxième projet par ordre de priorité afficheront une valeur Heures disponibles , à savoir la différence entre le montant total des Heures disponibles et ce qui a déjà été budgété pour le premier projet de la colonne Heures budgétaires , etc. Pour plus d’informations sur la planification des ressources dans le planificateur de ressources, voir [Ressources de budget dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Si aucune heure n’a été planifiée pour le premier projet (par ordre de priorité) pour un utilisateur, mais que des heures ont été prévues pour le deuxième projet pour le même utilisateur, l’utilisateur affichera la totalité des heures disponibles pour les deux projets.

Nous vous recommandons de mettre à jour la colonne Heures budgétées pour vos utilisateurs dans l’ordre des projets dans le planificateur de ressources, afin de vous assurer que vous pouvez afficher précisément les Heures disponibles pour l’utilisateur à tout moment.

>[!NOTE]
>
>Comme la priorité de planification de projet est propre à chaque gestionnaire de ressources, votre projet de deuxième priorité peut être un projet prioritaire pour un autre utilisateur qui consulte les mêmes projets dans son planificateur de ressources. Si un autre gestionnaire de ressources met en budget une ressource pour son premier projet, les Heures disponibles diminueront pour cette ressource pour votre premier projet en fonction de cette modification.
>
>L’utilisateur qui met le budget des heures alloue d’abord cette ressource et réduit le nombre d’heures disponibles pour cette ressource dans l’ensemble du système. Le montant des Heures disponibles doit être mis à jour pour tous les utilisateurs dès que les Heures budgétisées sont enregistrées pour une ressource dans le planificateur de ressources.
>
>Pour plus d’informations sur les heures disponibles, voir [Disponibilité et allocation des ressources](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
