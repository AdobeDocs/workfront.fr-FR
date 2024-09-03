---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Lightroom
description: Avec les modules Adobe Lightroom, vous pouvez démarrer un scénario de fusion Adobe Workfront en fonction des événements de votre compte Adobe Lightroom.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: e48bdf18-49f0-436e-9182-16c9da2b3169
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 23%

---

# Modules [!DNL Adobe Lightroom]

<!--Add Connection info-->

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Lightroom] et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
      <td>
        <p>[!UICONTROL Pro] ou version supérieure</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produit</td>
      <td>Votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice de [!DNL Workfront].

&#42;&#42;Pour plus d’informations sur les [!DNL Adobe Workfront Fusion] licences, voir [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Conditions préalables

Avant d’utiliser le connecteur [!DNL Adobe Lightroom], vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez disposer d’un compte [!DNL Adobe Lightroom].

## Création d’une connexion à Adobe Lightroom



## Modules Adobe Lightroom et leurs champs

Lorsque vous configurez les modules [!DNL Adobe Lightroom], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Adobe Lightroom] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Autre](#other)
* [Ressources](#assets)
* [Albums](#albums)

### Autre

* [Contrôle de l’intégrité](#health-check)
* [Récupération des métadonnées du catalogue d’utilisateurs](#retrieve-user-catalog-metadata)

#### Contrôle de l’intégrité

Ce module d’action récupère un ID de version de serveur Lightroom, indiquant si le service Lightroom est en cours d’exécution.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>Si vous souhaitez fournir des informations d’identification spécifiques pour vous assurer qu’un serveur spécifique est en cours d’exécution, cliquez sur Ajouter un élément et saisissez les informations d’identification.</p><p>Les en-têtes d’autorisation sont ajoutés automatiquement.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Récupération des métadonnées du catalogue d’utilisateurs

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>Si vous souhaitez fournir des informations d’identification spécifiques pour vous assurer que vous pouvez accéder au compte utilisateur approprié, cliquez sur Ajouter un élément et saisissez les informations d’identification.</p><p>Les en-têtes d’autorisation sont ajoutés automatiquement.</p>
      </td>
    </tr>
  </tbody>
</table>

### Ressources

* [Création d’un fichier d’origine de ressource](#create-an-asset-external-xmp-develop-setting-file)
* [Création d’une ressource](#create-an-asset)
* [Création d’une ressource externe XMP développement d’un fichier de paramètres](#create-an-asset-external-xmp-develop-setting-file)
* [Générer des rendus pour un fichier d’origine](#generate-renditions-for-an-original-file)
* [Obtenir une ressource de catalogue](#get-a-catalog-asset)
* [Obtenir le dernier paramètre de développement de XMP de ressources externes](#get-the-latest-asset-external-xmp-develop-setting-file)
* [Obtention du dernier rendu de ressource](#get-the-latest-asset-rendition)
* [Récupération des ressources](#retrieve-assets)

#### Création d’un fichier d’origine de ressource

Ce module d’action crée et charge un fichier d’origine pour une ressource.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la ressource pour laquelle vous souhaitez créer et charger un fichier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Longueur du contenu en octets]</td>
      <td>
        <p>Saisissez ou mappez la longueur du contenu en octets.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Période]</td>
      <td>
        <p>Entrez ou mappez la plage d’octets pour la requête, y compris les premiers et derniers octets et la longueur d’entité, comme défini dans la norme RFC 2616. Doit être inclus uniquement lorsque les données sont trop volumineuses pour être chargées dans un seul appel.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content type]</td>
      <td>
        <p>Sélectionnez le type de contenu du nouveau fichier.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Création d’une ressource

Ce module d’action crée une ressource avec des métadonnées initiales et des informations d’importation.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue dans lequel la ressource sera créée.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la nouvelle ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type de ressource]</td>
      <td>
        <p>Indiquez si la ressource est une image ou une vidéo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user created]</td>
      <td>
        <p>Entrez ou mappez une date au format <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mise à jour de l’utilisateur Datetime]</td>
      <td>
        <p>Entrez ou mappez une date au format <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Date de capture]</td>
      <td>
        <p>Entrez ou mappez une date au format <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Création d’une ressource externe XMP développement d’un fichier de paramètres

Ce module d’action prend en charge deux workflows. Le premier workflow consiste à charger le fichier de paramètres de développement XMP externe de la ressource. Le deuxième workflow consiste à créer un fichier de paramètres de développement de XMP externe en le copiant à partir du fichier de paramètres de développement xmp externe d’une autre ressource.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Longueur du contenu en octets]</td>
      <td>
        <p>Saisissez ou mappez la longueur du contenu en octets.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Télécharger un nouveau fichier ou copier XMP/développer un fichier]</td>
      <td>
        <p>Choisissez si vous téléchargez un nouveau fichier ou si vous copiez un fichier à partir d’une ressource existante.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la ressource vers laquelle vous souhaitez charger ou copier un fichier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Lien vers XMP/développer un fichier]</td>
      <td>
        <p>Saisissez ou mappez un lien vers le fichier que vous souhaitez charger ou copier.</p><p>Ce fichier doit être au format JSON lors de la copie d’un fichier ou au format XML lors du téléchargement d’un fichier.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Générer des rendus pour un fichier d’origine

Ce module d’action génère de manière asynchrone des rendus pour un fichier d’origine.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type(s) de rendu (séparés par des points-virgules)]</td>
      <td>
        <p>Saisissez le type de rendu à créer. Si vous entrez plusieurs types, séparez-les par un point-virgule (;). <p>Types possibles :</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Longueur du contenu en octets]</td>
      <td>
        <p>Saisissez ou mappez la longueur du contenu en octets.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la ressource pour laquelle vous souhaitez créer un rendu d’un fichier.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Obtenir une ressource de catalogue

Ce module d’action récupère des informations sur une seule ressource dans un catalogue. Le catalogue doit être détenu par l’utilisateur dont les informations d’identification sont représentées dans la connexion utilisée dans ce module.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la ressource pour laquelle vous souhaitez récupérer des informations.</p>
      </td>
    </tr>
  </tbody>
</table>


#### Obtenir la dernière ressource externe XMP développer un fichier de paramètres

Ce module d’action récupère le fichier de paramètres XMP externe de ressource le plus récent.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la ressource associée au fichier de paramètres de développement XMP.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Obtention du dernier rendu de ressource

Ce module d’action récupère le dernier rendu de ressource du type spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la ressource associée au fichier de paramètres de développement XMP.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type de rendu]</td>
      <td>
        <p>Sélectionnez le type de rendu à récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Récupération des ressources

Ce module d’action récupère les ressources détenues par l’utilisateur dont les informations d’identification sont représentées dans la connexion utilisée dans ce module.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Date et heure de début]</td>
      <td>
        <p>Saisissez ou mappez un horodatage. Le module renvoie les enregistrements qui ont été mis à jour après cet horodatage.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Retour des ressources capturées avant]</td>
      <td>
        <p>Saisissez une date au format <code>YYYY-MM-DDT00:00:00</code>. Le module renvoie les résultats capturés avant cette date.</p><p> Ce champ ne peut pas être utilisé avec le champ <code>Return assets captured after</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre maximal de ressources renvoyées]</td>
      <td>
        <p>Définissez le nombre maximal de ressources que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution. Ce nombre doit être inférieur ou égal à 100.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SHA256 Valeur de hachage du fichier d’origine]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Masquer les ressources qui se trouvent dans les piles ?"]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Valeurs du sous-type de ressource]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset IDs]</td>
      <td>
        <p>Entrez ou mappez jusqu’à 100 identifiants de ressource, séparés par des virgules.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Types de ressources à exclure]</td>
      <td>
        <p>Sélectionnez cette option si vous souhaitez exclure des ressources complètes ou incomplètes. Pour inclure toutes les ressources, laissez ce champ vide.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Valeurs du groupe]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Valeurs du nom]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL État favori]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### Albums

* [Ajout de ressources à un album](#add-assets-to-an-album)
* [Création d’un album](#create-an-album)
* [Suppression d’un album](#delete-an-album)
* [Obtenir un album](#get-an-album)
* [Liste des ressources d’un album](#list-assets-of-an-album)
* [Récupération des albums](#retrieve-albums)
* [Mettre à jour un album](#update-album)

#### Ajout de ressources à un album

Ce module d’action ajoute une ou plusieurs ressources à l’album spécifié. Vous pouvez ajouter jusqu’à 50 ressources dans un cycle d’exécution.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue contenant l’album auquel vous souhaitez ajouter des ressources.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’album]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de l’album auquel vous souhaitez ajouter des ressources.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets]</td>
      <td>
        <p>Pour chaque ressource à ajouter à l’album, cliquez sur <b>Ajouter un élément</b> et saisissez les champs suivants.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de la ressource à ajouter à l’album.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Cette ressource est-elle une couverture d’album ?]</td>
      <td>
        <p>Indiquez si vous souhaitez que cette ressource s’affiche comme image représentant l’album.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Order]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Metadata]</td>
      <td>
        <p>Entrez ou mappez les métadonnées que vous souhaitez inclure à la ressource. Il doit s’agir d’une chaîne de texte unique d’une longueur maximale de 1 à 24 caractères.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote ID]</td>
      <td>
        <p>Saisissez l’identifiant de la ressource.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Création d’un album

Ce module d’action crée un album dans Lightroom.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue dans lequel vous souhaitez créer un album.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’album]</td>
      <td>
        <p>Saisissez ou mappez un identifiant pour le nouvel album.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtype]</td>
      <td>
        <p>Sélectionnez le sous-type de l’album.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Clé API]</td>
      <td>
        <p>Saisissez la clé API du service qui crée l’album.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user created]</td>
      <td>
        <p>Entrez ou mappez une date au format <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mise à jour de l’utilisateur Datetime]</td>
      <td>
        <p>Entrez ou mappez une date au format <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nom de l’album]</td>
      <td>
        <p>Saisissez ou mappez un nom pour le nouvel album.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL ID de couverture]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant d’une ressource à utiliser comme couverture de cet album.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote ID]</td>
      <td>
        <p>Saisissez l’identifiant de la ressource.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Created date]</td>
      <td>
        <p>Entrez ou mappez une date au format <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Date de mise à jour]</td>
      <td>
        <p>Entrez ou mappez une date au format <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL L L’album est-il supprimé ?]</td>
      <td>
        <p>Activez cette option si le contenu affilié en externe a été supprimé.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL de l’emplacement pour modifier le contenu affilié]</td>
      <td>
        <p>S’il existe une URL permettant aux utilisateurs d’éditer le contenu de cet album, saisissez l’URL ici.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL de l’emplacement pour afficher le contenu affilié]</td>
      <td>
        <p>S’il existe une URL permettant aux utilisateurs d’afficher le contenu de cet album, saisissez l’URL ici.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Suppression d’un album

Ce module d’action supprime un album.

L’album supprimé doit avoir été créé par la même application cliente qui le supprime maintenant, et doit être de sous-type `project` ou `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue contenant l’album que vous souhaitez supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’album]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de l’album à supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Supprimer des albums enfants ?]</td>
      <td>
        <p>Indiquez si vous souhaitez supprimer les albums enfants de l’album supprimé.</p>
      </td>
    </tr>
  </tbody>
</table>

### Obtenir un album

Ce module d’action récupère l’album spécifié

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue contenant l’album que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’album]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de l’album que vous souhaitez récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Liste des ressources d’un album

Ce module d’action récupère une liste de ressources dans l’album spécifié.



#### Récupération des albums

Ce module d’action récupère une liste d’albums dans le catalogue spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue qui contient les albums que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtypes]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de l’album que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nom de l’album qui précède les résultats actuels]</td>
      <td>
        <p>Si vous paginez vos résultats, saisissez ou mappez le nom du dernier album sur la page précédente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre maximal d’albums renvoyés]</td>
      <td>
        <p>Définissez le nombre maximal de ressources que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution. La valeur par défaut de ce champ est 100. Ce module peut renvoyer plus d’albums que cette limite si plusieurs albums à la limite de la limite ont la même valeur <code>name_after</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Mettre à jour l’album

Ce module d’action met à jour l’album spécifié.

L’album mis à jour doit avoir été créé par la même application cliente que celle qui le met maintenant à jour et doit être de sous-type `project` ou `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Lightroom], voir <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Créer une connexion à [!DNL Adobe Lightroom]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de catalogue]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du catalogue contenant l’album que vous souhaitez mettre à jour.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’album]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant de l’album que vous souhaitez mettre à jour.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Autres champs</td>
      <td>
      <td>Pour obtenir une description des autres champs de ce module, voir <a href="#create-an-album" class="MCXref xref" >Créer un album</a> dans cet article.</td>
      </td>
    </tr>
  </tbody>
</table>
