---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Créer ou modifier un package de promotion environnementale
description: La fonctionnalité de promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Découvrez comment créer un package de promotion d’environnement que vous pourrez ensuite installer dans un autre environnement.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 2e4bcd6400971104e9138fab0faf20d33af32e51
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 17%

---

# Créer ou modifier un package de promotion environnementale

Vous devez créer dans l’environnement un package que vous souhaitez copier des objets **à partir de**. Par exemple, si vous configurez un projet dans votre environnement Sandbox d’actualisation personnalisée et que vous le faites passer à votre environnement de production, vous devez créer le module dans votre environnement Sandbox d’actualisation personnalisée.

>[!IMPORTANT]
>
>Si votre environnement de test d’actualisation personnalisée est actualisé pendant que vous configurez l’objet pour la promotion de l’environnement, cette configuration sera perdue lors de l’actualisation. Nous vous recommandons de ne pas actualiser votre sandbox d’actualisation personnalisée à moins que tous les objets et packages de promotion d’environnement en cours n’aient été promus avec succès.

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

1. Accédez à l’environnement dans lequel vous souhaitez créer le module. Il s’agit de l’environnement dans lequel vous copiez des objets **à partir de**.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **System** dans le volet de navigation de gauche, puis **Environment Promotion**.
1. Cliquez sur **Créer un module**.

   La page Nouveau kit de promotion s’ouvre.

1. Dans le champ **Nom du module** , saisissez un nom pour le module.
1. Dans le champ **Description** , saisissez une description pour ce package.
1. Pour ajouter un objet au package, dans le volet de navigation de gauche, sélectionnez le type d’objet à ajouter.
1. Sélectionnez un ou plusieurs objets dans la liste qui s’affiche ou saisissez le nom dans la barre de recherche et sélectionnez l’objet lorsqu’il apparaît dans la liste. Vous pouvez sélectionner plusieurs objets dans la liste.

   La liste comprend jusqu’à 500 objets du type d’objet sélectionné. Pour localiser un objet qui ne figure pas dans la liste, utilisez la barre de recherche.
1. Cliquez sur **Ajouter (X Objets)** pour ajouter les objets sélectionnés au package.

   >[!INFO]
   >
   >**Exemple**
   >
   >Si vous avez sélectionné trois projets à ajouter au projet, le bouton indique **Ajouter 3 projets**.

   Les objets que vous avez ajoutés apparaissent dans la zone Contenu du module située à droite de la page.

1. Pour ajouter un autre type d’objet, répétez les étapes 7 à 9.
1. (Facultatif) Pour supprimer un objet du module, passez la souris sur l’objet dans la zone Contenu du module, puis cliquez sur le X en regard de l’objet.
1. Après avoir ajouté tous les objets de votre choix au module, cliquez sur **Enregistrer et fermer** pour enregistrer le module sans l’assembler.

   Ou

   Cliquez sur **Enregistrer et assembler** pour enregistrer et assembler le package.

   >[!NOTE]
   >
   >* Les boutons Enregistrer et Fermer et Enregistrer et Assembler sont disponibles si un package porte à la fois un nom comportant cinq caractères ou plus et qu’au moins un objet y est ajouté.
   >* Vous ne pouvez pas assembler un module qui est dans un état installable tel que Tests ou Actif.

## Modifier ou assembler un package existant

Un package doit être à l’état `DRAFT` pour être modifié.

1. Accédez à l’environnement dans lequel vous souhaitez modifier le module. Il s’agit de l’environnement dans lequel le module a été créé à l’origine.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **System** dans le volet de navigation de gauche, puis **Environment Promotion**.
1. Sélectionnez le package dans la liste affichée.
1. (Conditionnel) Pour afficher les modules désactivés, activez l’option **Afficher les modules abandonnés** .
1. (Facultatif) Pour afficher le contenu, y compris tous les objets et leurs sous-objets, cliquez sur la flèche déroulante en regard du type d’objet dans la section **Contenu** .
1. (Facultatif) Pour afficher les installations précédentes et les tentatives d’installation de ce package, cliquez sur **Déploiements**.
1. (Facultatif) Pour modifier le module, cliquez sur **Modifier le module** dans l’angle supérieur droit de l’écran.
Un package doit être à l’état `DRAFT` pour être modifié. Pour déplacer le package vers l’état `DRAFT`, dans le champ **Status**, sélectionnez `Draft`. Vous pouvez ensuite continuer à modifier le module.
1. Pour installer le package, cliquez sur **Installer** dans le coin supérieur droit de l’écran.

   Pour plus d&#39;informations sur l&#39;installation d&#39;un package, voir [Installation d&#39;un package de promotion d&#39;environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
