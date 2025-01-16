---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Vue d’ensemble du scénario Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 54%

---

# Vue d’ensemble du scénario [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Présentation du scénario](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>Les scénarios [!DNL Workfront Fusion] ne doivent pas être confondus avec les scénarios [!DNL Workfront Scenario Planner]. Pour plus d’informations sur les scénarios [!DNL Workfront Scenario Planner], consultez la section[ Vue d’ensemble de  [!DNL Scenario Planner] ](../../scenario-planner/scenario-planner-overview.md).

Le rôle de [!DNL Adobe Workfront Fusion] est d’automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches, plutôt que de répéter les mêmes tâches encore et encore. La plateforme fonctionne en liant les actions dans et entre les applications et les services pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Un scénario se compose d’une série de modules qui indiquent comment les données doivent être transformées dans une application ou transférées entre les applications et les services web.

## Présentation des éléments de scénario

Un scénario est constitué de différents éléments. La compréhension de la terminologie de ces éléments facilite l’utilisation de la documentation.

### Scénario

Un **scénario** est une série d’étapes automatisées créées par l’utilisateur ou l’utilisatrice pour déplacer et manipuler des données. Le terme « scénario » fait référence à l’ensemble du groupe d’étapes connectées.

![Scénario](assets/entire-scenario-scenario.png)

### Déclencheur

Un scénario commence par un **déclencheur**. Le déclencheur recherche les données nouvelles et mises à jour et démarre le scénario lorsque certaines conditions configurées dans le module s’appliquent. Les Triggers peuvent être configurés pour démarrer un scénario selon un planning (interrogation) ou chaque fois que des modifications de données se produisent (instant).

![ Déclencheur ](assets/scenario-trigger.png)

### Module

Le déclencheur est suivi d’un certain nombre de **modules**. Un module représente une seule étape dans un scénario qui exécute une action spécifique. Les modules sont configurés et liés ensemble pour créer des scénarios.

![Module ](assets/scenario-module.png)

### Itinéraire

Un scénario peut être divisé en **itinéraires**. Une route est une section du scénario qui peut être utilisée ou non pour un lot de données donné. Les itinéraires sont configurés à l&#39;aide d&#39;un module de routeur et de filtres.

![Route](assets/scenario-route.png)

### Segment de scénario

Un segment de scénario est une section d’un scénario qui se compose d’une série de modules contigus qui se connectent tous à la même application. Les segments de scénario représentent souvent un workflow court dans l’application.

![Segment de scénario](assets/scenario-segment.png)

### Connecteur

Un connecteur correspond à l’ensemble des modules d’une application donnée. Workfront Fusion offre des connecteurs à de nombreuses applications de travail courantes, telles que Workfront, Salesforce et Jira, ainsi que des connecteurs génériques qui peuvent être utilisés pour n’importe quel service web.

![Connecteurs ](assets/scenario-connectors.png)



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
