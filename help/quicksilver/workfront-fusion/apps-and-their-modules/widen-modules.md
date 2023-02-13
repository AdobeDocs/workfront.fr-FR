---
title: Modules étendus
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!UICONTROL Largeur], ainsi que de la connecter à plusieurs applications et services tiers.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 1%

---

# [!DNL Widen] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!UICONTROL Largeur], ainsi que de la connecter à plusieurs applications et services tiers.

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

Pour utiliser [!UICONTROL Largeur] modules, vous devez disposer d’un [!UICONTROL Largeur] compte .

## Connexion [!DNL Widen] to [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Vous pouvez créer une connexion à votre [!DNL Widen] compte directement depuis l’intérieur d’un [!DNL Widen] module .

1. Dans n’importe quel [!DNL Widen] module, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Sélectionnez la [!DNL Widen] domaine auquel vous souhaitez vous connecter.
1. Saisissez le jeton correspondant à votre [!DNL Widen] compte . Pour plus d’informations sur la localisation de ce jeton, voir [[!DNL Widen] FAQ sur les API](https://community.widen.com/collective/s/article/API-FAQs).
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## [!DNL Widen] modules et leurs champs

Lorsque vous configurez [!DNL Widen] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Widen] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencher des modules](#trigger-modules)
* [Modules d’action](#action-modules)
* [Modules de recherche](#search-modules)

### Déclencher des modules

#### [!UICONTROL Affichage des ressources]

Ce module de déclenchement lance un scénario lorsqu’une ressource est créée ou mise à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’événement]</td> 
   <td> <p>Indiquez si vous souhaitez regarder de nouvelles ressources ou des ressources mises à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Développer]</td> 
   <td> <p>Sélectionnez les propriétés à inclure dans la sortie du module en plus des champs de la ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit utiliser au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules d’action

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Lecture des informations sur les ressources]](#read-asset-info)
* [[!UICONTROL Ajout de ressources aux collections]](#add-assets-to-collections)
* [[!UICONTROL Suppression de ressources de la collection]](#remove-assets-from-collection)
* [[!UICONTROL Mise à jour des métadonnées de ressource]](#update-asset-metadata)
* [[!UICONTROL Télécharger le fichier]](#download-file)
* [[!UICONTROL Télécharger] un fichier](#upload-a-file)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Widen] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Widen] modules.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version de l’API]</td> 
   <td>Indiquez si vous souhaitez utiliser la dernière version de la variable [!DNL Widen] API ou version 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez ou mappez l’URL de votre appel API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Lecture des informations sur les ressources]

Ce module d’action récupère une ressource individuelle à l’aide de son identifiant unique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la ressource pour laquelle vous souhaitez lire les informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Développer]</td> 
   <td> <p>Sélectionnez les propriétés à inclure dans la sortie du module en plus des champs de la ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajout de ressources aux collections]

Ce module d’action ajoute une ou plusieurs ressources aux collections.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de collections]</td> 
   <td> <p>Pour chaque collection à laquelle vous souhaitez ajouter des ressources :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’[!UICONTROL ID de collection].</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressources]</td> 
   <td> <p>Pour chaque ressource à ajouter à une collection :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de ressource.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit utiliser au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression de ressources de la collection]

Ce module d’action supprime une ou plusieurs ressources des collections.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de collections]</td> 
   <td> <p>Pour chaque collection dont vous souhaitez supprimer les ressources :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de la collection.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de ressources</td> 
   <td> <p>Pour chaque ressource à supprimer d’une collection :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de ressource.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit utiliser au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mise à jour des métadonnées de ressource]

Ce module d’action met à jour les champs de métadonnées d’une ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la ressource dont vous souhaitez mettre à jour les métadonnées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de métadonnées]</td> 
   <td> <p>Sélectionnez le type de métadonnées pour les métadonnées que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Sélectionnez les champs de métadonnées à mettre à jour. Pour chaque champ, saisissez la nouvelle valeur du champ.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit utiliser au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger le fichier]

Ce module d’action télécharge une ressource à partir de votre [!DNL Widen] compte .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la ressource que vous souhaitez télécharger.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chargement d’un fichier]

Ce module d’action télécharge un fichier dans votre [!DNL Widen] compte .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger le profil]</td> 
   <td> <p>Sélectionnez le profil de chargement que le module doit utiliser.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Méthode de téléchargement]</td> 
   <td> <p>Sélectionnez le mode de chargement du fichier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL À Partir D’Un Fichier]</strong> </p> <p>Sélectionnez ou mappez le fichier source à partir d’un module précédent.</p> </li> 
     <li> <p><strong>[!UICONTROL Par URL]</strong> </p> <p>Saisissez ou mappez l’URL du fichier que vous souhaitez charger.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du fichier]</td> 
   <td>Saisissez ou mappez un nom pour le fichier chargé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de métadonnées]</td> 
   <td>Sélectionnez le type de métadonnées du fichier que vous souhaitez charger.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Sélectionnez les champs de métadonnées que vous souhaitez inclure dans le téléchargement de fichier. Pour chaque champ, saisissez la [!UICONTROL valeur] du champ.</td> 
  </tr> 
 </tbody> 
</table>

### Modules de recherche

* [[!UICONTROL Lecture des ressources de collection]](#read-collection-assets)
* [[!UICONTROL Recherche de ressources]](#search-assets)

#### [!UICONTROL Lecture des ressources de collection]

Ce module d’action récupère une liste de ressources dans une collection.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de collection]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la collection contenant les ressources que vous souhaitez lire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Saisissez ou mappez le numéro du premier élément que vous souhaitez répertorier. C'est une façon de paginer les enregistrements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trier Par]</td> 
   <td> <p>Sélectionnez la propriété par laquelle vous souhaitez trier les ressources. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordre]</td> 
   <td>Indiquez si vous souhaitez trier les ressources par ordre croissant ou décroissant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Recherche de ressources]

Ce module de recherche récupère une liste de ressources qui correspondent à des critères de recherche spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Widen] compte à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Requête de recherche]</td> 
   <td> <p>Saisissez les critères selon lesquels vous souhaitez rechercher des ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trier Par]</td> 
   <td> <p>Sélectionnez le mode de tri des ressources. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordre]</td> 
   <td>Indiquez si vous souhaitez trier les ressources par ordre croissant ou décroissant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inclure supprimée]</td> 
   <td>Activez cette option pour inclure les ressources supprimées dans la recherche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inclure archivée]</p> </td> 
   <td> <p>Activez cette option pour inclure les ressources archivées dans la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rechercher du texte du document]</td> 
   <td>Activez cette option pour inclure le texte du document dans votre recherche ou la valeur false pour inclure uniquement les ressources pour lesquelles le titre correspond aux critères de recherche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>Saisissez ou mappez le numéro du premier élément pour lequel vous souhaitez récupérer les détails. C'est une façon de paginer les enregistrements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>Activez cette option pour autoriser le défilement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Développer]</td> 
   <td> <p>Sélectionnez les propriétés à inclure dans la sortie du module en plus des champs de la ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>
