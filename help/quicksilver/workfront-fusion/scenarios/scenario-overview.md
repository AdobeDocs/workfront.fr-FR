---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Présentation du scénario Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] présentation du scénario

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une [!DNL Adobe Workfront Fusion] en plus d’une [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] Les scénarios ne doivent pas être confondus avec [!DNL Workfront Scenario Planner] scénarios. Pour plus d’informations sur [!DNL Workfront Scenario Planner] scénarios, voir [Le [!DNL Scenario Planner] aperçu](../../scenario-planner/scenario-planner-overview.md).

Le rôle de [!DNL Adobe Workfront Fusion] est d’automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches plutôt que de répéter les mêmes tâches encore et encore. Il fonctionne en liant les actions dans et entre les applications et les services pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Un scénario comprend une série de modules qui indiquent comment les données doivent être transformées dans une application ou transférées entre les applications et les services web.

## Exemple : Automatisation des processus dans [!DNL Adobe Workfront]

>[!NOTE]
>
>Cette fonctionnalité est disponible pour les licences suivantes :
>
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail]
>


[!DNL Workfront Fusion] permet d’automatiser des workflows simples ou complexes dans des [!DNL Workfront], ce qui vous permet de gagner du temps et de vous assurer que le processus est exécuté de manière cohérente.

Dans cet exemple, le scénario se déclenche lorsqu’un champ spécifié change dans une tâche ou un problème dans [!DNL Workfront]. Lorsqu’il est déclenché, le scénario obtient des informations dans le projet associé et crée une mise à jour personnalisée pour une personne affectée à un rôle spécifique dans le projet.

![](assets/fusion-template-example-350x102.png)

## Exemple : Connexion [!DNL Workfront] vers une autre application ou un autre service web

>[!NOTE]
>
>Cette fonctionnalité est disponible pour la licence suivante :
>
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail]
>


[!DNL Workfront Fusion] peut également se connecter à d’autres applications et services web. Vous pouvez accéder à d’autres applications, les importer, les manipuler ou les exporter, en les intégrant à Workfront ou entre elles. De nombreuses applications sont dédiées [!DNL Workfront Fusion] connecteurs. S’il n’existe aucun connecteur dédié pour l’application à laquelle vous souhaitez accéder, vous pouvez utiliser [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] ou [!UICONTROL SOAP] modules pour se connecter à l’application via son API.

Dans cet exemple, le scénario se déclenche lorsqu’un utilisateur est ajouté à un événement [!DNL Excel] feuille de calcul. Le scénario vérifie si l’utilisateur se trouve dans [!DNL Workfront]. Si ce n’est pas le cas, le scénario crée l’utilisateur dans [!DNL Workfront] et ajoute leur ID utilisateur Workfront à la feuille de calcul.

![](assets/fusion-integration-example--350x171.png)

Pour obtenir la liste des connecteurs dédiés, voir [Applications et leurs modules](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] peut se connecter à pratiquement n’importe quel service Web. Si l’application avec laquelle vous souhaitez travailler n’a pas de [!DNL Workfront Fusion] connecteur, vous pouvez utiliser les modules suivants pour vous connecter directement au service web :
>
>* [[!UICONTROL HTTP] modules](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] module](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] modules](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

