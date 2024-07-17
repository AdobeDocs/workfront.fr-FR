---
title: Modules Widen
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!UICONTROL Widen] et les connecter à plusieurs applications et services tiers.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 31%

---

# Modules [!DNL Widen]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!UICONTROL Widen], et les connecter à plusieurs applications et services tiers.

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

Pour utiliser les modules [!UICONTROL Widen], vous devez disposer d’un compte [!UICONTROL Widen].

## Connecter [!DNL Widen] à [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Vous pouvez créer une connexion à votre compte [!DNL Widen] directement à partir de l’intérieur d’un module [!DNL Widen].

1. Dans un module [!DNL Widen], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Sélectionnez le domaine [!DNL Widen] auquel vous souhaitez vous connecter.
1. Saisissez le jeton de votre compte [!DNL Widen]. Pour plus d’informations sur la localisation de ce jeton, consultez la [[!DNL Widen] FAQ sur l’API](https://community.widen.com/collective/s/article/API-FAQs).
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Widen] et leurs champs

Lorsque vous configurez des modules [!DNL Widen], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Widen] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Modules déclencheurs](#trigger-modules)
* [Modules d’action](#action-modules)
* [Modules de recherche](#search-modules)

### Modules déclencheurs

#### [!UICONTROL Surveiller les ressources]

Ce module de déclenchement lance un scénario lorsqu’une ressource est créée ou mise à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit utiliser au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules d’action

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Lire les informations sur les ressources]](#read-asset-info)
* [[!UICONTROL Ajouter des ressources aux collections]](#add-assets-to-collections)
* [[!UICONTROL Supprimer des ressources de la collection]](#remove-assets-from-collection)
* [[!UICONTROL Mise à jour des métadonnées de ressource]](#update-asset-metadata)
* [[!UICONTROL Télécharger le fichier]](#download-file)
* [[!UICONTROL Télécharger] un fichier](#upload-a-file)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Widen]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Widen].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version de l’API]</td> 
   <td>Indiquez si vous souhaitez utiliser la dernière version de l’API [!DNL Widen] ou la version 1.0.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez ou mappez l’URL de votre appel API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation à votre place.</p> </td> 
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

#### [!UICONTROL Lire les informations sur les ressources]

Ce module d’action récupère une ressource individuelle à l’aide de son identifiant unique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter des ressources aux collections]

Ce module d’action ajoute une ou plusieurs ressources aux collections.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>Pour chaque ressource à ajouter à une collection :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de ressource.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit utiliser au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer des ressources de la collection]

Ce module d’action supprime une ou plusieurs ressources des collections.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td role="rowheader">ASSETS ID</td> 
   <td> <p>Pour chaque ressource à supprimer d’une collection :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de ressource.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
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
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de ressources que le module doit utiliser au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger le fichier]

Ce module d’action télécharge une ressource à partir de votre compte [!DNL Widen].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la ressource que vous souhaitez télécharger.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un fichier]

Ce module d’action charge un fichier dans votre compte [!DNL Widen].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger le profil]</td> 
   <td> <p>Sélectionnez le profil de chargement que le module doit utiliser.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Méthode de téléchargement]</td> 
   <td> <p>Sélectionnez le mode de chargement du fichier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL À partir du fichier]</strong> </p> <p>Sélectionnez ou mappez le fichier source à partir d’un module précédent.</p> </li> 
     <li> <p><strong>[!UICONTROL Par URL]</strong> </p> <p>Saisissez ou mappez l’URL du fichier que vous souhaitez charger.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
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
* [[!UICONTROL Rechercher des ressources]](#search-assets)

#### [!UICONTROL Lecture des ressources de collection]

Ce module d’action récupère une liste de ressources dans une collection.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des ressources]

Ce module de recherche récupère une liste de ressources qui correspondent à des critères de recherche spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Widen] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Widen] à [!DNL Workfront Fusion] </a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>
