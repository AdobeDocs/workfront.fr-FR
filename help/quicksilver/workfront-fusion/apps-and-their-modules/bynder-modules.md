---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Bynder
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Bynder], ainsi que de la connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 0%

---

# [!DNL Bynder] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Bynder], ainsi que de la connecter à plusieurs applications et services tiers.

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

Pour utiliser [!DNL Bynder] modules, vous devez disposer d’un [!DNL Bynder] compte .

## Connexion [!DNL Bynder] vers Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Créer une connexion à [!DNL Bynder] de [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Générer une [!UICONTROL ID client] et [!UICONTROL Secret du client] in [!DNL Bynder] (Facultatif)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Créer une connexion à [!DNL Bynder] de [!DNL Workfront Fusion]

Vous pouvez créer une connexion à partir de [!DNL Workfront Fusion] à [!DNL Bynder] compte directement depuis l’intérieur d’un [!DNL Bynder] module .

1. Dans n’importe quel [!DNL Bynder] module, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Sélectionnez la [!DNL Bynder] domaine auquel vous souhaitez vous connecter.
1. (Facultatif) Cliquez sur **[!UICONTROL Paramètres avancés]**, puis entrez votre [!UICONTROL ID client] et [!UICONTROL Secret du client].

   Pour plus d’informations sur la génération de l’ID client et du secret client, voir [Génération d’un identifiant client et d’un secret client dans [!DNL Bynder] (Facultatif)](#generate-a-client-id-and-client-secret-in-bynder-optional) dans cet article.

1. Dans le [!UICONTROL login] , saisissez votre nom d’utilisateur (adresse électronique) et votre mot de passe.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

### Générer une [!UICONTROL ID client] et [!UICONTROL Secret du client] in [!DNL Bynder] (Facultatif)

Si vous souhaitez créer une connexion à l’aide de l’identifiant client et du secret client, vous pouvez les générer à partir de votre [!DNL Bynder] compte . L’identifiant du client et le secret du client sont générés lorsque vous créez une application dans [!DNL Bynder].

Pour obtenir des instructions sur la création d’une application dans [!DNL Bynder], voir [Applications Oauth 2.0](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) dans le [!DNL Bynder] documentation.

>[!NOTE]
>
>Lors de la création de l’application dans [!DNL Bynder], saisissez ce qui suit en tant que `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] modules et leurs champs

Lorsque vous configurez [!DNL Bynder] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Bynder] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)
* [Triggers](#triggers)

### Actions

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Lecture des métadonnées de ressource]](#read-asset-metadata)
* [[!UICONTROL Mise à jour des métadonnées de ressource]](#update-asset-metadata)
* [[!UICONTROL Ajout de ressources à une collection]](#add-assets-to-a-collection)
* [[!UICONTROL Suppression de ressources de la collection]](#remove-assets-from-collection)
* [[!UICONTROL Ajout d’une balise aux ressources]](#add-a-tag-to-assets)
* [[!UICONTROL Suppression d’une balise] à partir de ressources](#remove-a-tag-from-assets)
* [[!UICONTROL Télécharger une ressource]](#download-asset)
* [[!UICONTROL Chargement d’une ressource]](#upload-asset)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Bynder] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Bynder] modules.

Lors de la configuration de ce module, les champs suivants s’affichent.

Le module renvoie un code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Saisissez un chemin relatif à <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
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

#### [!UICONTROL Lecture des métadonnées de ressource]

Ce module d’action lit les métadonnées d’une ressource.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td>Saisissez ou mappez l’identifiant de la ressource pour laquelle vous souhaitez récupérer des métadonnées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mise à jour des métadonnées de ressource]

Ce module d’action met à jour les métadonnées d’une ressource existante.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td>Saisissez ou mappez l’identifiant de la ressource pour laquelle vous souhaitez mettre à jour les métadonnées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Sélectionnez les champs pour lesquels vous souhaitez saisir des informations, puis saisissez ou mappez les informations avec lesquelles vous souhaitez mettre à jour les métadonnées dans ces champs. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaproperties]</p> </td> 
   <td>Sélectionnez les options à mettre à jour, puis saisissez ou mappez les informations dans ces propriétés. Les propriétés des métadonnées sont des informations sur la ressource qui ne représentent pas de champs spécifiques dans la ressource.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajout de ressources à une collection]

Ce module d’action ajoute une ou plusieurs ressources à une collection.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de collection]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la collection dans laquelle vous souhaitez ajouter des ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource à ajouter à la collection, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’ID de ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression de ressources de la collection]

Ce module d’action supprime une ou plusieurs ressources d’une collection.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de collection]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la collection dans laquelle vous souhaitez supprimer des ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource à supprimer de la collection, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’ID de ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajout d’une balise aux ressources]

Ajout d’une balise à une ou plusieurs ressources

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de balise]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la balise à ajouter aux ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource à baliser, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’ID de ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’une balise des ressources]

Suppression d’une balise d’une ou de plusieurs ressources

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de balise]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la balise à supprimer des ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource dont vous souhaitez supprimer une balise, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’ID de ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger une ressource]

Ce module d’action télécharge une seule ressource.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td>Saisissez ou mappez l’identifiant de la ressource que vous souhaitez télécharger.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version de la ressource]</td> 
   <td> <p>Saisissez ou mappez la version de la ressource que vous souhaitez télécharger. Pour télécharger la dernière version de la ressource, laissez le champ vide.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chargement d’une ressource]

Ce module d’action charge une seule ressource.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enregistrer sous]</td> 
   <td> <p>Sélectionnez le mode d’enregistrement du fichier que vous téléchargez.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nouvelle ressource]</strong> </p> <p>Sélectionnez les champs et propriétés de métadonnées pour lesquels vous souhaitez saisir des informations, puis saisissez les informations dans ces champs.</p> <p>Saisissez ou mappez l’identifiant de la marque que vous souhaitez utiliser pour la ressource chargée.</p> </li> 
     <li> <p><strong>[!UICONTROL Nouvelle version de ressource]</strong> </p> <p>Saisissez l’identifiant de la ressource pour laquelle vous téléchargez une nouvelle version.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fichier source]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Enregistrement de liste]](#list-record)
* [[!UICONTROL Recherche de ressources]](#search-for-assets)

#### [!UICONTROL Enregistrement de liste]

Ce module de recherche récupère tous les éléments d’un type spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez répertorier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Lire toutes les collections]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Lire les informations sur toutes les balises]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Lire toutes les ressources d’une collection]</strong> </p> <p>Saisissez ou mappez l’identifiant de la collection dont vous souhaitez répertorier les ressources.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Recherche de ressources]

Ce module de recherche recherche des ressources en fonction des critères que vous fournissez.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critères]</td> 
   <td> <p>Renseignez les critères de recherche. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Sélectionnez le champ que vous souhaitez utiliser dans votre recherche.</p> </li> 
     <li> <p><strong>[!UICONTROL Opérateur logique]</strong> </p> <p>Sélectionnez l’opérateur que vous souhaitez utiliser dans votre recherche.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Saisissez ou mappez la valeur à rechercher dans le champ sélectionné. Le type de valeur doit être identique au type de données du champ sélectionné. </p> <p>Pour plus d’informations sur les types de données, voir <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Types de données d’élément dans [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Jeu de résultats]</td> 
   <td>Indiquez si vous souhaitez renvoyer la première ressource correspondante ou toutes les ressources correspondantes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trier par]</td> 
   <td> <p>Sélectionnez le champ en fonction duquel vous souhaitez effectuer un tri.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Direction du tri]</td> 
   <td> <p>Indiquez si vous souhaitez trier par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Triggers

#### [!UICONTROL Affichage des ressources]

Ce module de déclenchement lance un scénario lorsqu’une ressource est créée ou mise à jour.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Bynder] compte à [!DNL Workfront Fusion], voir <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] to [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Collections]</td>
   <td> <p>Sélectionnez la collection que vous souhaitez surveiller pour de nouvelles ressources. Pour afficher toutes les collections, laissez ce champ vide.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limite]</td>

<td> <p>Saisissez le nombre maximum d'enregistrements que le module doit renvoyer au cours de chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>
