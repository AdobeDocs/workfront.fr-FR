---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Utiliser le serveur MCP Adobe Workfront
description: Utilisez le serveur Adobe Workfront MCP pour rechercher, créer, mettre à jour et gérer des éléments Workfront par le biais d’une conversation en langage naturel dans une plateforme agentique d’IA.
author: Courtney
feature: Get Started with Workfront
source-git-commit: e009d9d52ddb478759c11a20967d48049f797d97
workflow-type: tm+mt
source-wordcount: '1875'
ht-degree: 0%

---


# Utiliser le serveur MCP Adobe Workfront

Le serveur MCP [!DNL Adobe Workfront] vous permet de rechercher, créer, mettre à jour et gérer des éléments Workfront en demandant à une plateforme agentique d’IA de vous fournir des informations en langage naturel. La plateforme décide des actions Workfront à appeler et gère la conversation avec Workfront pour vous.

>[!IMPORTANT]
>
>Actuellement, le serveur Workfront MCP est disponible uniquement pour les clients qui utilisent AWS.

## Conditions préalables

* Vous devez configurer la connexion entre votre plateforme IA agentic et le serveur Workfront MCP. Pour obtenir des instructions de configuration, voir [Configuration du serveur MCP Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).
* Votre instance Workfront doit être activée sur le système Adobe Identity Management (IMS).
* Vous devez disposer d’un compte Workfront avec le niveau d’accès et les autorisations d’objet nécessaires pour les éléments que vous souhaitez utiliser.
* Pour utiliser MCP avec Workfront Planning, votre entreprise doit disposer d’un package Workfront incluant Adobe Workfront Planning.

Cet article suppose que vous avez déjà configuré la connexion. Pour plus d’informations sur la configuration, voir [Configuration du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Outils disponibles

Le serveur MCP Workfront expose un ensemble d’outils que la plateforme agentic d’IA appelle en votre nom. Par exemple, les outils permettant de rechercher Workfront, de créer des éléments, de mettre à jour des champs et de gérer les approbations. Pour obtenir la liste de référence complète, voir [Outils de serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Lorsque vous connectez une plateforme IA agentic à Workfront, celle-ci agit dans Workfront à l’aide de votre compte et de vos autorisations Workfront. Les actions de la plateforme ont le même effet que les actions que vous effectuez directement dans l’interface de Workfront.<br>
>
>Vous et votre fournisseur de plateforme agentic d’IA êtes responsables des actions de la plateforme dans Workfront. Adobe n’est pas responsable des modifications apportées par la plateforme AI agentic à vos données Workfront.<br>
>
>Avant de laisser la plateforme agentique d’IA traiter une demande, vérifiez que vous comprenez ce qu’elle a l’intention de faire, en particulier pour les actions qui modifient ou suppriment des données.


## Exemples de questions

Une fois la connexion établie, saisissez les requêtes en langage naturel dans votre plateforme agentique d’IA. La plateforme agentic d’IA décide des actions Workfront à appeler et renvoie les résultats.

>[!NOTE]
>
>Certaines actions peuvent ne pas être disponibles en raison des commandes d’administration dans la zone Configuration de Workfront . Par exemple, vous ne pourrez peut-être pas créer d’éléments si votre administrateur Workfront a désactivé les actions d’écriture pour le serveur MCP.


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

<!--
* *Remove Anna Jones from all approvals in this project, and replace with Sione Carter.*
-->


### Utiliser les enregistrements Planning

>[!IMPORTANT]
>
>* Pour utiliser MCP avec Workfront Planning, votre entreprise doit disposer d’un package Workfront incluant Adobe Workfront Planning.

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


## Considérations

Lorsque vous utilisez le serveur Workfront MCP, tenez compte des points suivants :

### La plateforme agentique d’IA peut utiliser des informations provenant de stades antérieurs de la conversation

Les plateformes d’intelligence artificielle réutilisent parfois des données antérieures à une conversation au lieu de demander la dernière version à Workfront. Si quelque chose a changé dans Workfront depuis la dernière consultation de la plateforme agentic d’IA, des informations obsolètes risquent de s’afficher.

Pour forcer la plateforme agentique d’IA à récupérer des données récentes, demandez-les explicitement. Par exemple :

* *Obtenez les dernières données de Workfront. Ne pas utiliser les résultats mis en cache.*

### Rechercher les mises à jour du serveur MCP Workfront

Vous pouvez actualiser régulièrement votre connexion au serveur MCP Workfront pour vous assurer que vous disposez des outils et fonctionnalités les plus récents.

La plupart des mises à jour doivent se produire automatiquement. Nous vous recommandons toutefois de consulter régulièrement les notes de mise à jour de Workfront.


## Données et sécurité

Les outils de serveur MCP Workfront sont cohérents avec le fonctionnement des appels API. Workfront ne stocke pas d’invites, de réponses ni d’autres données. Toutes les données Workfront que vous demandez sont accessibles dans la plateforme Workfront.

Votre niveau d’accès et vos autorisations d’objet déterminent ce que vous pouvez demander ou écrire dans Workfront. Votre administrateur Workfront contrôle les actions de lecture et d’écriture MCP dans la zone Configuration de Workfront .

### Quelles données quittent Workfront ?

Le fournisseur de plateforme agentic AI a accès aux données Workfront avec lesquelles vous interagissez par le biais du serveur MCP Workfront. Consultez votre fournisseur de plateformes d’IA agentic pour plus d’informations.


### Comment les fournisseurs de plateformes d’intelligence artificielle gèrent vos données Workfront

Workfront n’a pas de contrôle sur la manière dont le fournisseur de plateforme AI agentic gère vos données Workfront. Consultez votre fournisseur de plateformes d’IA agentic pour plus d’informations.

## Résolution des problèmes d’utilisation quotidiens

+++ Développez pour afficher les conseils de dépannage pour une utilisation quotidienne du serveur Workfront MCP.

| Problème | Cause probable | Corriger |
| --- | --- | --- |
| La plateforme IA agentic vous donne des informations dépassées. | La plateforme agentique d’IA réutilise les données des étapes précédentes de la conversation. | Demandez de nouvelles données à Workfront. |
| La plateforme agentic d’IA a renvoyé des données provenant d’éléments Workfront incorrects. | La plateforme de l&#39;IA agentic a choisi les mauvais éléments en fonction d&#39;une formulation ambiguë. | Demandez à nouveau avec des noms, des identifiants ou des filtres plus spécifiques. |
| Une mise à jour ou une suppression n’a pas pris effet dans Workfront. | Votre administrateur Workfront a désactivé les actions d’écriture pour le serveur MCP Workfront ou vous n’êtes pas autorisé à effectuer l’action sur l’élément spécifique. | Confirmez auprès de la plateforme d’agence IA que l’action a exécutée. Vérifiez ensuite que les actions d’écriture sont activées pour le serveur MCP Workfront et que vous êtes autorisé à modifier l’élément. |

Pour plus d’informations sur les problèmes de configuration et d’authentification, voir [Dépannage de la configuration et de l’authentification](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) dans [Configuration du serveur MCP Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Questions fréquentes

+++ Développez pour afficher les questions fréquentes sur l’utilisation du serveur Workfront MCP.

### Qu’est-ce qu’une plateforme agentique d’IA ?

Une plateforme agentique d’IA est un outil d’IA qui peut agir en votre nom dans
d&#39;autres systèmes, pas seulement de répondre aux questions. Lorsque vous en connectez un à Workfront
par le biais du serveur MCP, il peut rechercher, créer, mettre à jour et supprimer Workfront
éléments basés sur ce que vous lui demandez en langage naturel. Claude en est un exemple
Ordinateur de bureau, ChatGPT et autres clients d’IA compatibles avec MCP.


### Dois-je être un administrateur Workfront pour utiliser le serveur MCP Workfront ?

Non. Tout utilisateur de Workfront peut utiliser le serveur MCP de Workfront via un
Plateforme agentique d’IA. La plateforme IA agentic agit à l’aide de votre Workfront
le compte, le niveau d’accès et les autorisations d’objet, afin que vous puissiez uniquement faire ce que vous
pourrait déjà le faire directement dans Workfront.

### Pourquoi la plateforme IA AEM ne peut-elle pas créer, mettre à jour ou supprimer des éléments pour moi ?

Votre administrateur Workfront contrôle les actions MCP autorisées dans le
Zone Configuration de Workfront. Si les actions d’écriture sont désactivées, la plateforme agentique d’IA
peut toujours rechercher et lire les éléments Workfront, mais ne peut pas apporter de modifications. Vous pouvez également
vous avez besoin du niveau d’accès et des autorisations d’objet appropriés pour les éléments spécifiques
vous travaillez avec.

### La plateforme agentic d’IA me demandera-t-elle des informations avant de modifier ou de supprimer des données Workfront ?

Cela dépend de la plateforme agentic de l&#39;IA, pas de Workfront. La plupart des plateformes
vous invite à confirmer avant l’exécution d’une action, en particulier pour les suppressions.
Avant d’approuver une demande, lisez ce que la plateforme indique qu’elle est sur le point de faire -
les modifications se produisent dans Workfront comme si vous les aviez effectuées
vous-même dans l’interface.

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### Pourquoi la plateforme agentic d’IA a-t-elle renvoyé les mauvais éléments Workfront ?

La plateforme IA agentic sélectionne les éléments en fonction des mots que vous avez utilisés. Si votre
la demande est ambiguë (par exemple, deux projets portent des noms similaires), elle
Je pourrais choisir le mauvais. Demandez à nouveau avec des noms, des identifiants, des dates plus précis.
ou des filtres pour limiter les résultats.


### Avec quels éléments Workfront puis-je travailler via une plateforme agentique d’IA ?

Tous les éléments auxquels vous avez accès dans Workfront via votre niveau d’accès et
autorisations d’objet. Cela inclut les projets, tâches, événements, documents,
les approbations, les enregistrements Planning, etc.

### D’autres personnes peuvent-elles voir mes conversations avec la plateforme IA agentic ?

Workfront ne stocke pas vos invites ni les réponses de la plateforme agentic d&#39;IA.
La personne qui fournit votre plateforme agentique d’IA contrôle la manière dont vos conversations
sont stockées ou partagées. Vérifiez auprès de votre fournisseur de plateforme IA agentic pour connaître
détails.

### Dois-je connaître l’API Workfront ou l’outil MCP à utiliser ?

Non. La plateforme agentic d’IA traduit votre requête en langage naturel en
les bonnes actions Workfront et les bons outils pour vous. Si vous
vous connaissez déjà l’API Workfront, les actions vous sembleront familières,
mais ce n&#39;est pas une exigence.

### Mes données Workfront sont-elles envoyées au fournisseur de plateformes d’agence IA ou stockées par celui-ci ?

Pour plus d’informations, voir [Données et sécurité](#data-and-security) dans cette
article.

### Que se passe-t-il lorsqu’une nouvelle version du serveur MCP Workfront est publiée ?

Le serveur MCP se met généralement à jour automatiquement, mais vous devrez peut-être actualiser votre connexion au serveur MCP à certains moments pour voir les outils et fonctionnalités les plus récents.

### Puis-je utiliser le serveur MCP Workfront si mon instance Workfront n’est pas activée sur le système Adobe Identity Management (IMS) ?

Non. Votre instance Workfront doit être activée sur Adobe Identity Management System (IMS) pour utiliser le serveur MCP Workfront. Si vous ne savez pas si votre instance est activée sur IMS, contactez votre administrateur Workfront.


+++
