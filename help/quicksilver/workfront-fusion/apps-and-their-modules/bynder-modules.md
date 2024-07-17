---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Bynder
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Bynder] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1661'
ht-degree: 29%

---

# Modules [!DNL Bynder]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Bynder] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Conditions préalables

Pour utiliser des modules [!DNL Bynder], vous devez disposer d’un compte [!DNL Bynder].

## Connexion de [!DNL Bynder] à Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Créez une connexion à  [!DNL Bynder] à partir de [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Générez un [!UICONTROL ID client] et un [!UICONTROL  secret client] dans  [!DNL Bynder] (facultatif)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Créez une connexion à [!DNL Bynder] à partir de [!DNL Workfront Fusion]

Vous pouvez créer une connexion de [!DNL Workfront Fusion] à votre compte [!DNL Bynder] directement depuis un module [!DNL Bynder].

1. Dans un module [!DNL Bynder], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Sélectionnez le domaine [!DNL Bynder] auquel vous souhaitez vous connecter.
1. (Facultatif) Cliquez sur **[!UICONTROL Paramètres avancés]**, puis saisissez votre [!UICONTROL ID client] et [!UICONTROL Secret client].

   Pour plus d’informations sur la génération de l’ID client et du secret client, voir [Génération d’un identifiant client et d’un secret client dans [!DNL Bynder] (facultatif)](#generate-a-client-id-and-client-secret-in-bynder-optional) de cet article.

1. Dans la fenêtre [!UICONTROL login] , saisissez votre nom d’utilisateur (adresse électronique) et votre mot de passe.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

### Générez un [!UICONTROL identifiant client] et un [!UICONTROL secret client] dans [!DNL Bynder] (facultatif)

Si vous souhaitez créer une connexion à l’aide de l’identifiant du client et du secret du client, vous pouvez les générer à partir de votre compte [!DNL Bynder]. L’identifiant du client et le secret du client sont générés lorsque vous créez une application dans [!DNL Bynder].

Pour obtenir des instructions sur la création d’une application dans [!DNL Bynder], voir [Oauth 2.0 Apps](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) dans la documentation [!DNL Bynder].

>[!NOTE]
>
>Lors de la création de l’application dans [!DNL Bynder], saisissez le texte suivant : `redirect uri` :
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## Modules [!DNL Bynder] et leurs champs

Lorsque vous configurez des modules [!DNL Bynder], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Bynder] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)
* [Déclencheurs](#triggers)

### Actions

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Lecture des métadonnées de ressource]](#read-asset-metadata)
* [[!UICONTROL Mise à jour des métadonnées de ressource]](#update-asset-metadata)
* [[!UICONTROL Ajouter des ressources à une collection]](#add-assets-to-a-collection)
* [[!UICONTROL Supprimer des ressources de la collection]](#remove-assets-from-collection)
* [[!UICONTROL Ajouter une balise aux ressources]](#add-a-tag-to-assets)
* [[!UICONTROL  Supprimer une balise] des ressources](#remove-a-tag-from-assets)
* [[!UICONTROL Télécharger la ressource]](#download-asset)
* [[!UICONTROL Télécharger la ressource]](#upload-asset)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Bynder]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Bynder].

Lors de la configuration de ce module, les champs suivants s’affichent.

Le module renvoie un code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Saisissez un chemin relatif à <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td>Saisissez ou mappez l’identifiant de la ressource pour laquelle vous souhaitez récupérer des métadonnées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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

#### [!UICONTROL Ajouter des ressources à une collection]

Ce module d’action ajoute une ou plusieurs ressources à une collection.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de collection]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la collection dans laquelle vous souhaitez ajouter des ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource à ajouter à la collection, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’ID de la ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer des ressources de la collection]

Ce module d’action supprime une ou plusieurs ressources d’une collection.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de collection]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la collection dans laquelle vous souhaitez supprimer des ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource que vous souhaitez supprimer de la collection, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’identifiant de la ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une balise aux ressources]

Ajout d’une balise à une ou plusieurs ressources

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de balise]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la balise à ajouter aux ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource que vous souhaitez baliser, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’identifiant de la ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une balise des ressources]

Suppression d’une balise d’une ou de plusieurs ressources

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de balise]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la balise à supprimer des ressources.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Pour chaque ressource à partir de laquelle vous souhaitez supprimer une balise, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis saisissez ou mappez l’identifiant de la ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger la ressource]

Ce module d’action télécharge une seule ressource.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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

#### [!UICONTROL Télécharger la ressource]

Ce module d’action charge une seule ressource.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enregistrer sous]</td> 
   <td> <p>Sélectionnez le mode d’enregistrement du fichier que vous téléchargez.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nouvelle ressource]</strong> </p> <p>Sélectionnez les champs et propriétés de métadonnées pour lesquels vous souhaitez saisir des informations, puis saisissez les informations dans ces champs.</p> <p>Saisissez ou mappez l’identifiant de la marque que vous souhaitez utiliser pour la ressource chargée.</p> </li> 
     <li> <p><strong>[!UICONTROL Nouvelle version de la ressource]</strong> </p> <p>Saisissez l’identifiant de la ressource pour laquelle vous téléchargez une nouvelle version.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [](#list-record)
* [[!UICONTROL Rechercher des ressources]](#search-for-assets)

#### 

Ce module de recherche récupère tous les éléments d’un type spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des ressources]

Ce module de recherche recherche des ressources en fonction des critères que vous fournissez.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critères]</td> 
   <td> <p>Renseignez les critères de recherche. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Sélectionnez le champ à utiliser dans votre recherche.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Déclencheurs

#### [!UICONTROL Surveiller les ressources]

Ce module de déclenchement lance un scénario lorsqu’une ressource est créée ou mise à jour.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Bynder] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Bynder] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>Saisissez le nombre maximum d'enregistrements que le module doit renvoyer au cours de chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>
