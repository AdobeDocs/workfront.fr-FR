---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion de la génération d’erreurs dans Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 82%

---

# Gestion de la génération d’erreurs dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Configurer `throw` solution de contournement d’erreur](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans certains cas, vous pouvez arrêter de force l’exécution du scénario suivie de la phase [Restauration](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) ou [Engagement](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) ou arrêter le traitement d’un itinéraire et éventuellement le stocker dans la file d’attente d’exécutions incomplètes.

Actuellement, les directives de gestion des erreurs ne peuvent pas être utilisées en dehors de la portée d’un [Itinéraire du gestionnaire d’erreurs](../../workfront-fusion/errors/error-handling.md#error) et [!DNL Adobe Workfront Fusion] ne propose pas de module qui vous permettrait de générer (lancer) facilement des erreurs de manière conditionnelle.

Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre des exécutions incomplètes dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Pour plus d’informations sur les directives de gestion des erreurs, voir [Directives de gestion des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Solution pour la génération

Pour générer de manière conditionnelle une erreur, vous pouvez configurer un module afin qu’il échoue volontairement lors de son exécution. Une possibilité consiste à utiliser le module [!UICONTROL JSON] > [!UICONTROL Parse JSON] (voir [Modules JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configuré pour générer éventuellement une erreur (BundleValidationError dans ce cas) :

Vous pouvez ensuite joindre l’une des directives de gestion des erreurs à l’itinéraire de gestion des erreurs :

* Forcer l’exécution du scénario à s’arrêter et à exécuter la phase Restauration : [!UICONTROL Restaurer]
* Forcer l’exécution du scénario à s’arrêter et à exécuter la phase Engagement : [!UICONTROL Engager]
* Arrêter le traitement d’un itinéraire : [!UICONTROL Ignorer]
* Arrêter le traitement d’un itinéraire et le stocker dans la file d’attente du dossier d’exécutions incomplètes : [!UICONTROL Rompre]

L’exemple suivant illustre l’utilisation de la directive [!DNL Rollback] :

![](assets/rollback-directive-350x175.png)
