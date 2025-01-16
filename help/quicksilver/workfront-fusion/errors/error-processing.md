---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Traiter les erreurs dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 94%

---

# Traitement des erreurs dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Types d’erreur](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/error-processing.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Il arrive qu’une erreur se produise pendant l’exécution d’un scénario. Cela se produit généralement lorsqu’un service n’est pas disponible en raison d’un échec de connexion à un service ou d’un échec de validation. Cet article traite des erreurs courantes que vous pouvez rencontrer.

[!DNL Adobe Workfront Fusion] fait la distinction entre plusieurs types d’erreurs de base. Il réagira différemment en fonction du type d’erreur qui s’est produite.

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erreur de connexion

`ConnectionError`

L’erreur de connexion est l’une des erreurs les plus courantes, généralement causée par l’indisponibilité du service tiers pour diverses raisons (surcharge, maintenance, panne, etc.). Le traitement par défaut de cette erreur dépend du module sur lequel elle a été rencontrée :

* Si l’erreur se produit dans le premier module, l’exécution du scénario est interrompue par un message d’avertissement. [!DNL Workfront Fusion] tente ensuite à plusieurs reprises de réexécuter le scénario à des intervalles de temps croissants (ceux-ci sont expliqués ci-dessous). Si toutes les tentatives échouent, [!DNL Workfront Fusion] désactive le scénario.
* Si l’erreur de connexion se produit sur un autre module que le premier, les étapes suivantes dépendent de l’option [Autoriser le stockage d’exécutions incomplètes](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) dans les paramètres avancés du scénario :

   * Si cette option est activée, l’exécution du scénario est déplacée vers le dossier [!UICONTROL Exécutions incomplètes] où [!DNL Workfront Fusion] tente à plusieurs reprises de réexécuter le scénario à des intervalles de temps de plus en plus longs. Si toutes les tentatives échouent, l’exécution restera dans le dossier des exécutions incomplètes en attendant une résolution manuelle par la personne.

     Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre les exécutions incomplètes dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Si cette option est désactivée, l’exécution du scénario se termine par une erreur suivie d’une phase de restauration. [!DNL Workfront Fusion] tente ensuite à plusieurs reprises de réexécuter le scénario à des intervalles de temps de plus en plus longs. Si toutes les tentatives échouent, [!DNL Workfront Fusion] désactive le scénario.

### Intervalles de temps de plus en plus longs

L’algorithme consistant à allonger de façon multiplicative les intervalles de temps entre les tentatives lorsqu’une erreur se produit est connu sous le nom de backoff exponentiel. Les intervalles de temps de plus en plus longs sont définis comme suit :

1. 10 minutes
1. 1 heure
1. 3 heures
1. 12 heures
1. 24 heures

La raison principale de l’utilisation d&#39;intervalles de temps de plus en plus longs dans [!DNL Workfront Fusion] est d’éviter que les scénarios fréquemment exécutés ne consomment des opérations sur des tentatives qui échouent à plusieurs reprises.

>[!INFO]
>
>**Exemple :**
>
>Un scénario contient le déclencheur [!DNL Google Sheets] [!UICONTROL Surveiller des lignes]. [!DNL Google Sheets] est indisponible pendant 30 minutes pour cause de maintenance lorsque [!DNL Workfront Fusion] démarre le scénario, et ne peut donc pas récupérer de nouvelles lignes. Le scénario s’arrête et tente un nouvel essai 10 minutes après. Comme [!DNL Google Sheets] n’est toujours pas disponible, [!DNL Workfront Fusion] n’est toujours pas en mesure d’obtenir des informations sur les nouvelles lignes. La prochaine exécution du scénario est prévue dans 1 heure. [!DNL Google Sheets] est à nouveau disponible à ce moment-là, et le scénario s’exécute avec succès.

## Erreur de données

`DataError`

Une erreur de données est générée lorsqu’un élément est incorrectement mappé et ne passe pas la validation effectuée du côté de [!DNL Workfront Fusion] ou du côté du service tiers utilisé.

Si cette erreur se produit, le scénario, jusqu’à l’endroit où le module a échoué, est déplacé dans le dossier des exécutions incomplètes où vous pouvez résoudre le problème. Cependant, le scénario ne s’arrête pas et continue à s’exécuter selon son planning. Pour arrêter l’exécution du scénario lorsque Erreur de données apparaît, activez l’option Traitement séquentiel dans le panneau des paramètres du scénario.

Si vous n’avez pas activé l’option [!UICONTROL Autoriser le stockage d’exécutions incomplètes] dans les paramètres du scénario, l’exécution du scénario se termine par une erreur et une restauration est effectuée.

Pour plus d’informations sur le mappage, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre les exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Pour plus d’informations sur le panneau des paramètres du scénario, voir [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Pour plus d’informations sur les planifications, voir [Planifier un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Erreur de données dupliquées

`DuplicateDataError`

Si [!DNL Workfront Fusion] tente d’insérer deux fois le même lot dans un service qui n’autorise pas les données dupliquées, une erreur de données dupliquées est générée. Si cette erreur se produit, [!DNL Workfront Fusion] procède de la même manière que pour l’erreur de données.

## Erreur de jeton d’accès invalide

`InvalidAccessTokenError`

Une erreur de jeton d’accès invalide se produit lorsque [!DNL Workfront Fusion] ne peut pas accéder à votre compte enregistré auprès d’un service tiers. Cela se produit généralement lorsque vous révoquez les droits d’accès à [!DNL Workfront Fusion] dans l’administration d’un service donné, mais que les scénarios connexes continuent de s’exécuter selon le planning prévu.

Si cette erreur se produit, l’exécution d’un scénario est immédiatement interrompue. Le reste du scénario, à partir du module où l’erreur s’est produite, est déplacé dans le dossier des exécutions incomplètes.

Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre les exécutions incomplètes dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Erreur de limite de taux

`RateLimitError`

Si une limite fixée par un service donné est dépassée, une erreur de limite de taux est générée. Si cette erreur se produit, [!DNL Workfront Fusion] procède de la même manière que pour l’erreur de connexion.

Pour plus d’informations, voir [Erreur de connexion](#connection-error).

## Erreur de données incomplètes

`IncompleteDataError`

Une erreur de données incomplètes ne se produit qu’avec des déclencheurs. Cette erreur est générée si un déclencheur ne parvient pas à télécharger les données requises à partir d’un service donné.

Si un scénario se termine par l’erreur `IncompleteDataError`, son comportement ultérieur dépendra du paramètre [!UICONTROL Nombre maximal d’erreurs consécutives].

Pour plus d’informations, voir [Nombre d’erreurs consécutives](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) dans l’article [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exemple :**
>
>Dans un scénario, le déclencheur [!DNL Workfront] [!UICONTROL Surveiller l’enregistrement] est défini pour surveiller les documents. Le scénario s’exécute pendant que vous téléchargez un document volumineux, tel qu’une longue vidéo. Étant donné que [!UICONTROL Workfront Fusion] tente de télécharger la vidéo alors qu’elle est encore en cours de chargement sur Workfront, le scénario se termine par l’erreur `IncompleteDataError`.

## Erreur d’exécution

`RuntimeError`

Si une autre erreur (non mentionnée ci-dessus) apparaît pendant l’exécution du scénario, elle est signalée comme `RunTimeError`.

Si un scénario se termine par l’erreur `RuntimeError`, son comportement ultérieur dépendra du paramètre [!UICONTROL Nombre maximal d’erreurs consécutives]. Pour plus d’informations, voir [Nombre d’erreurs consécutives](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) dans l’article [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Si un scénario commence par un déclenchement instantané, le paramètre [!UICONTROL Nombre maximal d’erreurs consécutives] est ignoré et le scénario est désactivé immédiatement après l’apparition de la première erreur. Pour plus d’informations, voir [Déclencheurs instantanés](../../workfront-fusion/modules/module-types.md#instant) dans l’article [Types de modules](../../workfront-fusion/modules/module-types.md).

## Erreur d’incohérence

`InconsistencyError`

Si l’une des erreurs décrites ci-dessus se produit pendant la phase d’engagement ou de restauration, le scénario se termine par une erreur d’incohérence. Pour plus d’informations, voir [Exécution du scénario, cycles et phases dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si cette erreur apparaît dans un scénario, l’exécution de celui-ci est immédiatement interrompue.

## Avertissement

Lors de l’exécution d’un scénario, vous pouvez recevoir un avertissement vous informant d’un problème. Toutefois, cela n’empêche pas le scénario de se dérouler avec succès.

Par exemple, un avertissement peut apparaître lorsque la taille maximale autorisée des fichiers est dépassée et que l’option [!UICONTROL Activer la perte de données] est désactivée. Pour plus d’informations, voir [Activer la perte de données](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) dans l’article [Panneau des paramètres de scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
