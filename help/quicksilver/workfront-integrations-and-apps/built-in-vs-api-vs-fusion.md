---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Méthodes d’intégration Adobe Workfront
description: Vous pouvez intégrer des [!DNL Adobe Workfront] avec des applications tierces. Ces intégrations peuvent étendre l’utilité de [!DNL Workfront] et adaptez-le aux besoins de votre organisation. Vous pouvez utiliser l’une ou l’autre de ces intégrations, selon celle qui est la plus utile pour une tâche donnée.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---

# Méthodes d’intégration Adobe Workfront

Vous pouvez intégrer des [!DNL Adobe Workfront] avec des applications tierces. Ces intégrations peuvent étendre l’utilité de [!DNL Workfront] et adaptez-le aux besoins de votre organisation. Vous pouvez utiliser l’une ou l’autre de ces intégrations, selon celle qui est la plus utile pour une tâche donnée.

## Intégrations intégrées

Workfront fournit diverses intégrations que vous pouvez configurer directement à partir de Workfront ou d’une autre application en installant le module complémentaire Workfront pour cette application. Ces intégrations intégrées couvrent de nombreux scénarios d’utilisation courants et se concentrent sur l’extension et la connexion des expériences utilisateur pour les utilisateurs finaux.

Les intégrations intégrées de Workfront se concentrent principalement sur la productivité et la collaboration personnelles. Ces intégrations réduisent les interruptions dans le workflow d’un utilisateur individuel, ce qui lui permet de recevoir des notifications Workfront, d’accéder aux informations et d’agir sur les tâches de Workfront sans quitter l’application intégrée.

Les avantages des intégrations intégrées peuvent inclure les avantages suivants :

* La plupart de ces intégrations intégrées sont disponibles sans frais supplémentaires. (Les autres nécessitent un achat supplémentaire.)
* Les intégrations intégrées couvrent la plupart des applications les plus courantes utilisées par les entreprises, telles que [!DNL Slack], [!DNL Google Drive]ou [!DNL Adobe] les produits tels que [!DNL Adobe Creative Cloud] ou [!DNL Adobe Experience Manager] Ressources. Si votre entreprise utilise déjà ces applications, l’intégration s’effectuera sans problème dans le workflow existant de vos utilisateurs.
* Intégration [!DNL Workfront] avec une application fréquemment utilisée peut augmenter l’adoption de vos utilisateurs.

>[!INFO]
>
>**Exemple:**
>
>Avec le [!DNL Workfront for Microsoft Teams integration], vous pouvez recevoir des notifications dans [!DNL Microsoft Teams] à propos de [!DNL Workfront] tâches. Sans quitter [!DNL Microsoft Teams], vous pouvez effectuer des actions telles que l’approbation, la commentaires ou la modification de l’état des tâches. Toute modification apportée à des tâches à partir de [!DNL Microsoft Teams] sont reflétés dans [!DNL Workfront] ainsi que .

Pour plus d’informations sur les intégrations intégrées, y compris une liste des intégrations intégrées actuellement disponibles, voir [[!DNL Adobe Workfront] présentation des intégrations intégrées](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Applications OAuth2 personnalisées

Adobe [!DNL Workfront] Les administrateurs peuvent créer des applications OAuth2 pour votre instance de [!DNL Workfront], qui permettent à d’autres applications d’accéder à [!DNL Workfront]. Vos utilisateurs peuvent alors autoriser ces autres applications à accéder à leurs [!DNL Workfront] data. Ainsi, vous pouvez intégrer Workfront aux applications de votre choix, y compris vos propres applications internes.

>[!NOTE]
>
>Dans le contexte d’OAuth2, &quot;création d’une application&quot; fait référence au processus de création de ce type de lien d’accès entre une application et un serveur tel que Workfront.

Avantages de la création d’une [!UICONTROL OAuth2] l’application peut comprendre les éléments suivants :

* Les utilisateurs peuvent utiliser ces intégrations directement dans [!DNL Workfront], comme pour les intégrations intégrées.
* Configuration ou utilisation d’un [!UICONTROL OAuth2] L’application ne nécessite pas de connaissances techniques supplémentaires, telles que la connaissance du [!DNL Workfront] API.
* Votre entreprise peut utiliser des logiciels qui ne sont pas proposés en tant que [!DNL Workfront] application intégrée. Vous pouvez toujours intégrer ce logiciel à [!DNL Workfront] en utilisant une [!UICONTROL OAuth2] , même si le logiciel appartient à votre entreprise.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] propose une API publique (interface de programmation d’application) qui vous permet d’étendre et d’améliorer votre expérience Workfront. L’objectif de la variable [!DNL Workfront] L’API permet de simplifier la création de vos propres intégrations avec [!DNL Workfront] en introduisant une architecture REST-ful qui fonctionne sur HTTP. Le [!DNL Workfront] L’API nécessite des connaissances techniques, mais il s’agit d’un outil très puissant pour récupérer, créer et modifier des données. Vous pouvez personnaliser les appels d’API pour exécuter des fonctions très spécifiques.

En outre, [!DNL Workfront] propose une API Event Subscription. Lorsqu’une action se produit sur une [!DNL Workfront] compatible avec les abonnements aux événements, vous pouvez configurer [!DNL Workfront] pour envoyer une réponse au point de terminaison souhaité. Cela signifie que les applications tierces peuvent recevoir des mises à jour de [!DNL Workfront] les interactions via la variable [!DNL Workfront] API peu après.

Avantages de l’utilisation de la variable [!DNL Workfront] L’API peut inclure les éléments suivants :

* Vous pouvez utiliser la variable [!DNL Workfront] API permettant de se connecter à presque tout autre service Web ou application offrant une API publique. Il est donc possible d&#39;intégrer [!DNL Workfront] avec pratiquement tous les services web ou applications que vous souhaitez utiliser.
* Le [!DNL Workfront] La flexibilité de l’API s’étend également aux logiciels propriétaires de votre entreprise. Vous pouvez utiliser et modifier des [!DNL Workfront] données de votre propre logiciel.
* Comme les API sont si communes aux logiciels, vos développeurs internes les connaissent probablement. [!DNL Workfront] utilise une API REST-ful, le type d’API le plus courant, ce qui facilite encore la mise à niveau rapide de vos développeurs.

>[!INFO]
>
>**Exemple:**
>
>L’appel API suivant place un commentaire dans le flux de mise à jour de la tâche avec l’identifiant spécifié.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Pour plus d’informations sur la variable [!DNL Workfront] API, voir [Principes de base des API](../wf-api/general/api-basics.md).

Pour plus d’informations sur les abonnements aux événements, voir [API d’abonnement à un événement](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] vous permet d’automatiser les workflows. Avec le [!DNL Workfront Fusion for Work Automation and Integration] , vous pouvez créer ces automatisations sur plusieurs applications et services web, créant ainsi des scénarios dans lesquels les applications travaillent ensemble pour exécuter une tâche. Un scénario est une représentation visuelle de la tâche ou du workflow créé à l’aide de modules, qui sont des tâches discrètes telles que &quot;Télécharger un document&quot; ou &quot;Créer un projet&quot;. Vous assemblez les modules pour définir le workflow, puis celui-ci s’exécute automatiquement lorsqu’une condition de déclenchement est remplie.

Avantages de [!DNL Workfront Fusion] peuvent inclure les éléments suivants :

* [!DNL Workfront Fusion] ne nécessite pas autant de connaissances techniques que l’API, car l’interface visuelle vous aide à comprendre et à configurer le workflow. Cela signifie qu’il peut être utilisé par des individus en dehors d’une équipe de développement, ce qui peut vous faire gagner du temps et de l’argent à votre organisation.
* Depuis [!DNL Workfront Fusion] fonctionne via l’API ; elle peut accéder à la plupart des applications et services web. De nombreuses applications disposent de modules pour effectuer des appels API. Vous pouvez également utiliser les modules HTTP, SOAP ou JSON pour interagir avec des services web qui n’ont pas de [!DNL Workfront Fusion] connecteur.

>[!INFO]
>
>**Exemple:**
>
>Les éléments suivants [!DNL Workfront] module dans [!DNL Workfront Fusion] est configuré pour ajouter un commentaire au projet sélectionné. Une fois le module exécuté, le commentaire est visible dans le flux de mise à jour du projet dans Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Pour plus d’informations sur [!DNL Workfront Fusion], voir [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
