---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Méthodes d’intégration d’Adobe Workfront
description: Vous pouvez intégrer  [!DNL Adobe Workfront]  à des applications tierces. Ces intégrations peuvent étendre l’utilitaire de  [!DNL Workfront] et l’adapter aux besoins de votre entreprise. Vous pouvez utiliser l’une ou l’autre de ces intégrations, selon celle qui est la plus utile pour une tâche donnée.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 1%

---

# Méthodes d’intégration d’Adobe Workfront

Vous pouvez intégrer [!DNL Adobe Workfront] à des applications tierces, ainsi qu’à d’autres produits [!DNL Adobe]. Ces intégrations peuvent étendre l’utilitaire de [!DNL Workfront] et l’adapter aux besoins de votre entreprise. Vous pouvez utiliser l’une ou l’autre de ces intégrations, selon celle qui est la plus utile pour une tâche donnée.

## Intégrations intégrées

Workfront fournit diverses intégrations que vous pouvez configurer directement à partir de Workfront ou d’une autre application en installant le module complémentaire Workfront pour cette application. Ces intégrations intégrées couvrent de nombreux scénarios d’utilisation courants et se concentrent sur l’extension et la connexion des expériences utilisateur pour les utilisateurs finaux.

Les intégrations intégrées de Workfront se concentrent principalement sur la productivité et la collaboration personnelles. Ces intégrations réduisent les interruptions dans le workflow d’un utilisateur individuel, ce qui lui permet de recevoir des notifications Workfront, d’accéder aux informations et d’agir sur les tâches de Workfront sans quitter l’application intégrée.

Les avantages des intégrations intégrées peuvent inclure les avantages suivants :

* La plupart de ces intégrations intégrées sont disponibles sans frais supplémentaires. (Les autres nécessitent un achat supplémentaire.)
* Les intégrations intégrées couvrent la plupart des applications les plus courantes utilisées par les entreprises, telles que les produits [!DNL Slack], [!DNL Google Drive] ou [!DNL Adobe] tels que [!DNL Adobe Creative Cloud] ou [!DNL Adobe Experience Manager] Assets. Si votre entreprise utilise déjà ces applications, l’intégration s’effectuera sans problème dans le workflow existant de vos utilisateurs.
* L’intégration de [!DNL Workfront] à une application fréquemment utilisée peut augmenter l’adoption de vos utilisateurs.

>[!INFO]
>
>**Exemple :**
>
>Avec [!DNL Workfront for Microsoft Teams integration], vous pouvez recevoir des notifications dans [!DNL Microsoft Teams] sur vos tâches [!DNL Workfront]. Sans quitter [!DNL Microsoft Teams], vous pouvez effectuer des actions comme approuver, commenter ou modifier l’état des tâches. Toutes les modifications que vous apportez aux tâches de [!DNL Microsoft Teams] sont également répercutées dans [!DNL Workfront].

Pour plus d’informations sur les intégrations natives, y compris une liste des intégrations natives actuellement disponibles, consultez la [[!DNL Adobe Workfront] présentation des intégrations natives](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Applications OAuth2 personnalisées

Les administrateurs d&#39;Adobe [!DNL Workfront] peuvent créer des applications OAuth2 pour votre instance de [!DNL Workfront], ce qui permet à d&#39;autres applications d&#39;accéder à [!DNL Workfront]. Vos utilisateurs peuvent alors autoriser ces autres applications à accéder à leurs données [!DNL Workfront]. Ainsi, vous pouvez intégrer Workfront aux applications de votre choix, y compris vos propres applications internes.

>[!NOTE]
>
>Dans le contexte d’OAuth2, &quot;création d’une application&quot; fait référence au processus de création de ce type de lien d’accès entre une application et un serveur tel que Workfront.

La création d’une application [!UICONTROL OAuth2] offre les avantages suivants :

* Les utilisateurs peuvent utiliser ces intégrations directement dans [!DNL Workfront], comme les intégrations intégrées.
* La configuration ou l’utilisation d’une application [!UICONTROL OAuth2] ne nécessite aucune connaissance technique supplémentaire, telle que la connaissance de l’API [!DNL Workfront].
* Votre entreprise peut utiliser un logiciel qui n’est pas proposé en tant qu’application [!DNL Workfront] intégrée. Vous pouvez toujours intégrer ce logiciel à [!DNL Workfront] en utilisant une application [!UICONTROL OAuth2], même si le logiciel appartient à votre entreprise.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## API [!DNL Workfront]

[!DNL Workfront] offre une API publique (interface de programmation d’application) qui vous permet d’étendre et d’améliorer votre expérience Workfront. L’objectif de l’API [!DNL Workfront] est de simplifier la création de vos propres intégrations avec [!DNL Workfront] en introduisant une architecture REST-ful qui fonctionne sur HTTP. L’API [!DNL Workfront] nécessite des connaissances techniques, mais il s’agit d’un outil très puissant pour récupérer, créer et modifier des données. Vous pouvez personnaliser les appels d’API pour exécuter des fonctions très spécifiques.

[!DNL Workfront] propose en outre une API d’abonnement à un événement. Lorsqu’une action se produit sur un objet [!DNL Workfront] pris en charge par les abonnements aux événements, vous pouvez configurer [!DNL Workfront] pour envoyer une réponse au point de terminaison souhaité. Cela signifie que les applications tierces peuvent recevoir des mises à jour provenant d’interactions [!DNL Workfront] via l’API [!DNL Workfront] peu de temps après leur apparition.

L’utilisation de l’API [!DNL Workfront] peut présenter les avantages suivants :

* Vous pouvez utiliser l’API [!DNL Workfront] pour vous connecter à presque tout autre service Web ou application qui offre une API publique. Il est donc possible d&#39;intégrer [!DNL Workfront] à presque tous les services Web ou applications que vous souhaitez utiliser.
* La flexibilité de l’API [!DNL Workfront] s’étend également aux logiciels propriétaires de votre entreprise. Vous pouvez utiliser et modifier des données [!DNL Workfront] depuis votre propre logiciel.
* Comme les API sont si communes aux logiciels, vos développeurs internes les connaissent probablement. [!DNL Workfront] utilise une API REST-ful, le type d’API le plus courant, ce qui facilite encore la mise à niveau rapide de vos développeurs.

>[!INFO]
>
>**Exemple :**
>
>L’appel API suivant place un commentaire dans le flux de mise à jour de la tâche avec l’identifiant spécifié.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Pour plus d’informations sur l’API [!DNL Workfront], voir [Principes de base des API](../wf-api/general/api-basics.md).

Pour plus d’informations sur les abonnements aux événements, voir [API d’abonnement à un événement](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] vous permet d’automatiser les workflows. Avec la licence [!DNL Workfront Fusion for Work Automation and Integration], vous pouvez créer ces automatisations sur plusieurs applications et services web, créant ainsi des scénarios dans lesquels les applications travaillent ensemble pour exécuter une tâche. Un scénario est une représentation visuelle de la tâche ou du workflow créé à l’aide de modules, qui sont des tâches discrètes telles que &quot;Télécharger un document&quot; ou &quot;Créer un projet&quot;. Vous assemblez les modules pour définir le workflow, puis celui-ci s’exécute automatiquement lorsqu’une condition de déclenchement est remplie.

Les avantages de [!DNL Workfront Fusion] peuvent inclure les avantages suivants :

* [!DNL Workfront Fusion] ne nécessite pas autant de connaissances techniques que l’API, car l’interface visuelle vous aide à comprendre et à configurer le workflow. Cela signifie qu’il peut être utilisé par des personnes extérieures à une équipe de développement, ce qui peut vous faire gagner du temps et de l’argent.
* Étant donné que [!DNL Workfront Fusion] utilise l’API, il peut accéder à la plupart des applications et services web. De nombreuses applications disposent de modules pour effectuer des appels API, ou vous pouvez utiliser les modules HTTP, SOAP ou JSON pour interagir avec des services web qui n’ont pas de connecteur dédié [!DNL Workfront Fusion].

>[!INFO]
>
>**Exemple :**
>
>Le module [!DNL Workfront] suivant dans [!DNL Workfront Fusion] est configuré pour ajouter un commentaire au projet sélectionné. Une fois le module exécuté, le commentaire est visible dans le flux de mise à jour du projet dans Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Pour plus d&#39;informations sur [!DNL Workfront Fusion], voir [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
