---
product-area: projects
navigation-topic: financials
title: Modifier la devise d’un projet
description: En tant que personne gestionnaire de projet, vous pouvez configurer un projet afin qu’il utilise une devise autre que la devise par défaut de votre système Adobe Workfront. Vous pouvez ainsi afficher des informations financières sur votre projet dans la devise souhaitée lors du calcul des revenus et des coûts de main-d’oeuvre.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 100%

---

# Modifier la devise d’un projet

En tant que personne gestionnaire de projet, vous pouvez configurer un projet afin qu’il utilise une devise autre que la devise par défaut de votre système Adobe Workfront. Vous pouvez ainsi afficher des informations financières sur votre projet dans la devise souhaitée lors du calcul des revenus et des coûts de main-d’oeuvre.

Avant de pouvoir utiliser d’autres devises comme décrit dans cette section, l’administrateur ou administratrice de Workfront doit d’abord activer et configurer plusieurs devises, comme décrit dans l’article [Configurer les taux de change](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

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

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Le cas échéant) Si vous sélectionnez une autre devise que la devise par défaut définie pour votre système Workfront, indiquez le taux de la devise que vous avez sélectionnée, car il est lié à la devise définie comme devise de base dans le système.
1. Cliquez sur **Enregistrer les modifications**.
