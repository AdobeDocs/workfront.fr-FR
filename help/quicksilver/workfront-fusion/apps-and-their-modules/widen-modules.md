---
title: Modules Widen
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 93%

---

# Modules [!DNL Widen]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Élargir les modules](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/widen-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!UICONTROL Widen] et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Conditions préalables

Pour utiliser les modules [!UICONTROL Widen], vous devez avoir un compte [!UICONTROL Widen].

## Informations sur l’API Widen

Le connecteur Widen utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.10.11</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!DNL Widen] à [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Vous pouvez créer une connexion à votre compte [!DNL Widen] directement à partir d’un module [!DNL Widen].

1. Dans n’importe quel module [!DNL Widen], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Sélectionnez le domaine [!DNL Widen] auquel vous souhaitez vous connecter.
1. Saisissez le jeton de votre compte [!DNL Widen]. Pour savoir comment trouver ce jeton, voir [[!DNL Widen] Questions fréquentes sur l’API ](https://community.widen.com/collective/s/article/API-FAQs).
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Widen] et leurs champs

Lorsque vous configurez les modules [!DNL Widen], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Widen] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Modules déclencheurs](#trigger-modules)
* [Modules d’action](#action-modules)
* [Modules de recherche](#search-modules)

### Modules déclencheurs

#### [!UICONTROL Surveiller les ressources]

Lorsqu’une ressource est créée ou mise à jour, ce module de déclenchement lance un scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event type]</td> 
   <td> <p>Indiquez si vous souhaitez surveiller les nouvelles ressources ou les ressources mises à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Sélectionnez les propriétés que vous souhaitez inclure dans la sortie du module en plus des champs de la resssource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum de ressources avec lesquelles vous souhaitez que le module travaille au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules d’action

* [[!UICONTROL Personnaliser un appel API]](#custom-api-call)
* [[!UICONTROL Lire les informations sur les ressources]](#read-asset-info)
* [[!UICONTROL Ajouter des ressources aux collections]](#add-assets-to-collections)
* [[!UICONTROL Supprimer des ressources de la collection]](#remove-assets-from-collection)
* [[!UICONTROL Mettre à jour des métadonnées des ressources]](#update-asset-metadata)
* [[!UICONTROL Télécharger le fichier]](#download-file)
* [[!UICONTROL Charger] un fichier](#upload-a-file)

#### [!UICONTROL Personnaliser un appel API]

Ce module d’action vous permet d’effectuer un appel personnalisé et authentifié à l’API [!DNL Widen]. Cela vous permet de créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Widen].

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Sélectionnez si vous souhaitez utiliser la dernière version de l’API [!DNL Widen], ou la version 1.0.</td> 
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
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, mettez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire les informations sur les ressources]

Ce module d’action permet de retrouver une ressource individuelle grâce à son ID unique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a>dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Saisissez ou mappez l’ID de la ressource dont vous souhaitez lire les informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Sélectionnez les propriétés que vous souhaitez inclure dans la sortie du module en plus des champs de la resssource.</p> </td> 
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
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez dans cet article la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>Pour chaque collection à laquelle vous souhaitez ajouter des ressouces :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’[!UICONTROL Collection ID].</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>Pour chaque ressource que vous souhaitez ajouter à une collection :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de la ressource.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum de ressources avec lesquelles vous souhaitez que le module travaille au cours de chaque cycle d’exécution de scénario.</p> </td> 
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
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez dans cet article la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>Pour chaque collection dont vous souhaitez supprimer les ressources :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de la collection.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de la ressource</td> 
   <td> <p>Pour chaque ressource que vous souhaitez supprimer d’une collection :</p> 
    <ol> 
     <li value="1"> <p> Cliquez sur <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Saisissez ou mappez l’ID de la ressource.</p> </li> 
     <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum de ressources avec lesquelles vous souhaitez que le module travaille au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour les métadonnées d’une ressource]

Ce module d’action met à jour les champs de métadonnées d’une ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a>dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Saisissez ou mappez l’ID de la ressource dont vous souhaitez mettre à jour les métadonnées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata type]</td> 
   <td> <p>Sélectionnez le type de métadonnées pour les métadonnées que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Sélectionnez les champs de métadonnées que vous souhaitez mettre à jour. Pour chaque champ, saisissez la nouvelle valeur du champ.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum de ressources avec lesquelles vous souhaitez que le module travaille au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un fichier]

Ce module d’action télécharge une ressource depuis votre compte [!DNL Widen].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a>dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la ressource que vous souhaitez télécharger.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Charger un fichier]

Ce module d’action charge un fichier dans votre compte [!DNL Widen].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], voir <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Profile]</td> 
   <td> <p>Sélectionnez le profil de chargement que vous souhaitez que le module utilise.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Method]</td> 
   <td> <p>Sélectionnez la manière dont vous souhaitez charger le fichier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL From File]</strong> </p> <p>Sélectionnez ou mappez le fichier source d’un module précédent.</p> </li> 
     <li> <p><strong>[!UICONTROL By URL]</strong> </p> <p>Saisissez ou mappez l’URL du fichier que vous souhaitez charger.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Saisissez ou mappez un nom pour le fichier chargé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata Type]</td> 
   <td>Sélectionnez le type de métadonnées pour le fichier que vous souhaitez charger.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Sélectionnez les champs de métadonnées que vous souhaitez inclure dans le chargement du fichier. Pour chaque champ, saisissez la [!UICONTROL value] du champ.</td> 
  </tr> 
 </tbody> 
</table>

### Modules de recherche

* [[!UICONTROL Lire les ressources de la collection]](#read-collection-assets)
* [[!UICONTROL Rechercher des ressources]](#search-assets)

#### [!UICONTROL Lire les ressources de la collection]

Ce module d’action permet de récupérer une liste de ressource au sein d’une collection.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a>dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Saisissez ou mappez l’ID de la collection qui contient les ressources que vous souhaitez lire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Saisissez ou mappez le numéro du premier élément que vous souhaitez répertorier. Il s’agit d’un moyen de paginer les enregistrements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>Sélectionnez la propriété par laquelle vous souhaitez trier les ressources. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Indiquez si vous souhaitez trier les ressources par ordre croissant ou décroissant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des ressources]

Ce module de recherche permet d’obtenir une liste des ressources correspondant aux critères de recherche spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Widen] à [!DNL Workfront Fusion], consultez la section <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search query]</td> 
   <td> <p>Saisissez les critères selon lesquels vous souhaitez rechercher des ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>Sélectionnez la manière dont vous souhaitez trier les ressources. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Indiquez si vous souhaitez trier les ressources par ordre croissant ou décroissant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include deleted]</td> 
   <td>Activez cette option pour inclure les ressources supprimées dans la recherche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archived]</p> </td> 
   <td> <p>Activez cette option pour inclure les ressources archivées dans la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search document text]</td> 
   <td>Activez cette option pour inclure le texte du document dans votre recherche, ou désactivez-la pour n’inclure que les ressources dont le titre correspond aux critères de recherche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>Saisissez ou affichez le numéro du premier élément dont vous souhaitez obtenir les détails. Il s’agit d’un moyen de paginer les enregistrements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>Activez cette option pour permettre le défilement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Sélectionnez les propriétés que vous souhaitez inclure dans la sortie du module en plus des champs de la resssource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
 </tbody> 
</table>
