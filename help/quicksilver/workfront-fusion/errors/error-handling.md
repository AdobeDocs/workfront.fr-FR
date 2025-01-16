---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gérer les erreurs dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 88%

---

# Gestion des erreurs dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Ajouter la gestion des erreurs](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/error-handling.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Lorsque des erreurs se produisent pendant l’exécution d’un scénario, c’est généralement parce qu’un service est indisponible en raison d’une défaillance, qu’un service répond avec des données inattendues ou que la validation des données d’entrée échoue.

Si un module génère une erreur pendant l’exécution du scénario et qu’aucun itinéraire de gestion des erreurs n’est attaché au module, la logique de gestion des erreurs par défaut s’exécute, comme décrit dans [Traitement des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

En ajoutant un itinéraire du gestionnaire des erreurs à un module, vous pouvez remplacer la logique de gestion des erreurs par défaut par la vôtre. [!DNL Adobe Workfront Fusion] propose cinq directives différentes qui peuvent être insérées à la fin des itinéraires de votre gestionnaire d’erreurs.

Pour plus d’informations, consultez [Directives pour la gestion des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Itinéraire du gestionnaire d’erreurs

Pour ajouter un itinéraire du gestionnaire des erreurs à un module, procédez comme suit :

1. Cliquez avec le bouton droit de la souris sur le module et sélectionnez **[!UICONTROL Ajouter un gestionnaire d’erreurs]** :

   ![](assets/error-handler-route.png)

   Le module affiche une liste de directives ainsi que les applications utilisées dans votre scénario.

1. Si le module auquel vous avez ajouté un gestionnaire d’erreurs est le dernier module de votre itinéraire, sélectionnez l’une des directives.

   Ou

   Ajoutez un ou plusieurs modules à l’itinéraire du gestionnaire d’erreurs.

   Si vous ajoutez d’autres modules à l’itinéraire, la directive [!UICONTROL Ignorer] est appliquée par défaut et, en cas d’erreur, les modules suivants de cet itinéraire sont traités.


>[!INFO]
>
>Dans cet exemple, si une erreur survient lors de l’exécution du module [!UICONTROL Créer un dossier], la directive [!UICONTROL Ignorer] sera appliquée automatiquement et le scénario passera au module suivant sur l’itinéraire du gestionnaire d’erreurs.
>
>Cependant, s’il n’y a pas d’erreur, le scénario passera à [!UICONTROL Lister tous les fichiers d’un module de dossier] en suivant l’itinéraire habituel.
>
>![](assets/if-there-is-no-error-350x234.png)

Notez qu’un itinéraire du gestionnaire des erreurs est composé de cercles transparents, tandis qu’un itinéraire normal est composé de cercles pleins.

## Directives de gestion des erreurs

Les directives sont brièvement expliquées ci-dessous. Pour plus d’informations, consultez [Directives pour la gestion des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Il existe au total cinq directives qui peuvent être regroupées dans les catégories suivantes selon que l’exécution d’un scénario doive se poursuivre ou non.

Les directives suivantes garantissent la poursuite de l’exécution d’un scénario :

* **[!UICONTROL Reprendre]** : permet de spécifier une sortie de substitution pour le module avec l’erreur. Le statut d’exécution du scénario est marqué comme un succès.
* **[!UICONTROL Ignorer]** : ignore l’erreur. Le statut d’exécution du scénario est marqué comme un succès.
* **[!UICONTROL Interrompre]** : enregistre l’entrée dans la file d’attente des exécutions incomplètes. Le statut d’exécution du scénario est marqué comme un avertissement. Pour plus d’informations, consultez [Voir et résoudre les exécutions incomplètes dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Si l’exécution d’un scénario doit s’arrêter en cas d’erreur, utilisez l’une des directives suivantes :

* **[!UICONTROL Restaurer]** : arrête immédiatement l’exécution du scénario et marque son statut comme une erreur.
* **[!UICONTROL Valider]** : arrête immédiatement l’exécution du scénario et marque son statut comme un succès.

Pour plus d’informations sur la gestion des erreurs, consultez ce qui suit :

* [Directives pour la gestion des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Gestion avancée des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)