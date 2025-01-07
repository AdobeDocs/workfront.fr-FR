---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Créer ou modifier un package de promotion environnementale
description: La fonctionnalité de promotion d’environnement est destinée à fournir la possibilité de déplacer des objets liés à la configuration d’un environnement à un autre. Découvrez comment créer un package de promotion d’environnement que vous pouvez ensuite installer dans un autre environnement.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 839b53afb9233ef0e36e981b243c8b2593b45f0f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 15%

---

# Créer ou modifier un package de promotion environnementale

Vous devez créer un package dans l’environnement à partir duquel vous souhaitez copier les objets ****. Par exemple, si vous configurez un projet dans votre environnement de sandbox d’actualisation personnalisée et que vous le promouvez dans votre environnement de production, vous devez créer le package dans votre environnement de sandbox d’actualisation personnalisée.

>[!IMPORTANT]
>
>Si votre sandbox d’actualisation personnalisée est actualisé pendant que vous configurez l’objet pour la promotion de l’environnement, cette configuration est perdue lors de l’actualisation. Nous vous recommandons de ne pas actualiser votre sandbox d’actualisation personnalisée tant que tous les objets et packages de promotion d’environnement en attente n’ont pas été promus avec succès.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Plan <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td> Prime ou Ultimate (nouveaux plans uniquement)
   </td>
  </tr>
  <tr>
   <td>Licences <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créer un package

1. Accédez à l’environnement dans lequel vous souhaitez créer le package. Il s’agit de l’environnement à partir duquel vous copiez des objets ****.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Cliquez sur **Créer un package**.

   La page Nouveau package de promotion s’ouvre.

1. Dans le champ **Nom du package**, saisissez un nom pour le package.
1. Dans le champ **Description**, saisissez une description du package.
1. Pour ajouter un objet au package, dans le volet de navigation de gauche, sélectionnez le type d’objet à ajouter.
1. Sélectionnez un ou plusieurs objets dans la liste qui s’affiche ou saisissez le nom dans la barre de recherche et sélectionnez l’objet lorsqu’il apparaît dans la liste. Vous pouvez sélectionner plusieurs objets dans la liste.

   La liste comprend jusqu’à 500 objets du type d’objet sélectionné. Pour localiser un objet qui ne figure pas dans la liste, utilisez la barre de recherche.
1. Cliquez sur **Ajouter (X objets)** pour ajouter les objets sélectionnés au package.

   >[!INFO]
   >
   >**Exemple**
   >
   >Si vous avez sélectionné trois projets à ajouter au projet, le bouton indique **Ajouter 3 projets**.

   Les objets que vous avez ajoutés s’affichent dans la zone Contenu du package située à droite de la page.

1. Pour ajouter un autre type d’objet, répétez les étapes 7 à 9.
1. (Facultatif) Pour supprimer un objet du package, passez la souris sur l’objet dans la zone Contenu du package, puis cliquez sur le X en regard de l’objet .
1. Après avoir ajouté tous les objets souhaités au package, cliquez sur **Enregistrer et fermer** pour enregistrer le package sans l’assembler.

   Ou

   Cliquez sur **Enregistrer et assembler** pour enregistrer et assembler le package.

   >[!NOTE]
   >
   >* Les boutons Enregistrer et Fermer et Enregistrer et assembler sont disponibles si un package possède à la fois un nom comportant cinq caractères ou plus et au moins un objet ajouté.
   >* Vous ne pouvez pas assembler un package dont le statut peut être installé, tel que Test ou Actif.

## Modifier ou assembler un package existant

Un package doit avoir `DRAFT` statut pour être modifié.

1. Accédez à l’environnement dans lequel vous souhaitez modifier le package. Il s’agit de l’environnement dans lequel le package a été créé à l’origine.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Sélectionnez le package dans la liste qui s&#39;affiche.
1. (Conditionnel) Pour afficher les packages désactivés, activez l’option **Afficher les packages retirés**.
1. (Facultatif) Pour afficher le contenu, y compris tous les objets et leurs sous-objets, cliquez sur la flèche déroulante en regard du type d’objet dans la section **Contenu**.
1. (Facultatif) Pour afficher les installations précédentes et les tentatives d’installation de ce package, cliquez sur **Déploiements**.
1. (Facultatif) Pour modifier le package, cliquez sur **Modifier le package** dans le coin supérieur droit de l’écran.
Un package doit avoir `DRAFT` statut pour être modifié. Pour déplacer le package vers `DRAFT` statut, dans le champ **Statut**, sélectionnez `Draft`. Vous pouvez ensuite continuer à modifier le package.
1. Pour installer le package, cliquez sur **Installer** dans le coin supérieur droit de l’écran.

   Pour obtenir des instructions sur l’installation d’un package, voir [Installation d’un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).

## Créer un package à partir d’une comparaison d’objets

Vous pouvez créer un package directement à partir d’une comparaison d’objets.

1. Créez une comparaison d’objets, comme décrit dans la section [Comparer des objets entre des environnements](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).
1. Dans la comparaison générée, sélectionnez les objets que vous souhaitez inclure dans le package.
1. Cliquez sur **Créer un package** dans le coin supérieur droit de l’écran.
1. Saisissez un nom et une description pour le package.
1. Cliquez sur **Créer un package** dans la fenêtre Créer un package .

   Le package est généré.
