---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules SDL Managed Translation
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 80%

---

# Modules [!DNL SDL Managed Translation]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules de traduction gérés par SDL](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/sdl-managed-translation-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez connecter votre compte [!DNL SDL Managed Translation] à plusieurs applications et services tiers.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Informations sur l&#39;API de traduction gérée par SDL

Le connecteur de traduction gérée SDL utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>https://languagecloud.sdl.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.4.26</td> 
  </tr>
 </tbody> 
 </table>

## Modules [!DNL SDL Managed Translation]

>[!NOTE]
>
>Le délai d’expiration de l’opération pour les appels à [!DNL SDL Managed Translation] est de **120 secondes**.

### Fichiers

#### [!UICONTROL Télécharger le fichier traduit]

Ce module récupère le contenu d’un seul fichier traduit, contenu dans le projet spécifié. Si le fichier demandé n’est pas encore au statut « Téléchargement », le contenu du fichier peut ne pas encore être entièrement traduit. Si le fichier adopte le statut Téléchargement et que vous l’avez récupéré, veillez à marquer le fichier comme terminé à l’aide de la méthode `Cancel or Complete File`.

#### [!UICONTROL Charger un fichier]

Ce module permet le chargement de fichiers à des fins de traduction ou d’inclusion dans un projet de traduction en tant que document de référence. Les chargements doivent être envoyés à l’aide de l’instruction multipart/form-data et peuvent contenir plusieurs fichiers. Vous devez spécifier la valeur `ProjectOptionId` qui doit être utilisée pour évaluer le ou les fichiers chargés. Cela détermine si chaque fichier que vous téléchargez peut être traduit ou doit être traité comme référence. Dans le cas des archives (fichiers `zip `, `rar`, `7z` et `tar`), l’application examine le contenu de l’archive et indique si l’archive dans son ensemble peut être traduite ou si elle contient un mélange de fichiers traduisibles et non traduisibles.

>[!NOTE]
>
>Il n’est pas recommandé de charger plusieurs fichiers à la fois, car cela peut augmenter le risque d’échec.

#### [!UICONTROL Ajouter un fichier de référence]

Ce module ajoute un fichier de référence.

### Projets

#### [!UICONTROL Créer un projet]

Ce module permet de créer le projet spécifié.

#### Annuler ou terminer un projet

Ce module annule ou met fin au projet spécifié. Si le projet attend d’être téléchargé, il passe par toutes les étapes finales du workflow et finit par se terminer. Si le projet est en attente d’approbation ou si la sélection du fournisseur est annulée. Si le projet possède un autre statut, la demande échoue.

#### [!UICONTROL Télécharger le projet sous forme d’archive]

Ce module récupère le fichier `zip` avec les fichiers traduits pour le projet spécifié.

#### [!UICONTROL Lire un projet]

Ce module récupère le projet spécifié.

#### [!UICONTROL Obtenir les projets au statut]

Ce module récupère tous les projets disponibles au statut spécifié. Cette méthode permet de paginer les résultats, en spécifiant les paramètres de requête `$top`, `$skip` et `$orderby`.

#### [!UICONTROL Obtenir la liste des projets]

Permet d’obtenir une liste basique de tous les projets, avec des informations générales sur chaque projet. Cette méthode permet de paginer les résultats en spécifiant les paramètres de requête `$top`, `$skip` et `$orderby`.

#### [!UICONTROL Rechercher les options de création du projet]

Ce module permet d’obtenir les options de création du projet.

### Autre

#### [!UICONTROL Effectuer un appel API]

Ce module effectue un appel API autorisé et arbitraire.
