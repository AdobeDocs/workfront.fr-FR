---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Split.io
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Split.io] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1801'
ht-degree: 24%

---

# Modules [!DNL Split.io]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Split.io] et les connecter à plusieurs applications et services tiers.

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

Pour utiliser des modules [!DNL Split.io], vous devez disposer d’un compte [!DNL Split.io].

## Connecter [!DNL Split.io] à [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Vous pouvez créer une connexion à votre compte [!DNL Split.io] directement à partir de l’intérieur d’un module [!DNL Split.io].

1. Dans un module [!DNL Split.io], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Saisissez le nom de la connexion.
1. Entrez votre clé d’API [!DNL Split.io].

   Pour plus d’informations sur les [!DNL Split.io] clés d’API, voir [Clés d’API](https://help.split.io/hc/en-us/articles/360019916211-API-keys) dans la documentation [!DNL Split.io].

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Split.io] et leurs champs

Lorsque vous configurez des modules [!DNL split.io], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL split.io] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)

### Actions

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Obtenir la division]](#get-split)
* [[!UICONTROL Obtenir la définition de division dans l’environnement]](#get-split-definition-in-environment)
* [[!UICONTROL Créer une division]](#create-split)
* [[!UICONTROL Supprimer la division]](#delete-split)
* [[!UICONTROL Créer une définition de division dans l’environnement]](#create-split-definition-in-environment)
* [[!UICONTROL Supprimer la définition de division de l’environnement]](#remove-split-definition-from-environment)
* [[!UICONTROL Définition de division de mise à jour partielle dans l’environnement]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Associer des balises]](#associate-tags)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL split.io]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL split.io].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit utiliser au cours de chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir la division]

Ce module d’action récupère la division.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail qui contient la division que vous souhaitez récupérer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Saisissez ou mappez le nom de la division que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir la définition de division dans l’environnement]

Ce module d’action récupère une définition de division spécifique de l’environnement désigné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail qui contient la définition de division que vous souhaitez récupérer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom ou ID de l’environnement]</td> 
   <td>Sélectionnez ou mappez l’environnement qui contient la définition de division que vous souhaitez récupérer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Saisissez ou mappez le nom de la division pour laquelle vous souhaitez récupérer la définition de division.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une division]

Ce module d’action crée une nouvelle division dans votre organisation, à partir d’un type de trafic.

>[!NOTE]
>
>L’API ne configure pas la division dans aucun environnement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail dans lequel vous souhaitez créer la division.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou nom du type de trafic]</td> 
   <td>Sélectionnez ou mappez le type de trafic que vous souhaitez utiliser pour créer la division.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Saisissez ou mappez un nom pour le partage que vous souhaitez créer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Description]</td> 
   <td>Saisissez ou mappez une description [!UICONTROL split] pour le partage que vous souhaitez créer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer la division]

Ce module d’action supprime une division de votre organisation. Cela déconfigure automatiquement la définition de division de tous les environnements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail dans lequel vous souhaitez supprimer la division.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Saisissez ou mappez le nom du partage que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une définition de division dans l’environnement]

Ce module d’action configure une définition de partage pour un environnement spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail dans lequel vous souhaitez créer une définition de division.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom ou ID de l’environnement]</td> 
   <td>Sélectionnez ou mappez l’environnement dans lequel vous souhaitez créer une définition de partage.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Saisissez ou mappez le nom du partage pour lequel vous souhaitez créer une définition.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Saisissez ou mappez les commentaires à ajouter à la définition de partage.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>Pour chaque règle de ciblage à ajouter à la définition, cliquez sur <b>[!UICONTROL Ajouter un élément]</b>, puis saisissez ou mappez la règle.</p> <p>Pour plus d’informations sur les règles de ciblage, voir <a href="https://docs.split.io/reference#create-split-definition-in-environment">Création d’une définition de partage dans un environnement</a> dans la documentation [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Règle par défaut]</td> 
   <td> <p>Saisissez ou mappez la règle que vous souhaitez que le partage utilise pour le trafic qui ne répond pas aux spécifications des autres règles.</p> <p>Pour plus d’informations sur les règles de ciblage, voir <a href="https://docs.split.io/reference#create-split-definition-in-environment">Création d’une définition de partage dans un environnement</a> dans la documentation [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Traitement par défaut]</td> 
   <td> <p>Saisissez ou mappez le traitement que vous souhaitez que la division utilise si la division est terminée ou si le client n’est pas inclus dans l’affectation du trafic.</p> <p>Pour plus d'informations sur les traitements, voir <a href="https://docs.split.io/reference#create-split-definition-in-environment">Création d'une définition de partage dans un environnement</a> dans la documentation [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Traitements]</td> 
   <td> <p>Pour chaque traitement à ajouter à la définition, cliquez sur <b>[!UICONTROL Ajouter un élément]</b>, puis saisissez ou mappez le traitement.</p> <p>Pour plus d'informations sur les traitements, voir <a href="https://docs.split.io/reference#create-split-definition-in-environment">Création d'une définition de partage dans un environnement</a> dans la documentation [!DNL Split.io].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer la définition de division de l’environnement]

Ce module d’action déconfigure une définition de division pour un environnement spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail dans lequel vous souhaitez supprimer une définition de division.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom ou ID de l’environnement]</td> 
   <td>Sélectionnez ou mappez l’environnement dans lequel vous souhaitez supprimer une définition de partage.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Saisissez ou mappez le nom de la division pour laquelle vous souhaitez supprimer une définition.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Saisissez ou mappez les commentaires à ajouter à la définition de partage.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Définition de division de mise à jour partielle dans l’environnement]

Ce module d’action met à jour une définition de division pour un environnement spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail dans lequel vous souhaitez mettre à jour une définition de partage.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom ou ID de l’environnement]</td> 
   <td>Sélectionnez ou mappez l’environnement dans lequel vous souhaitez mettre à jour une définition de partage.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Saisissez ou mappez le nom du partage pour lequel vous souhaitez mettre à jour une définition.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mettre à jour le contenu]</td> 
   <td> <p>Pour chaque attribut de la division que vous souhaitez mettre à jour, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez ou mappez les modifications souhaitées.</p> <p>Pour plus d’informations, voir <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Définition de fractionnement de mise à jour partielle dans l’environnement</a> dans la documentation [!DNL Split.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Saisissez ou mappez les commentaires à ajouter à la définition de partage.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Associer des balises]

Ce module d’action ajoute des balises à l’objet spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail dans lequel vous souhaitez ajouter une balise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Name]</td> 
   <td>Saisissez ou mappez le nom de l’objet auquel vous souhaitez ajouter des balises,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’objet]</td> 
   <td> <p>Saisissez ou mappez le type d’objet auquel vous souhaitez ajouter des balises.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>Pour chaque balise à ajouter, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez ou mappez la balise.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Obtenir des espaces de travail]](#get-workspaces)
* [[!UICONTROL Obtenir des environnements]](#get-environments)
* [[!UICONTROL Obtenir des fragments]](#get-splits)
* [[!UICONTROL Définition de la division de liste dans un environnement]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Obtenir les types de trafic]](#get-traffic-types)

#### [!UICONTROL Obtenir des espaces de travail]

Ce module de recherche récupère les espaces de travail d’une organisation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’espaces de travail que le module doit récupérer au cours de chaque cycle d’exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des environnements]

Ce module de recherche récupère une liste d’environnements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail contenant les environnements que vous souhaitez répertorier.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des fragments]

Ce module de recherche récupère une liste de divisions.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail contenant les divisions que vous souhaitez répertorier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal de divisions que le module doit récupérer au cours de chaque cycle d’exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Définition de la division de liste dans un environnement]

Ce module de recherche récupère une liste de définitions de division dans un environnement donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail qui contient les définitions de division que vous souhaitez répertorier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom ou ID de l’environnement]</td> 
   <td>Sélectionnez ou mappez l’environnement qui contient les définitions de division que vous souhaitez répertorier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal de définitions de division que le module doit récupérer au cours de chaque cycle d’exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir les types de trafic]

Ce module de recherche récupère une liste des types de trafic.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Split.io] à [!DNL Workfront Fusion], voir <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Split.io] à [!UICONTROL Workfront Fusion] </a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’espace de travail qui contient les types de trafic que vous souhaitez répertorier.</td> 
  </tr> 
 </tbody> 
</table>
