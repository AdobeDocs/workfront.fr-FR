---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Traitement des erreurs dans [!DNL Adobe Workfront Fusion]
description: Il arrive qu’une erreur se produise lors de l’exécution d’un scénario. Cela se produit généralement si un service n’est pas disponible en raison d’un échec de connexion à un service ou si une validation échoue. Cet article présente les erreurs courantes que vous pouvez rencontrer.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# Traitement des erreurs dans [!DNL Adobe Workfront Fusion]

Il arrive qu’une erreur se produise lors de l’exécution d’un scénario. Cela se produit généralement si un service n’est pas disponible en raison d’un échec de connexion à un service ou si une validation échoue. Cet article présente les erreurs courantes que vous pouvez rencontrer.

[!DNL Adobe Workfront Fusion] fait la distinction entre plusieurs types d’erreur de base. Il réagira différemment selon le type d’erreur qui s’est produit.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erreur de connexion

`ConnectionError`

L’erreur de connexion est l’une des erreurs les plus courantes causées par l’indisponibilité du service tiers pour diverses raisons (surcharge, maintenance, panne, etc.). La gestion par défaut de cette erreur dépend du module sur lequel elle a été rencontrée :

* Si l’erreur se produit sur le premier module, l’exécution du scénario est arrêtée avec un message d’avertissement. [!DNL Workfront Fusion] puis tente à plusieurs reprises de réexécuter le scénario à des intervalles de temps croissants (comme expliqué ci-dessous). Si toutes les tentatives échouent, [!DNL Workfront Fusion] désactive le scénario.
* Si l’erreur de connexion se produit sur un autre module que le premier, les étapes suivantes dépendent de la variable [Autoriser le stockage d’exécutions incomplètes](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) dans les paramètres avancés du scénario :

   * Si cette option est activée, l’exécution du scénario est déplacée vers le [!UICONTROL Exécutions incomplètes] dossier où [!DNL Workfront Fusion] tente de manière répétée de réexécuter le scénario à des intervalles de temps accrus. Si toutes les tentatives échouent, l’exécution reste dans le dossier Exécutions incomplètes en attente d’une résolution manuelle de l’utilisateur.

     Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Si cette option est désactivée, l’exécution du scénario se termine par une erreur suivie d’une phase de restauration. [!DNL Workfront Fusion] puis tente à plusieurs reprises de réexécuter le scénario à des intervalles de temps plus importants. Si toutes les tentatives échouent, [!DNL Workfront Fusion] désactive le scénario.

### Augmentation des intervalles de temps

L’algorithme d’intervalles de temps multipliés par plusieurs entre les tentatives lorsqu’une erreur se produit est appelé backoff exponentiel. Les intervalles de temps croissants sont définis comme suit :

1. 10 minutes
1. 1 heure
1. 3 heures
1. 12 heures
1. 24 heures

La raison principale pour laquelle les intervalles de temps augmentent [!DNL Workfront Fusion] empêche les scénarios fréquemment exécutés de consommer des opérations lors de tentatives répétées d’échec.

>[!INFO]
>
>**Exemple:**
>
>Un scénario contient la variable [!DNL Google Sheets] trigger [!UICONTROL Lignes de contrôle]. [!DNL Google Sheets] est indisponible pendant 30 minutes en raison de la maintenance lorsque [!DNL Workfront Fusion] démarre le scénario, de sorte qu’il ne peut pas récupérer de nouvelles lignes. Le scénario s’arrête et réessaye dans 10 minutes. Parce que [!DNL Google Sheets] est toujours indisponible, [!DNL Workfront Fusion] ne peut toujours pas obtenir d’informations sur les nouvelles lignes. La prochaine exécution du scénario est planifiée dans 1 heure. [!DNL Google Sheets] est à nouveau disponible à ce moment et le scénario s’exécute correctement.

## Erreur de données

`DataError`

Une erreur de données est générée lorsqu’un élément est incorrectement mappé et ne transmet pas la validation effectuée sur l’événement [!DNL Workfront Fusion] côté ou côté du service tiers utilisé.

Si cette erreur se produit, le scénario, jusqu’à l’emplacement où le module a échoué, est déplacé vers le dossier des exécutions incomplètes où vous pouvez résoudre le problème. Cependant, le scénario ne s’arrête pas et continue de s’exécuter selon son planning. Pour arrêter l’exécution du scénario lorsque l’erreur Données s’affiche, activez l’option Traitement séquentiel dans le panneau Paramètres du scénario .

Si vous n’avez pas activé la variable [!UICONTROL Autoriser le stockage d’exécutions incomplètes] dans les paramètres du scénario, l’exécution du scénario se termine par l’erreur et une restauration est effectuée.

Pour plus d’informations sur le mappage, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Pour plus d’informations sur les exécutions incomplètes, voir [Affichage et résolution d’exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Pour plus d’informations sur le panneau des paramètres du scénario, voir [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Pour plus d’informations sur les plannings, voir [Planification d’un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Erreur de duplication des données

`DuplicateDataError`

If [!DNL Workfront Fusion] tente d’insérer le même lot deux fois dans un service qui n’autorise pas la duplication des données ; une erreur de duplication des données est générée. Si cette erreur se produit, [!DNL Workfront Fusion] fonctionne de la même manière que pour l’erreur de données.

## Erreur de jeton d’accès non valide

`InvalidAccessTokenError`

Une erreur de jeton d’accès non valide se produit lorsque [!DNL Workfront Fusion] ne peut pas accéder à votre compte enregistré auprès d’un service tiers. Cela se produit généralement lorsque vous révoquez des droits d’accès pour [!DNL Workfront Fusion] dans l’administration d’un service donné, mais les scénarios connexes continuent de s’exécuter conformément au planning.

Si cette erreur se produit, l’exécution d’un scénario est immédiatement arrêtée. Le reste du scénario commençant à partir du module où l’erreur s’est produite est déplacé vers le dossier des exécutions incomplètes.

Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Erreur de limite de taux

`RateLimitError`

Si une limite définie par un service donné est dépassée, une erreur de limite de taux est générée. Si cette erreur se produit, [!DNL Workfront Fusion] se déroule de la même manière que pour l’erreur de connexion.

Pour plus d’informations, voir [Erreur de connexion](#connection-error).

## Erreur de données incomplète

`IncompleteDataError`

Une erreur de données incomplète se produit uniquement avec les déclencheurs. Cette erreur est générée si un déclencheur ne parvient pas à télécharger les données requises à partir d’un service donné.

Si un scénario se termine par la variable `IncompleteDataError`, son comportement supplémentaire dépendra de la définition de la variable [!UICONTROL Nombre max. d&#39;erreurs consécutives].

Pour plus d’informations, voir [Nombre d&#39;erreurs consécutives](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) dans l’article [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exemple:**
>
>Un scénario comprend la variable [!DNL Workfront] trigger [!UICONTROL Surveiller les enregistrements] configuré pour surveiller les documents. Le scénario s’exécute pendant le téléchargement d’un document volumineux, tel qu’une longue vidéo. Parce que [!UICONTROL Workfront Fusion] tente de télécharger la vidéo alors qu’elle est toujours téléchargée vers Workfront. Le scénario se termine par la variable `IncompleteDataError`.

## Erreur d’exécution

`RuntimeError`

Si une autre erreur (non mentionnée ci-dessus) s’affiche lors de l’exécution du scénario, elle est signalée comme `RunTimeError`.

Si un scénario se termine par la variable `RuntimeError`, son comportement supplémentaire dépendra de la définition de la variable [!UICONTROL Nombre max. d&#39;erreurs consécutives]. Pour plus d’informations, voir [Nombre d&#39;erreurs consécutives](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) dans l’article [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Si un scénario commence par un déclencheur instantané, le paramètre de [!UICONTROL Nombre max. d&#39;erreurs consécutives] est ignorée et le scénario est désactivé immédiatement une fois la première erreur survenue. Pour plus d’informations, voir [Déclencheurs instantanés](../../workfront-fusion/modules/module-types.md#instant) dans l’article [Types de modules](../../workfront-fusion/modules/module-types.md).

## Erreur d’incohérence

`InconsistencyError`

Si une erreur décrite ci-dessus se produit pendant la phase de validation ou de restauration, un scénario se termine par une erreur d’incohérence. Pour plus d’informations, voir [Exécution de scénarios, cycles et phases dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Si cette erreur apparaît dans un scénario, l’exécution du scénario est immédiatement arrêtée.

## Avertissement

Lors de l’exécution d’un scénario, un avertissement vous informe d’un problème. Toutefois, cela n’empêche pas la réalisation du scénario.

Par exemple, un avertissement peut s’afficher lorsque la taille de fichier maximale autorisée est dépassée et que la variable [!UICONTROL Perte de données] est désactivée. Pour plus d’informations, voir [Perte de données](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) dans l’article [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
