---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Compétences disponibles pour une installation directe
description: Workfront propose des compétences que vous pouvez installer directement dans votre LLM.
author: Becky
feature: Get Started with Workfront
source-git-commit: 20f5a513d8d33ecf8770f35bc73ee799a7de939e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---


# Compétences disponibles pour une installation directe

Workfront propose des compétences que vous pouvez installer directement dans votre LLM. Les compétences guident l’utilisation de ces outils pour des tâches spécifiques, avec les étapes adéquates déjà intégrées.

Vous trouverez ces compétences dans le référentiel GitHub des compétences Adobe .

>[!NOTE]
>
>Actuellement, ces compétences ne sont disponibles que pour Claude.
>Pour obtenir des instructions sur la configuration de Claude avec Adobe, voir [Prise en main](https://developer.adobe.com/adobe-for-creativity/getting-started/) dans la documentation d’Adobe Developer.

## Installez une compétence du référentiel GitHub de Workfront dans Claude.

1. Accédez au [référentiel de compétences ](https://github.com/adobe/skills/tree/main/plugins/workfront) sur GitHub.
1. Téléchargez le dossier de compétences que vous souhaitez utiliser.
1. Copiez le dossier dans votre bibliothèque de compétences Claude.

   * Claude Desktop : `~/Library/Application Support/Claude/skills/` (macOS) ou équivalent.
   * Code Claude : `~/.claude/skills/`.

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## Compétences actuellement disponibles

| Compétence / Lien vers le dossier | Description des compétences | Disponible pour |
|---|---|---|
| [architecte de solution Planning](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | Configurez un espace de travail Workfront Planning pour répondre à vos besoins et répondre aux questions sur Workfront Planning. | Claude |
