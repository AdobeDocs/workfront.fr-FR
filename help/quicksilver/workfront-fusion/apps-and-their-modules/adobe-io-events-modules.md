---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Adobe I/O des modules d’événements
description: Avec les modules Événements d’Adobe I/O, vous pouvez lancer un scénario de fusion Adobe Workfront basé sur les événements de vos applications d’Adobe.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 18ad8098-9742-44d2-97cd-b0c2b5591538
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 42%

---

# Adobe I/O des modules d’événements

Avec les modules Événements d’Adobe I/O, vous pouvez lancer un scénario de fusion Adobe Workfront basé sur les événements dans les comptes et services d’Adobe qui n’ont pas de connecteur de fusion Workfront dédié.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou niveau supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan, Travail</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront Fusion**</td> 
   <td> <p>Workfront Fusion pour l’automatisation et l’intégration du travail </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter Adobe Workfront Fusion ainsi qu’Adobe Workfront pour utiliser les fonctionnalités décrites dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

&#42;&#42; Pour plus d’informations sur les licences Adobe Workfront Fusion, voir [Licences Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Conditions préalables

Avant de pouvoir utiliser le connecteur Adobe I/O Events, vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez disposer d’un compte Adobe actif.

## Informations sur l’API des événements d’Adobe I/O

Le connecteur Adobe I/O Events utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>https://api.adobe.io/events</td> 
  </tr>
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.6.7</td> 
  </tr>
 </tbody> 
 </table>

## Création d’une connexion à des événements d’Adobe I/O

Pour créer une connexion pour vos modules Événements d’Adobe I/O :

1. Cliquez sur Ajouter en regard de la zone Connexion .

1. Remplissez les champs suivants :

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">Nom de la connexion</td>
        <td>
          <p>Saisissez un nom pour cette connexion.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Type</td>
        <td>
          <p>Indiquez si vous souhaitez vous connecter à un compte de service ou à un compte personnel.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Portées supplémentaires</td>
        <td>Pour ajouter d’autres portées, cliquez sur <b>Ajouter un élément</b> et saisissez la portée.</td>
      </tr>
      <tr>
        <td role="rowheader">ID client</td>
        <td>Saisissez votre ID client d’Adobe. Vous pouvez le trouver dans la section Informations d’identification de Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Clé secrète client</td>
        <td>Saisissez votre secret client Adobe. Vous pouvez le trouver dans la section Informations d’identification de Adobe Developer Console</td>
      </tr>
      </tr>
        <tr>
        <td role="rowheader">ID d’organisation du client</td>
        <td>Saisissez votre ID d’organisation du client. Vous pouvez le trouver dans l’URL d’identification du projet : <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">ID d’identification</td>
        <td>Saisissez votre ID d’identification. Vous pouvez le trouver dans l’URL d’identification du projet : <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">Identifiant de l’organisation IMS</td>
        <td>Saisissez votre ID d’organisation Adobe. Vous pouvez le trouver dans la section Informations d’identification de Adobe Developer Console</td>
      </tr>
        <tr>
        <td role="rowheader">ID de projet</td>
        <td>Saisissez votre ID de projet. Vous pouvez le trouver dans l’URL d’identification du projet : <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">WORKSPACE ID</td>
        <td>Pour afficher l’Workspace ID de votre projet, téléchargez les détails du projet à partir de la page d’aperçu du projet dans Adobe Developer Console. </td>
      </tr>
    </tbody>
    </table>

1. Cliquez sur **Continuer** pour enregistrer la connexion et revenir au module.

## Adobe I/O des modules d’événements et de leurs champs

Lorsque vous configurez les modules [!DNL Adobe I/O Events], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Adobe I/O Events] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### Création d’une enregistrement d’événement

Ce module d’action utilise un webhook pour créer une description d’événement. Vous pouvez configurer un webhook ici. Si vous utilisez un webhook existant, les champs de ce module sont en lecture seule.

Pour créer un webhook :

1. Cliquez sur **Ajouter** en regard du champ Webhook.
1. Remplissez les champs suivants :

   <table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Webhook name]</td>
        <td>Saisissez le nom de ce webhook.</td>
       </tr>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe I/O Events], voir <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Créer une connexion à [!DNL Adobe I/O Events]</a> dans cet article.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Description du webhook]
         </td>
         <td>
           Saisissez une description pour ce webhook.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event provider]
         </td>
         <td>
           Sélectionnez le produit ou le compte à partir duquel vous souhaitez créer des événements.
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event type]
         </td>
         <td>
           Sélectionnez les événements que le webhook doit surveiller. Le scénario se déclenche lorsque ces événements se produisent.
         </td>
       </tr>
     </tbody>
   </table>

1. Cliquez sur Enregistrer pour enregistrer le webhook et revenir au module.

### Actions

#### Obtenir tous les événements d’un journal

Ce module de recherche récupère tous les événements à enregistrer dans un journal.

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe I/O Events], voir <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Créer une connexion à [!DNL Adobe I/O Events]</a> dans cet article.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL ID d’enregistrement]
         </td>
         <td>
           Sélectionnez l’enregistrement pour lequel vous souhaitez récupérer les événements.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Maximum number of returned records]
         </td>
         <td>
              Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario. 
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Événements de retour qui se produisent après]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Rechercher]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Dernière version]
         </td>
         <td>
         Activez cette option pour renvoyer le dernier événement.
         </td>
       </tr>
     </tbody>
   </table>

#### Effectuer un appel API personnalisé.

Ce module d’action effectue un appel API personnalisé à l’API [!DNL Adobe I/O Events].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe I/O Events], voir <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Créer une connexion à [!DNL Adobe I/O Events]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Saisir un chemin relatif à <code>https://api.adobe.io/events</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
  <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p>  
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion ajoute automatiquement des en-têtes d’autorisation et des en-têtes x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Saisissez la chaîne de requête.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets autour de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Recherches

#### Obtention des ID de fournisseur et d’événement

Ce module de recherche récupère les identifiants d’événements d’Adobe I/O pour le fournisseur et les événements spécifiés.

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe I/O Events], voir <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Créer une connexion à [!DNL Adobe I/O Events]</a> dans cet article.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event provider]
         </td>
         <td>
           Sélectionnez le fournisseur pour lequel vous souhaitez récupérer l’ID.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event type]
         </td>
         <td>
              Sélectionnez les événements pour lesquels vous souhaitez fournir des identifiants. Les événements sont disponibles en fonction du fournisseur d’événements. 
         </td>
       </tr>
     </tbody>
   </table>

<!--

Watch Events

This trigger module starts a scenario when an event occurs in the chosen Adobe product or service.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The source of the events you want to watch</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

-->
