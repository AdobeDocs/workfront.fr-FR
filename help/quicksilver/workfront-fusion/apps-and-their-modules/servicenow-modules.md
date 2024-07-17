---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules ServiceNow
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL ServiceNow] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 37%

---

# Modules [!DNL ServiceNow]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL ServiceNow] et les connecter à plusieurs applications et services tiers.

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

Pour utiliser des modules [!DNL ServiceNow], vous devez disposer d’un compte [!DNL ServiceNow].

## Connecter [!DNL ServiceNow] à [!DNL Workfront Fusion]

Pour créer une connexion pour vos modules [!DNL ServiceNow] :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone [!UICONTROL Connexion] lorsque vous commencez à configurer le premier module [!DNL ServiceNow].
1. Saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>Saisissez un nom pour la nouvelle connexion [!DNL ServiceNow].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>Saisissez votre nom d’utilisateur [!DNL ServiceNow].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>Saisissez votre mot de passe ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instance]</p> </td> 
      <td> <p>Entrez l’adresse de votre compte [!DNL ServiceNow] sans <code>https://</code> (généralement <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Modules [!UICONTROL ServiceNow] et leurs champs

Lorsque vous configurez des modules [!DNL ServiceNow], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL ServiceNow] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Si un enregistrement personnalisé est sélectionné dans un champ &quot;[!UICONTROL Type d’enregistrement]&quot;, le chargement des champs personnalisés peut prendre un certain temps.
>
>S’il n’existe aucun enregistrement personnalisé, la liste déroulante est vide.

* [[!UICONTROL Surveiller les enregistrements]](#watch-records)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Désactiver un utilisateur]](#deactivate-a-user)
* [[!UICONTROL Télécharger une pièce jointe]](#download-an-attachment)
* [[!UICONTROL Télécharger une pièce jointe]](#upload-an-attachment)
* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)
* [[!UICONTROL Rechercher des enregistrements]](#search-for-records)

### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement active un scénario lorsqu’un enregistrement est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Indiquez si vous souhaitez regarder les nouveaux enregistrements ou les enregistrements mis à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL ServiceNow]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL ServiceNow].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relative]</td> 
   <td> <p>Saisissez l’adresse sur le serveur web avec lequel le module doit interagir.</p> <p>Vous pouvez saisir une URL relative, ce qui signifie que vous n’avez pas à inclure le protocole (tel que <code>http://</code>) au début. Cela indique au serveur web que l’interaction se produit sur le serveur.</p> <p>Par exemple : <code>[!DNL /api/conversations].create</code></p> </td> 
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

### [!UICONTROL Lire un enregistrement]

Ce module d’action lit un enregistrement [!DNL ServiceNow] à l’aide de l’ID système.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Saisissez ou mappez l’identifiant unique [!DNL ServiceNow] de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si l'enregistrement que vous souhaitez lire se trouve dans une table personnalisée ou une table standard.</td> 
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

### [!UICONTROL Désactiver un utilisateur]

Ce module d’action désactive un utilisateur de [!DNL ServiceNow] à l’aide de l’ID système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> Saisissez ou mappez l’identifiant unique [!DNL ServiceNow] de l’utilisateur que le module doit désactiver.</td> 
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
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID du système de pièce jointe]</td> 
   <td> Saisissez ou mappez l’identifiant unique [!DNL ServiceNow] de la pièce jointe que vous souhaitez que le module télécharge.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Télécharger une pièce jointe]

Ce module d’action charge une pièce jointe dans un enregistrement [!DNL ServiceNow].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom de la table]</td> 
   <td>Saisissez ou mappez le nom de la table dans laquelle vous souhaitez charger la pièce jointe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID système]</td> 
   <td>Saisissez ou mappez l'identifiant unique [!DNL ServiceNow] du système dans lequel vous souhaitez charger la pièce jointe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Saisissez ou mappez un nom pour la pièce jointe</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du fichier]</td> 
   <td>Saisissez ou mappez le fichier que vous souhaitez charger vers [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un nouvel enregistrement [!DNL ServiceNow].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si vous souhaitez créer un enregistrement dans une table personnalisée ou une table standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL ServiceNow] que le module doit créer. Vous pouvez ensuite remplir les champs disponibles pour ce type d’enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action crée un nouvel enregistrement [!DNL ServiceNow].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Saisissez ou mappez l’identifiant unique [!DNL ServiceNow] de l’enregistrement que vous souhaitez que le module soit mis à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si l'enregistrement à mettre à jour se trouve dans une table personnalisée ou standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL ServiceNow] que le module doit mettre à jour. Vous pouvez ensuite remplir les champs disponibles pour ce type d’enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un incident ou un utilisateur.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Indiquez si vous souhaitez supprimer un incident ou un utilisateur.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID système]</td> 
   <td>Saisissez ou mappez l’identifiant unique [!DNL ServiceNow] de l’enregistrement que vous souhaitez que le module supprime.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Rechercher des enregistrements]

Ce module recherche des enregistrements à l’aide des critères que vous sélectionnez.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte ServiceNow à [!DNL Workfront Fusion], voir <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL ServiceNow] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de tableau]</td> 
   <td>Indiquez si la table que vous souhaitez rechercher est une table personnalisée ou standard.</td> 
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
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de recherche]</td> 
   <td> <p>Sélectionnez le type de recherche que le module doit exécuter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Requête avancée]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Requête de recherche]</p> <p>Saisissez la requête de recherche personnalisée. Pour plus d’informations sur les [!DNL ServiceNow] requêtes de recherche personnalisées, consultez la <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">documentation sur les requêtes ServiceNow</a>.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les champs que le module doit générer.</td> 
  </tr> 
 </tbody> 
</table>
