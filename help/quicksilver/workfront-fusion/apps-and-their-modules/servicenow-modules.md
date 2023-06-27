---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules ServiceNow
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL ServiceNow], ainsi que de la connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1613'
ht-degree: 1%

---

# [!DNL ServiceNow] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL ServiceNow], ainsi que de la connecter à plusieurs applications et services tiers.

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
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL ServiceNow] modules, vous devez disposer d’un [!DNL ServiceNow] compte .

## Connexion [!DNL ServiceNow] to [!DNL Workfront Fusion]

Pour créer une connexion pour votre [!DNL ServiceNow] modules :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] lorsque vous commencez à configurer la première [!DNL ServiceNow] module .
1. Saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nom de la connexion]</p> </td> 
      <td>Saisissez un nom pour la nouvelle [!DNL ServiceNow] connection</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>Saisissez votre [!DNL ServiceNow] nom d’utilisateur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>Saisissez votre mot de passe ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instance]</p> </td> 
      <td> <p>Saisissez l’adresse de votre [!DNL ServiceNow] compte sans <code>https://</code> (généralement <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] modules et leurs champs

Lorsque vous configurez [!DNL ServiceNow] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL ServiceNow] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Si un enregistrement personnalisé est sélectionné dans un[!UICONTROL Type d’enregistrement]&quot;, le chargement des champs personnalisés peut prendre un certain temps.
>
>S’il n’existe aucun enregistrement personnalisé, la liste déroulante est vide.

* [[!UICONTROL Surveiller les enregistrements]](#watch-records)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Désactivation d’un utilisateur]](#deactivate-a-user)
* [[!UICONTROL Téléchargement d’une pièce jointe]](#download-an-attachment)
* [[!UICONTROL Chargement d’une pièce jointe]](#upload-an-attachment)
* [[!UICONTROL Création d’un enregistrement]](#create-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Suppression d’un enregistrement]](#delete-a-record)
* [[!UICONTROL Recherche d’enregistrements]](#search-for-records)

### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement active un scénario lorsqu’un enregistrement est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si le tableau que vous souhaitez regarder est un tableau personnalisé ou standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td>Sélectionnez le type d’enregistrement à regarder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Sélectionnez le type de valeurs à afficher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Indiquez si vous souhaitez regarder les nouveaux enregistrements ou les enregistrements mis à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL ServiceNow] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL ServiceNow] modules.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relative]</td> 
   <td> <p>Saisissez l’adresse sur le serveur web avec lequel le module doit interagir.</p> <p>Vous pouvez saisir une URL relative, ce qui signifie que vous n’avez pas besoin d’inclure le protocole (tel que <code>http://</code>) au début. Cela indique au serveur web que l’interaction se produit sur le serveur.</p> <p>Par exemple : <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lire un enregistrement]

Ce module d’action lit une [!DNL ServiceNow] Enregistrez à l’aide de l’ID système.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Saisissez ou mappez l’unique [!DNL ServiceNow] Identifiant de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si l'enregistrement que vous souhaitez lire se trouve dans une table personnalisée ou une table standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type de [!DNL ServiceNow] enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Sélectionnez le type de valeurs à afficher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Désactivation d’un utilisateur]

Ce module d’action désactive un utilisateur dans [!DNL ServiceNow] en utilisant l’ID système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> Saisissez ou mappez l’unique [!DNL ServiceNow] Identifiant de l’utilisateur que le module doit désactiver.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Téléchargement d’une pièce jointe]

Ce module d’action télécharge une pièce jointe dans une [!DNL ServiceNow] enregistrement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID du système de pièce jointe]</td> 
   <td> Saisissez ou mappez l’unique [!DNL ServiceNow] Identifiant de la pièce jointe que vous souhaitez que le module télécharge.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Chargement d’une pièce jointe]

Ce module d’action télécharge une pièce jointe dans une [!DNL ServiceNow] enregistrement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom de la table]</td> 
   <td>Saisissez ou mappez le nom de la table dans laquelle vous souhaitez charger la pièce jointe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID système]</td> 
   <td>Saisissez ou mappez l’unique [!DNL ServiceNow] Identifiant du système sur lequel vous souhaitez charger la pièce jointe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du fichier]</td> 
   <td>Saisissez ou mappez un nom pour la pièce jointe</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du fichier]</td> 
   <td>Saisissez ou mappez le fichier vers lequel vous souhaitez effectuer le téléchargement. [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Création d’un enregistrement]

Ce module d’action crée une [!DNL ServiceNow] enregistrement.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si vous souhaitez créer un enregistrement dans une table personnalisée ou une table standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type de [!DNL ServiceNow] enregistrement que vous souhaitez que le module crée. Vous pouvez ensuite remplir les champs disponibles pour ce type d’enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action crée une [!DNL ServiceNow] enregistrement.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Saisissez ou mappez l’unique [!DNL ServiceNow] Identifiant de l’enregistrement que vous souhaitez que le module soit mis à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si l'enregistrement à mettre à jour se trouve dans une table personnalisée ou une table standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type de [!DNL ServiceNow] enregistrement que vous souhaitez que le module soit mis à jour. Vous pouvez ensuite remplir les champs disponibles pour ce type d’enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Suppression d’un enregistrement]

Ce module d’action supprime un incident ou un utilisateur.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Indiquez si vous souhaitez supprimer un incident ou un utilisateur.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID système]</td> 
   <td>Saisissez ou mappez l’unique [!DNL ServiceNow] Identifiant de l’enregistrement que vous souhaitez supprimer du module.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Recherche d’enregistrements]

Ce module recherche des enregistrements à l’aide des critères que vous sélectionnez.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si la table à rechercher est une table personnalisée ou standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td>Sélectionnez le type d’enregistrement à rechercher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Jeu de résultats]</td> 
   <td>Indiquez si vous souhaitez que le module renvoie tous les enregistrements qui correspondent aux critères, ou uniquement le premier enregistrement à correspondre. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de recherche]</td> 
   <td> <p>Sélectionnez le type de recherche que le module doit exécuter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Requête avancée]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Query]</p> <p>Saisissez la requête de recherche personnalisée. Pour plus d’informations sur [!DNL ServiceNow] requêtes de recherche personnalisées, voir <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">Documentation de la requête ServiceNow</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Critères de recherche]</p> <p>Indiquez les critères de recherche du module. Pour plus d’informations sur la configuration des filtres de recherche, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajout d’un filtre à un scénario dans Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Trier par]</p> <p>Indiquez le champ selon lequel le module doit trier les résultats et s’ils doivent être triés par ordre croissant ou décroissant.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Sélectionnez le type de valeurs à afficher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
 </tbody> 
</table>
