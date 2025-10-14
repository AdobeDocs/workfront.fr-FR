---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Méthodes d’intégration d’Adobe Workfront
description: Vous pouvez intégrer  [!DNL Adobe Workfront]  à des applications tierces. Ces intégrations permettent d’étendre l’utilité de  [!DNL Workfront]  et de l’adapter aux besoins de votre organisation. Vous pouvez utiliser tout ou partie de ces intégrations, en fonction de leur utilité vis-à-vis d’une tâche donnée.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 98%

---

# Méthodes d’intégration d’Adobe Workfront

Vous pouvez intégrer [!DNL Adobe Workfront] à des applications tierces, mais aussi à d’autres produits [!DNL Adobe]. Ces intégrations permettent d’étendre l’utilité de [!DNL Workfront] et de l’adapter aux besoins de votre organisation. Vous pouvez utiliser tout ou partie de ces intégrations, en fonction de leur utilité vis-à-vis d’une tâche donnée.

## Intégrations intégrées

Workfront fournit diverses intégrations que vous pouvez configurer directement à partir de Workfront ou d’une autre application en installant le module complémentaire Workfront pour cette application. Ces intégrations intégrées couvrent de nombreux scénarios d’utilisation courants et permettent d’élargir et de relier les expériences des utilisateurs et utilisatrices finaux.

Les intégrations intégrées de Workfront se concentrent principalement sur la productivité et la collaboration personnelles. Ces intégrations réduisent les interruptions dans le workflow d’une personne, ce qui lui permet de recevoir des notifications Workfront, d’accéder aux informations et d’agir sur les éléments de travail Workfront sans quitter l’application intégrée.

Les avantages des intégrations intégrées peuvent inclure les points suivants :

* La plupart de ces intégrations intégrées sont disponibles sans frais supplémentaires. (Les autres sont payantes.)
* Les intégrations intégrées couvrent la plupart des applications les plus courantes des entreprises, telles que [!DNL Slack], [!DNL Google Drive], ou les produits [!DNL Adobe] comme [!DNL Adobe Creative Cloud] ou [!DNL Adobe Experience Manager] Assets. Si votre entreprise utilise déjà ces applications, l’intégration s’effectuera aisément dans le workflow existant de vos utilisateurs et utilisatrices.
* L’intégration de [!DNL Workfront] dans une application fréquemment utilisée peut augmenter le niveau d’acceptation de vos utilisateurs et utilisatrices.

>[!INFO]
>
>**Exemple :**
>
>Avec l’[!DNL Workfront for Microsoft Teams integration], vous pouvez recevoir des notifications dans [!DNL Microsoft Teams] à propos de vos éléments de travail [!DNL Workfront]. Sans quitter [!DNL Microsoft Teams], vous pouvez effectuer des actions telles que l’approbation, l’ajout de commentaires ou la modification du statut des éléments de travail. Toute modification apportée à des éléments de travail à partir de [!DNL Microsoft Teams] est également reflétée dans [!DNL Workfront].

Pour plus d’informations sur les intégrations intégrées, et notamment pour obtenir une liste des intégrations intégrées actuellement disponibles, voir la section Vue d’ensemble des intégrations intégrées [[!DNL Adobe Workfront] &#x200B;](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Personnaliser les applications OAuth2

Les équipes d’administration Adobe [!DNL Workfront] peuvent créer des applications OAuth2 pour votre instance de [!DNL Workfront], qui permettent à d’autres applications d’accéder à [!DNL Workfront]. Vos utilisateurs et utilisatrices peuvent alors autoriser ces autres applications à accéder à leurs données [!DNL Workfront]. Vous pouvez ainsi intégrer Workfront aux applications de votre choix, y compris à vos propres applications internes.

>[!NOTE]
>
>Dans le contexte d’OAuth2, la « création d’une application » fait référence au processus de création de ce type de lien d’accès entre une application et un serveur tel que Workfront.

Les avantages de la création d’une application [!UICONTROL OAuth2] peuvent comprendre les points suivants :

* Les utilisateurs et utilisatrices peuvent utiliser ces intégrations directement dans [!DNL Workfront], comme pour les intégrations intégrées.
* La configuration ou l’utilisation d’une application [!UICONTROL OAuth2] ne nécessite pas de connaissances techniques supplémentaires, telles que le fonctionnement de l’API [!DNL Workfront].
* Votre organisation peut utiliser des logiciels qui ne sont pas proposés en tant qu’applications intégrées [!DNL Workfront]. Vous pouvez toujours intégrer ces logiciels à [!DNL Workfront] en utilisant une application [!UICONTROL OAuth2], même si le logiciel appartient à votre organisation.

Pour plus d’informations, voir la section [Créer des applications OAuth2 pour les intégrations Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## API [!DNL Workfront]

[!DNL Workfront] propose une API (interface de programmation d’application) publique qui vous permet de prolonger et d’améliorer votre expérience Workfront. L’objectif de l’API [!DNL Workfront] est de simplifier la création de vos propres intégrations avec [!DNL Workfront] en introduisant une architecture REST-ful qui fonctionne sur HTTP. L’API [!DNL Workfront] nécessite certaines connaissances techniques, mais représente un outil très puissant pour récupérer, créer et modifier des données. Vous pouvez personnaliser les appels API afin d’exécuter des fonctions très spécifiques.

En outre, [!DNL Workfront] propose une API d’abonnement à un événement. Lorsqu’une action se produit sur un objet [!DNL Workfront] compatible avec les abonnements aux événements, vous pouvez configurer [!DNL Workfront] pour qu’il envoie une réponse au point d’entrée souhaité. Cela signifie que les applications tierces peuvent recevoir des mises à jour à partir des interactions [!DNL Workfront] via l’API [!DNL Workfront] peu après leur création.

Les avantages de l’utilisation de l’API [!DNL Workfront] peuvent inclure les points suivants :

* Vous pouvez utiliser l’API [!DNL Workfront] pour vous connecter à quasiment tous les autres services web ou applications offrant une API publique. Il est donc possible d’intégrer [!DNL Workfront] dans pratiquement tous les services web ou applications que vous souhaitez utiliser.
* La flexibilité de l’API [!DNL Workfront] s’étend également aux logiciels propriétaires de votre entreprise. Vous pouvez utiliser et modifier les données [!DNL Workfront] depuis votre propre logiciel.
* Les API étant très communes dans les logiciels, vos équipes de développement internes les connaissent probablement. [!DNL Workfront] utilise une API REST-ful, le type le plus courant, ce qui facilite encore davantage la mise en application rapide pour votre équipe de développement.

>[!INFO]
>
>**Exemple :**
>
>L’appel API suivant place un commentaire dans le flux de mise à jour de la tâche avec l’identifiant spécifié.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Pour plus d’informations sur l’API [!DNL Workfront], voir la section [Principes de base des API](../wf-api/general/api-basics.md).

Pour plus d’informations sur les abonnements aux événements, voir la section [API d’abonnement aux événements](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] vous permet d’automatiser les workflows. Avec la licence [!DNL Workfront Fusion for Work Automation and Integration], vous pouvez créer ces automatisations sur plusieurs applications et services web en élaborant des scénarios dans lesquels les applications fonctionnent ensemble pour exécuter une tâche. Un scénario est une représentation visuelle de la tâche ou du workflow, créée à l’aide de modules, qui sont des tâches indépendantes telles que « Télécharger un document » ou « Créer un projet ». Vous assemblez les modules pour définir le workflow, puis celui-ci s’exécute automatiquement lorsqu’une condition de déclenchement est remplie.

Les avantages de [!DNL Workfront Fusion] peuvent inclure les points suivants :

* [!DNL Workfront Fusion] ne nécessite pas autant de connaissances techniques que l’API, car l’interface visuelle vous aide à comprendre et à configurer le workflow. Cela signifie qu’il peut être utilisé par des personnes extérieures à une équipe de développement, ce qui peut faire gagner du temps et de l’argent à votre organisation.
* Puisque [!DNL Workfront Fusion] fonctionne via l’API, il peut accéder à la plupart des applications et services web. De nombreuses applications disposent de modules pour effectuer des appels API. Vous pouvez également utiliser les modules HTTP, SOAP ou JSON pour interagir avec des services web qui ne possèdent pas de connecteur [!DNL Workfront Fusion] dédié.

>[!INFO]
>
>**Exemple :**
>
>Le module [!DNL Workfront] suivant dans [!DNL Workfront Fusion] est configuré pour ajouter un commentaire au projet sélectionné. Une fois le module exécuté, le commentaire est visible dans le flux de mise à jour du projet dans Workfront.
>
>![Exemple : ajout d’un commentaire dans Fusion](assets/fusion-example-comment-350x416.png)

Pour plus d’informations sur [!DNL Workfront Fusion], voir [[!DNL Adobe Workfront Fusion]](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/home).
