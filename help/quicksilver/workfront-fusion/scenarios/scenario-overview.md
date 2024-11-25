---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Vue d’ensemble du scénario Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: f8ea4a1c40cd3fc4664a5a3b1c3a900e874d78b1
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 61%

---

# Vue d’ensemble du scénario [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>Les scénarios [!DNL Workfront Fusion] ne doivent pas être confondus avec les scénarios [!DNL Workfront Scenario Planner]. Pour plus d’informations sur les scénarios [!DNL Workfront Scenario Planner], consultez la section[ Vue d’ensemble de  [!DNL Scenario Planner] ](../../scenario-planner/scenario-planner-overview.md).

Le rôle de [!DNL Adobe Workfront Fusion] est d’automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches, plutôt que de répéter les mêmes tâches encore et encore. La plateforme fonctionne en liant les actions dans et entre les applications et les services pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Un scénario se compose d’une série de modules qui indiquent comment les données doivent être transformées dans une application ou transférées entre les applications et les services web.

## Présentation des éléments du scénario

Un scénario est constitué d’éléments différents. La compréhension de la terminologie de ces éléments facilite l’utilisation de la documentation.

### Scénario

Un **scénario** est une série d’étapes automatisées créée par l’utilisateur, créée pour déplacer et manipuler des données. Le terme &quot;scénario&quot; fait référence à l’ensemble des étapes connectées.

![Scénario](assets/entire-scenario-scenario.png)

### Déclencheur

Un scénario commence par un **trigger**. Le déclencheur recherche les données nouvelles et mises à jour et lance le scénario lorsque certaines conditions configurées dans le module s’appliquent. Les déclencheurs peuvent être configurés pour démarrer un scénario dans un planning (interrogation) ou chaque fois que des changements de données se produisent (instantanés).

![Déclencheur](assets/scenario-trigger.png)

### Module

Le déclencheur est suivi d&#39;un certain nombre de **modules**. Un module représente une seule étape dans un scénario qui effectue une action spécifique. Les modules sont configurés et assemblés ensemble pour créer des scénarios.

![Module](assets/scenario-module.png)

### Route

Un scénario peut être divisé en **itinéraires**. Un itinéraire est une section du scénario qui peut ou non être utilisée pour un lot donné de données. Les itinéraires sont configurés à l&#39;aide d&#39;un module de routeur et de filtres.

![Route](assets/scenario-route.png)

### Segment de scénario

Un segment de scénario est une section d’un scénario qui consiste en une série de modules contigus qui se connectent tous à la même application. Les segments de scénario représentent souvent un processus court dans l’application.

![Segment de scénario](assets/scenario-segment.png)

### Connecteur

Un connecteur est l’ensemble des modules d’une application donnée. Workfront Fusion offre des connecteurs à de nombreuses applications de travail courantes, telles que Workfront, Salesforce et Jira, ainsi que des connecteurs génériques qui peuvent être utilisés pour n’importe quel service Web.

![Connecteurs](assets/scenario-connectors.png)



## Exemple : Automatisation des processus au sein de [!DNL Adobe Workfront]

>[!NOTE]
>
>Cette fonctionnalité est disponible pour les licences suivantes :
>
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail]

[!DNL Workfront Fusion] vous permet d’automatiser des flux de travail simples ou complexes au sein de [!DNL Workfront], ce qui vous permet de gagner du temps et de vous assurer que le processus est exécuté de manière cohérente.

Dans cet exemple, le scénario se déclenche lorsqu’un champ spécifié est modifié dans une tâche ou un problème dans [!DNL Workfront]. Lorsqu’il est déclenché, le scénario récupère des informations dans le projet concerné et crée une mise à jour personnalisée pour une personne affectée à un rôle spécifique dans le projet.

![](assets/fusion-template-example-350x102.png)

## Exemple : Connecter [!DNL Workfront] à une autre application ou à un service web

>[!NOTE]
>
>Cette fonctionnalité est disponible pour la licence suivante :
>
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail]
>

[!DNL Workfront Fusion] peut également se connecter à d’autres applications et services web. Vous pouvez accéder, importer, manipuler ou exporter des données à partir d’autres applications, en les intégrant à Workfront ou entre elles. De nombreuses applications disposent de connecteurs [!DNL Workfront Fusion] dédiés. S’il n’existe pas de connecteur dédié à l’application à laquelle vous souhaitez accéder, vous pouvez utiliser les modules [!UICONTROL HTTP] ou [!UICONTROL SOAP] de [!DNL Workfront Fusion] pour vous connecter à l’application via son API.

Dans cet exemple, le scénario se déclenche lors de l’ajout d’un utilisateur ou d’une utilisatrice à une feuille de calcul [!DNL Excel]. Le scénario vérifie si l’utilisateur ou l’utilisatrice est dans [!DNL Workfront]. Si ce n’est pas le cas, le scénario crée l’utilisateur ou l’utilisatrice dans [!DNL Workfront] et ajoute son ID d’utilisateur ou d’utilisatrice Workfront à la feuille de calcul.

![](assets/fusion-integration-example--350x171.png)

Pour obtenir une liste des connecteurs dédiés, voir [Les applications et leurs modules](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] peut se connecter à presque tous les services web. Si l’application avec laquelle vous souhaitez travailler ne dispose pas d’un connecteur [!DNL Workfront Fusion] dédié, vous pouvez utiliser les modules suivants pour vous connecter directement au service web :
>
>* [[!UICONTROL Modules ]HTTP](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* Module [[!UICONTROL SOAP] ](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL Modules ]JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
