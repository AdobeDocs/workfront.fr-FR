---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]
description: Cet article décrit les directives que vous pouvez utiliser pour la gestion des erreurs dans vos scénarios  [!DNL Adobe Workfront Fusion] .
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 24%

---

# Directives pour la gestion des erreurs dans [!DNL Adobe Workfront Fusion]

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

## Directives de gestion des erreurs

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Restaurer</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>L’exécution du scénario est arrêtée immédiatement et une phase de <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">restauration</a> est lancée sur tous les modules afin de tenter de les rétablir à leur état initial. Les modules suivants ne sont pas traités.</p> <p>Sauf quelques types d’erreur, le scénario est désactivé après le nombre d’erreurs consécutives spécifiées dans les paramètres du scénario. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Nombre d’erreurs consécutives</a>.</p> <p>Le statut d’exécution du scénario est marqué comme « erreur ».</p> <p>Remarque : Il s’agit du comportement par défaut si aucun itinéraire de gestionnaire d’erreurs n’est associé au module et que le paramètre <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Autoriser le stockage des exécutions incomplètes]</a> sous [!UICONTROL Paramètres du scénario] n’est pas coché.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Valider</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>L’exécution du scénario est arrêtée immédiatement et une phase de validation est lancée sur tous les modules. Les modules suivants ne sont pas traités.</p> <p>Tous les lots non traités sont ignorés.</p> <p>L’état d’exécution du scénario est marqué comme "succès". Pour plus d’informations sur les phases de validation, voir <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Validation</a> dans l’article <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Exécution de scénario, cycles et phases dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reprendre</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Une sortie de substitution est spécifiée et fournie au module qui rencontre une erreur.</p> <p>Les modules suivants sont traités.</p> <p>Le statut d’exécution du scénario est marqué comme « succès ».</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorer</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>L’erreur est ignorée et les modules suivants ne sont pas traités.</p> <p>S’il existe des bundles non traités, l’exécution du scénario se poursuit normalement.</p> <p>Le statut d’exécution du scénario est marqué comme « succès ».</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Interrompre</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>Le statut de l’exécution du scénario est stocké dans la file d’attente des exécutions incomplètes où l’erreur peut être résolue manuellement. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Affichage et résolution d’exécutions incomplètes dans Adobe Workfront Fusion</a>. </p> <p>Il y a cependant quelques exceptions. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Autoriser le stockage d’exécutions incomplètes</a> dans l’article <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Panneau des paramètres de scénario dans Adobe Workfront Fusion</a>.</p> <p>Les modules suivants ne sont pas traités.</p> <p>S’il existe des bundles non traités, l’exécution du scénario se poursuit normalement.</p> <p>L’état d’exécution du scénario est marqué comme "avertissement" lorsque l’option [!UICONTROL Terminer automatiquement l’exécution] est désactivée.</p> <p>Pour plus d’informations, voir la section <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> ci-dessous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Réessayer</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>Dans certains cas, il peut s’avérer utile de réexécuter un module en échec pendant deux ou trois fois lorsqu’il est possible que la raison de l’échec soit dépassée au fil du temps.</p> <p>Workfront Fusion ne propose actuellement pas la directive Retry (Réessayer), bien que plusieurs solutions puissent être utilisées pour imiter ses fonctionnalités. Pour plus d’informations, voir <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Gestion des erreurs de reprise dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Actuellement, les directives de gestion des erreurs ne peuvent pas être utilisées en dehors d’un itinéraire de gestion des erreurs.
>
>   Pour plus d’informations, voir [Route du gestionnaire d’erreurs](../../workfront-fusion/errors/error-handling.md#error) dans l’article [Gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] ne propose actuellement pas de module Throw qui vous permettrait de générer facilement (générer) des erreurs de manière conditionnelle, bien qu’une solution puisse être utilisée pour imiter ses fonctionnalités.
>
>   Pour plus d’informations, reportez-vous à la section [Solution pour Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw) de l’article [Gestion des erreurs de lancement dans Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Interrompre {#break}

Lorsqu’une erreur est traitée par la directive [!DNL Break], un enregistrement est créé dans le dossier Exécutions incomplètes . Cet enregistrement stocke l’état d’exécution du scénario, ainsi que les données des modules précédents. L’enregistrement fait référence au module d’origine de l’erreur et contient des informations sur les données reçues par le module en tant qu’entrée. Pour chaque lot de données à l’origine de l’erreur, un enregistrement distinct est créé.

Pour plus d’informations, voir [Affichage et résolution d’exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Résolution des erreurs résultant de la directive Break

Vous pouvez résoudre l’erreur manuellement en mettant à jour le scénario (si nécessaire) et en l’exécutant une seule fois.

Vous pouvez également configurer le scénario pour qu’il traite automatiquement une exécution incomplète en exécutant à nouveau le scénario. Pour configurer le module afin de traiter les exécutions incomplètes :

1. Dans le module Break, activez l’option [!UICONTROL **Exécuter automatiquement**] .
1. Dans le champ **Nombre de tentatives** , saisissez ou mappez le nombre maximal de tentatives que vous souhaitez que le module tente de relancer l’exécution.

   Ce nombre doit être compris entre 1 et 100.
1. Dans le champ **Intervalle entre les tentatives** , saisissez ou mappez le nombre de minutes entre chaque tentative de nouvelle tentative.

Lorsque cette option est activée, lorsqu’une erreur se produit, l’exécution incomplète est récupérée (après le temps spécifié dans le champ [!UICONTROL Intervalle entre les tentatives]) et exécutée avec les données d’entrée d’origine. Cette opération se répète jusqu’à ce que l’exécution du module se termine sans erreur ou jusqu’à ce que le Nombre de tentatives spécifié soit atteint.

>[!NOTE]
>
>Si la tentative initiale de reprise échoue, l’intervalle entre les reprises augmente de manière exponentielle toutes les autres tentatives.


Lorsque l’option &quot;Exécution terminée automatiquement&quot; est activée, l’exécution du scénario est marquée comme &quot;Succès&quot;, car la reprise automatique du gestionnaire d’erreurs de coupure gère automatiquement le problème. Dans ce cas, les utilisateurs ne reçoivent pas d’e-mail sur l’exécution ayant échoué.

Lorsque &quot;Exécution terminée automatiquement&quot; est désactivée, l’exécution est marquée comme &quot;Avertissement&quot;.

Il existe certaines exceptions aux exécutions stockées sous Exécution incomplète et, avec certains types d’erreur, la reprise automatique d’une exécution de scénario n’est pas possible.

Pour plus d’informations, voir [Autoriser le stockage d’exécutions incomplètes](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) dans l’article [Panneau des paramètres de scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Pour plus d’informations, voir [Gestion avancée des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
