---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
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
ht-degree: 44%

---

# Modules [!DNL Adobe Workfront Planning]

Avec les modules [!DNL Adobe Workfront Planning], vous pouvez déclencher un scénario lorsque des événements se produisent dans la planification Workfront. Vous pouvez également créer, lire, mettre à jour et supprimer des enregistrements, ou effectuer un appel API personnalisé vers votre compte [!DNL Adobe Workfront Planning].

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

## Créer une connexion à [!DNL Adobe Workfront Planning]

Vous pouvez créer une connexion à votre compte [!DNL Workfront Planning] directement à partir de l’intérieur d’un module [!DNL Workfront Fusion].

1. Dans n&#39;importe quel module d&#39;application [!DNL Workfront Planning], cliquez sur **[!UICONTROL Ajouter]** en regard de la zone [!UICONTROL Connexion].
1. Nommez cette connexion.
1. Indiquez si vous souhaitez vous connecter à un environnement de production ou à un environnement hors production.
1. Choisissez si vous vous connectez à un compte de service ou à un compte personnel.
1. Cliquez sur **[!UICONTROL connexion SAML dans]** pour créer la connexion et revenir au module.

## Modules [!DNL Adobe Workfront Planning] et leurs champs

### Événements de contrôle

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
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>Indiquez si vous souhaitez consulter des enregistrements, des types d’enregistrement ou des espaces de travail.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>Vous pouvez définir des filtres pour ne surveiller que les enregistrements qui répondent aux critères sélectionnés.</p> <p>Pour chaque filtre, saisissez le champ que le filtre doit évaluer, l’opérateur et la valeur que le filtre doit autoriser. Vous pouvez utiliser plusieurs filtres en ajoutant des règles ET.</p> <p>Remarque : vous ne pouvez pas modifier les filtres dans les webhooks [!DNL Workfront] existants. Pour configurer différents filtres pour les abonnements aux événements [!DNL Workfront], supprimez le webhook actuel et créez-en un nouveau.</p> <p>Pour plus d’informations sur les filtres d’événements, voir <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Filtres d’abonnement aux événements dans les modules [!DNL Workfront] &gt; [!UICONTROL Surveiller les événements]</a> de l’article sur les modules Workfront.</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">[!UICONTROL Objets à surveiller]</td>
      <td>Indiquez si vous souhaitez vérifier les nouvelles données. des enregistrements mis à jour, nouveaux et mis à jour ou supprimés.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Exclure les mises à jour effectuées par cette connexion]</p>
      </td>
      <td>Activez cette option pour empêcher le déclenchement du scénario lorsqu’une modification est effectuée par la connexion utilisée par ce module. Cela empêche qu’une autre instance du scénario soit déclenchée si ce scénario exécute une action de déclenchement.</td> 
      </tr>
  </tbody>
</table>

### Suppression d’un type d’enregistrement

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
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de type d’enregistrement]</p>
      </td>
      <td>Saisissez ou mappez l’identifiant du champ à supprimer.</td> 
      </tr>
  </tbody>
</table>

### Effectuer un appel API personnalisé

Ce module effectue un appel API personnalisé à l’API [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
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
        <p>[!UICONTROL Version de l’API]</p>
      </td>
      <td>
        <p>Sélectionnez la version d’API que vous souhaitez utiliser. Si vous ne sélectionnez pas de version, la version la plus récente est utilisée par défaut.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Remplacement du chemin de l’API]</p>
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
        <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation.</p>
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
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

### Création d’un enregistrement

Cette action crée un seul enregistrement dans la planification Workfront.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de type d’enregistrement]</p>
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

### Suppression d’un enregistrement

Ce module d’action supprime l’enregistrement spécifié dans la planification Workfront.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez supprimer.</td> 
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

### Obtention d’un enregistrement

Ce module d’action récupère un seul enregistrement de [!DNL Adobe Workfront Planning], spécifié par son identifiant.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez récupérer.</td>
    </tr>
  </tbody>
</table>

### Obtention des enregistrements par type d’enregistrement

Ce module d&#39;action récupère tous les enregistrements du type spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Sélectionnez ou mappez l’espace de travail qui contient les enregistrements que vous souhaitez récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
      <td>Sélectionnez le type d’enregistrement que vous souhaitez récupérer.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Nombre maximal d’enregistrements renvoyés]</p>
      </td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tbody>
</table>

### Obtention des types d’enregistrement

Ce module d’action récupère une liste de types d’enregistrement dans un compte [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
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
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Workfront Planning], voir <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Créer la connexion à [!DNL Adobe Workfront Planning]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Saisissez ou mappez le type d’enregistrement que vous souhaitez mettre à jour . Les types d’enregistrement disponibles sont basés sur votre compte de planification Workfront.</td> 
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
