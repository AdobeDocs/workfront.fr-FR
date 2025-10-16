---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Prise en main de l’intégration de GenStudio for Performance Marketing et de Workfront Proof
description: Prise en main de l’intégration de GenStudio for Performance Marketing et de Workfront Proof
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 7%

---

# Prise en main de l’intégration de GenStudio for Performance Marketing et de Workfront Proof

Grâce à l’intégration entre GenStudio for Performance Marketing et Workfront Proof, vous pouvez :

* Utiliser les modèles de BAT Workfront pour définir les workflows de révision et d’approbation

* Examinez et approuvez le contenu du brouillon GenStudio for Performance Marketing dans le lecteur de vérification Workfront.

* Afficher les décisions de révision dans GenStudio for Performance Marketing pour l’approbation et la publication finales

Pour plus d’informations sur la révision et l’approbation dans GenStudio for Performance Marketing, voir Intégration de [Workfront Proof à GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/approve/proof-integration).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> 
   <p>Tous</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Standard </p> 
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td> 
   <p> Vous devez disposer de GenStudio for Performance Marketing et vous devez être ajouté au produit en tant qu’utilisateur dans Admin Console. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Exigences d’intégration

* Workfront et GenStudio for Performance Marketing doivent être déployés sur la même organisation Identity Management System (IMS).

* Les utilisateurs ne peuvent appartenir qu’à une seule instance Workfront au sein de l’organisation IMS.

* L’instance Workfront doit être activée sur l’expérience unifiée Adobe.

* L’intégration doit être activée dans la zone Configuration de Workfront .


## Activation de l’intégration dans Workfront

Pour activer cette intégration, vous devez être administrateur système.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Dans le panneau de gauche, cliquez sur **Révision et approbation** > **Adobe GenStudio**.
1. Activez **Utiliser les validations de BAT**.
   ![activer la relecture pour le paramètre GenStudio](assets/enable-proofing-gs.png)

## Utiliser les modèles de BAT Workfront pour définir les workflows de validation

Si le processus de révision du contenu de votre entreprise est souvent répété ou révisé par les mêmes personnes, vous pouvez utiliser des modèles de BAT pour automatiser les workflows de révision et d’approbation.

### Création d’un modèle de BAT dans Workfront

Vous pouvez créer des modèles simples en une seule étape pour un ou deux réviseurs ou vous pouvez créer des modèles automatisés en plusieurs étapes pour des révisions complexes comportant de nombreuses étapes et dépendances.

Pour plus d’informations sur la création de workflows et de modèles automatisés dans Workfront, voir

* [Vue d’ensemble des workflows automatisés](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [Créer et gérer des modèles de workflows automatisés](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

### Choisir ou modifier le modèle dans GenStudio for Performance Marketing

Lorsque l’utilisateur lance une révision dans GenStudio for Performance Marketing, il choisit simplement le modèle dont il a besoin. Les utilisateurs peuvent facilement modifier n’importe quel modèle de workflow d’épreuve, ajouter ou supprimer des réviseurs et des étapes, à tout moment.

Pour plus d’informations, voir [Demander la révision et l’approbation](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/approve/request-review).

## Examinez et approuvez le contenu du brouillon GenStudio for Performance Marketing dans le lecteur de vérification Workfront.

Vous pouvez réviser et approuver le contenu provisoire directement dans GenStudio for Performance Marketing, dans le lecteur de vérification de Workfront.

Avec la visionneuse de relecture, vous pouvez :

* Laisser un commentaire
* Brouillon de mise en forme pour indiquer ce qui doit être modifié
* Prendre une décision

Pour plus d’informations, voir [Révision et modification du contenu](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/approve/review-and-edit).


>[!IMPORTANT]
>
>Les utilisateurs doivent installer le [Révision de contenu interactif avec l’outil de révision Adobe Workfront](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md) avant de pouvoir commencer à réviser les brouillons dans GenStudio for Performance Marketing.


## Afficher les décisions de révision dans GenStudio for Performance Marketing pour l’approbation et la publication finales

Une fois que la ressource a passé le processus de révision et d’approbation, vous pouvez afficher la décision de révision et publier le contenu directement depuis GenStudio for Performance Marketing.

Pour plus d’informations, voir [Publication du contenu approuvé](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/approve/publish-content).
