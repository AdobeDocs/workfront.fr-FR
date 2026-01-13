---
product-area: projects
navigation-topic: use-the-home-area
title: Utiliser le widget Mes requêtes
description: Vous pouvez envoyer des requêtes dans le widget Mes requêtes . Vous pouvez également personnaliser le widget avec des filtres et des colonnes.
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 9e4f67b4f5b03e1fc4f8e1a9ab00cc42b9796325
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 13%

---

# Utiliser le widget Mes requêtes

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

>[!IMPORTANT]
>
>Cet article décrit le nouveau widget Mes requêtes . La nouvelle expérience de demande doit être activée pour afficher le nouveau widget.
>Vous pouvez activer la nouvelle expérience de demande dans la zone des Demandes .

Le widget Mes requêtes affiche les requêtes que vous avez envoyées. Vous pouvez filtrer les requêtes, rechercher des requêtes spécifiques ou ajuster l’ordre et la visibilité des colonnes. Vous pouvez également créer une requête à partir du widget Mes requêtes .

>[!NOTE]
>
>* Lorsque le widget Mes requêtes se charge, il affiche jusqu’à 50 requêtes. Pour afficher davantage de requêtes, faites défiler la liste vers le bas.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence</strong></td> 
   <td> <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
    <tr> 
   <td role="rowheader"><strong>Produits supplémentaires</strong></td> 
   <td> Vous devez disposer d’Adobe Workfront Planning pour afficher les demandes Planning ou les formulaires de demande</td> 
  </tr> 
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>Accès en affichage ou supérieur à tout objet pour lequel vous êtes tagué dans une conversation ou pour lequel vous devez résoudre une approbation (projets, tâches, problèmes, documents)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations [!UICONTROL View] ou supérieures pour les projets, les tâches, les problèmes, les documents pour lesquels vous faites l’objet d’un tag dans une conversation ou pour lesquels devez résoudre une approbation.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une requête

Vous pouvez créer une demande directement à partir du widget Mes demandes .

Pour plus d’informations, consultez la section [Créer une demande](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) de l’article Création d’éléments de travail et de projets à partir de la zone Accueil.

<div class="preview">

## Copier une requête

Vous pouvez copier une demande dans le widget Mes demandes, la modifier et l’envoyer en tant que nouvelle demande.

Pour obtenir des instructions, consultez [&#x200B; Copier et envoyer des requêtes dans la nouvelle expérience de requête &#x200B;](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md#copy-and-submit-requests-in-the-new-requesting-experience) dans l’article Copier et envoyer des requêtes .

</div>

## Filtrage des requêtes

Le widget Mes requêtes comprend un filtre personnalisable qui vous permet de contrôler les requêtes qui apparaissent dans le widget. Vous pouvez configurer ce filtre pour différents champs et valeurs et empiler des conditions à l’aide des opérateurs AND et OR.

Pour configurer le filtre dans le widget Mes requêtes :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Pour ajouter le widget **Mes requêtes** à votre écran d’accueil. Cliquez sur **Personnaliser** et recherchez **Mes requêtes**.
1. Dans le widget Mes requêtes, cliquez sur **Filtrer**.
1. Dans le champ le plus à gauche, sélectionnez ce par quoi vous souhaitez filtrer. Les options disponibles sont les suivantes :

   * Espace de travail
   * Type d’objet
   * Date d’entrée
   * Formulaire de demande
   * Statut
   * Saisie effectuée par

   <span class="preview">Dans l’environnement Aperçu , vous pouvez également filtrer selon les champs personnalisés qui ont été ajoutés en tant que colonne      à la vue.</span>

1. Dans le champ suivant, sélectionnez l’opérateur que vous souhaitez utiliser pour cette condition de filtre. Les opérateurs disponibles dépendent du champ sélectionné.
1. (Conditionnel) Si un champ apparaît à droite de l’opérateur, sélectionnez la valeur en fonction de laquelle vous souhaitez appliquer un filtre.
1. (Facultatif) Pour ajouter une autre condition de filtre, cliquez sur **Ajouter une condition** et répétez les étapes 4 à 6.
1. (Facultatif et conditionnel) Si vous disposez de plusieurs conditions, basculez la valeur Et ou Ou en cliquant sur **Et** ou **Ou** à gauche de la condition.

Le filtre est enregistré automatiquement.

>[!TIP]
>
>Si votre organisation a acheté Workfront Planning, le widget Mes demandes inclura les demandes Workfront et Workfront Planning.
> 
>* Pour filtrer uniquement les requêtes Workfront, définissez le filtre sur **Type d’objet** > **Comporte l’un des** > **Problèmes**.
>* Pour filtrer uniquement les requêtes Workfront Planning, définissez le filtre sur **Type d’objet** > **N’a aucun des** > **Problèmes**.

## Ajuster ou ajouter des colonnes

Vous pouvez choisir parmi les colonnes disponibles celles qui apparaissent dans le widget Mes requêtes et définir leur ordre.

Les colonnes disponibles sont les suivantes :

* Objet
* Objet créé
* Type d’objet
* Statut
* Formulaire de demande
* Date d’entrée
* Saisie effectuée par

Pour ajuster les colonnes du widget Mes requêtes :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Pour ajouter le widget **Mes requêtes** à votre écran d’accueil. Cliquez sur **Personnaliser** et recherchez **Mes requêtes**.
1. Dans le widget Mes requêtes, cliquez sur **Colonnes**.
1. (Facultatif) Pour réorganiser les colonnes, cliquez sur la poignée de déplacement ![poignée](assets/drag-handle.png) de la colonne à déplacer et faites-la glisser aux emplacements souhaités. La colonne en haut de la liste apparaît dans le widget Mes requêtes en tant que colonne tout à gauche.
1. (Facultatif) Utilisez le bouton (bascule) pour contrôler si une colonne est affichée dans le widget Mes requêtes .
1. <span class="preview">Pour ajouter un champ personnalisé sous forme d’une colonne, cliquez sur l’icône **Ajouter une colonne** ![Ajouter une colonne](assets/add-column.png) à droite de l’écran, puis cliquez sur l’icône plus en regard du champ de formulaire personnalisé que vous souhaitez ajouter sous forme de colonne au widget.</span>

   <span class="preview">Vous pouvez ajouter des champs personnalisés sur les formulaires joints à l’objet dans la liste sous forme de colonnes.</span>

Les préférences de colonne sont enregistrées automatiquement.

## Requêtes de recherche

Pour rechercher des requêtes spécifiques dans le widget Mes requêtes :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Pour ajouter le widget **Mes requêtes** à votre écran d’accueil. Cliquez sur **Personnaliser** et recherchez **Mes requêtes**.
1. Dans la barre de recherche située en haut à droite du widget Mes requêtes , saisissez le terme que vous souhaitez rechercher.

   Les requêtes qui contiennent le terme sont surlignées en orange.

1. (Facultatif) Pour accéder directement aux requêtes en surbrillance, cliquez sur les flèches haut ou bas de la barre de recherche.

<div class="preview">

## Accéder à un objet créé par une requête

Vous trouverez des objets créés par une requête dans le widget Mes requêtes .

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Pour ajouter le widget **Mes requêtes** à votre écran d’accueil. Cliquez sur **Personnaliser** et recherchez **Mes requêtes**.
1. Recherchez la requête qui a créé l’objet .
1. Cliquez sur le nom de l’objet dans la colonne **Objet créé** de cette requête.

   La page de l’objet s’ouvre.

</div>
