---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion des erreurs de reprise dans  [!DNL Adobe Workfront Fusion]
description: Dans certains cas, il est utile de réexécuter un module en échec plusieurs fois s’il est possible que cette situation d’échec passe avec le temps.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 100%

---

# Gestion des erreurs de reprise dans [!DNL Adobe Workfront Fusion]

Dans certains cas, il est utile de réexécuter un module en échec s’il est possible que cette situation d’échec passe avec le temps.

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

## Solutions de contournement à la directive de gestion des erreurs de [!UICONTROL reprise]

[!UICONTROL Adobe Workfront Fusion] ne propose actuellement pas de directive de gestion des erreurs de [!UICONTROL reprise] ; cependant, deux solutions peuvent être utilisées pour imiter sa fonctionnalité. Pour plus d’informations, voir [Directives de gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Utiliser la directive [!UICONTROL Interrompre]

1. Dans le panneau des paramètres du scénario, activez l’option **[!UICONTROL Autoriser le stockage des exécutions incomplètes]**.

   Pour plus d’informations, voir [Panneau des paramètres du scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Associez un itinéraire de gestionnaire d’erreur au module, tel que décrit dans [Gestion des erreurs dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Liez la directive [!UICONTROL Interrompre] à l’itinéraire du gestionnaire d’erreur et configurez-la.

   Pour plus d’informations, voir [Directives de gestion des erreurs dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Inconvénients

* L’intervalle de reprise minimal est d’une minute.
* Si le module traite plusieurs lots et que le traitement d’un lot échoue, l’exécution partielle (uniquement le lot à l’origine de l’erreur) est déplacée vers le dossier des exécutions incomplètes et planifiée pour les reprises, conformément aux paramètres de la directive [!UICONTROL Interrompre]. Cependant, l’exécution en cours se poursuit et le module continue à traiter les lots suivants. Vous pouvez activer l’option « [!UICONTROL Traitement séquentiel] » dans les [!UICONTROL Paramètres du scénario] pour empêcher le scénario de s’exécuter à nouveau jusqu’à ce que l’exécution stockée dans le dossier Exécutions incomplètes ait été résolue.

  Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre des exécutions incomplètes dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Utiliser le module [!UICONTROL Répéteur]

1. Utilisez le module **[!UICONTROL Répéteur]** et définissez son champ **[!UICONTROL Se répète]** sur le nombre maximal de tentatives.
1. Liez le module potentiellement défaillant au module **[!UICONTROL Répéteur]**.
1. Associez un itinéraire de gestionnaire d’erreur à ce module (voir [Gestion des erreurs dans  [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Liez le module **[!UICONTROL Outils] > [!UICONTROL Veille]** sur l’itinéraire du gestionnaire d’erreur et définissez son champ **[!UICONTROL Délai]** sur le nombre de secondes entre les tentatives.

1. Liez la directive **[!UICONTROL Ignorer]** après le module **[!UICONTROL Outils] > [!UICONTROL Veille]** (voir [Directives de gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Liez le module **[!UICONTROL Outils] > [!UICONTROL Définir la variable]** après le module potentiellement défaillant et configurez-le pour stocker le résultat du module dans une variable nommée, par exemple : `Result`.

1. Liez le module **[!UICONTROL Agrégateur de tableau]** après **[!UICONTROL Outils] > [!UICONTROL Définir la variable]** et sélectionnez le module **[!DNL Repeater]** dans son champ Module source.

1. Liez le module **[!UICONTROL Outils] > [!UICONTROL Obtenir une variable]** au module **[!UICONTROL Agrégateur de tableau]** et configurez-le pour obtenir la valeur de la variable `Result`.

1. Insérez le module **[!UICONTROL Outils] > [!UICONTROL Obtenir une variable]** entre le module **[!UICONTROL Répéteur]** et le module potentiellement défaillant et configurez-le pour obtenir la valeur de la variable `Result`.

1. Insérez un filtre entre le module **[!UICONTROL Outils] > [!UICONTROL Obtenir une variable]** et le module potentiellement défaillant pour ne continuer que si la variable `Result` n’existe pas.

>[!INFO]
>
>**Exemple :** voici un exemple de scénario où le module [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête] représente le module potentiellement défaillant :
>
>![](assets/http-make-request-350x116.png)
>
>Si le résultat du module potentiellement défaillant est trop complexe pour être stocké dans une variable simple, vous pouvez utiliser un magasin de données pour stocker/récupérer le résultat. Le magasin de données ne contiendrait qu’un seul enregistrement. La clé de l’enregistrement peut être, par exemple, `Result`.
>
>Pour plus d’informations sur les magasins de données, voir [Magasins de données dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Inconvénient

Cette solution peut sembler trop complexe et est également plus exigeante en termes d’opérations.
