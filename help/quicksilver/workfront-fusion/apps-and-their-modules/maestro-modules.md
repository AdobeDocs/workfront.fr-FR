---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Adobe Maestro
description: Avec la variable [!DNL Adobe Maestro] modules, vous pouvez lancer une [!DNL Adobe Workfront Fusion] selon les événements de votre [!DNL Adobe] Créez, lisez ou mettez à jour des contrats et d’autres enregistrements de compte Maestro, recherchez des enregistrements à l’aide de critères que vous définissez et téléchargez des documents.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: fe0c867b218879c1d0d969112eb62878782a40ad
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# [!DNL Adobe Maestro] modules

Avec la variable [!DNL Adobe Maestro] , vous pouvez déclencher un scénario lorsque des événements se produisent dans Maestro. Vous pouvez également créer, lire, mettre à jour et supprimer des enregistrements, ou effectuer un appel API personnalisé vers votre [!DNL Adobe Maestro] compte .

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
   <td>
   <p>Exigences de licence actuelles : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de l’[!UICONTROL Select] ou de l’[!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Créer une connexion à [!DNL Adobe Maestro]

Vous pouvez créer une connexion à votre [!DNL Maestro] compte directement depuis l’intérieur d’un [!DNL Workfront Fusion] module .

1. Dans n’importe quel [!DNL Maestro] module d’application, cliquez **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] de la boîte.
1. Saisissez un nom pour cette connexion.
1. Indiquez si vous souhaitez vous connecter à un environnement de production ou à un environnement hors production.
1. Choisissez si vous vous connectez à un compte de service ou à un compte personnel.
1. Cliquez sur **[!UICONTROL Connexion SAML]** pour créer la connexion et revenir au module .

## [!DNL Adobe Maestro] modules et leurs champs

### Événements de contrôle

Ce module de déclenchement lance un scénario lorsqu’un enregistrement, un type d’enregistrement ou un espace de travail est créé, mis à jour ou supprimé dans Maestro.

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
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type d’objet]</td>
      <td>Indiquez si vous souhaitez consulter des enregistrements, des types d’enregistrement ou des espaces de travail.</td>
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

Ce module d’action supprime un seul type d’enregistrement dans Maestro par son identifiant.

>[!WARNING]
>
>La suppression d’un type d’enregistrement dans Maestro supprime également tous les enregistrements de la table des types d’enregistrement.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
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

Ce module effectue un appel API personnalisé à la fonction [!DNL Adobe Maestro] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Saisissez un chemin relatif à https://&lt;DOMAINE_WORKFRONT&gt;/ATask/api/&lt;VERSION_API&gt;/</p>
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
        <p>Saisissez un chemin relatif à https://&lt;DOMAINE_WORKFRONT&gt;/ATask/api/&lt;VERSION_API&gt;/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Méthode [!UICONTROL]</p>
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
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


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
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

Cette action crée un seul enregistrement dans Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de type d’enregistrement]</p>
      </td>
      <td>Saisissez ou mappez le type d’enregistrement que vous souhaitez créer. Les types d’enregistrement disponibles sont basés sur votre compte Maestro.</td> 
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

Ce module d’action supprime l’enregistrement spécifié dans Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
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

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
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

Ce module d’action récupère un seul enregistrement de [!DNL Adobe Maestro], spécifié par son identifiant.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
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
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
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
      <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</td> 
  </tbody>
</table>

### Obtention des types d’enregistrement

Ce module d’action récupère une liste de types d’enregistrement dans une [!DNL Adobe Maestro] compte .

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
    </tr>
  </tbody>
</table>

### Mettre à jour l’enregistrement

Cette action met à jour un seul enregistrement dans Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Maestro], voir <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Créer une connexion à [!DNL Adobe Maestro]</a> dans cet article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Saisissez ou mappez le type d’enregistrement que vous souhaitez mettre à jour . Les types d’enregistrement disponibles sont basés sur votre compte Maestro.</td> 
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

### Recherche d’enregistrements

Ce module d’action récupère une liste d’enregistrements en fonction des critères que vous spécifiez.

>[!NOTE]
>
>Ce module est en construction.

