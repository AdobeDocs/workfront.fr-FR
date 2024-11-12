---
title: Création d’objets Workfront à l’aide d’automatismes d’enregistrement Workfront Planning
description: Vous pouvez configurer des automatisations dans la planification Workfront qui, lorsqu’elles sont activées, créent des objets dans Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: cfaacc4137ebfa7f2ed057522d43bd82715011df
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---


# Création d’objets à l’aide d’automatismes d’enregistrement Workfront Planning

Vous pouvez configurer des automatisations dans la planification Workfront qui, lorsqu’elles sont activées, créent des objets dans la planification Workfront ou Workfront.

Vous activez l&#39;automatisation dans les enregistrements. L’objet créé est connecté à l’enregistrement Planning dans lequel vous avez activé l’automatisation.

Par exemple, vous pouvez créer une automatisation qui prend une campagne de planification Workfront et crée un projet dans Workfront pour suivre la progression de cette campagne. Le projet sera connecté à la campagne de planification Workfront.

Pour plus d&#39;informations sur les enregistrements connectés, consultez la [présentation des enregistrements connectés](/help/quicksilver/planning/records/connected-records-overview.md).


## Configuration d’une automatisation dans la planification Workfront

Vous devez configurer une automatisation dans la planification Workfront avant de pouvoir l’utiliser pour créer des objets.

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) et sélectionnez **Automations**.

   La liste des automatisations disponibles s’ouvre.

1. Cliquez sur **Créer une automatisation** dans le coin supérieur droit de l’écran.
1. Dans le champ **Texte de bouton**, saisissez le texte que vous souhaitez afficher sur le bouton. Les utilisateurs cliqueront sur ce bouton lors de l’utilisation de l’automatisation pour créer un objet Workfront.
1. (Facultatif) Pour ajouter une icône au bouton, sélectionnez une icône parmi les options disponibles.
1. Dans le champ **Créer un type de** , sélectionnez l’objet que vous souhaitez que l’automatisation crée.

   Les objets disponibles sont les suivants :

   * Projet
   * Portfolio
   * Programme
   * Groupe

1. Dans le champ **Sélectionner le champ à utiliser dans le nom du projet** , sélectionnez un champ d’enregistrement. Le contenu de ce champ sera utilisé comme nom pour le nouvel objet.
1. Dans le champ **Sélectionner le champ pour lier le projet créé** , sélectionnez un champ d’enregistrement. Le nouvel objet apparaît dans ce champ lors de l’affichage de l’enregistrement dans Workfront Planning.
1. Sélectionnez d’autres options disponibles pour le type d’objet que vous créez.
1. Cliquez sur **Créer**

L’automatisation apparaît dans la liste des automatisations et peut être utilisée dans les enregistrements.

## Utilisation d’une automatisation de planification Workfront pour créer un objet

1. Dans Workfront Planning, ouvrez la page de type d’enregistrement contenant les enregistrements que vous souhaitez utiliser pour créer des objets Workfront.
1. Sélectionnez un ou plusieurs enregistrements.
1. Cliquez sur le bouton d’automatisation près du coin inférieur droit de l’écran.

   Dans cet exemple, il s’agit du bouton Créer un projet .

   ![Bouton Automatisation](assets/automation-custom-button.png)

>[!NOTE]
>
>Nous vous recommandons de vérifier que l’objet a été créé et connecté comme prévu.

