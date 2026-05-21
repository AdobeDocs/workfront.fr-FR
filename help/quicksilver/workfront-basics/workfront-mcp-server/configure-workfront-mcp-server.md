---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configuration du serveur MCP Adobe Workfront
description: Configurez votre instance Workfront et votre plateforme d’IA agentic pour pouvoir travailler avec Workfront par le biais de conversations en langage naturel.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---


# Configuration du serveur MCP Adobe Workfront

Le serveur MCP [!DNL Adobe Workfront] vous permet de travailler avec vos données Workfront par le biais d’une conversation en langage naturel sur une plateforme agentique d’IA prise en charge, telle que Claude ou ChatGPT.

Avant de pouvoir connecter une plateforme agentique d’IA à Workfront, un administrateur Workfront doit activer l’accès au serveur MCP dans votre instance Workfront. Les étapes exactes pour connecter une plateforme IA agentic sont différentes pour chaque plateforme AI agentic prise en charge.

Pour plus d’informations sur le serveur Workfront MCP, consultez la section [Présentation du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Plateformes d’IA et d’ingénierie prises en charge

Le serveur Workfront MCP prend actuellement en charge les plateformes d’agents IA suivantes :

* [!DNL Claude]
* [!DNL ChatGPT]

## Conditions préalables

Avant de pouvoir connecter Workfront à une plateforme agentique d’IA, vous devez :

* disposer d’un compte [!DNL Adobe Workfront] actif avec l’autorisation d’accéder aux données que vous souhaitez utiliser ;
* Avoir accès à une plateforme agentic d’IA telle que [!DNL Claude].

### Conditions préalables d’administration

L’accès au serveur MCP est contrôlé par deux administrateurs distincts.

* **Votre administrateur Workfront** contrôle l’accès au serveur MCP pour votre instance Workfront. L’accès est activé par défaut dans les Préférences système. Aucune action n’est donc requise, sauf si votre administrateur a choisi de le désactiver. <!-- TODO: link to the System Preferences AI preferences article once the Enable MCP toggle is documented there. -->

* Si vous utilisez une version d’entreprise d’une plateforme AI agentic, l’administrateur de cette plateforme doit activer le connecteur [!DNL Adobe Workfront] pour votre organisation.


## Connecter Workfront à Claude

Vous vous connectez à Workfront une fois par compte [!DNL Claude]. La connexion vous authentifie à une instance Workfront spécifique et vous restez connecté jusqu’à ce que vous choisissiez de vous déconnecter.

### Connexion à partir du répertoire des connecteurs

+++ Développez pour afficher les instructions détaillées relatives à la connexion de Workfront à [!DNL Claude].

Pour connecter Workfront à [!DNL Claude] :

1. Ouvrez [!DNL Claude].

1. Accédez à la zone des connecteurs.

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. Recherchez **[!DNL Adobe Workfront]** dans la liste des connecteurs.

   Si vous ne le voyez pas, reportez-vous à la section [Conditions préalables d’administration](#admin-prerequisites) de cet article.

1. Cliquez sur **Connecter**.

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. Lorsque vous y êtes invité, connectez-vous à votre instance Workfront.

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. Une fois l’authentification terminée, vous êtes connecté.

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

+++

### Se connecter avec une URL

+++ Développez pour afficher les instructions détaillées permettant de connecter Workfront à [!DNL Claude] avec une URL.

Pour connecter Workfront à [!DNL Claude] avec une URL :

1. Connectez-vous à [Claude](https://claude.ai) à l’aide de vos informations d’identification.
1. Dans le menu de gauche, sélectionnez l’icône **Personnaliser**.
1. Sélectionnez **Connecteurs**, puis sélectionnez l’icône **+** pour ajouter un connecteur.
1. Sélectionnez le bouton **Créer une application**.
1. Attribuez au connecteur le nom souhaité (par exemple, « Workfront ») et saisissez l’URL de serveur MCP souhaitée : `https://mcp.workfront.adobe.com/mcp/v1/workfront`

1. Une fois le connecteur créé, une fenêtre de connexion s’affiche. Authentifiez-vous à l’aide de vos informations d’identification Adobe ID. Veillez à sélectionner l’instance Workfront souhaitée si vous appartenez à plusieurs instances.

+++

### Personnaliser le comportement de Claude avec des compétences

[!DNL Claude] prend en charge des jeux d’instructions créés par l’utilisateur appelés compétences. Vous pouvez utiliser une compétence pour personnaliser [!DNL Claude] comportement avec Workfront. Par exemple, vous pouvez créer une compétence qui [!DNL Claude] indique de toujours récupérer des données récentes à partir de Workfront au lieu de vous fier à des résultats antérieurs.

Pour en savoir plus sur les compétences [!DNL Claude], consultez la documentation utilisateur [Claude](https://code.claude.com/docs/en/skills) ou demandez de l’aide à Claude au sujet des compétences.

## Se connecter à ChatGPT

1. Connectez-vous à [ChatGPT](https://chatgpt.com) à l’aide de vos informations d’identification.
1. Dans le coin inférieur gauche, sélectionnez **votre nom** → **Paramètres**.
1. Sélectionnez **Applications**, puis activez **mode Développeur**.
1. Sélectionnez le bouton **Créer une application**.
1. Attribuez à l’application le nom souhaité (par exemple, « Workfront ») et saisissez l’URL du serveur MCP souhaité : `https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. Assurez-vous que l’authentification est définie sur **OAuth** (défini par défaut), puis cochez la case d’acceptation pour continuer.
1. Une fois l’application créée, une fenêtre de connexion s’affiche. Authentifiez-vous à l’aide de vos informations d’identification Adobe ID. Veillez à sélectionner l’instance Workfront souhaitée si vous appartenez à plusieurs instances.

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
>La déconnexion seule ne change pas d’instance Workfront. Vous devez déconnecter et reconnecter le connecteur.

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
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
|---|---|---|
| Le connecteur [!DNL Adobe Workfront] est introuvable dans [!DNL Claude]. | Votre administrateur [!DNL Claude] ne l’a pas activée. | Contactez votre administrateur [!DNL Claude] (et non votre administrateur Workfront) et demandez-lui d’activer le connecteur [!DNL Adobe Workfront]. |
| Vous vous êtes connecté, mais vous ne pouvez pas voir vos données. | Vous vous êtes authentifié sur la mauvaise instance Workfront. | Déconnectez le connecteur, reconnectez-vous et authentifiez-vous sur l’instance appropriée. |
| L&#39;authentification a échoué ou la connexion a cessé de fonctionner. | Votre session d’authentification a expiré ou une erreur de connexion s’est produite. | Déconnectez-vous et reconnectez le connecteur. |
| Vous souhaitez passer à une autre instance Workfront. | Une seule connexion vous lie à une instance. | Déconnectez-vous, reconnectez-vous et authentifiez-vous sur la nouvelle instance. |
| Vous ne pouvez pas vous connecter à Workfront, ou un message indiquant que l’accès au serveur MCP est désactivé s’affiche. | Votre administrateur Workfront a désactivé l’accès au serveur MCP pour votre instance. | Contactez votre administrateur Workfront et demandez-lui d’activer l’accès au serveur MCP dans les Préférences système. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Pour une résolution des problèmes au jour le jour après votre connexion (par exemple, résultats obsolètes ou comportement inattendu), reportez-vous à la section [&#x200B; Utiliser le serveur Adobe Workfront MCP &#x200B;](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++


<!--
+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++

-->