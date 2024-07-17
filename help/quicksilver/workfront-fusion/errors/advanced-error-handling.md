---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion avancée des erreurs dans  [!DNL Adobe] Workfront Fusion
description: Les techniques avancées de gestion des erreurs incluent le filtrage et l’imbrication.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 12%

---

# Gestion avancée des erreurs dans [!DNL Adobe Workfront Fusion]

Les techniques avancées de gestion des erreurs incluent le filtrage et l’imbrication.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
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

## Filtrage

Il existe deux types de filtrage qui peuvent avoir lieu sur un itinéraire de gestionnaire d’erreurs.

* [Ajout d’un filtre sur l’itinéraire du gestionnaire d’erreurs](#adding-a-filter-to-the-error-handler-route)
* [Ajout d’un routeur suivi de filtres à l’itinéraire du gestionnaire d’erreurs](#adding-a-router-followed-by-filters-to-the-error-handler)

### Ajout d’un filtre sur l’itinéraire du gestionnaire d’erreurs

Vous pouvez utiliser un filtre pour contrôler les erreurs qui sont traitées par l’itinéraire du gestionnaire d’erreurs. Cela vous permet de traiter uniquement des types d’erreurs spécifiques. Si une erreur ne transfère pas le filtre, elle est traitée comme si aucun itinéraire de gestionnaire d’erreurs n’était défini pour le module donné.

>[!INFO]
>
>**Exemple :**
>
>![](assets/filter-error-handling-350x238.png)

### Ajout d’un [!UICONTROL routeur] suivi de filtres au gestionnaire d’erreurs

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>Dans cet exemple, l’erreur se produit au niveau du module [!UICONTROL Créer un dossier] (A), qui a un itinéraire normal et un itinéraire de gestionnaire d’erreurs. Ce dernier est suivi d&#39;un routeur avec un itinéraire ayant un filtre qui définit un type d&#39;erreur spécifique (Erreur de données), et l&#39;autre qui est l&#39;itinéraire par défaut pour toutes les autres erreurs. Le premier itinéraire se termine par la directive [!UICONTROL Reprendre] qui contient des valeurs de substitution pour que le scénario reprenne à partir du module A ([!UICONTROL Créer un dossier]), tandis que le second itinéraire se termine par la directive [!UICONTROL Rollback] qui arrête l’exécution du scénario immédiatement.

Voir [Traitement des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) pour plus d’informations sur les différents types d’erreurs, sur la manière dont [!DNL Workfront Fusion] les traite et les évalue.

### Exemple de scénario

Vous pouvez configurer cet exemple de scénario pour comprendre comment ces filtres fonctionnent pour la gestion des erreurs.

Utilisez un dossier [!DNL Dropbox] existant pour charger un fichier au lieu d&#39;en créer un nouveau.

Si vous utilisez le module [!UICONTROL Créer un dossier] sur [!DNL Dropbox] et qu’il existe déjà un dossier portant le même nom, le module génère une erreur de données comme illustré ci-dessous :

![](assets/dropbox-350x276.png)

Le scénario complet :

![](assets/dropbox-scenario-350x190.png)

1. Le module [!UICONTROL Tools] > [!UICONTROL Set Variable] contient le nom du dossier
1. Le module [!UICONTROL HTTP] >[!UICONTROL Obtenir un fichier] récupère le fichier qui doit être chargé dans le dossier.
1. Le module [!UICONTROL Dropbox] >[!UICONTROL Créer un dossier] renvoie une erreur si un dossier existe déjà avec le même nom que celui mappé dans le module
1. L’itinéraire du gestionnaire d’erreurs (bulles transparentes) contient un routeur pour filtrer les erreurs.
1. Le premier itinéraire correspond à un type d’erreur spécifié appelé Erreur de données , comme nous le savons déjà :

   1. Si une erreur de données se produit et que les détails de l’erreur transitent par le filtre, le [!UICONTROL Dropbox] >[!UICONTROL Répertorier tous les fichiers/sous-dossiers dans un module de dossiers] répertorie tous les dossiers dans [!DNL Dropbox]
   1. Le filtre suivant correspond aux noms des dossiers.
   1. La directive [!UICONTROL Reprendre] spécifie l’ID de dossier et le chemin d’accès au dossier du dossier existant et l’exécution du scénario reprend à partir du module [!UICONTROL Dropbox] >[!UICONTROL Créer un module de dossier], mais au lieu d’essayer de créer un nouveau dossier, cette fois-ci, elle utilise les valeurs de la directive [!UICONTROL Reprendre] pour migrer vers le module suivant et charger le dossier existant

1. Le deuxième itinéraire correspond à toutes les autres erreurs et se termine par la directive [!UICONTROL Rollback] qui entraîne l’arrêt immédiat du scénario.

Voici une explication détaillée de la 5ème déclaration :

Pour utiliser le dossier existant dans vos modules suivants ([!UICONTROL Télécharger un fichier] ci-dessous), vous devez ajouter un itinéraire de gestionnaire d’erreurs au module et récupérer le chemin du dossier à mapper dans le module de directive [!UICONTROL Reprendre] qui suit :

![](assets/add-error-handler-route-350x113.png)

Le filtre sur la première route est défini pour gérer uniquement l’erreur particulière (Erreur de données) qui s’affiche lorsqu’un dossier portant le même nom existe déjà :

![](assets/condition-350x327.png)

Le module [!UICONTROL Dropbox] >[!UICONTROL Répertorier tous les fichiers d’un dossier] est configuré pour renvoyer tous les dossiers dans le dossier cible. Le filtre suivant transmet uniquement celui que nous essayions de créer à l’origine (le nom du dossier est stocké dans la version 33. Nom de dossier (élément) :

![](assets/condition2-350x193.png)

Finalement, la directive [!UICONTROL Reprendre] fournit le chemin d’accès au dossier en tant que sortie pour le module en échec. Notez que l’ID de dossier a été laissé vide, car il n’est pas nécessaire pour le module &#39;[!UICONTROL Upload a file]&#39; :

![](assets/flow-control-350x190.png)

## Imbrication

Quel que soit l’emplacement d’un module, les itinéraires des gestionnaires d’erreurs peuvent être créés et implémentés sur tous les modules, à l’exception des routeurs. Il est donc possible de créer un itinéraire de gestionnaire d’erreurs pour un module qui fait déjà partie d’un itinéraire de gestionnaire d’erreurs existant créé pour un autre module.

Voici un exemple d’itinéraire de gestionnaire d’erreur imbriqué :

![](assets/nested-error-handling-route-350x174.png)

Dans ce scénario, le deuxième itinéraire du gestionnaire d’erreurs est imbriqué sous le premier itinéraire du gestionnaire d’erreurs. Ainsi, si le [!UICONTROL Dropbox] >[!UICONTROL Créer un module de dossiers] rencontre une erreur, l’exécution passe à l’Itinéraire 1, si le filtre [!UICONTROL Erreur de données survenue] est transmis, le module suivant est exécuté par le module de directive [!UICONTROL Reprendre] si une erreur n’a pas lieu avec le [!UICONTROL Dropbox] >[!UICONTROL Répertorier tous les fichiers/dossiers 11} dans un module de dossiers.]

Cependant, si une erreur se produit avec ce module [!DNL Dropbox], l’exécution passe à la Route 2 du gestionnaire d’erreurs et se termine par la directive [!UICONTROL Ignorer] . Le module [!UICONTROL Reprendre la directive] n’est pas exécuté dans ce cas.

Il s’agit d’une combinaison de gestionnaires de filtrage et d’imbrication d’erreurs.

