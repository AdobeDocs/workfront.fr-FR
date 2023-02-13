---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]
description: Cet article décrit les directives que vous pouvez utiliser pour la gestion des erreurs dans votre [!DNL Adobe Workfront Fusion] scénarios.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 50b43cd4bafdfc3379eb1d73c12e15c791e28dbe
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Directives de gestion des erreurs

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Retour arrière</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>L’exécution du scénario est arrêtée immédiatement et une <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Retour arrière</a> est lancée sur tous les modules afin de les rétablir à leur état initial. Les modules suivants ne sont pas traités.</p> <p>Sauf quelques types d’erreur, le scénario est désactivé après le nombre d’erreurs consécutives spécifiées dans les paramètres du scénario. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Nombre d'erreurs consécutives</a>.</p> <p>L’état d’exécution du scénario est marqué comme "erreur".</p> <p>Remarque : Il s’agit du comportement par défaut si aucun itinéraire de gestionnaire d’erreur n’est associé au module et à la variable <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Autoriser le stockage des exécutions incomplètes]</a> n’est pas coché sous [!UICONTROL Paramètres du scénario].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Valider</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>L’exécution du scénario est arrêtée immédiatement et une phase de validation est lancée sur tous les modules. Les modules suivants ne sont pas traités.</p> <p>Tous les lots non traités sont ignorés.</p> <p>L’état d’exécution du scénario est marqué comme "succès". Pour plus d’informations sur les phases de validation, voir <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Commit</a> dans l’article <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Exécution de scénarios, cycles et phases dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reprendre</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Une sortie de substitution est spécifiée et fournie au module qui rencontre une erreur.</p> <p>Les modules suivants sont traités.</p> <p>L’état d’exécution du scénario est marqué comme "succès".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorer</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>L’erreur est ignorée et les modules suivants ne sont pas traités.</p> <p>S’il existe des lots non traités, l’exécution du scénario se poursuit normalement.</p> <p>L’état d’exécution du scénario est marqué comme "succès".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Rompre</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>L’état de l’exécution du scénario est stocké dans la file d’attente des exécutions incomplètes où l’erreur peut être résolue manuellement. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Affichage et résolution d’exécutions incomplètes dans Adobe Workfront Fusion</a>. </p> <p>Il existe cependant quelques exceptions. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Autoriser le stockage d’exécutions incomplètes</a> dans l’article <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Panneau des paramètres du scénario dans Adobe Workfront Fusion</a>.</p> <p>Les modules suivants ne sont pas traités.</p> <p>S’il existe des lots non traités, l’exécution du scénario se poursuit normalement.</p> <p>L’état d’exécution du scénario est marqué comme "avertissement" lorsque l’option [!UICONTROL Terminer automatiquement l’exécution] est désactivée.</p> <p>Voir <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> pour plus d’informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Réessayer</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>Dans certains cas, il peut s’avérer utile de réexécuter un module en échec pendant deux ou trois fois lorsqu’il est possible que la raison de l’échec soit dépassée au fil du temps.</p> <p>Workfront Fusion ne propose actuellement pas la directive Retry (Réessayer), bien que plusieurs solutions puissent être utilisées pour imiter ses fonctionnalités. Pour plus d’informations, voir <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Réessayer la gestion des erreurs dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Actuellement, les directives de gestion des erreurs ne peuvent pas être utilisées en dehors de la portée d’un itinéraire de gestion des erreurs et [!DNL Workfront Fusion] ne propose actuellement pas de module Throw qui vous permettrait de générer facilement des erreurs (de génération) de manière conditionnelle, bien qu’une solution puisse être utilisée pour imiter ses fonctionnalités. Pour plus d’informations, voir [Itinéraire du gestionnaire d’erreurs](../../workfront-fusion/errors/error-handling.md#error) dans l’article [Gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md). Voir aussi [Solution de contournement pour le lancement](../../workfront-fusion/errors/throw.md#workarou) dans l’article [Gestion des erreurs de lancement dans Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Rompre {#break}

Lorsqu’une erreur est traitée par la variable [!DNL Break] , un enregistrement est créé dans la variable [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) qui stocke l’état de l’exécution du scénario avec les données des modules précédents. Pour chaque lot de données à l’origine de l’erreur, un enregistrement distinct est créé.

L’enregistrement fait référence au module d’origine de l’erreur et contient des informations sur les données reçues par le module en tant qu’entrée. Pour plus d’informations, voir [Affichage et résolution d’exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Ici, vous pouvez résoudre l’erreur manuellement en mettant à jour le scénario (si nécessaire) et en l’exécutant une fois.

En revanche, en activant la variable [!UICONTROL Exécution terminée automatiquement] sous les paramètres de la directive Break, elle peut être configurée pour traiter automatiquement une exécution incomplète en exécutant à nouveau le scénario après le nombre de minutes spécifié.

Lorsque cette option est activée, lorsqu’une erreur se produit, l’exécution incomplète est récupérée (après l’heure indiquée dans la variable [!UICONTROL Intervalle entre les tentatives] ) et exécutés avec les données d’entrée d’origine. Cette opération se répète jusqu’à ce que l’exécution du module se termine sans erreur ou jusqu’à ce que le Nombre de tentatives spécifié soit atteint.

>[!NOTE]
>
>Si la tentative initiale de reprise échoue, l’intervalle entre les reprises augmente de manière exponentielle toutes les autres tentatives.

Lorsque l’option &quot;Exécution terminée automatiquement&quot; est activée, l’exécution du scénario est marquée comme &quot;Succès&quot;, car la reprise automatique du gestionnaire d’erreurs de coupure gère automatiquement le problème. Dans ce cas, les utilisateurs ne reçoivent pas d’e-mail sur l’exécution ayant échoué.

Lorsque &quot;Exécution terminée automatiquement&quot; est désactivée, l’exécution est marquée comme &quot;Avertissement&quot;.

![](assets/break-directive-350x241.png)

Toutefois, il existe certaines exceptions aux exécutions stockées sous Exécution incomplète et, avec certains types d’erreur, la reprise automatique d’une exécution de scénario n’est pas possible. Pour plus d’informations, voir [Autoriser le stockage d’exécutions incomplètes](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) dans l’article [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Pour plus d’informations, voir [Gestion avancée des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
