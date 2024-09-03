---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Déclencheurs instantanés (webhooks) dans  [!DNL Adobe Workfront Fusion]
description: De nombreux services proposent des webhooks pour envoyer des notifications instantanées chaque fois que le service est modifié. Pour traiter ces notifications, nous vous recommandons d’utiliser des déclencheurs instantanés. Cet article décrit l’utilisation et la fonctionnalité des déclencheurs instantanés dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 100%

---

# Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]

De nombreux services proposent des webhooks pour envoyer des notifications instantanées chaque fois que le service est modifié. Pour traiter ces notifications, nous vous recommandons d’utiliser des déclencheurs instantanés. Leur balise permet de les reconnaître facilement dans [!DNL Adobe Workfront Fusion] :

![](assets/instant-350x256.png)

Si le service ne fournit pas de webhooks, vous devez utiliser des déclencheurs d’attente active pour enquêter périodiquement auprès du service.

Pour une introduction vidéo aux webhooks dans Workfront Fusion, consultez :

* [Présentation des webhooks](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Webhooks intermédiaires](https://video.tv.adobe.com/v/3427030/){target=_blank}

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir [[!DNL Adobe Workfront Fusion] Licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Afficher la file d’attente d’un webhook

Tous les messages des webhooks entrants sont stockés dans la file d’attente du webhook.

1. Cliquez sur **[!UICONTROL Webhooks]** dans le menu de gauche.
1. Recherchez le webhook dont vous souhaitez consulter la file d’attente.
1. Cliquez sur le bouton avec une icône de camion et le nombre de webhooks reçus.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Les données entrantes du webhook sont toujours stockées dans la file d’attente, quel que soit le réglage de l’option [!UICONTROL Données] confidentielles (décrite dans [Panneau des paramètres de scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Dès que les données sont traitées dans un scénario, elles sont définitivement supprimées du système.

## Planifier des déclencheurs instantanés

Si votre scénario contient un déclencheur instantané, vous pouvez planifier son exécution immédiate :

![](assets/schedule-setting-350x185.png)

Dans ce cas, votre scénario s’exécutera immédiatement lorsque [!DNL Workfront Fusion] recevra de nouvelles données du service. Après l’exécution du scénario, le nombre total de webhooks en attente dans la file d’attente est compté. Le scénario effectue, ensuite, autant de cycles qu’il y a de webhooks en attente, en traitant un webhook par cycle. Pour plus d’informations, consultez la section [Exécution, cycles et phases d’un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Un cycle n’est pas la même chose qu’un scénario. Il peut y avoir plusieurs cycles au sein d’un même scénario.
>* Lorsque vous exécutez un scénario avec un déclencheur instantané prévu pour être immédiat, les exceptions suivantes s’appliquent :
>
>     * L’intervalle entre deux exécutions n’est pas soumis à l’intervalle minimum prévu par le plan tarifaire.
>
>       Par exemple, une fois que le scénario a terminé son exécution, la file d’attente du webhook est à nouveau vérifiée. Si des webhooks sont en attente, le scénario s’exécute à nouveau immédiatement, en traitant à nouveau tous les webhooks en attente.
>   
>     * Le paramètre de scénario « Nombre maximal de cycles » est ignoré et fixé à 100, ce qui signifie qu’un maximum de 100 webhooks en attente sont traités au cours de l’exécution d’un seul scénario (à raison d’un événement par cycle).
>


Si vous utilisez un paramètre de planification autre que [!UICONTROL Immédiatement], le scénario s’exécute aux intervalles spécifiés. Plusieurs webhooks pouvant se trouver dans la file d’attente pendant l’intervalle, il est recommandé de fixer le [[!UICONTROL nombre maximal de cycles]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) à une valeur supérieure à la valeur par défaut de 1, afin de traiter davantage de webhooks en une seule exécution de scénario :

1. Cliquez sur l’icône [!UICONTROL Paramètres de scénario] ![](assets/gear-icon-settings.png) en bas de votre scénario.
1. Dans la boîte de dialogue **[!UICONTROL Paramètres de scénario]** qui s’affiche, saisissez un nombre dans la zone **[!UICONTROL Nombre max. de cycles]** pour indiquer le nombre de webhooks de la file d’attente que vous souhaitez lancer à chaque fois que vous exécutez le scénario.

## Limites de débit

La limite de débit actuelle est de 5 webhooks par seconde. Si la limite est dépassée, un code de statut 429 est renvoyé.

## Expiration des webhooks inactifs

Un webhook qui n’a pas été affecté à un scénario depuis plus de 120 heures est supprimé.

## Payloads des webhooks

[!DNL Workfront Fusion] stocke les payloads des webhooks pendant 30 jours. L’accès à un payload de webhook plus de 30 jours après sa création génère l’erreur « [!UICONTROL Échec de la lecture du fichier depuis le stockage] ».

## Gestion des erreurs

Lorsqu’il comporte une erreur avec un déclencheur instantané, le scénario :

* s’arrête immédiatement — lorsque le scénario est configuré pour s’exécuter [!UICONTROL Immédiatement] ;
* s’arrête après 3 tentatives infructueuses (3 erreurs) — lorsque le scénario est configuré pour s’exécuter comme planifié.

Si une erreur se produit pendant l’exécution du scénario, le webhook est replacé dans la file d’attente pendant la phase de restauration du déclencheur instantané. Dans ce cas, vous avez la possibilité de corriger le scénario et de le réexécuter. Pour plus d’informations, voir [Restauration](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) dans l’article [Exécution, cycles et phases du scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si votre scénario comporte un module de réponse webhook, l’erreur est envoyée à la réponse webhook. Le module de réponse webhook est toujours exécuté en dernier (dans le cas où l’option [!UICONTROL Validation automatique] dans les paramètres du scénario n’est pas activée). Pour plus d’informations, voir [Répondre aux webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) dans l’article [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhooks personnalisés

Vous pouvez créer vos propres webhooks. Pour plus d’informations, voir [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Désactivation de webhook

Les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

* Le webhook n’a été connecté à aucun scénario depuis plus de 5 jours.
* Le webhook est utilisé uniquement dans les scénarios inactifs, qui sont inactifs depuis plus de 30 jours.

Les webhooks désactivés sont supprimés et désinscrits automatiquement s’ils ne sont connectés à aucun scénario et s’ils sont restés désactivés pendant plus de 30 jours.


