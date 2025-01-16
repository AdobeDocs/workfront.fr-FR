---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Directives de gestion des erreurs dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 92%

---

# Directives pour la gestion des erreurs dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Directives relatives au traitement des erreurs](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/directives-for-error-handling.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

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

## Directives pour la gestion des erreurs

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Restaurer</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>L’exécution du scénario s’arrête immédiatement et une phase de <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">restauration</a> démarre sur tous les modules afin de tenter de rétablir leur état initial. Les modules suivants ne sont pas traités.</p> <p>À l’exception de certains types d’erreur, le scénario est désactivé après le nombre d’erreurs consécutives spécifié dans les paramètres du scénario. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Nombre d’erreurs consécutives</a>.</p> <p>Le statut d’exécution du scénario est marqué comme « erreur ».</p> <p>Note : il s’agit du comportement par défaut si aucun itinéraire de gestionnaire d’erreurs n’est associé au module et que le paramètre <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Allow storing incomplete executions]</a> dans les [!UICONTROL Scenario settings] n’est pas coché.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Valider</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>L’exécution du scénario est immédiatement arrêtée et une phase de validation est lancée pour tous les modules. Les modules suivants ne sont pas traités.</p> <p>Tous les lots non traités sont ignorés.</p> <p>Le statut d’exécution du scénario est marqué comme « succès ». Pour plus d’informations sur les phases de validation, voir <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Validation</a> dans l’article <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Exécution, cycles et phases de scénarios dans Adobe Workfront Fusion</a>.</p> </td> 
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
   <td> <p>Le statut de l’exécution du scénario est stocké dans la file d’attente des exécutions incomplètes où l’erreur peut être résolue manuellement. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Afficher et résoudre les exécutions incomplètes dans Adobe Workfront Fusion</a>. </p> <p>Il existe toutefois quelques exceptions. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Autoriser le stockage des exécutions incomplètes</a> dans l’article <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Le panneau des paramètres du scénario dans Adobe Workfront Fusion</a>.</p> <p>Les modules suivants ne sont pas traités.</p> <p>S’il existe des bundles non traités, l’exécution du scénario se poursuit normalement.</p> <p>Le statut d’exécution du scénario est marqué comme « avertissement » lorsque l’option [!UICONTROL Automatically complete execution] est désactivée.</p> <p>Voir la section <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> ci-dessous pour plus d’informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Réessayer</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>Dans certains cas, il peut être utile de réexécuter un module défaillant plusieurs fois lorsqu’il est possible que la raison de la défaillance disparaisse avec le temps.</p> <p>Workfront Fusion n’offre pas actuellement la directive de reprise, mais plusieurs solutions de contournement peuvent être utilisées pour imiter sa fonctionnalité. Pour plus d’informations, voir <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Gestion des erreurs de reprise dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Actuellement, les directives de gestion des erreurs ne peuvent pas être utilisées en dehors d’un itinéraire de gestion des erreurs.
>
>   Pour plus d’informations, voir [Itinéraire de gestion des erreurs](../../workfront-fusion/errors/error-handling.md#error) dans l’article [Gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] n’offre pas actuellement de module Throw qui vous permettrait de générer facilement des erreurs de manière conditionnelle (throw), bien qu’une solution de contournement puisse être employée pour imiter sa fonctionnalité.
>
>   Pour plus d’informations, voir [Solution de contournement pour Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw) dans l’article [Gestion des erreurs Throw dans Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Interrompre {#break}

Lorsqu’une erreur est traitée par la directive [!DNL Break], un enregistrement est créé dans le dossier des exécutions incomplètes. Cet enregistrement stocke l’état de l’exécution du scénario, ainsi que les données des modules précédents. L’enregistrement fait référence au module à l’origine de l’erreur et contient des informations sur les données reçues par le module en entrée. Un enregistrement distinct est créé pour chaque paquet de données à l’origine de l’erreur.

Pour plus d’informations, voir [Afficher et résoudre les exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Résoudre les erreurs résultant de la directive Interrompre

Vous pouvez résoudre l’erreur manuellement en mettant à jour le scénario (si nécessaire) et en l’exécutant une fois.

Vous pouvez également configurer le scénario pour qu’il traite automatiquement une exécution incomplète en réexécutant le scénario. Pour configurer le module afin qu’il traite les exécutions incomplètes, procédez comme suit :

1. Dans le module Interrompre, activez l’option [!UICONTROL **Terminer automatiquement l’exécution**].
1. Dans le champ **Nombre de tentatives**, saisissez ou mappez le nombre maximum de fois que vous voulez que le module réessaie l’exécution

   Ce nombre doit être compris entre 1 et 100.
1. Dans le champ **Intervalle entre les tentatives**, saisissez ou mappez le nombre de minutes entre chaque nouvelle tentative.

Si cette option est activée, en cas d’erreur, l’exécution incomplète est récupérée (après le délai spécifié dans le champ [!UICONTROL Intervalle entre les tentatives]) et exécutée avec les données d’entrée originales. Cette opération se répète jusqu’à ce que l’exécution du module se termine sans erreur ou jusqu’à ce que le nombre de tentatives spécifié soit atteint.

>[!NOTE]
>
>Si la première tentative échoue, l’intervalle entre les tentatives augmente de manière exponentielle à chaque nouvelle tentative.


Lorsque l’option « Terminer automatiquement l’exécution » est activée, l’exécution du scénario est marquée comme « Succès » parce que la reprise automatique du gestionnaire d’erreurs d’interruption traite automatiquement le problème. Dans ce cas, les personnes ne reçoivent pas d’e-mail concernant l’échec de l’exécution.

Lorsque l’option « Terminer automatiquement l’exécution » est désactivée, l’exécution est marquée comme « Avertissement ».

Il existe quelques exceptions à l’enregistrement des exécutions dans la rubrique Exécutions incomplètes et, pour certains types d’erreurs, la reprise automatique de l’exécution d’un scénario n’est pas possible.

Pour plus d’informations, voir [Autoriser le stockage des exécutions incomplètes](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) dans l’article [Panneau des paramètres du scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Pour plus d’informations, voir [Gestion avancée des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
