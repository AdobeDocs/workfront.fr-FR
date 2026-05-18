---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configuration du serveur MCP Adobe Workfront
description: Configurez votre instance Workfront et votre assistant d’IA pour pouvoir travailler avec Workfront par le biais de conversations en langage naturel.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 5%

---


# Configuration du serveur MCP Adobe Workfront

Le serveur MCP [!DNL Adobe Workfront] vous permet de travailler avec vos données Workfront par le biais d’une conversation en langage naturel dans un assistant d’IA pris en charge, tel que Claude ou ChatGPT.

Avant de pouvoir connecter un assistant d’IA à Workfront, un administrateur Workfront doit activer l’accès au serveur MCP dans votre instance Workfront. Les étapes exactes pour connecter un assistant d’IA sont différentes pour chaque assistant d’IA pris en charge.

Pour plus d’informations sur le serveur Workfront MCP, consultez la section [Présentation du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Assistants IA pris en charge

Le serveur Workfront MCP prend actuellement en charge les assistants d’IA suivants :

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir connecter Workfront à un assistant d’IA, vous devez :

* disposer d’un compte [!DNL Adobe Workfront] actif avec l’autorisation d’accéder aux données que vous souhaitez utiliser ;
* Avoir accès à un assistant d’IA comme [!DNL Claude].

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### Conditions préalables d’administration

L’accès au serveur MCP est contrôlé par deux administrateurs distincts. Tous deux doivent activer l’accès avant de pouvoir se connecter.

* **Votre administrateur Workfront** doit activer l’accès au serveur MCP dans votre instance Workfront.

* Si vous utilisez une version d’entreprise d’un assistant AI, votre administrateur d’assistant AI doit activer le connecteur [!DNL Adobe Workfront] pour votre organisation.


## Connecter Workfront à Claude

Vous vous connectez à Workfront une fois par compte [!DNL Claude]. La connexion vous authentifie à une instance Workfront spécifique et vous restez connecté jusqu’à ce que vous choisissiez de vous déconnecter.


>[!IMPORTANT]
>
>Si vous utilisez [!DNL Claude] Enterprise, **votre administrateur [!DNL Claude] Enterprise** doit activer le connecteur [!DNL Adobe Workfront] pour votre organisation. Tant que ce n’est pas le cas, le connecteur [!DNL Adobe Workfront] n’apparaît pas lorsque vous le recherchez dans [!DNL Claude]. Contactez d’abord votre administrateur [!DNL Claude].


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

### Vérifier votre connexion

Pour confirmer [!DNL Claude] est connecté à Workfront, demandez aux [!DNL Claude] de répertorier les actions rendues disponibles par le serveur MCP Workfront. Par exemple :

* *Quelles actions Workfront pouvez-vous entreprendre ?*
* *Liste des outils Workfront auxquels vous avez accès.*

[!DNL Claude] renvoie la liste des actions disponibles.

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### Basculer vers une autre instance Workfront

Chaque connexion authentifie [!DNL Claude] à une seule instance Workfront. Pour utiliser une autre instance, déconnectez-vous et reconnectez-vous.

Pour vous connecter à une autre instance Workfront :

1. Dans [!DNL Claude], déconnectez le connecteur [!DNL Adobe Workfront].
1. Reconnectez le connecteur.
1. Authentifiez-vous sur la nouvelle instance Workfront.

>[!NOTE]
>
>La déconnexion de [!DNL Claude] seule ne change pas d’instance Workfront. Vous devez déconnecter et reconnecter le connecteur.

## Personnaliser le comportement de Claude avec des compétences

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude] prend en charge des jeux d’instructions créés par l’utilisateur appelés compétences. Vous pouvez utiliser une compétence pour personnaliser [!DNL Claude] comportement avec Workfront. Par exemple, vous pouvez créer une compétence qui [!DNL Claude] indique de toujours récupérer des données récentes à partir de Workfront au lieu de vous fier à des résultats antérieurs.

## Résolution des problèmes de configuration et d’authentification

| Problème | Cause probable | Corriger |
|---|---|---|
| Le connecteur [!DNL Adobe Workfront] est introuvable dans [!DNL Claude]. | Votre administrateur [!DNL Claude] ne l’a pas activée. | Contactez votre administrateur [!DNL Claude] (et non votre administrateur Workfront) et demandez-lui d’activer le connecteur [!DNL Adobe Workfront]. |
| Vous vous êtes connecté, mais vous ne pouvez pas voir vos données. | Vous vous êtes authentifié sur la mauvaise instance Workfront. | Déconnectez le connecteur, reconnectez-vous et authentifiez-vous sur l’instance appropriée. |
| L&#39;authentification a échoué ou la connexion a cessé de fonctionner. | Votre session d’authentification a expiré ou une erreur de connexion s’est produite. | Déconnectez-vous et reconnectez le connecteur. |
| Vous souhaitez passer à une autre instance Workfront. | Une seule connexion vous lie à une instance. | Déconnectez-vous, reconnectez-vous et authentifiez-vous sur la nouvelle instance. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Pour une résolution des problèmes au jour le jour après votre connexion (par exemple, résultats obsolètes ou comportement inattendu), reportez-vous à la section [&#x200B; Utiliser le serveur Adobe Workfront MCP &#x200B;](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).

## Questions fréquentes sur la configuration

### Puis-je me connecter à plusieurs instances Workfront à la fois ?

Non. Chaque connexion lie un assistant d’IA à une seule instance Workfront. Pour basculer, déconnecter et reconnecter, authentification à la nouvelle instance.

### Cela fonctionne-t-il avec Claude Pro ou Claude Team, ou uniquement avec Claude Enterprise ?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### Quel administrateur l’active ?

Votre administrateur Workfront et votre administrateur d’assistant d’IA. Votre administrateur Workfront active l’accès au serveur MCP côté Workfront. Votre administrateur d’assistant AI active l’accès à Workfront du côté de l’assistant AI. Par [!DNL Claude], l’administrateur d’[!DNL Claude] Enterprise active le connecteur [!DNL Adobe Workfront].
