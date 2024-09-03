---
product-area: resource-management
navigation-topic: resource-planning
title: Vérifier la disponibilité et l’affectation des ressources à l’aide du planificateur de ressources Adobe Workfront
description: Vous pouvez afficher la disponibilité de vos ressources et le volume de travail prévu ou budgété pour vos projets dans le planificateur de ressources. Ces valeurs sont affichées en heures, en équivalent temps complet ou en coûts et sont organisées en colonnes.
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 100%

---

# Vérifier la disponibilité et l’affectation des ressources à l’aide du planificateur de ressources Adobe Workfront

Vous pouvez afficher la disponibilité de vos ressources et le volume de travail prévu ou budgété pour vos projets dans le planificateur de ressources. Ces valeurs sont affichées en heures, en équivalent temps complet ou en coûts et sont organisées en colonnes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro et supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès Affichage ou niveau supérieur aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Données financières</p> </li> 
     <li> <p>Utilisateurs</p> </li> 
     <li> <p>Projets</p> </li> 
    </ul> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur pour les projets que vous souhaitez afficher dans le planificateur de ressources.</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## Conditions préalables

Vous devez respecter toutes les conditions préalables requises pour utiliser le planificateur de ressources.Pour plus d’informations, voir [Vue d’ensemble du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>S’il manque une des conditions préalables requises pour le bon fonctionnement du planificateur de ressources, certains nombres peuvent être nuls ou les heures budgétées peuvent être grisées.

## Disponibilité et affectation des ressources

Les colonnes qui affichent la disponibilité et l’affectation de vos ressources changent en fonction de la vue que vous appliquez au planificateur de ressources. Pour plus d’informations sur l’affichage des informations dans le planificateur de ressources par projet, rôle ou utilisateur ou utilisatrice, voir [Vue d’ensemble de la navigation dans le planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Tenez compte des points suivants lorsque vous changez votre vue dans le planificateur de ressources :

* Lorsque vous appliquez les vues **Afficher par projet** ou **Afficher par rôle**, vous pouvez voir les colonnes suivantes :

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Heures disponibles, Équivalent temps complet ou Coût
   * Nombre d’heures prévues, Équivalent temps complet ou Coût
   * Heures budgétées, Équivalent temps complet ou Coût
   * Heures, Équivalent temps complet ou Variance des coûts
   * Heures nettes, Équivalent temps complet ou Coût

* Lorsque vous appliquez la vue **Afficher par utilisateur ou utilisatrice** vous pouvez voir les colonnes suivantes :

   * Heures ou équivalent temps complet disponibles
   * Nombre d’heures prévues ou équivalent temps complet prévu
   * Différence d’heure ou d’équivalent temps complet
   * Pourcentage d’allocation des heures prévues

>[!TIP]
>
>Les informations ne sont pas disponibles en tant que coût lors de l’application de la vue **Afficher par utilisateur ou utilisatrice** dans le planificateur de ressources.
>
>Pour plus d’informations sur l’affichage de chaque colonne, placez le pointeur de la souris sur le nom de la colonne dans laquelle le nombre s’affiche.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Pour plus d’informations sur les données affichées dans chaque colonne, voir les articles suivants :
>
>* [Vue d’ensemble des heures, de l’équivalent temps complet et des coûts dans les vues Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Afficher les heures disponibles, prévues et effectives ou l’équivalent temps complet dans le planificateur de ressources lors de l’utilisation de la vue utilisateur ou utilisatrice](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>

## Afficher les informations par heure, équivalent temps complet ou coût

1. Accédez au planificateur de ressources.

   Par défaut, les informations s’affichent par heures dans le planificateur de ressources.

1. Développez le menu déroulant.\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Heures</td> 
      <td>Affiche les informations de disponibilité et d’affectation en heures.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Temps complet</td> 
      <td> <p>Affiche les informations de disponibilité et d’affectation en équivalent temps complet.</p> <p>Pour plus d’informations sur le mode de calcul de l’équivalent temps complet dans le planificateur de ressources, voir <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Vue d’ensemble du calcul des heures et de l’équivalent temps complet pour les utilisateurs et utilisatrices et les rôles dans le planificateur de ressources</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts</td> 
      <td> <p>Affiche les informations de disponibilité et d’affectation par coût, si vous affichez le planificateur de ressources dans les vues Projet ou Rôle. Les informations affichent les valeurs dans la devise de votre système. Votre équipe d’administration Workfront définit la devise du système. Pour plus d’informations sur la configuration de la devise du système dans Workfront, voir <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a>.</p> <p><b>NOTE</b>

   Vous devez associer les utilisateurs et utilisatrices et les fonctions aux coûts par heure afin d’afficher les informations sur les coûts dans le planificateur de ressources.<br style="font-style: italic;">Pour plus d’informations sur l’association des coûts par heure aux fonctions, voir <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.<br style="font-style: italic;">Pour plus d’informations sur l’association des coûts par heure avec les utilisateurs et utilisatrices, voir <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’un utilisateur ou d’une utilisatrice</a>.<br style="font-style: italic;">Pour plus d’informations sur le mode de calcul du coût dans le planificateur de ressources, voir <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Calculer les coûts dans le planificateur de ressources</a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Personnaliser</td> 
      <td>Crée une vue personnalisée des colonnes qui s’affichent dans le planificateur de ressources. Sélectionnez les options à afficher dans le planificateur de ressources, comme décrit dans les étapes ci-dessous. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Le cas échéant) Si vous avez sélectionné **Personnaliser**, indiquez les options dans la zone **Personnaliser les mesures affichées** pour configurer votre vue personnalisée.

   ![](assets/planner-customize-view-box-350x114.png)

1. Dans la colonne **Type de vue** sur la gauche, sélectionnez l’une des vues suivantes :

   * Projet
   * Rôle
   * l’utilisateur ou de l’utilisatrice

1. Dans la section **Afficher les éléments sélectionnés**, sélectionnez le type d’information à afficher dans les colonnes de la vue sélectionnée.Le tableau suivant indique les options disponibles dans chaque vue :

   | **Option** | Vue utilisateur | Vue Projet | Vue Rôle |
   |---|---|---|---|
   | Disponible | ✔ | ✔ | ✔ |
   | Prévu | ✔ | ✔ | ✔ |
   | Budgété |   | ✔ | ✔ |
   | Variance |   | ✔ | ✔ |
   | Net |   | ✔ | ✔ |
   | Réel | ✔ |   |   |
   | Différence | ✔ |   |   |
   | Pourcentage | ✔ |   |   |

1. Sélectionnez **Utiliser les valeurs PLN (prévues) dans les calculs nets** pour utiliser les informations prévues au lieu des informations budgétées lors du calcul des valeurs nettes dans les vues Projet et Rôle.

   Lorsque vous sélectionnez cette option, Workfront calcule les valeurs nettes à l’aide de la formule suivante :

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**Cette option s’applique uniquement lorsque vous sélectionnez au moins une option pour personnaliser la vue dans la section Afficher les éléments sélectionnés.**

1. Cliquer sur **Enregistrer**.

   La vue personnalisée qui comprend les colonnes sélectionnées s’affiche.

   Le planificateur de ressources répertorie la vue personnalisée comme Personnalisée dans le menu déroulant Heures.

   >[!NOTE]
   >
   >Vous ne pouvez avoir qu’une seule vue personnalisée.

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Afficher le graphique de l’affectation des utilisateurs et utilisatrices

Vous pouvez afficher l’affectation prévue des utilisateurs et utilisatrices en fonction de leur disponibilité dans un graphique.

Pour afficher l’affectation des utilisateurs et utilisatrices dans un graphique :

1. Accédez au planificateur de ressources.

   Pour plus d’informations sur l’accès au planificateur de ressources, voir la section [Localiser le planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) dans l’article [Vue d’ensemble du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Sélectionnez **Par utilisateur ou utilisatrice**.

   >[!TIP]
   >
   >Vous ne pouvez afficher le graphique d’affectation des utilisateurs et utilisatrices que dans la vue Utilisateur ou utilisatrice.

1. Cliquez sur l’icône **Graphique d’affectation des utilisateurs et utilisatrices** ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png) pour afficher les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">% de disponibilité sans sur-allocation de tous les utilisateurs</td> 
      <td>Il s’agit de la durée pendant laquelle tous les utilisateurs et utilisatrices sont disponibles pour le travail au cours d’une période donnée, exprimée en pourcentage par rapport au temps total disponible. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">% de sur-allocation pour tous les utilisateurs </td> 
      <td> <p>Il s’agit de la durée pendant laquelle les utilisateurs et utilisatrices sont suraffectés au cours d’une période, exprimée en pourcentage par rapport au temps disponible total.</p> <p><b>NOTE</b>

   Une suraffectation se produit lorsque le nombre d’heures prévues est supérieur au nombre d’heures disponibles. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">% de sous-utilisation pour tous les utilisateurs</td> 
      <td> <p>Il s’agit de la durée pendant laquelle les utilisateurs et utilisatrices sont sous-utilisés au cours d’une période donnée, exprimée en pourcentage par rapport au temps disponible total.</p> <p><b>NOTE</b>

   La sous-utilisation se produit lorsque le nombre d’heures prévues est inférieur au nombre d’heures disponibles. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Il existe une surallocation pour au moins un utilisateur durant cette période</td> 
      <td>Cela indique qu’il existe une suraffectation d’au moins un utilisateur ou une utilisatrice au cours d’une période donnée, bien que la durée totale de tous les utilisateurs et utilisatrices ne soit pas suraffectée au cours de cette période.<br>Vous devez faire défiler la liste des utilisateurs et utilisatrices et les heures de ceux qui sont suraffectés sont surlignées en rouge.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Facultatif) Cliquez sur la zone **% de suraffectation pour tous les utilisateurs et utilisatrices** du graphique.\
   Tous les utilisateurs et utilisatrices suraffectés sont surlignés en rouge.
1. (Facultatif) Cliquez sur la zone **% de sous-utilisation pour tous les utilisateurs et utilisatrices** du graphique.\
   Tous les utilisateurs et utilisatrices sous-utilisés sont mis en surbrillance en bleu.

1. (Facultatif) Cliquez sur l’icône d’indicateur ![one_user_overallocation_marqueur.png](assets/one-user-overallocation-marker.png) qui montre où au moins une personne est sur-affectée.\
   Les personnes sur-affectées sont mises en surbrillance en rouge.

1. (Facultatif) Actualisez la page pour réduire le graphique.
