---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Comparaison d’objets entre des environnements
description: Vous pouvez comparer des objets entre des environnements pour vous assurer que vos packages de promotion d’environnement contiennent les objets dont vous avez besoin.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 085b0f04-5a9c-49b9-86d7-2363731ee067
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 12%

---

# Comparaison d’objets entre des environnements

Vous pouvez comparer des objets entre des environnements pour vous assurer que vos packages de promotion d’environnement contiennent les objets dont vous avez besoin.

Vous sélectionnez les environnements et les types d’objets à comparer. Workfront compare tous les objets des types sélectionnés dans les deux environnements et présente les données concernant les différences d’objets.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Licences Workfront</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td><p>Vous devez être un administrateur ou une administratrice Workfront.</p>
   </td>
  </tr>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Votre organisation doit se trouver sur la plateforme Adobe Business pour comparer des objets entre les environnements.

## Générer une comparaison d’objets

1. Accédez à un environnement dans lequel vous souhaitez comparer un objet.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Cliquez sur **Comparer les environnements** dans le coin supérieur droit de l’écran.
1. Dans le champ Environnement **Source**, sélectionnez l’environnement dans lequel vous souhaitez créer le package. Il s’agit de l’environnement à partir duquel vous copiez des objets **&#x200B;**.
1. Dans le champ **Environnement cible**, sélectionnez l’environnement dans lequel vous souhaitez installer le package. Il s’agit de l’environnement dans lequel vous copiez des objets **vers**.
1. Dans la zone **Objets à comparer**, sélectionnez les types d’objets à comparer entre les environnements.
1. Cliquez sur **Générer la comparaison** dans le coin supérieur droit de l’écran.

   La génération de la comparaison peut prendre un certain temps, selon le nombre et la taille des objets comparés.

## Afficher la comparaison des objets

Une fois la génération de la comparaison terminée, la comparaison s’affiche.

La liste inclut les objets du ou des types sélectionnés qui existent dans l’environnement source, si ces objets sont manquants dans l’environnement cible et s’il existe des différences de champ entre les deux.

>[!BEGINSHADEBOX]

![Exemple de comparaison](assets/environment-promotion-comparison.png)

Dans cet exemple :

* La première ligne montre un objet présent dans l’environnement cible, mais différent de l’environnement source.
* La deuxième ligne montre un objet présent dans l’environnement cible et identique à celui de l’environnement source.
* La troisième ligne montre un objet qui n’est pas présent dans l’environnement cible.

>[!ENDSHADEBOX]

Pour afficher les différences d’objet spécifiques :

1. Cliquez sur l’icône en forme de loupe ![icône de comparaison](assets/compare-icon.png) sur la ligne correspondant à cet objet.

   Une fenêtre s’ouvre avec tous les champs de cet objet. les différences sont indiquées en rouge.

## Créer un package à partir d’une comparaison d’objets

Vous pouvez créer un package directement à partir d’une comparaison d’objets.

Pour obtenir des instructions, consultez [Créer un package à partir d’une comparaison d’objets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison) dans l’article Créer ou modifier un package de promotion d’environnement.
