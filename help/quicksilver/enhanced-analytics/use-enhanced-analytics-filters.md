---
title: Appliquer des filtres dans Analytique améliorée
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Les filtres de la zone Analyses améliorées d’Adobe Workfront vous aident à vous concentrer sur des projets spécifiques ou des types de données spécifiques.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1486'
ht-degree: 5%

---

# Appliquer des filtres dans Analytique améliorée

<!-- Audited: 12/2023 -->

Les filtres de la zone Analyses améliorées d’Adobe Workfront vous aident à vous concentrer sur des projets spécifiques ou des types de données spécifiques. Les types de filtres que vous utilisez peuvent vous donner des informations sur les éléments suivants :

* Projets que vous possédez
* Vues de portefeuille ou de programme spécifiques
* Indicateurs de performance clés pour une période spécifique (semaine, trimestre, année fiscale)

Vous pouvez ajouter et supprimer des filtres selon vos besoins et Workfront conserve les filtres que vous appliquez même si vous vous déconnectez.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>
      <p>Nouveau : Tous</p>
      <p>ou</p>
      <p>Actuel : métier ou supérieur</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
      <p>Nouveau : Léger ou supérieur</p>
      <p>ou</p>
      <p>Actuel : révision ou supérieur</p>
   </td> 
  </tr>
  <tr> 
   <td>Configurations du niveau d’accès</td> 
   <td> <p>Affichage de l’accès aux projets</p> <p>Vous devez également disposer d’un accès en mode Affichage aux tâches, aux Portfolios et aux utilisateurs pour afficher des options de filtrage de champ de projet spécifiques.</p> <p>Remarque : Si des restrictions sont sélectionnées dans la section <strong>Définir des restrictions supplémentaires</strong> de la boîte de dialogue Modifier le niveau d’accès, il se peut que toutes les informations ne s’affichent pas dans les filtres ou sur la page Analyses améliorées après l’application du filtre.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Afficher</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytics amélioré, reportez-vous à la section [Conditions préalables](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) dans la [présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Modification du filtre de période {#change-the-date-range-filter}

Par défaut, les visualisations de la zone Analyses améliorées affichent les données des 60 derniers jours et des 15 prochains jours. Vous pouvez sélectionner une nouvelle période et l’appliquer à toutes les visualisations de la zone d’analyse améliorée. Si vous quittez la page, la plage de dates par défaut est appliquée la prochaine fois que vous y reviendrez.

>[!TIP]
>
>Vous pouvez également utiliser les touches de votre clavier pour naviguer, ouvrir et sélectionner une plage de dates dans le widget Calendrier.\
>Pour plus d’informations, reportez-vous à la section [Raccourcis clavier](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) de l’article [Présentation des analyses avancées](../enhanced-analytics/enhanced-analytics-overview.md).

Pour sélectionner une nouvelle période :

{{step1-to-analytics}}

1. En haut à droite, cliquez sur le champ Période pour ouvrir la vue Calendrier.
1. Utilisez les flèches situées au-dessus du calendrier pour localiser le mois de votre date de début, puis sélectionnez la date de début.

   ![Sélectionner une plage de dates](assets/filters-select-date-range-350x344.png)

1. Utilisez les flèches situées au-dessus du calendrier pour localiser le mois de votre date de fin, puis sélectionnez la date de fin.
1. (Facultatif) Pour effectuer un zoom avant sur une plage de dates plus petite, faites glisser la souris d’une date spécifique à une autre sur l’une des visualisations.

   Toutes les visualisations à l’écran se mettent à jour pour correspondre à la période sélectionnée. Un filtre Période s’affiche en regard de tout filtre existant. Ce filtre n’est pas conservé si vous vous déconnectez ou quittez la zone Analyses améliorées.

   ![Filtre Période](assets/timeframe-filter-350x220.png)

## Ajouter un filtre

Vous pouvez ajouter des filtres en fonction des champs de projet par défaut, des champs de formulaire personnalisés et des équipes d’accueil affectées aux projets.

>[!TIP]
>
>Vous pouvez également utiliser les touches de votre clavier pour accéder à et ajouter un nouveau filtre.\
>Pour plus d’informations, reportez-vous à la section [Raccourcis clavier](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) de l’article [Présentation des analyses avancées](../enhanced-analytics/enhanced-analytics-overview.md).

* [Ajouter un filtre de champ de projet](#add-a-project-field-filter)
* [Ajouter un filtre de formulaire personnalisé de projet](#add-a-project-custom-form-filter)
* [Ajout d’un filtre Équipe](#add-a-team-filter)

### Ajout d’un filtre de champ de projet {#add-a-project-field-filter}

Les filtres de champs de projet permettent de filtrer les données des projets et des tâches en fonction des valeurs saisies dans les champs inclus par défaut sur les projets.

Les types de filtre de champ de projet suivants sont disponibles :

| champ | Données affichées |
|---|---|
| **Projet** | Affiche les données uniquement pour le ou les projets sélectionnés. |
| **Programme** | Affiche uniquement les données des projets du ou des programmes sélectionnés. |
| **Portfolio** | Affiche uniquement les données des projets du ou des portefeuilles sélectionnés. |
| **Condition** | Affiche uniquement les données des projets qui présentent la ou les conditions sélectionnées le plus récemment (sur la cible, à risque ou en difficulté). |
| **Statut** | Affiche uniquement les données des projets dont les états ont été sélectionnés le plus récemment (terminé, en cours, en attente, annulé, etc.) |
| **Sponsor** | Affiche les données uniquement pour les projets avec le ou les sponsors sélectionnés. |
| **Propriétaire du projet** | Affiche les données uniquement pour les projets avec le ou les propriétaires de projet sélectionnés. |

Les filtres de formulaire personnalisés fonctionnent différemment. Pour plus d’informations, voir [Ajout d’un projet de filtre de formulaire personnalisé](#add-a-project-custom-form-filter).

Pour ajouter un filtre de champ de projet :

{{step1-to-analytics}}

1. En haut à gauche, cliquez sur **Ajouter un filtre**, puis sélectionnez le type de filtre souhaité.

   >[!NOTE]
   >
   >Différents types de filtre affichent des données différentes. Vous ne pouvez utiliser qu’un seul type de filtre dans un filtre. Une fois que vous l’avez sélectionné, un type de filtre ne peut plus être utilisé dans un autre filtre de champ de projet.

1. Recherchez les valeurs pour lesquelles vous souhaitez afficher des données en saisissant au moins trois caractères du texte dans le champ **Rechercher**, puis sélectionnez chaque valeur à inclure dans le filtre.

   Pour sélectionner toutes les valeurs actives, cliquez sur **Sélectionner tout**.

   ![Sélectionner la valeur de filtre](assets/select-filter-value-350x251.png)

1. Après avoir sélectionné toutes les valeurs souhaitées, cliquez sur **Appliquer le filtre**.

   Le projet repose sur les mises à jour les plus à droite pour refléter les filtres appliqués.

1. Répétez ces étapes pour chaque filtre à ajouter.

   Lorsque vous ajoutez des filtres, les données s’affichent dans les visualisations ci-dessous pour 50 projets au maximum.

   >[!TIP]
   >
   >Pour afficher les données de plus de 50 projets qui s’affichent par défaut, vous pouvez :
   >
   >   * Utilisez les flèches situées dans la partie inférieure gauche pour afficher les 50 projets suivants dans cette visualisation.\
   >     ![Flèche de pagination](assets/pagination-350x118.png)
   >   
   >   * Utilisez le menu déroulant **Trier par** sur une visualisation pour afficher les projets dans un ordre différent.\
   >     ![ Trier par menu](assets/sort-by-menu-350x247.png)

   Pour ajuster la période, voir [Modification du filtre de période](#change-the-date-range-filter).

### Ajout d’un filtre de formulaire personnalisé de projet

Le type de filtre de formulaire personnalisé permet de filtrer les données des projets et des tâches en fonction des valeurs saisies dans les champs de formulaire personnalisés des projets. Contrairement à d’autres types de filtres d’analyse améliorés, vous pouvez ajouter plusieurs filtres de formulaire personnalisés. Chaque filtre de formulaire personnalisé contient des valeurs saisies uniquement dans le champ sélectionné d’un formulaire personnalisé spécifique.

Pour ajouter un filtre de formulaire personnalisé :

{{step1-to-analytics}}

1. Dans le coin supérieur gauche de l’écran, cliquez sur **Ajouter un filtre**, puis sélectionnez **Formulaire personnalisé**.

   ![Sélectionner un filtre de formulaire personnalisé](assets/select-custom-form-filter-350x271.png)

1. Localisez le formulaire personnalisé que vous souhaitez en saisissant au moins trois caractères dans le champ **Rechercher**, puis sélectionnez le formulaire personnalisé.
1. Sélectionnez le champ de votre choix, puis effectuez l’une des actions suivantes en fonction du type de champ que vous ajoutez au filtre :

   >[!NOTE]
   >
   >Il n’est pas possible d’ajouter tous les types de champs de gestion personnalisés à un filtre. Actuellement, l’analyse avancée ne prend en charge que les types de champ répertoriés ci-dessous.

   * **Case à cocher**, **liste déroulante** ou **bouton radio** : sélectionnez chaque valeur du champ à inclure dans votre filtre ou cliquez sur la case à cocher **Tout sélectionner**.\
     ![Valeurs de case à cocher](assets/custom-form-filter-checkbox-350x255.png)

   * **Date** : utilisez les flèches pour accéder à un mois spécifique, puis sélectionnez la date dans le champ que vous souhaitez inclure dans votre filtre.\
     ![Valeur de date](assets/custom-form-filter-date-350x348.png)

   * **Texte** : entrez le texte dans le champ que vous souhaitez inclure dans votre filtre.\
     ![Valeur de texte](assets/custom-form-filter-text-350x90.png)

   * **Number** : entrez le nombre dans le champ que vous souhaitez inclure dans votre filtre.\
     ![Valeur de nombre](assets/custom-form-filter-number-350x93.png)

1. Après avoir saisi ou sélectionné les valeurs pour lesquelles vous souhaitez filtrer, cliquez sur **Appliquer le filtre**.

   Le projet repose sur les mises à jour les plus à droite pour refléter les filtres appliqués.

1. Répétez ces étapes pour chaque filtre à ajouter.

   Lorsque vous ajoutez des filtres, les données s’affichent dans les visualisations ci-dessous pour 50 projets au maximum.

   >[!TIP]
   >
   >Pour afficher les données de plus de 50 projets qui s’affichent par défaut, vous pouvez :
   >  
   >   * Utilisez les flèches situées dans la partie inférieure gauche pour afficher les 50 projets suivants dans cette visualisation.\
   >     ![Flèches de pagination](assets/pagination-350x118.png)
   >   
   >   * Utilisez le menu déroulant **Trier par** sur une visualisation pour afficher les projets dans un ordre différent.\
   >     ![ Trier par menu](assets/sort-by-menu-350x247.png)

   Pour ajuster la période, voir [Modification du filtre de période](#change-the-date-range-filter).

### Ajout d’un filtre Équipe {#add-a-team-filter}

{{step1-to-analytics}}

1. Dans le panneau de gauche, cliquez sur **Personnes**.

   ![Select People](assets/people-area-cropped-qs-350x276.png)

1. En haut à gauche de l&#39;écran, cliquez sur **Ajouter un filtre**, puis sélectionnez le filtre **Équipe** .
1. Localisez les équipes pour lesquelles vous souhaitez afficher des données en saisissant au moins trois caractères dans le champ **Rechercher**, puis sélectionnez chaque équipe à inclure dans le filtre. Pour sélectionner toutes les équipes, cliquez sur **Sélectionner tout**.

   ![Sélectionner les équipes](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Toutes les équipes sont incluses en tant qu’options de filtre, quel que soit votre niveau d’accès.

1. Après avoir sélectionné toutes les équipes souhaitées, cliquez sur **Appliquer le filtre**.

   Lorsque vous ajoutez des filtres, les données s’affichent dans les visualisations ci-dessous.

   Pour ajuster la période, voir [Modification du filtre de période](#change-the-date-range-filter).

## Supprimer un filtre

Vous pouvez supprimer un filtre à tout moment. Si vous supprimez un filtre, il ne s’affiche pas la prochaine fois que vous visitez la zone Analyses améliorées.

>[!TIP]
>
>Vous pouvez également utiliser les touches de votre clavier pour accéder à un filtre existant et le supprimer.\
>Pour plus d’informations, reportez-vous à la section [Raccourcis clavier](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) de l’article [Présentation des analyses avancées](../enhanced-analytics/enhanced-analytics-overview.md).

Pour supprimer un filtre :

{{step1-to-analytics}}

1. Si vous souhaitez supprimer un champ de projet ou un filtre de formulaire personnalisé, restez dans la zone **Travail**.

   Ou

   Si vous souhaitez supprimer un filtre Équipe, sélectionnez **Personnes** dans le panneau de gauche.

1. Recherchez le filtre souhaité et cliquez sur le **X** pour le supprimer.

   ![Supprimer](assets/remove-filter-350x213.png)

   Le filtre n’est plus actif et ne s’affiche plus tant que vous ne l’ajoutez pas à nouveau.
