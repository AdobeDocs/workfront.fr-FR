---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Activer le stockage dans le cloud Adobe pour votre organisation
description: Vous pouvez activer le stockage dans le cloud Adobe pour que votre entreprise puisse utiliser une solution de stockage unifié pour tous les produits Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 6%

---
# Activer le stockage dans le cloud Adobe pour votre organisation

le stockage dans le cloud d’Adobe est une solution de stockage unifiée dans le cloud qui sert de référentiel central pour les ressources des produits d’entreprise Adobe. Cet article décrit comment activer l’espace de stockage Adobe en tant qu’option de stockage par défaut pour l’ensemble de votre organisation ou pour des groupes spécifiques.

Il s’agit de l’action unique qui active la nouvelle expérience : une fois que vous l’activez, les nouveaux projets utilisent l’espace de stockage dans le cloud Adobe, qui inclut la visionneuse Frame.io et les approbations unifiées. Rien ne change jusqu’à ce que vous choisissiez d’activer l’espace de stockage Adobe dans le cloud.

Étant donné que vous contrôlez le minutage, vous pouvez tester l’expérience, mettre à jour vos scénarios Workfront Fusion et planifier les modifications des rapports avant que quiconque n’y travaille. Pour plus d’informations sur les différences et la planification de votre déploiement, consultez [Déplacer vers Workfront sur l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Fonctionnement des validations avec l’espace de stockage dans le cloud d’Adobe

L’espace de stockage dans le cloud Adobe détermine le service d’approbation utilisé par un projet. Le passage à une version de Workfront prenant en charge l’espace de stockage Adobe dans le cloud ne fait pas automatiquement basculer l’ensemble de votre organisation vers les approbations unifiées. Au lieu de cela, le service de validation dépend du modèle de stockage de chaque projet :

* **Les projets de stockage dans le cloud** utilisent par défaut les approbations unifiées, avec révision et approbation dans la visionneuse Frame.io.
* **Projets de stockage Workfront hérités** conservez le service d’approbation qu’ils utilisent déjà. Selon votre organisation, il peut s’agir d’approbations unifiées ou d’approbations de documents hérités.

Pour plus d’informations sur l’expérience de révision et d’approbation sur l’espace de stockage cloud d’Adobe, voir [Déplacer vers Workfront sur l’espace de stockage cloud d’Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

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

   * **Organisation entière** : cette option applique le fournisseur de stockage par défaut à l’ensemble de votre environnement Workfront. Chaque fois qu’un utilisateur crée un projet, le fournisseur de stockage par défaut est utilisé.
   * **Groupes spécifiques** : cette option applique le fournisseur de stockage par défaut uniquement à des groupes spécifiques de votre organisation. Chaque fois qu’un utilisateur des groupes spécifiés crée un projet, le fournisseur de stockage par défaut est utilisé.

     ![groupes de préférences de stockage](assets/configure-storage-preference.png)

1. Cliquer sur **Enregistrer**.

   >[!NOTE]
   >
   >Les projets existants conservent le modèle de stockage avec lequel ils ont été créés. Par exemple, les projets qui utilisent l’espace de stockage dans le cloud d’Adobe continuent à utiliser l’espace de stockage dans le cloud d’Adobe après avoir modifié la préférence de stockage par défaut.



## stockage dans le cloud Adobe dans les environnements sandbox

L’espace de stockage dans le cloud d’Adobe est disponible dans [!DNL Workfront] environnements sandbox. Vous pouvez ainsi tester la fonctionnalité décrite dans cet article avant de la déployer en production. Cependant, la visionneuse Frame.io n’étant pas disponible dans le sandbox, l’expérience complète de révision et d’approbation unifiée doit être validée en production.

Si vous disposez d’un sandbox d’actualisation personnalisé, vous devez l’actualiser après la mise à niveau vers une version de Workfront prenant en charge l’espace de stockage dans le cloud Adobe. L’actualisation permet au sandbox d’accéder à la fonctionnalité d’espace de stockage dans le cloud d’Adobe afin que vous puissiez commencer à la tester. Pour plus d’informations, voir [Environnement  [!DNL Adobe Workfront]  sandbox d’actualisation personnalisée](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).
