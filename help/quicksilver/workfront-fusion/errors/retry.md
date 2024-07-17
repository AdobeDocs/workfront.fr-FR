---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Réessayer la gestion des erreurs dans [!DNL Adobe Workfront Fusion]
description: Dans certains cas, il est utile de réexécuter un module en échec plusieurs fois s’il est possible que la raison de l’échec puisse s’interrompre au fil du temps.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 17%

---

# Réessayer la gestion des erreurs dans [!DNL Adobe Workfront Fusion]

Dans certains cas, il est utile de réexécuter un module en échec s’il est possible que la raison de l’échec soit dépassée au fil du temps.

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

## Solutions à la directive de gestion des erreurs [!UICONTROL Retry]

[!UICONTROL Adobe Workfront Fusion] n’offre actuellement pas la directive de gestion des erreurs [!UICONTROL Retry], bien que deux solutions puissent être utilisées pour imiter ses fonctionnalités. Pour plus d’informations, voir [Directives pour la gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Utilisation de la directive [!UICONTROL Break]

1. Dans le panneau des paramètres du scénario, activez l’option **[!UICONTROL Autoriser le stockage des exécutions incomplètes]** .

   Pour plus d’informations, voir [Panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Joignez un itinéraire de gestionnaire d’erreurs au module, comme décrit dans [Gestion des erreurs dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Liez la directive [!UICONTROL Break] à l’itinéraire du gestionnaire d’erreurs et configurez-la.

   Pour plus d’informations, voir [Directives pour la gestion des erreurs dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Inconvénients

* L’intervalle de reprise minimal est d’une minute.
* Si le module traite plusieurs lots et que le traitement d’un lot échoue, l’exécution partielle (seul le lot qui a provoqué l’erreur) est déplacée vers le dossier des exécutions incomplètes et planifiée pour les reprises conformément aux paramètres de la directive [!UICONTROL Break]. Cependant, l’exécution actuelle se poursuit et le module continue à traiter les lots suivants. Vous pouvez activer l’option &quot;[!UICONTROL Traitement séquentiel]&quot; dans les [!UICONTROL paramètres du scénario] pour empêcher le scénario de s’exécuter à nouveau jusqu’à ce que l’exécution stockée dans le dossier Exécutions incomplètes ait été résolue.

  Pour plus d’informations sur les exécutions incomplètes, voir [Affichage et résolution des exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Utilisation du module [!UICONTROL Répéteur]

1. Appliquez le module **[!UICONTROL Répéteur]** et définissez son champ **[!UICONTROL Répéter]** sur le nombre maximal de tentatives.
1. Liez le module potentiellement défaillant au module **[!UICONTROL Répéteur]** .
1. Joignez un itinéraire de gestionnaire d’erreurs à ce module (voir [Gestion des erreurs dans [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Reliez le module **[!UICONTROL Outils] > [!UICONTROL Dormir]** à l’itinéraire du gestionnaire d’erreurs et définissez son champ **[!UICONTROL Délai]** sur le nombre de secondes entre les tentatives.

1. Liez la directive **[!UICONTROL Ignorer]** après le module **[!UICONTROL Outils] > [!UICONTROL Dormir]** (voir [Directives pour la gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Liez le module **[!UICONTROL Tools] > [!UICONTROL Set variable]** (Définir la variable) après le module potentiellement défaillant et configurez-le pour stocker le résultat du module dans une variable nommée, par exemple, `Result`.

1. Liez le module **[!UICONTROL Agrégateur de tableau]** après le module **[!UICONTROL Outils] > [!UICONTROL Définir la variable]** et sélectionnez le module **[!DNL Repeater]** dans son champ Module Source.

1. Reliez le module **[!UICONTROL Tools] > [!UICONTROL Get variable]** au module **[!UICONTROL Array aggator]** et configurez-le pour obtenir la valeur de la variable `Result`.

1. Insérez le module **[!UICONTROL Tools] > [!UICONTROL Get variable]** entre le module **[!UICONTROL Répéteur]** et le module potentiellement défaillant et configurez-le pour obtenir la valeur de la variable `Result`.

1. Insérez un filtre entre ce module **[!UICONTROL Outils] > [!UICONTROL Obtenir la variable]** et le module potentiellement défaillant à continuer uniquement si la variable `Result` n&#39;existe pas.

>[!INFO]
>
>**Exemple :** Voici un exemple de scénario où le module [!UICONTROL HTTP] >[!UICONTROL Make a request] représente le module potentiellement défaillant :
>
>![](assets/http-make-request-350x116.png)
>
>Si le résultat du module potentiellement défaillant est trop complexe pour être stocké dans une variable simple, vous pouvez utiliser une banque de données pour stocker/récupérer le résultat. L’entrepôt de données ne contiendrait qu’un seul enregistrement. La clé de l’enregistrement peut être, par exemple, `Result`.
>
>Pour plus d’informations sur les entrepôts de données, voir [Stockages de données dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Bouton arrière

Cette solution peut sembler un peu trop complexe et plus exigeante en termes d&#39;opérations.
