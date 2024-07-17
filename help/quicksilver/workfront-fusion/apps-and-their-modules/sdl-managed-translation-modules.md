---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules SDL Managed Translation
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez connecter votre compte de traduction gérée SDL à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 24%

---

# Modules [!DNL SDL Managed Translation]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez connecter votre compte [!DNL SDL Managed Translation] à plusieurs applications et services tiers.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
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

## [!DNL SDL Managed Translation] Modules

>[!NOTE]
>
>Le délai d’expiration de l’opération pour les appels à [!DNL SDL Managed Translation] est de **120 secondes**.

### Fichiers

#### [!UICONTROL Télécharger le fichier traduit]

Ce module récupère le contenu d’un seul fichier traduit, contenu dans le projet spécifié. Si le fichier demandé n’est pas encore dans l’état &quot;Downland&quot; (En bas), le contenu du fichier peut ne pas encore être entièrement traduit. Si le fichier est à l’état Téléchargement et que vous l’avez récupéré, veillez à marquer le fichier comme terminé à l’aide de la méthode `Cancel or Complete File`.

#### [!UICONTROL Charger un fichier]

Ce module permet le chargement de fichiers à des fins de traduction ou d’inclusion dans un projet de traduction en tant que document de référence. Les chargements doivent être envoyés en multipart/form-data et peuvent contenir plusieurs fichiers. Vous spécifiez les `ProjectOptionId` qui doivent être utilisés pour évaluer le ou les fichiers chargés. Cela détermine si chaque fichier que vous téléchargez peut être traduit ou doit être traité comme référence. Dans le cas des archives (`zip `, `rar`, `7z`, `tar` fichiers), l’application examine le contenu de l’archive et indique si l’archive dans son ensemble peut être traduite ou si elle contient un mélange de fichiers traduisibles et non traduisibles.

>[!NOTE]
>
>Il n’est pas recommandé de charger plusieurs fichiers à la fois, car cela peut augmenter l’impact de tout échec.

#### [!UICONTROL Ajouter un fichier de référence]

Ce module ajoute un fichier de référence.

### Projets

#### [!UICONTROL Créer un projet]

Ce module crée le projet spécifié.

#### Annulation ou fin d’un projet

Ce module annule ou complète le projet spécifié. Si le projet attend d’être téléchargé, il passe par toutes les étapes finales du processus et finit par se terminer. Si le projet est en attente d’approbation ou si la sélection du fournisseur est annulée. Si le projet a un autre état, la demande échoue.

#### [!UICONTROL Télécharger le fichier zip du projet]

Ce module récupère le fichier `zip` des fichiers traduits pour le projet spécifié.

#### [!UICONTROL Lire un projet]

Ce module récupère le projet spécifié.

#### [!UICONTROL Obtenir des projets à l’état]

Ce module récupère tous les projets disponibles dans l’état spécifié. Cette méthode permet de paginer les résultats en spécifiant les paramètres de requête `$top`, `$skip` et `$orderby`.

#### [!UICONTROL Obtenir la liste des projets]

Obtient une liste simple de tous les projets, fournissant des informations générales sur chaque projet. Cette méthode permet aux résultats d’être des pages, en spécifiant les paramètres de requête `$top`, `$skip` et `$orderby`.

#### [!UICONTROL Rechercher les options de création de projet]

Ce module obtient les options de création de projet.

### Autre

#### [!UICONTROL Effectuer un appel API]

Ce module effectue un appel d’API autorisé arbitraire.
