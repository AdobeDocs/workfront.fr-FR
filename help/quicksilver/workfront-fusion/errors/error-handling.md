---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion des erreurs dans [!DNL Adobe Workfront Fusion]
description: Lorsque des erreurs se produisent lors de l’exécution d’un scénario, c’est généralement parce qu’un service n’est pas disponible en raison d’un échec, qu’il répond avec des données inattendues ou que la validation des données d’entrée échoue.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Gestion des erreurs dans [!DNL Adobe Workfront Fusion]

Lorsque des erreurs se produisent lors de l’exécution d’un scénario, c’est généralement parce qu’un service n’est pas disponible en raison d’un échec, qu’il répond avec des données inattendues ou que la validation des données d’entrée échoue.

Si un module renvoie une erreur lors de l’exécution du scénario et qu’aucun itinéraire de gestion des erreurs n’est associé au module, la logique de gestion des erreurs par défaut s’exécute, comme décrit dans la section [Traitement des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

En ajoutant un itinéraire de gestionnaire d’erreurs à un module, vous pouvez remplacer la logique de gestion des erreurs par défaut par la vôtre. [!DNL Adobe Workfront Fusion] propose cinq directives différentes qui peuvent être insérées à la fin des itinéraires de votre gestionnaire d’erreurs.

Pour plus d’informations, voir [Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Itinéraire du gestionnaire d’erreurs

Pour ajouter un itinéraire de gestionnaire d’erreurs à un module :

1. Cliquez avec le bouton droit sur le module et sélectionnez **[!UICONTROL Ajouter un gestionnaire d’erreurs]**:

   ![](assets/error-handler-route.png)

   Le module affiche une liste des directives ainsi que les applications utilisées dans votre scénario.

1. Si le module auquel vous avez ajouté un gestionnaire d’erreurs est le dernier module de votre itinéraire, sélectionnez l’une des directives.

   Ou

   Ajoutez un ou plusieurs modules à l’itinéraire du gestionnaire d’erreurs.

   Si vous ajoutez d’autres modules à l’itinéraire, la variable [!UICONTROL Ignorer] est appliquée par défaut et, en cas d’erreur, les modules suivants sur cet itinéraire sont traités.


>[!INFO]
>
>Dans cet exemple, si une erreur se produit lors de l’exécution de la variable [!UICONTROL Création d’un dossier] , [!UICONTROL Ignorer] est appliquée automatiquement et le scénario passe au module suivant sur l’itinéraire du gestionnaire d’erreurs.
>
>En revanche, en l’absence d’erreur, le scénario se déplace vers le [!UICONTROL Liste de tous les fichiers dans un module de dossiers] sur la route normale.
>
>![](assets/if-there-is-no-error-350x234.png)

Notez qu’un itinéraire de gestionnaire d’erreurs est composé de cercles transparents, tandis qu’un itinéraire normal est composé de cercles solides.

## Instructions de gestion des erreurs

Les directives sont brièvement expliquées ci-dessous. Pour plus d’informations, voir [Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Cinq directives au total peuvent être regroupées dans les catégories suivantes selon qu&#39;une exécution de scénario doit se poursuivre ou non.

Les directives suivantes garantissent qu’une exécution de scénario se poursuit :

* **[!UICONTROL Reprendre]**: Permet de spécifier une sortie de substitution pour le module avec l’erreur. L’état d’exécution du scénario est marqué comme succès.
* **[!UICONTROL Ignorer]**: ignore l’erreur. L’état d’exécution du scénario est marqué comme succès.
* **[!UICONTROL Rompre]**: Stocke l’entrée dans la file d’attente des exécutions incomplètes. L’état d’exécution du scénario est marqué comme avertissement. Pour plus d’informations, voir [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Si l’exécution d’un scénario doit s’arrêter en cas d’erreur, utilisez l’une des directives suivantes :

* **[!UICONTROL Retour arrière]**: Arrête immédiatement l’exécution du scénario et marque son état d’erreur
* **[!UICONTROL Commit]**: Arrête immédiatement l’exécution du scénario et marque son statut de succès.

Pour plus d’informations sur la gestion des erreurs, voir :

* [Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Gestion avancée des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)