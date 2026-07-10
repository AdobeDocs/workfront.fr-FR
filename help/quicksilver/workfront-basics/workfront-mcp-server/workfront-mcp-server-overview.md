---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Présentation du serveur MCP Adobe Workfront
description: Découvrez la fonction du serveur MCP Adobe Workfront et comment il vous permet de travailler avec Workfront par le biais d’une conversation en langage naturel dans une plateforme agentique d’IA.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 5592c1b93b5e44c732f92d626ed878d2c4647ceb
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 6%

---


# Présentation du serveur MCP Adobe Workfront

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

Le serveur MCP [!DNL Adobe Workfront] connecte votre instance Workfront à une plateforme agentic d’IA telle que [!DNL Claude] ou [!DNL ChatGPT]. À partir de la plateforme agentic d’IA, vous pouvez rechercher, créer, mettre à jour et gérer des éléments Workfront en effectuant des requêtes en langage naturel.

Par exemple, vous pouvez demander :

* *Afficher tous les projets actifs pour l’équipe Brand Marketing.*
* *Mettez à jour la tâche « Révision de la conception » pour qu’elle se termine le 18 avril.*
* *Envoyez un rappel aux approbateurs de la ressource « Vidéo de campagne de printemps » qui n’ont pas répondu.*

Vous n’avez pas besoin de connaître l’API Workfront ni le fonctionnement des serveurs MCP pour utiliser le serveur MCP Workfront.

>[!IMPORTANT]
>
>Actuellement, le serveur Workfront MCP est disponible uniquement pour les clients qui utilisent AWS.

## Qu’est-ce qu’un serveur MCP

Un serveur MCP est un point de connexion qui permet à une plateforme agentique d’IA de fonctionner avec un autre système. Le serveur MCP Workfront est ce à quoi votre plateforme d’IA agentic se connecte afin de pouvoir lire et agir sur vos données Workfront en votre nom.

MCP est l’acronyme de Model Context Protocol. Il s’agit de la norme qui définit la manière dont les plateformes d’IA et les systèmes externes communiquent entre eux.

## Configurer la connexion

Le serveur Workfront MCP fonctionne avec toute plateforme d’IA agentic compatible avec MCP, telle que [!DNL Claude] ou [!DNL ChatGPT]. Avant de pouvoir l’utiliser, les actions suivantes doivent être effectuées :

* Un administrateur Workfront doit activer l’accès au serveur MCP dans votre instance Workfront.
* Vous (ou votre administrateur) devez connecter votre plateforme IA agentic à Workfront.

Pour plus d’informations, voir [Configuration du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Commencer à utiliser le serveur MCP Workfront

Après la configuration, vous pouvez demander à votre plateforme IA agentic de rechercher, créer, mettre à jour et gérer les éléments Workfront en langage naturel.

Pour plus d’informations, notamment sur les demandes d’exemple, les éléments à garder à l’esprit et les informations sur les données et la sécurité, consultez la section [ Utiliser le serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).
