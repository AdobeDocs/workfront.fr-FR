---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Compétences disponibles pour une installation directe
description: Workfront propose des compétences que vous pouvez installer directement dans votre LLM.
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 7fd4c07f2ea1e47e7abb7d3dd78638a6a01d0f47
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Compétences disponibles pour une installation directe

Adobe Workfront propose des compétences que vous pouvez installer directement dans votre LLM. Les compétences guident l’utilisation de ces outils pour des tâches spécifiques, avec les étapes adéquates déjà intégrées.

Vous trouverez ces compétences sous forme de fichiers dans le référentiel GitHub des compétences Adobe. Ce référentiel contient des fichiers pour divers produits Adobe. Lorsque vous téléchargez ces fichiers et que vous les copiez à Claude, Claude peut alors utiliser les compétences décrites dans les fichiers.

Par exemple, les compétences d&#39;architecte de solution Planning permettent à Claude de répondre à des questions sur Workfront Planning et d&#39;effectuer certaines actions.

Il n’est pas nécessaire d’appeler ou de déclencher ces compétences après les avoir copiées dans le LLM. Au lieu de cela, vous pouvez interagir avec votre LLM comme vous le faites habituellement, en posant des questions en langage naturel, et le LLM utilise les informations et les actions décrites dans les compétences appropriées à la conversation.

>[!NOTE]
>
>Actuellement, ces compétences ne sont disponibles que pour Claude.
>Pour obtenir des instructions sur la configuration de Claude avec Adobe, voir [Prise en main](https://developer.adobe.com/adobe-for-creativity/getting-started/) dans la documentation d’Adobe Developer.

## Installer une compétence à partir du référentiel GitHub de Workfront dans Claude

1. Accédez au [référentiel de compétences &#x200B;](https://github.com/adobe/skills/tree/main/plugins/workfront) sur GitHub.
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
