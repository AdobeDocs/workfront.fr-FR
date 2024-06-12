---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Créer ou modifier un package de promotion d’environnement
description: La fonctionnalité de promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Découvrez comment créer un package de promotion d’environnement que vous pourrez ensuite installer dans un autre environnement.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: d249751b78e9d40fe7a351db14cbf0f3b7c79889
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 3%

---

# Créer ou modifier un package de promotion d’environnement

Vous devez créer, dans l’environnement, un module pour copier les objets. **de**. Par exemple, si vous configurez un projet dans votre environnement Sandbox d’actualisation personnalisée et que vous le faites passer à votre environnement de production, vous devez créer le module dans votre environnement Sandbox d’actualisation personnalisée.

>[!IMPORTANT]
>
>Si votre environnement de test d’actualisation personnalisée est actualisé pendant que vous configurez l’objet pour la promotion de l’environnement, cette configuration sera perdue lors de l’actualisation. Nous vous recommandons de ne pas actualiser votre sandbox d’actualisation personnalisée à moins que tous les objets et packages de promotion d’environnement en cours n’aient été promus avec succès.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Votre entreprise doit se conformer au nouveau modèle de tarification et avoir un plan Prime ou Ultimate.
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licences</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configurations du niveau d’accès
   </td>
   <td>Vous devez être un [!DNL Workfront] administrateur.
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Création d’un package

1. Accédez à l’environnement dans lequel vous souhaitez créer le module. C’est l’environnement dans lequel vous copiez des objets. **de**.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionner **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Cliquez sur **Créer un module**.

   La page Nouveau kit de promotion s’ouvre.

1. Dans le **Nom du module** , saisissez le nom du module.
1. Dans le **Description** , saisissez une description pour ce package.
1. Pour ajouter un objet au module, cliquez sur **Ajouter des objets** dans le volet de navigation de gauche, sélectionnez le type d’objet à ajouter.
1. Sélectionnez un ou plusieurs objets dans la liste ou saisissez le nom dans la barre de recherche et sélectionnez l’objet lorsqu’il apparaît dans la liste. Vous pouvez sélectionner plusieurs objets dans la liste.
1. Cliquez sur **Ajouter (objets X)** pour ajouter les objets sélectionnés au package.

   >[!INFO]
   >
   >**Exemple**
   >
   >Si vous avez sélectionné trois projets à ajouter au projet, le bouton indique : **Ajouter 3 projets**.

   Les objets que vous avez ajoutés apparaissent dans la zone Contenu du module située à droite de la page.

1. Pour ajouter un autre type d’objet, répétez les étapes 7 à 9.
1. (Facultatif) Pour supprimer un objet du module, passez la souris sur l’objet dans la zone Contenu du module, puis cliquez sur le X en regard de l’objet.
1. Après avoir ajouté tous les objets de votre choix au module, cliquez sur **Enregistrer et fermer** pour enregistrer le package sans l’assembler.

   Ou

   Cliquez sur **Enregistrer et assembler** pour enregistrer et assembler le module.

   >[!NOTE]
   >
   >* Les boutons Enregistrer et Fermer et Enregistrer et Assembler sont disponibles si un package porte à la fois un nom comportant cinq caractères ou plus et qu’au moins un objet y est ajouté.
   >* Vous ne pouvez pas assembler un module qui est dans un état installable tel que Tests ou Actif.

## Modifier ou assembler un package existant

1. Accédez à l’environnement dans lequel vous souhaitez créer le module. C’est l’environnement dans lequel vous copiez des objets. **de**.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionner **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Sélectionnez le package dans la liste affichée.
1. (Conditionnel) Pour afficher les modules désactivés, activez la variable **Afficher les packages retirés** .
1. (Facultatif) Pour afficher le contenu, y compris tous les objets et leurs sous-objets, cliquez sur la flèche de liste déroulante en regard du type d’objet dans la variable **Contenu** .
1. (Facultatif) Pour afficher les installations précédentes et les tentatives d’installation de ce package, cliquez sur **Déploiements**.
1. (Facultatif) Pour modifier le module, cliquez sur **Modifier le module** dans le coin supérieur droit de l’écran.
1. Pour installer le package, cliquez sur **Installer** dans le coin supérieur droit de l’écran.

   Pour plus d’informations sur l’installation d’un package, voir [Installer un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
