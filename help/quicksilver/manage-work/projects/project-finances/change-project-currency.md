---
product-area: projects
navigation-topic: financials
title: Modifier la devise du projet
description: En tant que personne gestionnaire de projet, vous pouvez configurer un projet afin qu’il utilise une devise autre que la devise par défaut de votre système Adobe Workfront. Vous pouvez ainsi afficher des informations financières sur votre projet dans la devise souhaitée lors du calcul des revenus et des coûts de main-d’oeuvre.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 98%

---

# Modifier la devise d’un projet

En tant que personne gestionnaire de projet, vous pouvez configurer un projet afin qu’il utilise une devise autre que la devise par défaut de votre système Adobe Workfront. Vous pouvez ainsi afficher des informations financières sur votre projet dans la devise souhaitée lors du calcul des revenus et des coûts de main-d’oeuvre.

Avant de pouvoir utiliser d’autres devises comme décrit dans cette section, l’administrateur ou administratrice de Workfront doit d’abord activer et configurer plusieurs devises, comme décrit dans l’article [Configurer les taux de change](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Tous </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Accès en modification aux projets</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Autorisations de gestion pour le projet</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la modification de la devise d’un projet dans Workfront

* Vous ne pouvez pas modifier la devise d’un projet s’il contient des informations financières.
* Les taux sont utilisés pour les coûts de main-d’oeuvre et les calculs des recettes, et sont utilisés ultérieurement à des fins de création de rapports.
* Si vous ne spécifiez pas d’autre devise pour un projet, Workfront suppose que la devise du projet est la devise par défaut du système. Pour plus d’informations sur la devise par défaut au niveau du système, voir [Configurer les taux de change](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Par défaut, tous les utilisateurs et utilisatrices de la licence complète ont accès aux devises et aux taux de change. L’administrateur ou administratrice de Workfront doit accorder un accès administratif supplémentaire aux **Taux de change** afin de permettre aux utilisateurs et utilisatrices de définir des taux spécifiques sur les projets.
* Les taux de change dans Workfront ne sont pas dynamiques. La valeur est définie par un administrateur ou une administratrice et doit être mise à jour en cas de modification des taux de change.
* Lorsque vous créez un rapport pour refléter la devise d’un projet, tous les rapports sont par défaut regroupés selon la devise par défaut du projet. Si vous créez un rapport avec plusieurs projets dont les taux de change sont différents, tous les regroupements appliqués au projet reflètent le taux de change par défaut au niveau du système. Pour plus d’informations, voir l’article [Créer des rapports de données financières avec des taux de change uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configurer la devise d’un projet

1. Accédez au projet dans lequel vous souhaitez modifier la devise par défaut.

   >[!TIP]
   >
   >Assurez-vous que le projet ne contient pas déjà des informations financières. Par exemple, assurez-vous qu’aucun coût prévu ou réel n’est associé au projet.

1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis accédez à la zone **Finance**.
1. Cliquez sur **Ajouter** dans le champ **Devise** et sélectionnez la devise à utiliser comme devise par défaut pour le projet. Toutes les devises que votre administrateur ou administratrice Workfront a définies pour votre instance Workfront s’affichent.

   ![Devise du projet](assets/currency-on-project-expanded-nwe.png)

1. (Le cas échéant) Si vous sélectionnez une autre devise que la devise par défaut définie pour votre système Workfront, indiquez le taux de la devise que vous avez sélectionnée, car il est lié à la devise définie comme devise de base dans le système.
1. Cliquez sur **Enregistrer les modifications**.
