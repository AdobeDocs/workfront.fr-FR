---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion avancée des erreurs dans [!DNL Adobe] Workfront Fusion
description: Les techniques de gestion avancée des erreurs comprennent le filtrage et l’imbrication.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 100%

---

# Gestion avancée des erreurs dans [!DNL Adobe Workfront Fusion]

Les techniques de gestion avancée des erreurs comprennent le filtrage et l’imbrication.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
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

## Filtrage

Deux types de filtrage peuvent être effectués sur un itinéraire de traitement des erreurs.

* [Ajouter un filtre à l’itinéraire du gestionnaire d’erreurs](#adding-a-filter-to-the-error-handler-route)
* [Ajouter un routeur suivi de filtres à l’itinéraire du gestionnaire d’erreurs](#adding-a-router-followed-by-filters-to-the-error-handler)

### Ajouter un filtre à l’itinéraire du gestionnaire d’erreurs

Vous pouvez utiliser un filtre pour contrôler les erreurs qui sont traitées par l’itinéraire du gestionnaire d’erreurs. Cela vous permet de ne traiter que certains types d’erreur. Si une erreur ne passe pas le filtre, elle sera traitée comme s’il n’y avait pas d’itinéraire de gestionnaire d’erreurs défini pour le module donné.

>[!INFO]
>
>**Exemple :**
>
>![](assets/filter-error-handling-350x238.png)

### Ajouter un [!UICONTROL routeur] suivi de filtres au gestionnaire d’erreurs

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>Dans cet exemple, l’erreur se produit dans le module (A) [!UICONTROL Créer un dossier], qui possède un itinéraire normal et un itinéraire de gestionnaire des erreurs. Ce dernier est suivi d’un routeur dont l’une des itinéraires est doté d’un filtre définissant un type d’erreur spécifique (une erreur de données se produit) et dont l’autre est l’itinéraire par défaut pour toutes les autres erreurs. Le premier itinéraire se termine par la directive [!UICONTROL Reprendre] qui contient des valeurs de substitution pour que le scénario reprenne à partir du module A ([!UICONTROL Créer un dossier]), tandis que le second itinéraire se termine par la directive [!UICONTROL Restaurer] qui arrête immédiatement l’exécution du scénario.

Voir [Gestion des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) pour plus d’informations sur les différents types d’erreur et sur la manière dont [!DNL Workfront Fusion] les traite et les évalue.

### Exemple de scénario

Vous pouvez mettre en place cet exemple de scénario pour comprendre comment ces filtres fonctionnent pour la gestion des erreurs.

Utiliser un dossier [!DNL Dropbox] existant pour charger un fichier au lieu d’en créer un nouveau

Si vous utilisez le module [!UICONTROL Créer un dossier] sur [!DNL Dropbox] et qu’un dossier portant le même nom existe déjà, le module produira une erreur de données comme indiqué ci-dessous :

![](assets/dropbox-350x276.png)

Scénario complet :

![](assets/dropbox-scenario-350x190.png)

1. Le module [!UICONTROL Outils] > [!UICONTROL Définir la variable] contient le nom du dossier.
1. Le module [!UICONTROL HTTP] > [!UICONTROL Obtenir un fichier] récupère le fichier qui doit être chargé dans le dossier.
1. Le module [!UICONTROL Dropbox] > [!UICONTROL Créer un dossier] génère une erreur s’il existe déjà un dossier portant le même nom que celui mappé dans le module.
1. L’itinéraire du gestionnaire d’erreurs (bulles transparentes) contient un routeur pour filtrer les erreurs.
1. Le premier itinéraire concerne un type d’erreur spécifique appelé erreur de données, comme nous le savons déjà :

   1. Si une erreur de données se produit et que les détails de l’erreur passent à travers le filtre, le module [!UICONTROL Dropbox] > [!UICONTROL Répertorier tous les fichiers/sous-dossiers dans un dossier] répertorie tous les dossiers dans [!DNL Dropbox].
   1. Le filtre suivant correspond aux noms de dossiers.
   1. La directive [!UICONTROL Reprendre] spécifie l’ID et le chemin d’accès du dossier existant et l’exécution du scénario reprend à partir du module [!UICONTROL Dropbox] > [!UICONTROL Créer un dossier], mais au lieu d’essayer de créer un dossier, il utilise cette fois les valeurs de la directive [!UICONTROL Reprendre] pour passer au module suivant et charger le fichier dans le dossier existant.

1. Le second itinéraire concerne toutes les autres erreurs et se termine par la directive [!UICONTROL Restaurer] qui entraîne l’arrêt immédiat du scénario.

Vous trouverez ci-dessous une explication détaillée de la 5ème instruction :

Afin d’utiliser le dossier existant dans vos modules suivants ([!UICONTROL Charger fichier] ci-dessous), vous devez ajouter un itinéraire de gestionnaire d’erreur au module et récupérer le chemin d’accès au dossier à mapper dans le module de directive [!UICONTROL Reprendre] qui suit :

![](assets/add-error-handler-route-350x113.png)

Le filtre du premier itinéraire est défini de manière à ne traiter que l’erreur particulière (erreur de données) qui apparaît lorsqu’un dossier portant le même nom existe déjà :

![](assets/condition-350x327.png)

Le module [!UICONTROL Dropbox] > [!UICONTROL Répertorier tous les fichiers dans un dossier] est configuré pour renvoyer tous les dossiers du dossier cible. Le filtre suivant ne s’applique qu’au dossier que nous avons essayé de créer à l’origine (le nom du dossier est stocké dans le nom de l’élément 33 du dossier) :

![](assets/condition2-350x193.png)

Finalement, la directive [!UICONTROL Reprendre] fournit le chemin d’accès au dossier en tant que sortie du module défaillant. Notez que l’ID de dossier a été laissé vide car il n’est pas nécessaire pour le module « [!UICONTROL Charger fichier] » :

![](assets/flow-control-350x190.png)

## Imbriquer

Quel que soit l’emplacement d’un module, des itinéraires de gestion des erreurs peuvent être créés et mis en œuvre sur tous les modules, à l’exception des routeurs. Il est donc possible de créer un itinéraire de gestion des erreurs pour un module qui fait déjà partie d’un itinéraire de gestion des erreurs existant créé pour un autre module.

Voici un exemple d’itinéraire de gestion derreur imbriqué :

![](assets/nested-error-handling-route-350x174.png)

Dans ce scénario, le deuxième itinéraire de gestion des erreurs est imbriqué dans le premier itinéraire de gestion des erreurs. Ainsi, si le module [!UICONTROL Dropbox] > [!UICONTROL Créer un dossier] rencontre une erreur, l’exécution passe à l’itinéraire 1, si le filtre [!UICONTROL Une erreur de données se produit] est appliqué, le module suivant est exécuté, suivi du module de directive [!UICONTROL Reprendre] si une erreur ne se produit pas avec le module [!UICONTROL Dropbox] > [!UICONTROL Répertorier tous les fichiers/sous-dossiers] dans un module de dossier.

Toutefois, si une erreur se produit avec ce module [!DNL Dropbox], l’exécution passe à l’itinéraire 2 de gestion d’erreurs et se termine par la directive [!UICONTROL Ignorer]. Le module [!UICONTROL Reprendre la directive] n’est pas exécuté dans ce cas.

Il s’agit d’une combinaison de filtrage et d’imbrication de gestionnaires d’erreurs.

