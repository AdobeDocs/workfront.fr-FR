---
title: Créer des applications App Builder avec des compétences en code Claude
description: Utilisez un ensemble de compétences en code Claude pour créer des applications Adobe Workfront App Builder personnalisées en décrivant ce que vous souhaitez, au lieu d’exécuter vous-même les étapes de configuration et de déploiement.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# Créer des applications App Builder avec des compétences en code Claude

Un ensemble de compétences [!DNL Claude] permet (ou tout faisceau de codage d’IA prenant en charge les compétences au format Claude, telles que [!DNL Claude Code] ou [!DNL OpenAI Codex]) de créer des applications de [!DNL Adobe App Builder] personnalisées pour les [!DNL Workfront]. Si vous avez accès à l’un de ces outils, vous pouvez créer une extension d’interface utilisateur en décrivant ce que vous souhaitez en anglais clair, sans avoir à passer par une expérience de développement ou des étapes de configuration manuelles.

Les extensions d’interface d’utilisation de Workfront, optimisées par Adobe App Builder, permettent aux clientes et clients et aux partenaires de créer des expériences d’utilisation personnalisées. Les extensions d’interface utilisateur vous permettent de modifier l’expérience Workfront de votre entreprise afin de mieux répondre aux besoins de l’entreprise, ce qui peut améliorer l’efficacité, offrir des expériences connectées transparentes, améliorer considérablement la satisfaction des utilisateurs et aider votre entreprise à réaliser sa vision unique.

Pour plus d’informations sur les extensions de l’interface utilisateur de Workfront, voir [Création d’applications personnalisées pour Workfront avec Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Compétences d’extensibilité de l’interface utilisateur

Les compétences Extensibilité de l’interface utilisateur permettent à un faisceau de codage d’IA de gérer la création d’extensions d’interface utilisateur dans Workfront. Vous décrivez la fonctionnalité que vous souhaitez et elle effectue les tâches pratiques, telles que la configuration des outils, la création de votre projet dans [!DNL Adobe App Builder], la création de l’application, son déploiement dans le cloud Adobe et sa mise en œuvre dans Workfront. Vous êtes impliqué dans le processus uniquement lorsqu’une décision ou une connexion nécessite une action de votre part. Cet article utilise [!DNL Claude] comme exemple, mais les instructions s’appliquent à tout faisceau de codage d’IA avec la prise en charge des compétences Claude .

## Conditions préalables

Avant de commencer, vérifiez que vous disposez des éléments suivants :

* **Un faisceau de codage d’IA qui prend en charge les compétences Claude** tel que [!DNL Claude Code].

  Pour plus d&#39;informations sur les compétences Claude, voir [Que sont les compétences ? &#x200B;](https://support.claude.com/en/articles/12512176-what-are-skills) dans la documentation Claude.

* **Accès aux compétences**.

  * Vous trouverez les compétences à l’adresse [&#128279;](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Si ce lien ne s’ouvre pas pour vous, demandez à votre administrateur de vous accorder l’accès.
  * Les compétences sont publiées dans Adobe Public Skills Marketplace ([adobe/skills](https://github.com/adobe/skills)). Dans [!DNL Claude Code], exécutez :

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
