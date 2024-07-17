---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]
description: De nombreux services fournissent des webhooks pour envoyer des notifications instantanées lorsqu’une modification spécifique se produit dans le service. Pour traiter ces notifications, nous vous recommandons d’utiliser des déclencheurs instantanés. Cet article décrit l’utilisation et les fonctionnalités des déclencheurs instantanés dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 23%

---

# Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]

De nombreux services fournissent des webhooks pour envoyer des notifications instantanées lorsqu’une modification spécifique se produit dans le service. Pour traiter ces notifications, nous vous recommandons d’utiliser des déclencheurs instantanés. Vous pouvez facilement les reconnaître dans [!DNL Adobe Workfront Fusion] à cause de leur balise :

![](assets/instant-350x256.png)

Si le service ne fournit pas de webhooks, vous devez utiliser des triggers d’interrogation pour interroger régulièrement le service.

Pour une vidéo d’introduction aux webhooks dans Workfront Fusion, voir :

* [Intro to Webhooks](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Webhooks intermédiaires](https://video.tv.adobe.com/v/3427030/){target=_blank}

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Affichage de la file d’attente d’un webhook

Tous les messages des webhooks entrants sont stockés dans la file d’attente du webhook.

1. Cliquez sur **[!UICONTROL Webhooks]** dans le menu de gauche.
1. Recherchez le webhook pour lequel vous souhaitez afficher la file d’attente.
1. Cliquez sur le bouton avec une icône de camion et le nombre de webhooks reçus.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Les données du webhook entrant sont toujours stockées dans la file d’attente, quelle que soit la manière dont vous avez défini l’option [!UICONTROL Data] est confidentielle (décrite dans [Le panneau des paramètres du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Dès que les données sont traitées dans un scénario, elles sont définitivement supprimées du système.

## Planification de déclencheurs instantanés

Si votre scénario contient un déclencheur instantané, vous pouvez planifier son exécution immédiate :

![](assets/schedule-setting-350x185.png)

Dans ce cas, votre scénario s’exécute immédiatement lorsque [!DNL Workfront Fusion] reçoit de nouvelles données du service. Une fois le scénario exécuté, le nombre total de webhooks en attente dans la file d’attente est comptabilisé et le scénario exécute autant de cycles que les webhooks en attente, en traitant un webhook par cycle. Pour plus d’informations, voir [Exécution de scénario, cycles et phases dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Un cycle n’est pas la même chose qu’une exécution de scénario. Il peut y avoir plusieurs cycles dans un scénario exécuté.
>* Lorsque vous exécutez un scénario avec un déclencheur instantané programmé pour être immédiat, les exceptions suivantes s’appliquent :
>
>     * L’intervalle entre deux exécutions n’est pas soumis à l’intervalle minimum conformément au plan de tarification.
>
>       Par exemple, une fois l’exécution du scénario terminée, la file d’attente du webhook est de nouveau vérifiée. S’il existe des webhooks en attente, le scénario s’exécute à nouveau immédiatement, en traitant à nouveau tous les webhooks en attente.
>   
>     * Le paramètre de scénario Nombre maximum de cycles est ignoré et défini sur 100, ce qui signifie qu’aucun plus de 100 webhooks en attente ne sera traité lors d’une seule exécution de scénario (à la vitesse d’1 événement par cycle).
>


Si vous utilisez un autre paramètre de planification que [!UICONTROL Immédiatement], le scénario s’exécute aux intervalles que vous spécifiez. Comme plusieurs webhooks peuvent être regroupés dans la file d’attente pendant l’intervalle, il est recommandé de définir le [[!UICONTROL nombre maximum de cycles]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) sur une valeur supérieure à la valeur par défaut 1 pour traiter plus de webhooks dans un scénario exécuté :

1. Cliquez sur l’icône [!UICONTROL Paramètres du scénario] ![](assets/gear-icon-settings.png) au bas de votre scénario.
1. Dans la zone **[!UICONTROL Paramètres du scénario]** qui s’affiche, saisissez un nombre dans la zone **[!UICONTROL Nombre max de cycles]** pour indiquer le nombre de webhooks de la file d’attente que vous souhaitez exécuter chaque fois que vous exécutez le scénario.

## Limites de taux

La limite de taux actuelle est de 5 webhooks par seconde. Si la limite est dépassée, un code d’état 429 est renvoyé.

## Expiration des webhooks inactifs

Un webhook qui n’a été affecté à aucun scénario pendant plus de 120 heures est supprimé.

## Payloads Webhook

[!DNL Workfront Fusion] stocke les payloads de webhook pendant 30 jours. L’accès à une payload de webhook plus de 30 jours après sa création entraîne l’erreur « [!UICONTROL Échec de la lecture du fichier à partir du stockage] ».

## Gestion des erreurs

En cas d’erreur dans votre scénario avec un déclencheur instantané, le scénario :

* S’arrête immédiatement lorsque le scénario est défini pour exécuter [!UICONTROL Immédiatement].
* S’arrête après 3 tentatives infructueuses (3 erreurs) : lorsque le scénario est défini pour s’exécuter comme prévu.

Si une erreur se produit lors de l’exécution du scénario, le webhook est placé à nouveau dans la file d’attente lors de la phase de restauration du déclencheur instantané. Dans une telle situation, vous avez la possibilité de corriger le scénario et de le réexécuter. Pour plus d’informations, voir [Restauration](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) dans l’article [Exécution de scénario, cycles et phases dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si votre scénario comporte un module de réponse Webhook, l’erreur est envoyée à la réponse Webhook. Le module de réponse Webhook est toujours exécuté en dernier (dans le cas où l’option [!UICONTROL Validation automatique] dans les paramètres du scénario n’est pas activée). Pour plus d’informations, voir [Réponse à webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) dans l’article [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhooks personnalisés

Vous pouvez créer vos propres webhooks. Pour plus d’informations, voir [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Désactivation de Webhook

Les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

* Le webhook n’est connecté à aucun scénario depuis plus de 5 jours.
* Le webhook est utilisé uniquement dans les scénarios inactifs (inactifs depuis plus de 30 jours).

Les webhooks désactivés sont supprimés et désinscrits automatiquement s’ils ne sont connectés à aucun scénario et s’ils sont restés désactivés pendant plus de 30 jours.


