---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Utiliser le serveur MCP Adobe Workfront
description: Utilisez le serveur MCP Adobe Workfront pour rechercher, créer, mettre à jour et gérer des éléments Workfront par le biais d’une conversation en langage naturel dans un assistant d’IA.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# Utiliser le serveur MCP Adobe Workfront

Le serveur MCP [!DNL Adobe Workfront] vous permet de rechercher, créer, mettre à jour et gérer des éléments Workfront en demandant à un assistant d’IA de vous répondre en anglais courant. L’assistant d’IA décide des actions Workfront à appeler et gère la conversation avec Workfront pour vous.

[!DNL Claude] est actuellement le seul assistant d’IA pris en charge, mais les exemples et les modèles de cet article s’appliquent à tout assistant d’IA qui prend en charge le serveur MCP Workfront.

Cet article suppose que vous avez déjà configuré la connexion. Pour plus d’informations sur la configuration, voir [Configuration du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Pour plus d’informations sur le serveur Workfront MCP, consultez la section [Présentation du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).



## Actions disponibles via le serveur MCP Workfront

Le serveur Workfront MCP couvre les actions relatives aux approbations, à la planification et aux workflows.

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>Un assistant d’IA agit dans Workfront à l’aide de votre compte et des autorisations Workfront. Vous et votre fournisseur d’assistant d’IA êtes responsables des actions que l’assistant d’IA entreprend en votre nom. Confirmez ce que l’assistant d’IA est sur le point de faire avant de le laisser continuer.


## Responsabilité des actions des assistants d&#39;IA

Lorsque vous connectez un assistant d’IA à Workfront, il agit dans Workfront à l’aide de votre compte et de vos autorisations Workfront. Les actions de l’assistant d’IA ont le même effet que les actions que vous effectuez directement dans l’interface de Workfront.

Vous et votre fournisseur d’assistant d’IA êtes responsables des actions que l’assistant d’IA entreprend dans Workfront. Adobe n’est pas responsable des modifications apportées par l’assistant d’IA à vos données Workfront.

Avant de laisser l’assistant d’IA traiter une demande, vérifiez que vous comprenez ce qu’il a l’intention de faire, en particulier pour les actions qui modifient ou suppriment des données.

### Actions principales

Le serveur MCP Workfront comprend les actions principales suivantes :

| Action | Fonctionnement |
|---|---|
| Créer | Crée de nouveaux éléments dans Workfront. |
| Recherche | Recherche et récupère des éléments de Workfront. |
| Mettre à jour | Modifie les éléments existants dans Workfront. |
| Supprimer | Supprime des éléments de Workfront. |
| Résoudre les noms de champ | Recherche les noms de champ Workfront corrects afin que l’assistant d’IA puisse créer des requêtes précises sur vos données. |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### Actions d&#39;approbation

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### Planifier les actions

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### Actions de workflow

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## Exemples de questions

Une fois la connexion établie, saisissez les requêtes en langage naturel dans l’assistant d’IA. L’assistant d’IA décide des actions Workfront à appeler et renvoie les résultats.

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### Rechercher et afficher votre travail

Demandez à l’assistant d’IA de rechercher dans Workfront les éléments qui correspondent à ce que vous recherchez. Par exemple :

* *Afficher tous les projets actifs pour l’équipe Brand Marketing.*
* *Obtenez-moi toutes les tâches assignées à Joan Harris.*
* *Afficher tous les événements du projet « Reconception de site web » dans la catégorie « Technique ».*

### Créer de nouveaux éléments

Demandez à l’assistant d’IA de créer des projets, des tâches ou d’autres éléments Workfront. Par exemple :

* *Créez un projet vierge appelé « Sandbox d’innovation du 2e trimestre » à partir du 10 mars et jusqu’au 30 avril. Me définir comme propriétaire.*
* *Ajoutez une nouvelle tâche appelée « AQ de la page de destination » au projet et planifiez-la du 22 au 26 avril.*
* *Créez un nouvel enregistrement de campagne appelé « Vente d’été 2026 »*

### Mettre à jour les éléments existants

Demandez à l’assistant AI d’apporter des modifications aux éléments déjà dans Workfront. Par exemple :

* *Mettez à jour la tâche « Révision de la conception » pour qu’elle se termine le 18 avril et affectez-la à l’équipe créative.*
* *Pour le projet « Lucent AI Launch - NA », repoussez l&#39;arrivée à la mi-avril et augmentez le budget à 150 000 $.*
* *Mettez à jour le champ du budget dans l’enregistrement « Campagne d’été » à 75 000,* $

### Supprimer les éléments

Demandez à l’assistant d’IA de supprimer des éléments Workfront. Par exemple :

* *Supprimez le projet appelé « Campagne de test Q1 »*
* *Supprimez la tâche « Imprimer la production de ressources » du projet.*
* *Supprimez l’enregistrement de la campagne nommé « Ancienne promotion »*

>[!WARNING]
>
>La suppression d’éléments dans Workfront par le biais d’un assistant d’IA est identique à leur suppression dans l’interface de Workfront. Confirmez ce que l’assistant d’IA est sur le point de supprimer avant de le laisser continuer.

### Utiliser les validations

Demandez à l’assistant AI de gérer les approbations de documents et de ressources. Par exemple :

* *Ajouter Sarah Chen et Miguel Alvarez en tant qu&#39;approbateurs sur le document actuel.*
* *Envoyez un rappel aux approbateurs de la ressource « Vidéo de campagne de printemps » qui n’ont pas répondu.*
* *Appliquer le modèle d’approbation « Lancement marketing » à la ressource « Vidéo de campagne de printemps »*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### Utiliser les enregistrements Planning

Demandez à l’assistant d’IA de gérer les enregistrements de planification. Par exemple :

* *Créez un nouvel enregistrement de planification appelé « Plan marketing T2 » pour l’équipe Brand Marketing.*
* *Ajoutez une nouvelle tâche appelée « Audit des médias sociaux » à l’enregistrement de planification.*
* *Mettez à jour la tâche « Audit des médias sociaux » pour qu’elle se termine le 18 avril et affectez-la à l’équipe créative.*

### Utiliser un workflow

Demandez à l’assistant d’IA de gérer le workflow. Par exemple :

* *Acheminer le projet « Q2 Innovation Sandbox » au Conseil d&#39;examen de l&#39;innovation.*
* *Mettre à jour l’enregistrement « Campagne d’été » vers le statut « Prêt pour le lancement »*
* *Valider l’enregistrement « Campagne d’été ».*


### Chaîner les requêtes à travers une conversation

Vous pouvez enchaîner les demandes dans une seule conversation. L’assistant d’IA conserve le contexte, de sorte que chaque requête peut s’appuyer sur la précédente. Par exemple :

1. Demandez à l’assistant d’IA de trouver un ensemble d’éléments : *Rechercher mes tâches en retard.*
1. Une fois que l’assistant d’IA a renvoyé la liste, demandez-lui d’agir sur les résultats : *Mettez-les tous à jour vers vendredi prochain*.

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considérations

Tenez compte des points suivants lorsque vous utilisez le serveur Workfront MCP.

### L’assistant d’IA peut utiliser des informations provenant de stades antérieurs de la conversation

Les assistants d’IA réutilisent parfois des données antérieures à une conversation au lieu de demander la dernière version de Workfront. Si quelque chose a changé dans Workfront depuis la dernière consultation de l’assistant d’IA, des informations obsolètes peuvent s’afficher.

Pour forcer l’assistant d’IA à récupérer des données récentes, demandez-les explicitement. Par exemple :

* *Obtenez les dernières données de Workfront. Ne pas utiliser les résultats mis en cache.*

### Le serveur MCP Workfront se met automatiquement à jour

Lorsqu’Adobe publie une nouvelle version du serveur MCP Workfront, votre assistant d’IA utilise automatiquement la nouvelle version. Vous n’avez pas besoin de vous reconnecter ou de changer quoi que ce soit de votre côté.

## Données et sécurité

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Quelles données quittent Workfront ?

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Gestion des données Workfront par les fournisseurs d’assistance d’IA

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Différences entre les assistants d’IA

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## Résolution des problèmes d’utilisation quotidiens

Pour plus d’informations sur les problèmes de configuration et d’authentification, voir [Dépannage de la configuration et de l’authentification](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) dans [Configuration du serveur MCP Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

| Problème | Cause probable | Corriger |
|---|---|---|
| L’assistant d’IA vous donne des informations obsolètes. | L’assistant d’IA réutilise les données d’un stade antérieur de la conversation. | Demandez à l’assistant d’IA de récupérer des données récentes à partir de Workfront. |
| L’assistant d’IA a renvoyé des données provenant d’éléments Workfront incorrects. | L’assistant d’IA a sélectionné les mauvais éléments en fonction d’une formulation ambiguë. | Demandez à nouveau avec des noms, des identifiants ou des filtres plus spécifiques. |
| Une mise à jour ou une suppression n’a pas pris effet dans Workfront. | L’assistant d’IA n’a pas encore appelé l’action ou vos autorisations ne l’autorisent pas. | Vérifiez auprès de l’assistant AI que l’action s’est exécutée, puis vérifiez vos autorisations Workfront. |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## Questions fréquentes

### Avec quels éléments Workfront puis-je travailler via un assistant d’IA ?

Tous les éléments auxquels vous avez accès dans Workfront via les niveaux d’accès et les autorisations d’objet.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Mes données Workfront sont-elles envoyées au fournisseur d’assistant d’IA ou stockées par celui-ci ?

Pour plus d’informations, voir [Données et sécurité](#data-and-security) dans cet article.

### Que se passe-t-il lorsqu’une nouvelle version du serveur MCP Workfront est publiée ?

Le serveur MCP se met automatiquement à jour. Vous n’avez pas besoin de vous reconnecter ni de modifier quoi que ce soit.

### Dois-je connaître l’API Workfront pour utiliser le serveur MCP Workfront ?

Non. L’assistant d’IA traduit vos requêtes en langage naturel en actions Workfront appropriées. Si vous connaissez déjà l’API Workfront, les actions vous sembleront familières, mais ce n’est pas obligatoire.
