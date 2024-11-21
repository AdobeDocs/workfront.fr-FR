---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules ServiceNow
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL ServiceNow]et le connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 97%

---

# Modules [!DNL ServiceNow]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL ServiceNow] et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL ServiceNow], vous devez disposer d’un compte [!DNL ServiceNow].

## Informations sur l’API ServiceNow

Le connecteur ServiceNow utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>https://{{connection.instance}/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.5.13</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!DNL ServiceNow] à [!DNL Workfront Fusion]

Pour créer une connexion pour vos modules [!DNL ServiceNow], procédez comme suit :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la case [!UICONTROL Connexion] lorsque vous commencez à configurer le premier module [!DNL ServiceNow].
1. Saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>Saisir un nom pour la nouvelle connexion [!DNL ServiceNow]</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>Saisissez votre nom d’utilisateur ou d’utilisatrice [!DNL ServiceNow]</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>Saisissez votre mot de passe ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instance]</p> </td> 
      <td> <p>Saisissez l’adresse de votre compte [!DNL ServiceNow] sans <code>https://</code> (généralement <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Les modules [!UICONTROL ServiceNow] et leurs champs

Lorsque vous configurez des modules [!DNL ServiceNow], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL ServiceNow] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir la section [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Si un enregistrement personnalisé est sélectionné dans un « [!UICONTROL Type d’enregistrement] », le chargement des champs personnalisés peut prendre un certain temps.
>
>S’il n’existe aucun enregistrement personnalisé, le menu déroulant est vide.

* [[!UICONTROL Surveiller les enregistrements]](#watch-records)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Désactiver un utilisateur ou une utilisatrice]](#deactivate-a-user)
* [[!UICONTROL Télécharger une pièce jointe]](#download-an-attachment)
* [[!UICONTROL Charger une pièce jointe]](#upload-an-attachment)
* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)
* [[!UICONTROL Rechercher des enregistrements]](#search-for-records)

### [!UICONTROL Surveiller des enregistrements]

Ce module déclencheur active un scénario lorsqu’un enregistrement est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Indiquez si le tableau que vous souhaitez surveiller est un tableau personnalisé ou standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>Sélectionnez le type d’enregistrement à surveiller.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Sélectionnez le type de valeurs à afficher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Indiquez si vous souhaitez surveiller les nouveaux enregistrements ou les enregistrements mis à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel personnalisé et authentifié à l’API [!DNL ServiceNow]. Cela vous permet de créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL ServiceNow].

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>Saisissez l’adresse sur le serveur web avec lequel le module doit interagir.</p> <p>Vous pouvez saisir une URL relative, ce qui signifie que vous n’avez pas besoin d’inclure le protocole (comme <code>http://</code>) au début. Cela indique au serveur web que l’interaction se produit sur le serveur.</p> <p>Par exemple : <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lire un enregistrement]

Ce module d’action lit un enregistrement [!DNL ServiceNow] à l’aide de l’ID système.

Le module renvoie tous les champs standard associés à l’enregistrement, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Saisissez ou mappez l’ID [!DNL ServiceNow] unique de l’enregistrement que le module doit lire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Indiquez si l’enregistrement que vous souhaitez lire se trouve dans un tableau personnalisé ou un tableau standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL ServiceNow] que le module doit lire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Sélectionnez le type de valeurs à afficher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Désactiver un utilisateur ou une utilisatrice]

Ce module d’action désactive un utilisateur ou une utilisatrice dans [!DNL ServiceNow] à l’aide de l’ID système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> Saisissez ou mappez l’ID [!DNL ServiceNow] unique de l’utilisateur ou l’utilisatrice que le module doit désactiver.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Télécharger une pièce jointe]

Ce module d’action télécharge une pièce jointe dans un enregistrement [!DNL ServiceNow].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment System ID]</td> 
   <td> Saisissez ou mappez l’ID [!DNL ServiceNow] unique de la pièce jointe que le module doit télécharger.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Charger une pièce jointe]

Ce module d’action charge une pièce jointe dans un enregistrement [!DNL ServiceNow].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table name]</td> 
   <td>Saisissez ou mappez le nom de la table dans laquelle vous souhaitez charger la pièce jointe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>Saisissez ou mappez l’ID [!DNL ServiceNow] unique du système dans lequel vous souhaitez charger la pièce jointe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Saisissez ou mappez un nom pour la pièce jointe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File content]</td> 
   <td>Saisissez ou mappez le fichier que vous souhaitez charger dans [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un enregistrement [!DNL ServiceNow].

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Indiquez si vous souhaitez créer un enregistrement dans un tableau personnalisé ou un standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL ServiceNow] que vous souhaitez que le module crée. Vous pouvez ensuite remplir les champs disponibles pour ce type d’enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action crée un enregistrement [!DNL ServiceNow].

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Saisissez ou mappez l’identifiant [!DNL ServiceNow] unique de l’enregistrement que vous souhaitez que le module mette à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Indiquez si l’enregistrement à mettre à jour se trouve dans un tableau personnalisé ou standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL ServiceNow] que vous souhaitez que le module mette à jour. Vous pouvez ensuite remplir les champs disponibles pour ce type d’enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un incident ou une personne.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Indiquez si vous souhaitez supprimer un incident ou une personne.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>Saisissez ou mappez l’identifiant [!DNL ServiceNow] unique de l’enregistrement que vous souhaitez que le module supprime.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Rechercher des enregistrements]

Ce module recherche des enregistrements en fonction des critères que vous sélectionnez.

Le module renvoie tous les champs standard associés à l’enregistrement, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connecter [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>Indiquez si le tableau que vous souhaitez rechercher est un tableau personnalisé ou standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>Sélectionnez le type d’enregistrement à rechercher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Indiquez si vous souhaitez que le module renvoie tous les enregistrements qui correspondent aux critères ou seulement le premier enregistrement correspondant. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal count of records].</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search type]</td> 
   <td> <p>Sélectionnez le type de recherche que vous souhaitez que le module effectue.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Advanced query]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Query]</p> <p>Saisissez la requête personnalisée. Pour plus d’informations sur les requêtes de recherche personnalisées [!DNL ServiceNow], voir <a href="https://docs.servicenow.com/fr-FR/bundle/washingtondc-platform-user-interface/page/administer/navigation-and-ui/concept/c_NavigationAndTheUserInterface.html">Documentation sur les requêtes ServiceNow</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Criteria]</p> <p>Saisissez les critères selon lesquels vous souhaitez que le module effectue une recherche. Pour plus d’informations sur la configuration des filtres de recherche, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajouter un filtre à un scénario dans Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Sort by]</p> <p>Indiquez le champ selon lequel le module doit trier les résultats et si ceux-ci doivent être triés par ordre croissant ou décroissant.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Sélectionnez le type de valeurs à afficher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
 </tbody> 
</table>
