---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules d'allocadia
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Allocadia et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# [!DNL Allocadia] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Allocadia], ainsi que de la connecter à plusieurs applications et services tiers.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Allocadia] modules, vous devez disposer d’un [!DNL Allocadia] compte .

## Connexion [!DNL Allocadia] to [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre [!DNL Allocadia] compte directement depuis l’intérieur d’une [!DNL Allocadia] module .

1. Dans n’importe quel [!DNL Allocadia] module, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Indiquez si vous souhaitez utiliser le serveur Amérique du Nord ou Europe.
1. Saisissez votre nom d’utilisateur et votre mot de passe.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## [!DNL Allocadia] modules et leurs champs

Lorsque vous configurez [!DNL Allocadia] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Allocadia] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Triggers

#### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement exécute un scénario lorsque des objets d’un type spécifique sont ajoutés, mis à jour ou les deux. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rohead"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte Allocadia à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connecter l’allocation] à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtre</td> 
   <td> <p>Indiquez si vous souhaitez que le scénario affiche New Records uniquement, [!UICONTROL Updated Records uniquement] ou New and Updated Records.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type d’entité</td> 
   <td>Sélectionnez le type d’enregistrement Allocadia que le module doit regarder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module. Les champs disponibles dépendent du type d’entité que vous avez sélectionné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit surveiller pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [Appel API personnalisé](#custom-api-call)
* [Lecture d’enregistrement](#read-record)
* [Créer un enregistrement](#create-record)
* [Supprimer l’enregistrement](#delete-record)
* [Mettre à jour l’enregistrement](#update-record)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Allocadia] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Allocadia] modules.

L’action est basée sur le type d’entité (type d’objet Allocadia) que vous spécifiez.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Allocadia] compte à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://api-na.allocadia.com/{version}</code> ou <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
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

#### [!UICONTROL Lecture d’enregistrement]

Ce module d’action lit les données d’un seul enregistrement dans [!DNL Allocadia].

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rohead"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Allocadia] compte à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type de [!DNL Allocadia] enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module. Les champs disponibles dépendent du [!UICONTROL Type d’entité] que vous avez sélectionné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’unique [!DNL Allocadia] Identifiant de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rohead"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Allocadia] compte à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Indiquez si vous souhaitez créer un enregistrement en fonction du choix de l’élément ou de la colonne.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Sélectionnez le budget dans lequel vous souhaitez créer un enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Sélectionnez la colonne à utiliser pour créer un nouvel enregistrement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>Saisie ou mappage d’un libellé pour le nouvel enregistrement</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer l’enregistrement]

Ce module d’action supprime un enregistrement particulier.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rohead"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Allocadia] compte à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td> <p>Sélectionnez le type d’entité à supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Élément de ligne]</strong> </p> <p>Saisissez l’identifiant de l’élément de ligne.</p> </li> 
     <li> <p><strong>[!UICONTROL Choix de colonne]</strong> </p> <p>Sélectionnez le budget à partir duquel vous souhaitez supprimer un enregistrement, puis saisissez l' ID de colonne et l' ID de choix.</p> </li> 
     <li> <p><strong>[!UICONTROL Balises de prévision]</strong> </p> <p>Sélectionnez le budget duquel vous souhaitez supprimer un enregistrement, puis saisissez l'identifiant de balise.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour l’enregistrement]

Ce module d’action met à jour un enregistrement, tel qu’un élément de ligne, un utilisateur ou un choix de colonnes.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Allocadia] à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type de [!DNL Allocadia] enregistrement que vous souhaitez que le module soit mis à jour. D’autres champs s’affichent en fonction du type d’entité sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Sélectionnez le budget dans lequel vous souhaitez mettre à jour un enregistrement. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Enregistrement de recherche]

Ce module de recherche recherche recherche des enregistrements dans un objet de la section [!DNL Allocadia] qui correspondent à la requête de recherche que vous spécifiez.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous indiquez le type d’enregistrement souhaité.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rohead"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Allocadia] compte à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type de [!DNL Allocadia] enregistrement que vous souhaitez que le module recherche. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Sélectionnez le budget à rechercher. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Jeu de résultats]</td> 
   <td>Indiquez si vous souhaitez que le module renvoie tous les enregistrements correspondants ou uniquement le premier enregistrement correspondant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critères de recherche]</td> 
   <td>Sélectionnez le champ à rechercher, sélectionnez l’opération, puis saisissez ou mappez la valeur à rechercher. Vous pouvez ajouter [!DNL AND] ou [!DNL OR] règles pour filtrer davantage votre recherche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module. Les champs disponibles dépendent du type d’entité que vous avez sélectionné.</p> </td> 
  </tr> 
 </tbody> 
</table>
