---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configuration du serveur MCP Adobe Workfront
description: Configurez votre instance Workfront et votre plateforme d’IA agentic pour pouvoir travailler avec Workfront par le biais de conversations en langage naturel.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 0445376ea187b589040c8fdc56ea0d11f44b0b37
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---


# Configuration du serveur MCP Adobe Workfront

Le serveur MCP [!DNL Adobe Workfront] vous permet d’utiliser vos données Workfront par le biais d’une conversation en langage naturel sur une plateforme agentique d’IA prise en charge.

Avant de pouvoir connecter une plateforme agentique d’IA à Workfront, un administrateur Workfront doit activer l’accès au serveur MCP dans votre instance Workfront. Les étapes exactes pour connecter une plateforme IA agentic sont différentes pour chaque plateforme AI agentic prise en charge.

>[!IMPORTANT]
>
>Actuellement, le serveur Workfront MCP est disponible uniquement pour les clients qui utilisent AWS. Les clients qui utilisent GCP ou Azure pourront utiliser cette fonctionnalité dans un avenir proche.

## Plateformes d’IA et d’ingénierie prises en charge

Le serveur MCP Workfront fonctionne avec toute plateforme agentique d’IA prenant en charge le protocole MCP (Model Context Protocol).

Cet article décrit les étapes de connexion pour :

* [!DNL Claude]
* [!DNL ChatGPT]

Si vous utilisez une autre plateforme d’IA agentic compatible avec les MCP (par exemple, [!DNL Gemini] ou [!DNL Microsoft Copilot]), suivez les étapes de la documentation de cette plateforme pour ajouter un serveur MCP personnalisé. Lorsque vous êtes invité à saisir l’URL du serveur MCP, saisissez l’URL de votre région :

| Région | URL |
| --- | --- |
| US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
| UE | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

## Conditions préalables

Avant de pouvoir connecter Workfront à une plateforme agentique d’IA, vous devez :

* disposer d’un compte [!DNL Adobe Workfront] actif autorisé à accéder aux données que vous souhaitez utiliser ;
* Avoir accès à une plateforme agentic d’IA telle que [!DNL Claude]
* Votre instance Workfront doit être activée sur le système Adobe Identity Management (IMS).
* Pour utiliser MCP avec Workfront Planning, votre entreprise doit disposer d’un package Workfront incluant Adobe Workfront Planning.


### Conditions préalables d’administration

L’accès au serveur MCP est contrôlé par deux administrateurs distincts.

* Votre administrateur Workfront contrôle l’accès au serveur MCP pour votre instance Workfront par le biais de deux boutons (bascule) dans les Préférences système : **Outils MCP en lecture seule** (activé par défaut) et **Outils MCP en écriture** (désactivé par défaut). Si vous trouvez des éléments Workfront via la plateforme agentic d’IA, mais que vous ne pouvez pas les créer, les mettre à jour ou les supprimer, demandez à votre administrateur Workfront d’activer les actions d’écriture.

  Pour plus d’informations, voir [Configuration des préférences système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* Si vous utilisez une version d’entreprise d’une plateforme AI agentic, l’administrateur de cette plateforme doit activer le connecteur [!DNL Adobe Workfront] pour votre organisation ou vous donner un accès URL personnalisé pour vous connecter au serveur MCP Workfront.


## Connecter Workfront à Claude

Vous vous connectez à Workfront une fois par compte [!DNL Claude]. La connexion vous authentifie à une instance Workfront spécifique et vous restez connecté jusqu’à ce que vous choisissiez de vous déconnecter.



### Connectez-vous au bureau Claude à partir du répertoire des connecteurs

>[!IMPORTANT]
>
>Actuellement, le connecteur Claude ne prend en charge que la connexion au serveur MCP Workfront dans la région des États-Unis.  Pour vous connecter à une instance Workfront dans la région UE, consultez la section [Se connecter au bureau Claude avec une URL](#connect-to-claude-desktop-with-a-url) dans cet article.

+++ Développez pour afficher les instructions détaillées relatives à la connexion de Workfront à [!DNL Claude].

Pour connecter Workfront à [!DNL Claude] :

1. Ouvrez [!DNL Claude].

1. Accédez à la zone des connecteurs.



1. Recherchez **[!DNL Adobe Workfront]** dans la liste des connecteurs.

   Si vous ne le voyez pas, reportez-vous à la section [Conditions préalables d’administration](#admin-prerequisites) de cet article.

1. Cliquez sur **Connecter**.



1. Lorsque vous y êtes invité, connectez-vous à votre instance Workfront.


1. Une fois l’authentification terminée, vous êtes connecté.



+++

### Se connecter à Claude avec une URL

+++ Développez pour afficher les instructions détaillées permettant de connecter Workfront à [!DNL Claude] avec une URL.

>[!NOTE]
>
>Pour effectuer cette procédure, vous devez être propriétaire dans un environnement Claude d’entreprise.
>
>Pour l’instruction de Claude sur l’exigence du propriétaire, voir [ Ajouter un connecteur personnalisé ](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp#:~:text=Note%3A%20While,has%20access%20to) dans la documentation Claude.

Pour connecter Workfront à [!DNL Claude] avec une URL :

1. Connectez-vous à [Claude](https://claude.ai) à l’aide de vos informations d’identification.
1. Dans le menu de gauche, sélectionnez l’icône **Personnaliser**.
1. Sélectionnez **Connecteurs**, puis sélectionnez l’icône **+** pour ajouter un connecteur.
1. Sélectionnez le bouton **Créer une application**.
1. Attribuez au connecteur le nom souhaité (par exemple, « Workfront ») et saisissez l’URL du serveur MCP souhaitée :

   | Région | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | UE | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. Une fois le connecteur créé, une fenêtre de connexion s’affiche. Authentifiez-vous à l’aide de vos informations d’identification Adobe ID. Veillez à sélectionner l’instance Workfront souhaitée si vous appartenez à plusieurs instances.

   >[!NOTE]
   >
   >Votre instance Workfront doit se connecter au serveur MCP correspondant à la région pour cette instance. Par exemple, une instance UE doit se connecter au serveur MCP UE.
   >
   >Lors de la sélection d’une instance, les instances qui ne sont pas compatibles avec la région du serveur MCP apparaissent grisées et vous ne pouvez pas vous y connecter.
   >
   >Pour vous connecter à une instance qui n’est pas compatible avec la région du serveur MCP, configurez une nouvelle connexion MCP avec l’URL appropriée pour cette région.

+++

### Personnaliser le comportement de Claude avec des compétences

[!DNL Claude] prend en charge des jeux d’instructions créés par l’utilisateur appelés compétences. Vous pouvez utiliser une compétence pour personnaliser [!DNL Claude] comportement avec Workfront. Par exemple, vous pouvez créer une compétence qui [!DNL Claude] indique de toujours récupérer des données récentes à partir de Workfront au lieu de vous fier à des résultats antérieurs.

Pour en savoir plus sur les compétences [!DNL Claude], consultez la documentation utilisateur [Claude](https://code.claude.com/docs/en/skills) ou demandez de l’aide à Claude au sujet des compétences.

## Se connecter à ChatGPT

1. Connectez-vous à [ChatGPT](https://chatgpt.com) à l’aide de vos informations d’identification.
1. Dans le coin inférieur gauche, sélectionnez **votre nom** → **Paramètres**.
1. Sélectionnez **Applications**, puis activez **mode Développeur**.
1. Sélectionnez le bouton **Créer une application**.
1. Attribuez à l’application le nom souhaité (par exemple, « Workfront ») et saisissez l’URL du serveur MCP souhaité :

   | Région | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | UE | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. Assurez-vous que l’authentification est définie sur **OAuth** (défini par défaut), puis cochez la case d’acceptation pour continuer.
1. Une fois l’application créée, une fenêtre de connexion s’affiche. Authentifiez-vous à l’aide de vos informations d’identification Adobe ID. Veillez à sélectionner l’instance Workfront souhaitée si vous appartenez à plusieurs instances.

   >[!NOTE]
   >
   >Votre instance Workfront doit se connecter au serveur MCP correspondant à la région pour cette instance. Par exemple, une instance UE doit se connecter au serveur MCP UE.
   >
   >Lors de la sélection d’une instance, les instances qui ne sont pas compatibles avec la région du serveur MCP apparaissent grisées et vous ne pouvez pas vous y connecter.
   >
   >Pour vous connecter à une instance qui n’est pas compatible avec la région du serveur MCP, configurez une nouvelle connexion MCP avec l’URL appropriée pour cette région.


### Personnaliser le comportement de ChatGPT avec les TPG personnalisés

ChatGPT prend en charge les assistants créés par l’utilisateur, appelés GPT personnalisés. Vous pouvez utiliser un GPT personnalisé pour personnaliser le comportement de ChatGPT avec votre connecteur. Par exemple, vous pouvez créer un GPT personnalisé qui indique à ChatGPT de toujours récupérer les nouvelles données de votre service connecté au lieu de s’appuyer sur des résultats antérieurs.

Pour en savoir plus sur les TPG personnalisés, consultez la documentation utilisateur de [ChatGPT](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) ou demandez de l’aide à ChatGPT sur les TPG personnalisés.

## Vérifier votre connexion

Pour confirmer que la plateforme IA agentic est connectée à Workfront, demandez à la plateforme AI agentic de répertorier les actions que le serveur MCP Workfront rend disponibles. Par exemple :

* *Quelles actions Workfront pouvez-vous entreprendre ?*
* *Liste des outils Workfront auxquels vous avez accès.*

Vous pouvez également consulter la liste complète des outils dans [Outils de serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Outils disponibles

Le serveur Workfront MCP expose un ensemble d’outils que la plateforme agentic d’IA connectée appelle en votre nom, par exemple, des outils pour rechercher des Workfront, créer des éléments, mettre à jour des champs et gérer les approbations. Pour obtenir la liste de référence complète, regroupée par zone de Workfront, consultez [Outils de serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Basculer vers une autre instance Workfront

Chaque connexion authentifie la plateforme agentic d’IA sur une seule instance Workfront. Pour utiliser une autre instance, déconnectez-vous et reconnectez-vous.

Pour vous connecter à une autre instance Workfront :

1. Dans la plateforme agentic d’IA, déconnectez le serveur MCP de Workfront.
1. Reconnectez le connecteur.
1. Authentifiez-vous sur la nouvelle instance Workfront.

>[!NOTE]
>
>* La déconnexion seule ne change pas d’instance Workfront. Vous devez déconnecter et reconnecter le connecteur.
>
>* Votre instance Workfront doit se connecter au serveur MCP correspondant à la région pour cette instance. Par exemple, une instance UE doit se connecter au serveur MCP UE.
>
>   Lors de la sélection d’une instance, les instances qui ne sont pas compatibles avec la région du serveur MCP apparaissent grisées et vous ne pouvez pas vous y connecter.
>
>   Pour vous connecter à une instance qui n’est pas compatible avec la région du serveur MCP, configurez une nouvelle connexion MCP avec l’URL appropriée pour cette région.


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |
   
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## Résolution des problèmes de configuration et d’authentification

+++ Développez pour afficher les conseils de dépannage pour la configuration et l’authentification du serveur Workfront MCP.

| Problème | Cause probable | Corriger |
| --- | --- | --- |
| Le connecteur [!DNL Adobe Workfront] est introuvable dans [!DNL Claude]. | Votre administrateur [!DNL Claude] ne l’a pas activée. | Contactez votre administrateur [!DNL Claude] (et non votre administrateur Workfront) et demandez-lui d’activer le connecteur [!DNL Adobe Workfront]. |
| Vous vous êtes connecté, mais vous ne pouvez pas voir vos données. | Vous vous êtes authentifié sur la mauvaise instance Workfront. | Déconnectez le connecteur, reconnectez-vous et authentifiez-vous sur l’instance appropriée. |
| L&#39;authentification a échoué ou la connexion a cessé de fonctionner. | Votre session d’authentification a expiré ou une erreur de connexion s’est produite. | Déconnectez-vous et reconnectez le connecteur. |
| Vous souhaitez passer à une autre instance Workfront. | Une seule connexion vous lie à une instance. | Déconnectez-vous, reconnectez-vous et authentifiez-vous sur la nouvelle instance. |
| Vous ne pouvez pas vous connecter à Workfront, ou un message indiquant que l’accès au serveur MCP est désactivé s’affiche. | Votre administrateur Workfront a désactivé l’accès au serveur MCP pour votre instance. | Contactez votre administrateur Workfront et demandez-lui d’activer l’accès au serveur MCP dans les Préférences système. |
| L’instance Workfront à laquelle vous souhaitez vous connecter est grisée et un message vous indique qu’elle n’est pas disponible pour vous connecter dans votre région | Votre serveur MCP est configuré pour une région différente (UE ou États-Unis) de votre instance. | Configurez le serveur MCP avec l’URL de la région à laquelle votre instance Workfront est affectée. |
| La plateforme agentic d’IA peut rechercher vos éléments Workfront, mais ne peut pas les créer, les mettre à jour ni les supprimer. | Votre administrateur Workfront a désactivé les actions d’écriture pour le serveur MCP Workfront. | Contactez votre administrateur Workfront et demandez-lui d’activer les actions d’écriture dans les Préférences système. |

Pour une résolution des problèmes au jour le jour après votre connexion (par exemple, résultats obsolètes ou comportement inattendu), reportez-vous à la section [ Utiliser le serveur Adobe Workfront MCP ](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++

## Questions fréquentes sur la configuration

+++ Développez pour afficher les questions fréquentes sur la configuration du serveur Workfront MCP.

### Puis-je me connecter à plusieurs instances Workfront en même temps ?

Non. Chaque connexion lie une plateforme agentique d’IA à une seule instance Workfront. Pour basculer, déconnecter et reconnecter, authentification à la nouvelle instance.

### Quel administrateur l’active ?

Votre administrateur Workfront et l’administrateur de votre plateforme AI agentic. Votre administrateur Workfront active l’accès au serveur MCP côté Workfront. L’administrateur de votre plateforme d’IA agentic active l’accès à Workfront du côté de cette plateforme. Par [!DNL Claude], l’administrateur d’[!DNL Claude] Enterprise active le connecteur [!DNL Adobe Workfront].

### Puis-je utiliser le serveur MCP Workfront si mon instance Workfront n’est pas activée sur le système Adobe Identity Management (IMS) ?

Non. Votre instance Workfront doit être activée sur Adobe Identity Management System (IMS) pour utiliser le serveur MCP Workfront. Si vous ne savez pas si votre instance est activée sur IMS, contactez votre administrateur Workfront.

+++ 
