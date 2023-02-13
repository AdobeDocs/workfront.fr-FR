---
product-area: projects
navigation-topic: financials
title: Modification de la devise du projet
description: En tant que chef de projet, vous pouvez configurer un projet afin qu’il utilise une devise autre que la devise par défaut de votre système Adobe Workfront. Vous pouvez ainsi afficher des informations financières sur votre projet dans la devise souhaitée lors du calcul des coûts et des recettes de main-d’oeuvre.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Modification de la devise du projet

En tant que chef de projet, vous pouvez configurer un projet afin qu’il utilise une devise autre que la devise par défaut de votre système Adobe Workfront. Vous pouvez ainsi afficher des informations financières sur votre projet dans la devise souhaitée lors du calcul des coûts et des recettes de main-d’oeuvre.

Avant de pouvoir utiliser d’autres devises comme décrit dans cette section, l’administrateur de Workfront doit d’abord activer et configurer plusieurs devises, comme décrit dans l’article . [Configurer les taux de change](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Considérations lors de la modification de la devise d’un projet dans Workfront

* Vous ne pouvez pas modifier la devise d’un projet s’il contient des informations financières.
* Les taux sont utilisés pour les coûts du travail ; Calculs de recettes et sont utilisés à l’avenir à des fins de création de rapports.
* Si vous ne spécifiez pas de devise différente pour un projet, Workfront suppose que la devise du projet est la devise par défaut du système. Pour plus d’informations sur la devise par défaut au niveau du système, voir [Configurer les taux de change](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Par défaut, tous les utilisateurs de la licence complète ont accès aux devises et aux taux de change. L’administrateur de Workfront doit accorder un accès administratif supplémentaire à **Taux de change** pour permettre aux utilisateurs de définir des taux spécifiques sur les projets.
* Les taux de change dans Workfront ne sont pas dynamiques. La valeur est définie par un administrateur et doit être mise à jour en cas de modification des taux de change.
* Lorsque vous créez un rapport pour refléter la devise d’un projet, tous les rapports sont par défaut regroupés par devise par défaut du projet. Si vous créez un rapport avec plusieurs projets dont les taux de change sont différents, tous les regroupements appliqués au projet reflètent le taux de change par défaut au niveau du système. Pour plus d’informations, voir l’article [Créer des rapports de données financières avec des taux de change uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configuration de la devise d’un projet

1. Accédez au projet dans lequel vous souhaitez modifier la devise par défaut.

   >[!TIP]
   >
   >Assurez-vous que le projet ne contient pas d’informations financières. Par exemple, assurez-vous qu’aucun coût planifié ou réel n’est associé au projet.

1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis accédez au **Finance** zone.
1. Cliquez sur **Ajouter** dans le **Devise** et sélectionnez la devise à utiliser comme devise par défaut pour le projet. Toutes les devises que votre administrateur Workfront a définies pour votre instance Workfront s’affichent.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Conditionnel) Si vous sélectionnez une autre devise que la devise par défaut définie pour votre système Workfront, indiquez le taux de la devise que vous avez sélectionnée, car il correspond à la devise définie comme devise de base dans le système.
1. Cliquez sur **Enregistrer les modifications**.
