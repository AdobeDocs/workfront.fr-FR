---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Utiliser le serveur MCP Adobe Workfront
description: Utilisez le serveur Adobe Workfront MCP pour rechercher, créer, mettre à jour et gérer des éléments Workfront par le biais d’une conversation en langage naturel dans une plateforme agentique d’IA.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 1%

---


# Utiliser le serveur MCP Adobe Workfront

Le serveur MCP [!DNL Adobe Workfront] vous permet de rechercher, de créer, de mettre à jour et de gérer des éléments Workfront en demandant à une plateforme agentique d’IA de vous répondre en anglais standard. La plateforme décide des actions Workfront à appeler et gère la conversation avec Workfront pour vous.

[!DNL Claude] est actuellement la seule plateforme agentic d’IA prise en charge, mais les exemples et les modèles de cet article s’appliquent à toute plateforme agentic d’IA prenant en charge le serveur MCP de Workfront.

Cet article suppose que vous avez déjà configuré la connexion. Pour plus d’informations sur la configuration, voir [Configuration du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Pour plus d’informations sur le serveur Workfront MCP, consultez la section [Présentation du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Outils disponibles

Le serveur Workfront MCP expose un ensemble d’outils que la plateforme agentic d’IA appelle à votre place, par exemple, des outils pour rechercher des Workfront, créer des éléments, mettre à jour des champs et gérer les approbations. Pour obtenir la liste de référence complète, regroupée par zone de Workfront, consultez [Outils de serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Lorsque vous connectez une plateforme IA agentic à Workfront, celle-ci agit dans Workfront à l’aide de votre compte et de vos autorisations Workfront. Les actions de la plateforme ont le même effet que les actions que vous effectuez directement dans l’interface de Workfront.
>
>Vous et votre fournisseur de plateforme agentic d’IA êtes responsables des actions de la plateforme dans Workfront. Adobe n’est pas responsable des modifications apportées par la plateforme IA agentic à vos données Workfront.
>
>Avant de laisser la plateforme agentique d’IA traiter une demande, vérifiez que vous comprenez ce qu’elle a l’intention de faire, en particulier pour les actions qui modifient ou suppriment des données.


## Exemples de questions

Une fois la connexion établie, saisissez les requêtes en langage naturel dans votre plateforme agentique d’IA. La plateforme agentic d’IA décide des actions Workfront à appeler et renvoie les résultats.

### Rechercher et afficher votre travail

Pour rechercher dans Workfront des éléments qui correspondent à ce que vous recherchez, demandez :

* *Afficher tous les projets actifs pour l’équipe Brand Marketing.*
* *Obtenez-moi toutes les tâches assignées à Joan Harris.*
* *Afficher tous les événements du projet « Reconception de site web » dans la catégorie « Technique ».*

### Créer de nouveaux éléments

Pour créer des projets, des tâches ou d’autres éléments Workfront, demandez :

* *Créez un projet vierge appelé « Sandbox d’innovation du 2e trimestre » à partir du 10 mars et jusqu’au 30 avril. Me définir comme propriétaire.*
* *Ajoutez une nouvelle tâche appelée « AQ de la page de destination » au projet et planifiez-la du 22 au 26 avril.*
* *Créez un nouvel enregistrement de campagne appelé « Vente d’été 2026 »*

### Mettre à jour les éléments existants

Pour apporter des modifications à des éléments déjà dans Workfront, demandez :

* *Mettez à jour la tâche « Révision de la conception » pour qu’elle se termine le 18 avril et affectez-la à l’équipe créative.*
* *Pour le projet « Lucent AI Launch - NA », repoussez l&#39;arrivée à la mi-avril et augmentez le budget à 150 000 $.*
* *Mettez à jour le champ du budget dans l’enregistrement « Campagne d’été » à 75 000,* $

### Supprimer les éléments

Pour supprimer des éléments Workfront, demandez :

* *Supprimez le projet appelé « Campagne de test Q1 »*
* *Supprimez la tâche « Imprimer la production de ressources » du projet.*
* *Supprimez l’enregistrement de la campagne nommé « Ancienne promotion »*

>[!WARNING]
>
>La suppression d’éléments dans Workfront par le biais d’une plateforme agentique d’IA est identique à leur suppression dans l’interface de Workfront. Confirmez ce que la plateforme d’agence d’IA est sur le point de supprimer avant de la laisser continuer.

### Utiliser les validations

Pour gérer les approbations de documents et de ressources, demandez :

* *Ajouter Sarah Chen et Miguel Alvarez en tant qu&#39;approbateurs sur le document actuel.*
* *Envoyez un rappel aux approbateurs de la ressource « Vidéo de campagne de printemps » qui n’ont pas répondu.*
* *Appliquer le modèle d’approbation « Lancement marketing » à la ressource « Vidéo de campagne de printemps »*


### Utiliser les enregistrements Planning

Pour gérer les enregistrements de planification, demandez :

* *Créez un nouvel enregistrement de planification appelé « Plan marketing T2 » pour l’équipe Brand Marketing.*
* *Ajoutez une nouvelle tâche appelée « Audit des médias sociaux » à l’enregistrement de planification.*
* *Mettez à jour la tâche « Audit des médias sociaux » pour qu’elle se termine le 18 avril et affectez-la à l’équipe créative.*

### Utiliser un workflow

Pour gérer le workflow, demandez :

* *Acheminer le projet « Q2 Innovation Sandbox » au Conseil d&#39;examen de l&#39;innovation.*
* *Mettre à jour l’enregistrement « Campagne d’été » vers le statut « Prêt pour le lancement »*
* *Valider l’enregistrement « Campagne d’été ».*


### Chaîner les requêtes à travers une conversation

Vous pouvez enchaîner les demandes dans une seule conversation. La plateforme agentic d’IA conserve le contexte, de sorte que chaque requête peut s’appuyer sur la précédente. Par exemple :

1. Demander un ensemble d&#39;éléments : *Rechercher mes tâches en retard.*
1. Après avoir obtenu la liste, demandez une action sur les résultats : *Mettez-les tous à jour vers vendredi prochain.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considérations

Tenez compte des points suivants lorsque vous utilisez le serveur Workfront MCP.

### La plateforme agentique d’IA peut utiliser des informations provenant de stades antérieurs de la conversation

Les plateformes d’intelligence artificielle réutilisent parfois des données antérieures à une conversation au lieu de demander la dernière version à Workfront. Si quelque chose a changé dans Workfront depuis la dernière consultation de la plateforme agentic d’IA, des informations obsolètes risquent de s’afficher.

Pour forcer la plateforme agentique d’IA à récupérer des données récentes, demandez-les explicitement. Par exemple :

* *Obtenez les dernières données de Workfront. Ne pas utiliser les résultats mis en cache.*

### Le serveur MCP Workfront se met automatiquement à jour

Lorsqu’Adobe publie une nouvelle version du serveur MCP Workfront, votre plateforme IA agentic utilise automatiquement la nouvelle version. Vous n’avez pas besoin de vous reconnecter ou de changer quoi que ce soit de votre côté.

## Données et sécurité

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Quelles données quittent Workfront ?

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Comment les fournisseurs de plateformes d’intelligence artificielle gèrent vos données Workfront

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Différences entre les plateformes d’IA et les agences

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## Résolution des problèmes d’utilisation quotidiens

+++ Développez pour afficher les conseils de dépannage pour une utilisation quotidienne du serveur Workfront MCP.

| Problème | Cause probable | Corriger |
|---|---|---|
| La plateforme IA agentic vous donne des informations dépassées. | La plateforme agentique d’IA réutilise les données des étapes précédentes de la conversation. | Demandez de nouvelles données à Workfront. |
| La plateforme agentic d’IA a renvoyé des données provenant d’éléments Workfront incorrects. | La plateforme de l&#39;IA agentic a choisi les mauvais éléments en fonction d&#39;une formulation ambiguë. | Demandez à nouveau avec des noms, des identifiants ou des filtres plus spécifiques. |
| Une mise à jour ou une suppression n’a pas pris effet dans Workfront. | La plateforme agentic d’IA n’a pas encore appelé l’action ou vos autorisations ne l’autorisent pas. | Confirmez auprès de la plateforme agentique d’IA que l’action a exécutée, puis vérifiez vos autorisations Workfront. |

Pour plus d’informations sur les problèmes de configuration et d’authentification, voir [Dépannage de la configuration et de l’authentification](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) dans [Configuration du serveur MCP Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Questions fréquentes

+++ Développez pour afficher les questions fréquentes sur l’utilisation du serveur Workfront MCP.

### Avec quels éléments Workfront puis-je travailler via une plateforme agentique d’IA ?

Tous les éléments auxquels vous avez accès dans Workfront via les niveaux d’accès et les autorisations d’objet.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Mes données Workfront sont-elles envoyées au fournisseur de plateformes d’agence IA ou stockées par celui-ci ?

Pour plus d’informations, voir [Données et sécurité](#data-and-security) dans cet article.

### Que se passe-t-il lorsqu’une nouvelle version du serveur MCP Workfront est publiée ?

Le serveur MCP se met automatiquement à jour. Vous n’avez pas besoin de vous reconnecter ni de modifier quoi que ce soit.

### Dois-je connaître l’API Workfront pour utiliser le serveur MCP Workfront ?

Non. La plateforme agentic d’IA traduit vos requêtes en langage naturel en actions Workfront appropriées. Si vous connaissez déjà l’API Workfront, les actions vous sembleront familières, mais ce n’est pas obligatoire.

+++
