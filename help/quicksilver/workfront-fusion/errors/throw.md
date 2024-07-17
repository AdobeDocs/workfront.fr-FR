---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion des erreurs de lancement dans Adobe Workfront Fusion
description: Dans certains cas, vous pouvez arrêter de force l’exécution du scénario suivie de la phase de restauration ou de validation ou arrêter le traitement d’un itinéraire et éventuellement le stocker dans la file d’attente Afficher et résoudre les exécutions incomplètes dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 30%

---

# Traitement des erreurs de lancement dans [!DNL Adobe Workfront Fusion]

Dans certains cas, vous pouvez arrêter de force l’exécution du scénario suivie de la phase [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) ou [Commit](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) ou arrêter le traitement d’un itinéraire et éventuellement le stocker dans la file d’attente d’exécutions incomplètes.

Actuellement, les directives de gestion des erreurs ne peuvent pas être utilisées en dehors de la portée d’un [itinéraire du gestionnaire d’erreurs](../../workfront-fusion/errors/error-handling.md#error) et [!DNL Adobe Workfront Fusion] n’offre pas de module qui vous permettrait de générer facilement (de générer) des erreurs de manière conditionnelle.

Pour plus d’informations sur les exécutions incomplètes, voir [Affichage et résolution des exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Pour plus d’informations sur les directives de gestion des erreurs, voir [Directives pour la gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Pour plus d&#39;informations sur les licences [!DNL Adobe Workfront Fusion], voir [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Solution pour le lancement

Pour générer de manière conditionnelle une erreur, vous pouvez configurer un module afin qu’il échoue volontairement lors de son opération. Une possibilité consiste à utiliser le module [!UICONTROL JSON] > [!UICONTROL Parse JSON] (voir [modules JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configuré pour renvoyer éventuellement une erreur (BundleValidationError dans ce cas) :

Vous pouvez ensuite joindre l’une des directives de gestion des erreurs à l’itinéraire de gestion des erreurs :

* Forcer l’exécution du scénario à s’arrêter et à effectuer la phase de restauration : [!UICONTROL Rollback]
* Forcer l’exécution du scénario à s’arrêter et à effectuer la phase de validation : [!UICONTROL Commit]
* Arrêter le traitement d’un itinéraire : [!UICONTROL Ignorer]
* Arrêtez le traitement d’un itinéraire et stockez-le dans la file d’attente du dossier d’exécutions incomplètes : [!UICONTROL Break]

L’exemple suivant illustre l’utilisation de la directive [!DNL Rollback] :

![](assets/rollback-directive-350x175.png)
