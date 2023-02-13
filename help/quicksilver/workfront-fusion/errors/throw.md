---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion des erreurs de lancement dans Adobe Workfront Fusion
description: Dans certains cas, vous pouvez arrêter de force l’exécution du scénario suivie de la phase de restauration ou de validation ou arrêter le traitement d’un itinéraire et éventuellement le stocker dans la file d’attente Afficher et résoudre les exécutions incomplètes dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Traitement des erreurs de lancement dans [!DNL Adobe Workfront Fusion]

Dans certains cas, vous pouvez arrêter de force l’exécution du scénario suivie de [Retour arrière](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) ou [Commit](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) ou pour arrêter le traitement d’un itinéraire et éventuellement le stocker dans la file d’attente d’exécutions incomplètes.

Actuellement, les directives de gestion des erreurs ne peuvent pas être utilisées en dehors de la portée d’une [Itinéraire du gestionnaire d’erreurs](../../workfront-fusion/errors/error-handling.md#error) et [!DNL Adobe Workfront Fusion] ne propose pas de module qui vous permettrait de générer facilement (de générer) des erreurs de manière conditionnelle.

Pour plus d’informations sur les exécutions incomplètes, voir [Affichage et résolution d’exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Pour plus d’informations sur les directives de gestion des erreurs, voir [Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Solution de contournement pour le lancement

Pour générer de manière conditionnelle une erreur, vous pouvez configurer un module afin qu’il échoue volontairement lors de son opération. Une possibilité consiste à utiliser la variable [!UICONTROL JSON] > [!UICONTROL Analyse JSON] (voir [Modules JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configuré pour générer éventuellement une erreur (BundleValidationError dans ce cas) :

Vous pouvez ensuite joindre une des directives de gestion des erreurs à l’itinéraire de gestion des erreurs :

* Forcer l’exécution du scénario à s’arrêter et à effectuer la phase de restauration : [!UICONTROL Retour arrière]
* Forcer l’exécution du scénario à s’arrêter et à effectuer la phase de validation : [!UICONTROL Commit]
* Arrêter le traitement d’un itinéraire : [!UICONTROL Ignorer]
* Arrêtez le traitement d’un itinéraire et stockez-le dans la file d’attente du dossier d’exécutions incomplètes : [!UICONTROL Rompre]

L’exemple suivant illustre l’utilisation de la variable [!DNL Rollback] directive :

![](assets/rollback-directive-350x175.png)
