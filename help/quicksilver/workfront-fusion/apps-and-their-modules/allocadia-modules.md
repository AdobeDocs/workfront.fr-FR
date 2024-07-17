---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Allocadia
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent l’attribut Allocadia et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 53%

---

# Modules [!DNL Allocadia]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Allocadia] et les connecter à plusieurs applications et services tiers.

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

Pour utiliser les modules [!DNL Allocadia], vous devez disposer d&#39;un compte [!DNL Allocadia].

## Connecter [!DNL Allocadia] à [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL Allocadia] directement depuis un module [!DNL Allocadia].

1. Dans un module [!DNL Allocadia], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Indiquez si vous souhaitez utiliser le serveur Amérique du Nord ou Europe.
1. Saisissez votre nom d’utilisateur et votre mot de passe.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Allocadia] et leurs champs

Lorsque vous configurez des modules [!DNL Allocadia], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Allocadia] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### [!UICONTROL Enregistrement de contrôle]

Ce module de déclenchement exécute un scénario lorsque des objets d’un type spécifique sont ajoutés, mis à jour ou les deux. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rohead"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Allocadia à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connecter l’affectation] à Workfront Fusion</a> dans cet article.</p> </td> 
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

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Allocadia]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Allocadia].

L’action est basée sur le type d’entité (type d’objet Allocadia) que vous spécifiez.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Allocadia] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://api-na.allocadia.com/{version}</code> ou <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Allocadia] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Allocadia] que le module doit lire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module. Les champs disponibles dépendent du [!UICONTROL Type d’entité] que vous avez sélectionné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant unique [!DNL Allocadia] de l’enregistrement que vous souhaitez que le module lise.</td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Allocadia] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Allocadia] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td> <p>Sélectionnez le type d’entité à supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Élément de ligne]</strong> </p> <p>Saisissez l’identifiant de l’élément de ligne.</p> </li> 
     <li> <p><strong>[!UICONTROL Choix De Colonne]</strong> </p> <p>Sélectionnez le budget à partir duquel vous souhaitez supprimer un enregistrement, puis saisissez l' ID de colonne et l' ID de choix.</p> </li> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!UICONTROL Allocadia] à [!DNL Workfront Fusion], voir <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Allocadia] que le module doit mettre à jour. D’autres champs s’affichent en fonction du type d’entité sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Sélectionnez le budget dans lequel vous souhaitez mettre à jour un enregistrement. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Enregistrement de recherche]

Ce module de recherche recherche des enregistrements d’un objet dans [!DNL Allocadia] qui correspondent à la requête de recherche que vous avez spécifiée.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous indiquez le type d’enregistrement souhaité.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rohead"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Allocadia] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Allocadia] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Allocadia] que le module doit rechercher. </td> 
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
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>Sélectionnez le champ à rechercher, sélectionnez l’opération, puis saisissez ou mappez la valeur à rechercher. Vous pouvez ajouter des règles [!DNL AND] ou [!DNL OR] pour filtrer davantage votre recherche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module. Les champs disponibles dépendent du type d’entité que vous avez sélectionné.</p> </td> 
  </tr> 
 </tbody> 
</table>
