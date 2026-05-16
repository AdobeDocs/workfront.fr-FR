---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Activation du stockage dans le cloud Adobe pour votre organisation
description: Vous pouvez activer le stockage dans le cloud Adobe pour que votre entreprise puisse utiliser une solution de stockage unifié pour tous les produits Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 8%

---

# Activer le stockage dans le cloud Adobe pour votre organisation

Le stockage dans le cloud d’Adobe est une solution de stockage unifié pour tous les produits Adobe. Il s’agit d’une solution de stockage dans le cloud qui sert de référentiel central pour les ressources des produits d’entreprise Adobe.

Le stockage dans le cloud d’Adobe est activé par défaut pour les nouveaux clients et peut être activé pour les clients existants lors du renouvellement du contrat.

Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>N’importe quel package de workflow</p></td> 
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

## Activer le stockage dans le cloud Adobe pour votre organisation

Pour activer le stockage dans le cloud Adobe pour votre organisation :

{{step-1-to-setup}}

1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Préférences**.
1. Faites défiler l’écran jusqu’à la section **Préférences de stockage**.
1. Dans le menu déroulant Par défaut, sélectionnez **Espace de stockage**.
1. (Facultatif) Si vous souhaitez utiliser une combinaison d’espace de stockage dans le cloud Adobe et de stockage Workfront hérité, cochez la case **Autoriser l’utilisateur à sélectionner le fournisseur de stockage**.

   >[!NOTE]
   >
   >L’activation de cette option permet aux utilisateurs de sélectionner le fournisseur de stockage lorsqu’ils créent un projet. L’espace de stockage dans le cloud Adobe est étiqueté comme « Nouveau projet », car il s’agit du fournisseur de stockage par défaut. L’ancien stockage Workfront est intitulé « Projet hérité ».
   >
   >![options du nouveau projet et du projet hérité](assets/new-esm-project.png)

1. Dans le menu déroulant S’applique à , choisissez l’une des options suivantes :

   - **Organisation entière** : cette option applique le fournisseur de stockage par défaut à l’ensemble de votre environnement Workfront. Chaque fois qu’un utilisateur crée un projet, le fournisseur de stockage par défaut est utilisé.
   - **Groupes spécifiques** : cette option applique le fournisseur de stockage par défaut uniquement à des groupes spécifiques de votre organisation. Chaque fois qu’un utilisateur des groupes spécifiés crée un projet, le fournisseur de stockage par défaut est utilisé

1. Cliquez sur **Enregistrer**.

   >[!NOTE]
   >
   >Les projets existants conservent le modèle de stockage avec lequel ils ont été créés. Par exemple, les projets qui utilisent l’espace de stockage dans le cloud d’Adobe continuent à utiliser l’espace de stockage dans le cloud d’Adobe après avoir modifié la préférence de stockage par défaut.

## stockage dans le cloud Adobe dans les environnements sandbox

L’espace de stockage dans le cloud d’Adobe est disponible dans [!DNL Workfront] environnements sandbox. Vous pouvez ainsi tester la fonctionnalité décrite dans cet article avant de la déployer en production. Cependant, la visionneuse Frame.io n’étant pas disponible dans le sandbox, l’expérience complète de révision et d’approbation unifiée doit être validée en production.

Si vous disposez d’un sandbox d’actualisation personnalisé, vous devez l’actualiser après la mise à niveau vers une version de Workfront prenant en charge l’espace de stockage dans le cloud Adobe. L’actualisation permet au sandbox d’accéder à la fonctionnalité d’espace de stockage dans le cloud d’Adobe afin que vous puissiez commencer à la tester. Pour plus d’informations, voir [Environnement  [!DNL Adobe Workfront]  sandbox d’actualisation personnalisée](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).
