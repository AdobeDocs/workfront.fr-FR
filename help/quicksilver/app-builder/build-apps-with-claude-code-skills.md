---
title: Créer des applications App Builder avec des compétences en code Claude
description: Utilisez un ensemble de compétences en code Claude pour créer des applications Adobe Workfront App Builder personnalisées en décrivant ce que vous souhaitez, au lieu d’exécuter vous-même les étapes de configuration et de déploiement.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: e5a288dcac20be9176d1541d531edaf0d8c99a8c
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---


# Créer des applications App Builder avec des compétences en code Claude

Un ensemble de compétences [!DNL Claude Code] [!DNL Claude] permet de créer des applications [!DNL Adobe App Builder] personnalisées pour les [!DNL Workfront]. Cela signifie que vous pouvez en créer un en décrivant ce que vous souhaitez en langage clair, sans être développeur ni écrire les étapes de configuration vous-même.

Les extensions d’interface d’utilisation de Workfront, optimisées par Adobe App Builder, permettent aux clientes et clients et aux partenaires de créer des expériences d’utilisation personnalisées. Les extensions d’interface utilisateur vous permettent de modifier l’expérience Workfront de votre entreprise afin de mieux répondre aux besoins de l’entreprise, ce qui peut améliorer l’efficacité, offrir des expériences connectées transparentes, améliorer considérablement la satisfaction des utilisateurs et aider votre entreprise à réaliser sa vision unique.

Pour plus d’informations sur les extensions de l’interface utilisateur de Workfront, voir [Création d’applications personnalisées pour Workfront avec Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Compétences d’extensibilité de l’interface utilisateur pour Claude

L’utilisation de [!DNL Adobe App Builder] peut être assez technique, ce qui peut créer des obstacles si un utilisateur n’est pas familier avec la procédure ou les techniques. Les compétences Extensibilité de l’interface utilisateur simplifient ce processus en utilisant [!DNL Claude]. Vous décrivez la fonctionnalité que vous souhaitez et [!DNL Claude] effectue le travail pratique, comme configurer les outils, créer votre projet dans [!DNL Adobe App Builder], créer l’application, la déployer sur le cloud Adobe et la faire fonctionner dans Workfront. Vous êtes impliqué dans le processus uniquement lorsqu’une décision ou une connexion nécessite une action de votre part.

## Conditions préalables

Avant de commencer, vérifiez que vous disposez des éléments suivants :

* **[!DNL Claude Code]** installé.
* **Accès aux compétences**.

  * Vous trouverez les compétences à l’adresse [&#128279;](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Si ce lien ne s’ouvre pas pour vous, demandez à votre administrateur de vous accorder l’accès.
  * Après avoir téléchargé les compétences, exécutez les commandes suivantes pour les configurer.

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* **[!DNL Adobe App Builder]l’accès, avec le rôle Développeur**. Votre organisation Adobe a besoin d’une licence App Builder, et vous devez y être ajouté en tant que développeur. C’est ce qui [!DNL Claude] permet d’ouvrir le Adobe Developer Console et de créer votre projet.

  Pour vérifier que cette condition préalable est remplie :

  1. Ouvrez l’[Adobe Developer Console](https://developer.adobe.com/console).
  1. Vérifiez que l’organisation affichée dans le coin supérieur droit est correcte.
  1. Cliquez sur **Créer un projet** > **Créer un projet à partir d’un modèle**.
  1. Vérifiez si **&#x200B;**&#x200B;apparaît dans la liste.

     * Si vous voyez **&#x200B;**&#x200B;dans la liste, vous avez accès.
     * S’il n’y a pas d’option **Créer un projet à partir d’un modèle** ou d’option **App Builder**, vous n’avez pas encore accès. Demandez à votre administrateur Workfront ou Adobe de vous ajouter en tant que développeur (dans Adobe Admin Console > Utilisateurs > Développeurs) et confirmez que votre organisation dispose d’une licence App Builder.
* **Le serveur MCP Workfront est connecté**, [!DNL Claude] utilise donc l’API Workfront réelle au lieu de deviner les types de données, les champs et les commandes.

  Pour vérifier si le serveur MCP Workfront est déjà connecté, demandez [!DNL Claude] : *« Voyez-vous les ressources MCP Workfront ?«*

  Pour plus d’informations et d’instructions, voir [Connexion de Workfront à Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude) dans l’article Configuration du serveur MCP Adobe Workfront.
