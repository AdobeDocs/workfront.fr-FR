---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Activer le stockage d’entreprise Adobe pour votre organisation
description: Vous pouvez activer le stockage d’entreprise Adobe pour que votre entreprise utilise une solution de stockage unifié pour tous les produits Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
source-git-commit: e70a65447fe508d055809271edad399d823f66dd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 11%

---

# Activer le stockage d’entreprise Adobe pour votre organisation

Le stockage d’entreprise Adobe est une solution de stockage unifié pour tous les produits Adobe. Il s’agit d’une solution de stockage dans le cloud qui sert de référentiel central pour les ressources des produits d’entreprise Adobe.

Le stockage d’entreprise Adobe est activé par défaut pour les nouveaux clients et peut être activé pour les clients existants lors du renouvellement du contrat.

Pour plus d’informations sur le stockage d’entreprise Adobe, consultez [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Activer le stockage d’entreprise Adobe pour votre organisation

Pour activer le stockage d’entreprise Adobe pour votre organisation :

{{step-1-to-setup}}

1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Préférences**.
1. Faites défiler l’écran jusqu’à la section **Préférences de stockage**.
1. Dans le menu déroulant Par défaut, sélectionnez **Stockage d’entreprise Adobe**.
1. (Facultatif) Si vous souhaitez utiliser une combinaison de stockage d’entreprise Adobe et de stockage Workfront hérité, cochez la case **Autoriser l’utilisateur à sélectionner le fournisseur de stockage**.

   >[!NOTE]
   >
   >L’activation de cette option permet aux utilisateurs de sélectionner le fournisseur de stockage lorsqu’ils créent un projet. Le stockage d’entreprise est étiqueté comme « Nouveau projet », car il s’agit du fournisseur de stockage par défaut. L’ancien stockage Workfront est intitulé « Projet hérité ».
   >
   >![options du nouveau projet et du projet hérité](assets/new-esm-project.png)

1. Dans le menu déroulant S’applique à , choisissez l’une des options suivantes :

   - **Organisation entière** : cette option applique le fournisseur de stockage par défaut à l’ensemble de votre environnement Workfront. Chaque fois qu’un utilisateur crée un projet, le fournisseur de stockage par défaut est utilisé.
   - **Groupes spécifiques** : cette option applique le fournisseur de stockage par défaut uniquement à des groupes spécifiques de votre organisation. Chaque fois qu’un utilisateur des groupes spécifiés crée un projet, le fournisseur de stockage par défaut est utilisé

1. Cliquez sur **Enregistrer**.
