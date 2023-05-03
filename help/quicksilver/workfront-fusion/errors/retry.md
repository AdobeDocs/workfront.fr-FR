---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Réessayer la gestion des erreurs dans [!DNL Adobe Workfront Fusion]
description: Dans certains cas, il est utile de réexécuter un module en échec plusieurs fois s’il est possible que la raison de l’échec puisse s’interrompre au fil du temps.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 184033c8957e955b3011f7e0845a73029f6b7aba
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Réessayer la gestion des erreurs dans [!DNL Adobe Workfront Fusion]

Dans certains cas, il est utile de réexécuter un module en échec s’il est possible que la raison de l’échec soit dépassée au fil du temps.

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

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Les solutions [!UICONTROL Réessayer] directive de gestion des erreurs

[!UICONTROL Adobe Workfront Fusion] n’offre actuellement pas la variable [!UICONTROL Réessayer] la directive de gestion des erreurs, bien que deux solutions puissent être utilisées pour imiter sa fonctionnalité. Pour plus d’informations, voir [Directives pour la gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Utilisez la variable [!UICONTROL Rompre] directive

1. Dans le panneau des paramètres du scénario, activez la variable **[!UICONTROL Autorisation de stockage des exécutions incomplètes]** .

   Pour plus d’informations, voir [Le panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Joindre un itinéraire de gestionnaire d’erreurs au module, comme décrit dans [Gestion des erreurs dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Liez la variable [!UICONTROL Rompre] à l’itinéraire du gestionnaire d’erreurs et configurez-le.

   Pour plus d’informations, voir [Directives de gestion des erreurs dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Inconvénients

* L’intervalle de reprise minimal est d’une minute.
* Si le module traite plusieurs lots et que le traitement d’un lot échoue, l’exécution partielle (seul le lot à l’origine de l’erreur) est déplacée vers le dossier des exécutions incomplètes et planifiée pour les reprises en fonction des [!UICONTROL Rompre] paramètres de la directive . Cependant, l’exécution actuelle se poursuit et le module continue à traiter les lots suivants. Vous pouvez activer le[!UICONTROL Traitement séquentiel]&quot; dans la variable [!UICONTROL Paramètres du scénario] pour empêcher le scénario de s’exécuter à nouveau jusqu’à ce que l’exécution stockée dans le dossier Exécutions incomplètes ait été résolue.

   Pour plus d’informations sur les exécutions incomplètes, voir [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Utilisez la variable [!UICONTROL Répéteur] module

1. Utilisez le **[!UICONTROL Répéteur]** et définissez ses **[!UICONTROL Répéter]** au nombre maximal de tentatives.
1. Liez le module potentiellement défaillant à la variable **[!UICONTROL Répéteur]** module .
1. Joindre un itinéraire de gestionnaire d’erreurs à ce module (voir [Gestion des erreurs dans [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Liez la variable **[!UICONTROL Outils] > [!UICONTROL Dormir]** sur l’itinéraire du gestionnaire d’erreurs et définissez ses **[!UICONTROL Délai]** du champ correspondant au nombre de secondes entre les tentatives.

1. Liez la variable **[!UICONTROL Ignorer]** à la suite de la **[!UICONTROL Outils] > [!UICONTROL Dormir]** (voir [Directives pour la gestion des erreurs dans Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Liez la variable **[!UICONTROL Outils] > [!UICONTROL Définir la variable]** après le module potentiellement défaillant et configurez-le pour stocker le résultat du module dans une variable nommée, par exemple : `Result`.

1. Liez la variable **[!UICONTROL Agrégateur de tableau]** après l’événement **[!UICONTROL Outils] > [!UICONTROL Définir la variable]** et sélectionnez la variable **[!DNL Repeater]** dans son champ Module source .

1. Liez la variable **[!UICONTROL Outils] > [!UICONTROL Get variable]** au module **[!UICONTROL Agrégateur de tableau]** et configurez-le pour obtenir la valeur de la variable `Result` .

1. Insérez le **[!UICONTROL Outils] > [!UICONTROL Get variable]** entre le module **[!UICONTROL Répéteur]** et le module potentiellement défaillant et le configurer pour obtenir la valeur de la variable `Result` .

1. Insérer un filtre entre ces **[!UICONTROL Outils] > [!UICONTROL Get variable]** et que le module potentiellement défaillant ne continue que si la variable `Result` n’existe pas.

>[!INFO]
>
>**Exemple :** Voici un exemple de scénario où la variable [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête] module représente le module potentiellement défaillant :
>
>![](assets/http-make-request-350x116.png)
>
>Si le résultat du module potentiellement défaillant est trop complexe pour être stocké dans une variable simple, vous pouvez utiliser une banque de données pour stocker/récupérer le résultat. L’entrepôt de données ne contiendrait qu’un seul enregistrement. La clé de l’enregistrement peut être, par exemple, `Result`.
>
>Pour plus d’informations sur les entrepôts de données, voir [Entrepôts de données dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Bouton arrière

Cette solution peut sembler un peu trop complexe et plus exigeante en termes d&#39;opérations.
