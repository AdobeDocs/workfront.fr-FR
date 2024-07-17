---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Traitement des erreurs dans  [!DNL Adobe Workfront Fusion]
description: Il arrive qu’une erreur se produise lors de l’exécution d’un scénario. Cela se produit généralement si un service n’est pas disponible en raison d’un échec de connexion à un service ou si une validation échoue. Cet article présente les erreurs courantes que vous pouvez rencontrer.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 10%

---

# Traitement des erreurs dans [!DNL Adobe Workfront Fusion]

Il arrive qu’une erreur se produise lors de l’exécution d’un scénario. Cela se produit généralement si un service n’est pas disponible en raison d’un échec de connexion à un service ou si une validation échoue. Cet article présente les erreurs courantes que vous pouvez rencontrer.

[!DNL Adobe Workfront Fusion] fait la distinction entre plusieurs types d’erreur de base. Il réagira différemment selon le type d’erreur qui s’est produit.

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
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## Erreur de connexion

`ConnectionError`

L’erreur de connexion est l’une des erreurs les plus courantes causées par l’indisponibilité du service tiers pour diverses raisons (surcharge, maintenance, panne, etc.). La gestion par défaut de cette erreur dépend du module sur lequel elle a été rencontrée :

* Si l’erreur se produit sur le premier module, l’exécution du scénario est arrêtée avec un message d’avertissement. [!DNL Workfront Fusion] tente ensuite à plusieurs reprises de réexécuter le scénario à des intervalles de temps croissants (ces informations sont expliquées ci-dessous). Si toutes les tentatives échouent, [!DNL Workfront Fusion] désactive le scénario.
* Si l’erreur de connexion se produit sur un autre module que le premier, les étapes suivantes dépendent de l’option [Autoriser le stockage des exécutions incomplètes](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) dans les paramètres avancés du scénario :

   * Si cette option est activée, l’exécution du scénario est déplacée vers le dossier [!UICONTROL Exécutions incomplètes] où [!DNL Workfront Fusion] tente à plusieurs reprises de réexécuter le scénario à des intervalles de temps croissants. Si toutes les tentatives échouent, l’exécution reste dans le dossier Exécutions incomplètes en attente d’une résolution manuelle de l’utilisateur.

     Pour plus d’informations sur les exécutions incomplètes, voir [Affichage et résolution des exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Si cette option est désactivée, l’exécution du scénario se termine par une erreur suivie d’une phase de restauration. [!DNL Workfront Fusion] tente ensuite à plusieurs reprises de réexécuter le scénario à des intervalles de temps plus importants. Si toutes les tentatives échouent, [!DNL Workfront Fusion] désactive le scénario.

### Augmentation des intervalles de temps

L’algorithme d’intervalles de temps multipliés par plusieurs entre les tentatives lorsqu’une erreur se produit est appelé backoff exponentiel. Les intervalles de temps croissants sont définis comme suit :

1. 10 minutes
1. 1 heure
1. 3 heures
1. 12 heures
1. 24 heures

La principale raison pour laquelle vous utilisez des intervalles de temps croissants dans [!DNL Workfront Fusion] est d’empêcher les scénarios fréquemment exécutés de consommer les opérations lors de tentatives répétées d’échec.

>[!INFO]
>
>**Exemple :**
>
>Un scénario contient le déclencheur [!DNL Google Sheets] [!UICONTROL Watch Rows]. [!DNL Google Sheets] n’est pas disponible pendant 30 minutes en raison de la maintenance lorsque [!DNL Workfront Fusion] démarre le scénario. Il ne peut donc pas récupérer de nouvelles lignes. Le scénario s’arrête et réessaye dans 10 minutes. [!DNL Google Sheets] n’étant toujours pas disponible, [!DNL Workfront Fusion] ne peut toujours pas obtenir d’informations sur les nouvelles lignes. La prochaine exécution du scénario est planifiée dans 1 heure. [!DNL Google Sheets] est à nouveau disponible à ce moment et le scénario s’exécute correctement.

## Erreur de données

`DataError`

Une erreur de données est générée lorsqu’un élément est incorrectement mappé et ne transmet pas la validation effectuée du côté [!DNL Workfront Fusion] ou du côté du service tiers utilisé.

Si cette erreur se produit, le scénario, jusqu’à l’emplacement où le module a échoué, est déplacé vers le dossier des exécutions incomplètes où vous pouvez résoudre le problème. Cependant, le scénario ne s’arrête pas et continue de s’exécuter selon son planning. Pour arrêter l’exécution du scénario lorsque l’erreur Données s’affiche, activez l’option Traitement séquentiel dans le panneau Paramètres du scénario .

Si vous n’avez pas activé l’option [!UICONTROL Autoriser le stockage des exécutions incomplètes] dans les paramètres du scénario, l’exécution du scénario se termine par l’erreur et une restauration est effectuée.

Pour plus d&#39;informations sur le mappage, voir [Mappage des informations d&#39;un module vers un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Pour plus d’informations sur les exécutions incomplètes, voir [Affichage et résolution des exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Pour plus d’informations sur le panneau des paramètres du scénario, voir [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Pour plus d’informations sur les plannings, voir [Planification d’un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Erreur de duplication des données

`DuplicateDataError`

Si [!DNL Workfront Fusion] tente d&#39;insérer le même lot deux fois dans un service qui n&#39;autorise pas les données en double, une erreur de données en double est générée. Si cette erreur se produit, [!DNL Workfront Fusion] continue de la même manière que pour l’erreur de données.

## Erreur de jeton d’accès non valide

`InvalidAccessTokenError`

Une erreur de jeton d’accès non valide se produit lorsque [!DNL Workfront Fusion] ne peut pas accéder à votre compte enregistré avec un service tiers. Cela se produit généralement lorsque vous révoquez les droits d’accès pour [!DNL Workfront Fusion] dans l’administration d’un service donné, mais les scénarios associés continuent à s’exécuter conformément au planning.

Si cette erreur se produit, l’exécution d’un scénario est immédiatement arrêtée. Le reste du scénario commençant à partir du module où l’erreur s’est produite est déplacé vers le dossier des exécutions incomplètes.

Pour plus d’informations sur les exécutions incomplètes, voir [Affichage et résolution des exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Erreur de limite de taux

`RateLimitError`

Si une limite définie par un service donné est dépassée, une erreur de limite de taux est générée. Si cette erreur se produit, [!DNL Workfront Fusion] continue de la même manière que pour l’erreur de connexion.

Pour plus d’informations, voir [Erreur de connexion](#connection-error).

## Erreur de données incomplète

`IncompleteDataError`

Une erreur de données incomplète se produit uniquement avec les déclencheurs. Cette erreur est générée si un déclencheur ne parvient pas à télécharger les données requises à partir d’un service donné.

Si un scénario se termine par le `IncompleteDataError`, son comportement supplémentaire dépendra de son paramètre de [!UICONTROL Nombre max d&#39;erreurs consécutives].

Pour plus d’informations, voir [Nombre d’erreurs consécutives](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) dans l’article [Panneau des paramètres de scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exemple :**
>
>Dans un scénario, le déclencheur [!DNL Workfront] [!UICONTROL Watch Record] est défini pour surveiller les documents. Le scénario s’exécute pendant le téléchargement d’un document volumineux, tel qu’une longue vidéo. Comme [!UICONTROL Workfront Fusion] tente de télécharger la vidéo alors qu’elle est toujours en cours de téléchargement vers Workfront, le scénario se termine par le `IncompleteDataError`.

## Erreur d’exécution

`RuntimeError`

Si une autre erreur (non mentionnée ci-dessus) s’affiche lors de l’exécution du scénario, elle est signalée sous la forme `RunTimeError`.

Si un scénario se termine par le `RuntimeError`, son comportement supplémentaire dépendra de son paramètre de [!UICONTROL Nombre max d&#39;erreurs consécutives]. Pour plus d’informations, voir [Nombre d’erreurs consécutives](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) dans l’article [Panneau des paramètres de scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Si un scénario commence par un déclencheur instantané, le paramètre [!UICONTROL Nombre max d’erreurs consécutives] est ignoré et le scénario est désactivé immédiatement une fois la première erreur survenue. Pour plus d’informations, voir [Instant Triggers](../../workfront-fusion/modules/module-types.md#instant) dans l’article [Types de modules](../../workfront-fusion/modules/module-types.md).

## Erreur d’incohérence

`InconsistencyError`

Si une erreur décrite ci-dessus se produit pendant la phase de validation ou de restauration, un scénario se termine par une erreur d’incohérence. Pour plus d’informations, voir [Exécution de scénario, cycles et phases dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si cette erreur apparaît dans un scénario, l’exécution du scénario est immédiatement arrêtée.

## Avertissement

Lors de l’exécution d’un scénario, un avertissement vous informe d’un problème. Toutefois, cela n’empêche pas la réalisation du scénario.

Par exemple, un avertissement peut s’afficher lorsque la taille de fichier maximale autorisée est dépassée et que l’option [!UICONTROL Activer la perte de données] est désactivée. Pour plus d’informations, voir [Activer la perte de données](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) dans l’article [Panneau des paramètres de scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
