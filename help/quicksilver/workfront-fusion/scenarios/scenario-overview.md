---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Vue d’ensemble du scénario d’Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion et une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 27158301e491d4ff45ce7987a81f841fb4525b2a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 26%

---

# [!DNL Adobe Workfront Fusion] - Présentation du scénario

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>Les scénarios [!DNL Workfront Fusion] ne doivent pas être confondus avec les scénarios [!DNL Workfront Scenario Planner]. Pour plus d’informations sur les scénarios [!DNL Workfront Scenario Planner], voir [The [!DNL Scenario Planner] overview](../../scenario-planner/scenario-planner-overview.md).

[!DNL Adobe Workfront Fusion] vise à automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches, plutôt que de répéter les mêmes tâches encore et encore. L’application fonctionne en reliant les actions au sein et entre les applications et les services, pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Un scénario se compose d’une série de modules qui indiquent comment les données doivent être transformées dans une application ou transférées entre les applications et les services web.

## Exemple : automatisation des processus dans [!DNL Adobe Workfront]

>[!NOTE]
>
>Cette fonctionnalité est disponible pour les licences suivantes :
>
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail]

[!DNL Workfront Fusion] vous permet d’automatiser des workflows simples ou complexes dans [!DNL Workfront], ce qui vous permet de gagner du temps et de vous assurer que le processus est exécuté de manière cohérente.

Dans cet exemple, le scénario se déclenche lorsqu’un champ spécifié change dans une tâche ou un problème dans [!DNL Workfront]. Lorsqu’il est déclenché, le scénario obtient des informations dans le projet associé et crée une mise à jour personnalisée pour une personne affectée à un rôle spécifique dans le projet.

![](assets/fusion-template-example-350x102.png)

## Exemple : connexion de [!DNL Workfront] à une autre application ou un autre service Web

>[!NOTE]
>
>Cette fonctionnalité est disponible pour la licence suivante :
>
>* [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail]
>

[!DNL Workfront Fusion] peut également se connecter à d’autres applications et services web. Vous pouvez accéder à d’autres applications, les importer, les manipuler ou les exporter, en les intégrant à Workfront ou entre elles. De nombreuses applications ont des connecteurs [!DNL Workfront Fusion] dédiés. S’il n’existe aucun connecteur dédié pour l’application à laquelle vous souhaitez accéder, vous pouvez utiliser les modules [!UICONTROL HTTP] ou [!UICONTROL SOAP] de [!DNL Workfront Fusion] pour vous connecter à l’application via son API.

Dans cet exemple, le scénario se déclenche lorsqu’un utilisateur est ajouté à une feuille de calcul [!DNL Excel]. Le scénario vérifie si l’utilisateur se trouve dans [!DNL Workfront]. Si ce n’est pas le cas, le scénario crée l’utilisateur dans [!DNL Workfront] et l’ajoute à nouveau à la feuille de calcul.

![](assets/fusion-integration-example--350x171.png)

Pour obtenir la liste des connecteurs dédiés, voir [Applications et leurs modules](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] peut se connecter à pratiquement n’importe quel service Web. Si l&#39;application avec laquelle vous souhaitez travailler ne dispose pas d&#39;un connecteur [!DNL Workfront Fusion] dédié, vous pouvez utiliser les modules suivants pour vous connecter directement au service web :
>
>* Modules [[!UICONTROL HTTP] ](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* Module [[!UICONTROL SOAP] ](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* Modules [[!UICONTROL JSON] ](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
