---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestion avancée des erreurs dans [!DNL Adobe] Workfront Fusion
description: Les techniques avancées de gestion des erreurs incluent le filtrage et l’imbrication.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Gestion avancée des erreurs dans [!DNL Adobe Workfront Fusion]

Les techniques avancées de gestion des erreurs incluent le filtrage et l’imbrication.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
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

## Filtrage

Il existe deux types de filtrage qui peuvent avoir lieu sur un itinéraire de gestionnaire d’erreurs.

* [Ajout d’un filtre sur l’itinéraire du gestionnaire d’erreurs](#adding-a-filter-to-the-error-handler-route)
* [Ajout d’un routeur suivi de filtres à l’itinéraire du gestionnaire d’erreurs](#adding-a-router-followed-by-filters-to-the-error-handler)

### Ajout d’un filtre sur l’itinéraire du gestionnaire d’erreurs

Vous pouvez utiliser un filtre pour contrôler les erreurs qui sont traitées par l’itinéraire du gestionnaire d’erreurs. Cela vous permet de traiter uniquement des types d’erreurs spécifiques. Si une erreur ne transfère pas le filtre, elle est traitée comme si aucun itinéraire de gestionnaire d’erreurs n’était défini pour le module donné.

>[!INFO]
>
>**Exemple:**
>
>![](assets/filter-error-handling-350x238.png)

### Ajouter un [!UICONTROL Routeur] suivi de filtres au gestionnaire d’erreurs

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>Dans cet exemple, l’erreur se produit à l’adresse [!UICONTROL Création d’un dossier] module (A), avec un itinéraire normal et un itinéraire de gestionnaire d’erreurs. Ce dernier est suivi d&#39;un routeur avec un itinéraire ayant un filtre qui définit un type d&#39;erreur spécifique (Erreur de données), et l&#39;autre qui est l&#39;itinéraire par défaut pour toutes les autres erreurs. Le premier itinéraire se termine par la variable [!UICONTROL Reprendre] qui contient des valeurs de remplacement pour que le scénario reprenne à partir du module A ([!UICONTROL Création d’un dossier]), tandis que le deuxième itinéraire se termine par le [!UICONTROL Retour arrière] qui arrête immédiatement l’exécution du scénario.

Voir [Traitement des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) pour plus d’informations sur les différents types d’erreur et sur la manière dont [!DNL Workfront Fusion] traite et évalue-les.

### Exemple de scénario

Vous pouvez configurer cet exemple de scénario pour comprendre comment ces filtres fonctionnent pour la gestion des erreurs.

Utilisez un [!DNL Dropbox] pour charger un fichier au lieu d’en créer un nouveau

Si vous utilisez la variable [!UICONTROL Création d’un dossier] module activé [!DNL Dropbox] et qu’un dossier portant le même nom existe déjà, le module génère une erreur de données comme illustré ci-dessous :

![](assets/dropbox-350x276.png)

Le scénario complet :

![](assets/dropbox-scenario-350x190.png)

1. Le [!UICONTROL Outils] > [!UICONTROL Définir la variable] module contient le nom du dossier
1. Le [!UICONTROL HTTP] >[!UICONTROL Obtention d’un fichier] récupère le fichier qui doit être chargé dans le dossier .
1. Le [!UICONTROL Dropbox] >[!UICONTROL Création d’un dossier] renvoie une erreur si un dossier porte déjà le même nom que celui mappé dans le module .
1. L’itinéraire du gestionnaire d’erreurs (bulles transparentes) contient un routeur pour filtrer les erreurs.
1. Le premier itinéraire correspond à un type d’erreur spécifié appelé Erreur de données , comme nous le savons déjà :

   1. Si une erreur de données se produit et que les détails de l’erreur transitent par le filtre, la variable [!UICONTROL Dropbox] >[!UICONTROL Liste de tous les fichiers/sous-dossiers dans un module de dossiers] répertorie tous les dossiers dans [!DNL Dropbox]
   1. Le filtre suivant correspond aux noms des dossiers.
   1. Le [!UICONTROL Reprendre] La directive spécifie l’ID de dossier et le chemin d’accès au dossier du dossier existant et l’exécution du scénario reprend à partir de [!UICONTROL Dropbox] >[!UICONTROL Création d’un dossier] mais au lieu d’essayer de créer un dossier, cette fois-ci, il utilise les valeurs de la variable [!UICONTROL Reprendre] pour passer au module suivant et charger le fichier dans le dossier existant

1. Le deuxième itinéraire correspond à toutes les autres erreurs et se termine par la variable [!UICONTROL Retour arrière] , ce qui entraîne l’arrêt immédiat du scénario.

Voici une explication détaillée de la 5ème déclaration :

Pour utiliser le dossier existant dans vos modules suivants ([!UICONTROL Chargement d’un fichier] ci-dessous), vous devez ajouter un itinéraire de gestionnaire d’erreurs au module et récupérer le chemin du dossier à mapper dans le [!UICONTROL Reprendre] module de directive qui suit :

![](assets/add-error-handler-route-350x113.png)

Le filtre sur la première route est défini pour gérer uniquement l’erreur particulière (Erreur de données) qui s’affiche lorsqu’un dossier portant le même nom existe déjà :

![](assets/condition-350x327.png)

Le [!UICONTROL Dropbox] >[!UICONTROL Liste de tous les fichiers d’un dossier] est configuré pour renvoyer tous les dossiers du dossier cible. Le filtre suivant transmet uniquement celui que nous essayions de créer à l’origine (le nom du dossier est stocké dans la version 33. Nom de dossier (élément) :

![](assets/condition2-350x193.png)

Finalement, la variable [!UICONTROL Reprendre] La directive fournit le chemin d’accès au dossier en tant que sortie pour le module en échec. Notez que l’ID de dossier a été laissé vide, car il n’est pas nécessaire pour le &quot;&quot;.[!UICONTROL Chargement d’un fichier]Module &#39; :

![](assets/flow-control-350x190.png)

## Imbrication

Quel que soit l’emplacement d’un module, les itinéraires des gestionnaires d’erreurs peuvent être créés et implémentés sur tous les modules, à l’exception des routeurs. Il est donc possible de créer un itinéraire de gestionnaire d’erreurs pour un module qui fait déjà partie d’un itinéraire de gestionnaire d’erreurs existant créé pour un autre module.

Voici un exemple d’itinéraire de gestionnaire d’erreur imbriqué :

![](assets/nested-error-handling-route-350x174.png)

Dans ce scénario, le deuxième itinéraire du gestionnaire d’erreurs est imbriqué sous le premier itinéraire du gestionnaire d’erreurs. Si la variable [!UICONTROL Dropbox] >[!UICONTROL Création d’un module de dossiers] rencontre une erreur, l’exécution passe à l’itinéraire 1, si la variable [!UICONTROL Erreur de données] est transmis, le module suivant est exécuté, suivi de la fonction [!UICONTROL Reprendre] module de directive si une erreur ne se produit pas avec la variable [!UICONTROL Dropbox] >[!UICONTROL Liste de tous les fichiers/sous-dossiers] dans un module de dossiers.

Cependant, si une erreur se produit avec cette opération [!DNL Dropbox] , puis l’exécution passe à l’itinéraire 2 du gestionnaire d’erreurs et se termine par [!UICONTROL Ignorer] . Le [!UICONTROL Reprendre la directive] n’est pas exécuté dans ce cas.

Il s’agit d’une combinaison de gestionnaires de filtrage et d’imbrication d’erreurs.

