---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules de traduction gérés SDL
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez connecter votre compte de traduction gérée SDL à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez connecter votre [!DNL SDL Managed Translation] compte à plusieurs applications et services tiers.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Modules

>[!NOTE]
>
>Délai d’expiration de l’opération pour les appels à [!DNL SDL Managed Translation] is **120 secondes**.

### Fichiers

#### [!UICONTROL Télécharger le fichier traduit]

Ce module récupère le contenu d’un seul fichier traduit, contenu dans le projet spécifié. Si le fichier demandé n’est pas encore dans l’état &quot;Downland&quot; (En bas), le contenu du fichier peut ne pas encore être entièrement traduit. Si le fichier est à l’état Téléchargement et que vous l’avez récupéré, veillez à marquer le fichier comme terminé à l’aide de la variable `Cancel or Complete File` .

#### [!UICONTROL Chargement d’un fichier]

Ce module permet le chargement de fichiers à des fins de traduction ou d’inclusion dans un projet de traduction en tant que document de référence. Les chargements doivent être envoyés en multipart/form-data et peuvent contenir plusieurs fichiers. Vous spécifiez la variable `ProjectOptionId` qui doit être utilisé pour évaluer le ou les fichiers chargés. Cela détermine si chaque fichier que vous téléchargez peut être traduit ou doit être traité comme référence. Dans le cas des archives (`zip `, `rar`, `7z`, `tar` (fichiers) l’application examine le contenu de l’archive et indique si l’archive dans son ensemble peut être traduite ou si elle contient un mélange de fichiers traduisibles et non traduisibles.

>[!NOTE]
>
>Il n’est pas recommandé de charger plusieurs fichiers à la fois, car cela peut augmenter l’impact de tout échec.

#### [!UICONTROL Ajout d’un fichier de référence]

Ce module ajoute un fichier de référence.

### Projets

#### [!UICONTROL Créer un projet]

Ce module crée le projet spécifié.

#### Annulation ou fin d’un projet

Ce module annule ou complète le projet spécifié. Si le projet attend d’être téléchargé, il passe par toutes les étapes finales du processus et finit par se terminer. Si le projet est en attente d’approbation ou si la sélection du fournisseur est annulée. Si le projet a un autre état, la demande échoue.

#### [!UICONTROL Télécharger le fichier compressé du projet]

Ce module récupère la variable `zip` fichier des fichiers traduits pour le projet spécifié.

#### [!UICONTROL Lecture d’un projet]

Ce module récupère le projet spécifié.

#### [!UICONTROL Obtention de projets à l’état]

Ce module récupère tous les projets disponibles dans l’état spécifié. Cette méthode permet de paginer les résultats, en spécifiant la variable `$top`, `$skip`, et `$orderby` paramètres de requête.

#### [!UICONTROL Obtenir la liste des projets]

Obtient une liste simple de tous les projets, fournissant des informations générales sur chaque projet. Cette méthode permet aux résultats d’être des pages, en spécifiant la variable `$top`, `$skip`, et `$orderby` paramètres de requête.

#### [!UICONTROL Rechercher les options de création de projet]

Ce module obtient les options de création de projet.

### Autre

#### [!UICONTROL Lancer un appel API]

Ce module effectue un appel d’API autorisé arbitraire.
