---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules SharePoint
description: Dans un [!DNL Adobe Workfront Fusion] vous pouvez automatiser les workflows qui utilisent SharePoint et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 83914e54638ffbef2b3ccee12c71b84ca7cc61d2
workflow-type: tm+mt
source-wordcount: '2660'
ht-degree: 0%

---

# [!DNL SharePoint] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL SharePoint], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL SharePoint] modules, vous devez disposer d’un [!DNL SharePoint] compte .

## Connexion [!DNL SharePoint] to [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connexion [!DNL SharePoint] to [!DNL Workfront Fusion] à l’aide d’une [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connexion [!DNL SharePoint] to [!DNL Workfront Fusion] utilisation des paramètres avancés](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connexion [!DNL SharePoint] to [!DNL Workfront Fusion] à l’aide d’une [!DNL Microsoft] account

Vous pouvez utiliser [!DNL Microsoft] pour créer une connexion à [!DNL SharePoint]. Pour obtenir des instructions sur la connexion à [!DNL Sharepoint] compte à [!DNL Workfront Fusion], voir [Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connexion [!DNL SharePoint] to [!DNL Workfront Fusion] utilisation des paramètres avancés

Pour se connecter [!DNL SharePoint] to [!DNL Workfront Fusion] sans [!DNL Microsoft] , vous avez besoin d’un identifiant client, d’un secret client et d’un identifiant client.

1. Cliquez sur **[!UICONTROL Ajouter]** près du haut de la **[!DNL SharePoint]** pour ouvrir la boîte de dialogue **[!UICONTROL Création d’une connexion]** de la boîte.

1. (Facultatif) Modifiez la valeur par défaut **[!UICONTROL Nom de la connexion]**.
1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
1. Saisissez le [!DNL SharePoint] **[!UICONTROL ID client]** et **[!UICONTROL Secret du client]**.

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre de connexion qui s’affiche, saisissez vos informations d’identification pour vous connecter à l’application si vous ne l’avez pas déjà fait.
1. (Conditionnel) Si un événement **[!UICONTROL Autoriser]** s’affiche, cliquez sur le bouton pour connecter l’application à [!DNL Workfront Fusion].

## [!DNL SharePoint] modules et leurs champs

Lorsque vous configurez [!DNL SharePoint] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL SharePoint] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Élément de lecteur](#drive-item)
* [Élément](#item)
* [Liste](#list)
* [Page (bêta)](#page-beta)
* [Site](#site)
* [Autre](#other)

### Élément de lecteur

* [Création d’un fichier](#create-a-file)
* [Création d’un dossier](#create-a-folder)
* [Obtention d’un fichier](#get-a-file)
* [Éléments du dossier de contrôle](#watch-folder-items)

#### Obtenir les modifications

Ce module renvoie les modifications qui ont été apportées dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du dossier dans lequel vous souhaitez récupérer les modifications.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID de dossier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement où vous souhaitez récupérer les modifications. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### Création d’un dossier

Ce module d’action crée un dossier dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du dossier que vous souhaitez créer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID de dossier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement où vous souhaitez créer le dossier. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du dossier]</td> 
   <td>Saisissez ou mappez un nom pour le nouveau dossier.</td> 
  </tr>
  </tbody> 
</table>

#### Obtention d’un fichier

Ce module d’action récupère le fichier SharePoint spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du fichier que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL File ID]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement du fichier. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Éléments du dossier de contrôle

Ce module de déclenchement lance un scénario lorsqu’un élément est mis à jour dans un dossier que vous sélectionnez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du fichier que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID de dossier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement du dossier que vous souhaitez voir. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Entrer le nombre maximal d’éléments [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Élément

* [[!UICONTROL Copier un élément]](#copy-an-item)
* [[!UICONTROL Création d’un élément]](#create-an-item)
* [[!UICONTROL Suppression d’un élément]](#delete-an-item)
* [[!UICONTROL Obtention d’un élément]](#get-an-item)
* [[!UICONTROL Éléments de liste]](#list-items)
* [[!UICONTROL Déplacer un élément]](#move-an-item)
* [[!UICONTROL Mettre à jour un élément]](#update-an-item)
* [[!UICONTROL Éléments de contrôle] (Planifié)](#watch-items-scheduled)


#### [!UICONTROL Copier un élément]

Ce module d’action copie un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Saisie des ID de site, de lecteur et de dossier</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste qui contiennent l’élément que vous souhaitez copier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Dans le champ Copier le type d’élément , indiquez si vous déplacez un champ ou un dossier.  Sélectionnez le site qui contient l’élément à copier, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destination]</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom]</td> 
   <td>Saisissez ou mappez un nom pour la nouvelle copie de l’élément. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un élément]

Ce module d’action crée un élément dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Créer un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et la liste dans laquelle vous souhaitez créer un élément.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>[!UICONTROL List ID]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste dans laquelle vous souhaitez créer un élément, puis sélectionnez la liste. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Pour chaque champ que vous souhaitez définir pour le nouvel élément, saisissez la clé du champ (identifie le champ) et la valeur que vous souhaitez que le nouvel élément ait pour ce champ.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un élément]

Ce module d’action supprime un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mettre à jour un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément à supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient l’élément à supprimer, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un élément]

Ce module d’action renvoie les données d’un élément spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste à partir de laquelle vous souhaitez récupérer un élément, sélectionnez la liste, puis sélectionnez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Éléments de liste]

Ce module d’action récupère une liste de tous les éléments d’une liste spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eléments de liste]</td> 
   <td> <p>Sélectionnez le mode d’identification de la liste à partir de laquelle vous souhaitez récupérer les éléments.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>[!UICONTROL List ID]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste à partir de laquelle vous souhaitez récupérer les éléments, puis sélectionnez la liste. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’éléments que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un élément]

Ce module d’action copie un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Saisie des ID de site, de lecteur et de dossier</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément à déplacer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Dans le champ Copier le type d’élément , indiquez si vous déplacez un champ ou un dossier. Sélectionnez le site qui contient l’élément à copier, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destination]</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom]</td> 
   <td>Saisissez ou mappez un nom pour l’élément déplacé. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un élément]

Ce module d’action met à jour un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mettre à jour un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément que vous souhaitez mettre à jour.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL List ID]</strong>, et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient l’élément que vous souhaitez mettre à jour, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Pour chaque champ que vous souhaitez mettre à jour pour le nouvel élément, saisissez la clé du champ (identifie le champ) et la nouvelle valeur que vous souhaitez que l’élément ait pour ce champ.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Éléments de contrôle] (Planifié)

Ce module de déclenchement lance un scénario lorsqu’un élément est créé ou modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listes de contrôle]</td> 
   <td>Choisissez si vous souhaitez regarder les listes par heure de création (nouveaux éléments) ou par heure de modification (éléments mis à jour).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Accéder au site et à l’ID de liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste à regarder.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>[!UICONTROL List ID]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez le site que vous souhaitez voir, puis sélectionnez la liste. Ces listes déroulantes récupèrent uniquement les sites suivis.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’éléments que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Liste

* [[!UICONTROL Création d’une liste]](#create-a-list)
* [[!UICONTROL Obtention d’une liste]](#get-a-list)
* [[!UICONTROL Listes de liste]](#list-lists)
* [[!UICONTROL Listes de contrôle]](#watch-lists)

#### [!UICONTROL Création d’une liste]

Ce module d’action crée une nouvelle liste dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de site]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste dans lesquels vous souhaitez créer une liste.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> où vous souhaitez créer une liste.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site sur lequel vous souhaitez créer une liste. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display Name]</td> 
   <td>Saisissez ou mappez un nom pour la nouvelle liste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour la nouvelle liste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ajouter des colonnes]</td> 
   <td>Pour chaque colonne à définir pour la nouvelle liste, saisissez une <strong>[!UICONTROL Name]</strong> pour le champ, puis sélectionnez l’option <strong>[!UICONTROL Type]</strong> de la valeur que vous souhaitez que la nouvelle colonne ait.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’une liste]

Ce module d’action renvoie les données d’une liste spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir une liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>ID de liste</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste que vous souhaitez récupérer, puis sélectionnez la liste. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listes de liste]

Ce module d’action récupère une liste de tous les éléments d’une liste spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site à partir duquel vous souhaitez récupérer les listes.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient les listes que vous souhaitez récupérer. La liste déroulante récupère uniquement les sites que vous suivez.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de listes que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listes de contrôle]

Ce module de déclenchement lance un scénario lorsqu’une liste est créée ou modifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listes de contrôle]</td> 
   <td>Choisissez si vous souhaitez regarder les listes par heure de création (nouveaux éléments) ou par heure de modification (éléments mis à jour).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Accéder au site et à l’ID de liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste à regarder.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> où se trouve la liste que vous souhaitez voir.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez le site que vous souhaitez voir. Le menu déroulant récupère uniquement le site que vous suivez.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de listes que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Page (bêta)

>[!NOTE]
>
>API dans la variable `beta` version dans [!DNL Microsoft Graph] sont sujettes à modification. L’utilisation de ces API dans les applications de production n’est pas prise en charge.

#### [!UICONTROL Obtention d’une page]

Ce module d’action renvoie les données d’une page spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir une page]</td> 
   <td> <p>Sélectionnez le mode d’identification de la page que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>et <strong>[!UICONTROL ID de page]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la page que vous souhaitez récupérer, puis sélectionnez la page.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site

* [[!UICONTROL Obtention d’un site]](#get-a-site)
* [[!UICONTROL Rechercher dans les sites]](#search-sites)

#### [!UICONTROL Obtention d’un site]

Ce module d’action renvoie les données d’un site spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir un site]</td> 
   <td> <p>Sélectionnez le mode d’identification de la page que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le site que vous souhaitez récupérer.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher dans les sites]

Ce module d’action recherche des sites en fonction d’un paramètre que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mot-clé du nom d’affichage]</td> 
   <td> <p>Saisissez ou mappez le terme de recherche que vous souhaitez rechercher sur les sites.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de sites que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### [!UICONTROL Lancer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL SharePoint] compte à [!DNL Workfront Fusion], voir <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à <code>https://graph.microsoft.com</code>. Exemple:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode [!UICONTROL]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Sélectionnez le type de données à envoyer dans l’appel API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Surveiller les événements

Ce module de déclenchement instantané démarre un scénario lorsqu’un élément est ajouté, mis à jour ou supprimé dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez un webhook existant ou cliquez sur Ajouter pour créer un nouveau webhook.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

