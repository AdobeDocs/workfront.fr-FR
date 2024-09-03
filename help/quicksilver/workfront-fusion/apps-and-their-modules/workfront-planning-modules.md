---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Workfront Planning
description: Avec les modules  [!DNL Adobe Workfront Planning] , vous pouvez lancer un scénario [!DNL Adobe Workfront Fusion] basé sur les événements de votre compte  [!DNL Adobe] Workfront Planning, créer, lire ou mettre à jour des accords et d’autres enregistrements, rechercher des enregistrements à l’aide de critères que vous définissez et télécharger des documents.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: e067c5ff34c31060ca6fd392289d845f53a5ef3a
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 84%

---

# Modules [!DNL Adobe Workfront Planning]

Avec les modules [!DNL Adobe Workfront Planning], vous pouvez déclencher un scénario lorsque des événements se produisent dans la planification Workfront. Vous pouvez également créer, lire, mettre à jour et supprimer des enregistrements, ou effectuer un appel API personnalisé vers votre compte [!DNL Adobe Workfront Planning].

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
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez la section licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Créer une connexion à [!DNL Adobe Workfront Planning]

Vous pouvez créer une connexion à votre compte [!DNL Workfront Planning] directement depuis l’intérieur d’un module [!DNL Workfront Fusion].

1. Dans n’importe quel module d’application [!DNL Workfront Planning], cliquez sur **[!UICONTROL Ajouter]** à côté de la zone [!UICONTROL Connexion].
1. Saisissez un nom pour cette connexion.
1. Indiquez si vous souhaitez vous connecter à un environnement de production ou à un environnement hors production.
1. Indiquez si vous vous connectez à un compte de service ou à un compte personnel.
1. Cliquez sur **[!UICONTROL Connexion SAML]** pour créer la connexion et revenir au module.

## Modules [!DNL Adobe Workfront Planning] et leurs champs

### Surveiller les événements

Ce module de déclenchement lance un scénario lorsqu’un enregistrement, un type d’enregistrement ou un espace de travail est créé, mis à jour ou supprimé dans Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Sélectionnez le webhook à utiliser ou cliquez sur Ajouter pour en créer un nouveau.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>Indiquez si vous souhaitez surveiller des enregistrements, des types d’enregistrement ou des espaces de travail.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>Vous pouvez définir des filtres pour ne surveiller que les enregistrements qui répondent aux critères sélectionnés.</p> <p>Pour chaque filtre, saisissez le champ que le filtre doit évaluer, l’opérateur et la valeur que le filtre doit autoriser. Vous pouvez utiliser plusieurs filtres en ajoutant des règles ET.</p> <p>Note : vous ne pouvez pas modifier les filtres dans les webhooks [!DNL Workfront] existants. Pour configurer différents filtres pour les abonnements aux événements [!DNL Workfront], supprimez le webhook actuel et créez-en un nouveau.</p> <p>Pour plus d’informations sur les filtres d’événements, voir <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Filtres d’abonnement aux événements dans les modules [!DNL Workfront] &gt; [!UICONTROL Surveiller les événements]</a> de l’article sur les modules Workfront.</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">[!UICONTROL Objects to watch]</td>
      <td>Indiquez si vous souhaitez surveiller les enregistrements. nouveaux, mis à jour, nouveaux et mis à jour ou supprimés.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Exclude updates made by this connection]</p>
      </td>
      <td>Activez cette option pour empêcher le déclenchement du scénario lorsqu’une modification est effectuée par la connexion utilisée par ce module. Cela empêche qu’une autre instance du scénario soit déclenchée si ce scénario exécute une action de déclenchement.</td> 
      </tr>
  </tbody>
</table>

### Supprimer un type d’enregistrement

Ce module d’action supprime un seul type d’enregistrement dans la planification Workfront par son identifiant.

>[!WARNING]
>
>La suppression d’un type d’enregistrement dans Workfront Planning supprime également tous les enregistrements de la table des types d’enregistrement.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Saisissez ou mappez l’ID du champ à supprimer.</td> 
      </tr>
  </tbody>
</table>

### Effectuer un appel API personnalisé.

Ce module lance un appel API personnalisé à l’API [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Saisissez un chemin relatif à https://&amp;ltWORKFRONT_DOMAIN&gt;/attask/api/&amp;ltAPI_VERSION&gt;/</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API version]</p>
      </td>
      <td>
        <p>Sélectionnez la version d’API que vous souhaitez utiliser. Si vous ne sélectionnez pas de version, la version la plus récente est utilisée par défaut.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API Path override]</p>
      </td>
      <td>
        <p>Saisissez un chemin relatif à https://&amp;ltWORKFRONT_DOMAIN&gt;/attask/api/&amp;ltAPI_VERSION&gt;/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] Ajoute automatiquement des en-têtes d’autorisation.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Pour chaque paire clé/valeur à ajouter à la chaîne de requête, cliquez sur <b>Ajouter un élément</b> et saisissez la clé et la valeur.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Workfront Planning by its ID.

>[!WARNING]
>
>Deleting a field in Workfront Planning deletes it and any data in it from every object of that record type in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Workfront Planning by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Créer un enregistrement

Cette action crée un seul enregistrement dans la planification Workfront.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Saisissez ou mappez le type d’enregistrement que vous souhaitez créer. Les types d’enregistrement disponibles sont basés sur votre compte de planification Workfront.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Autres champs</p>
      </td>
      <td>Ces champs sont basés sur le type d’enregistrement que vous avez sélectionné.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Supprimer un enregistrement

Ce module d’action supprime l’enregistrement spécifié dans la planification Workfront.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Saisissez ou mappez l’ID de l’enregistrement que vous souhaitez supprimer.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Obtenir un enregistrement

Ce module d’action récupère un seul enregistrement d’[!DNL Adobe Workfront Planning] spécifié par son ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Saisissez ou mappez l’ID de l’enregistrement que vous souhaitez récupérer.</td>
    </tr>
  </tbody>
</table>

### Obtenir des enregistrements par type d’enregistrement

Ce module d’action récupère tous les enregistrements du type spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Sélectionnez ou mappez l’espace de travail qui contient les enregistrements que vous souhaitez récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Sélectionnez le type d’enregistrement que vous souhaitez récupérer.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tbody>
</table>

### Obtenir des types d’enregistrement

Ce module d’action récupère une liste de types d’enregistrement dans un compte [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
  </tbody>
</table>

### Mettre à jour l’enregistrement

Cette action met à jour un seul enregistrement dans la planification Workfront.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer une connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Saisissez ou mappez le type d’enregistrement que vous souhaitez mettre à jour. Les types d’enregistrement disponibles sont basés sur votre compte de planification Workfront.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Autres champs</p>
      </td>
      <td>Ces champs sont basés sur le type d’enregistrement que vous avez sélectionné.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Rechercher des enregistrements

Ce module d’action récupère une liste d’enregistrements en fonction des critères que vous spécifiez.

>[!NOTE]
>
>Ce module est en construction.
