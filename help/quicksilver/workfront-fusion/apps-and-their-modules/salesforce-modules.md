---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Salesforce
description: Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent Salesforce et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2740'
ht-degree: 0%

---

# [!DNL Salesforce] modules

Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent [!DNL Salesforce], mais aussi de le connecter à plusieurs applications et services tiers.

Pour une vidéo d’introduction au connecteur Salesforce, voir :

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créez un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Toutes les éditions de [!DNL Salesforce] disposer d’un accès API. Pour plus d’informations, voir les informations sur [!DNL Salesforce] éditions avec accès API sur la page [!DNL Salesforce] Site communautaire.
>* Pour plus d’informations sur les erreurs spécifiques renvoyées par la variable [!DNL Salesforce] API, voir [!DNL Salesforce] Documentation API. Vous pouvez également vérifier l’état de la variable [!DNL Salesforce] API pour toutes les pannes de service possibles.
>

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

## Conditions préalables

Pour utiliser [!DNL Salesforce] modules, vous devez disposer d’un [!DNL Salesforce] compte .

## A propos de la recherche [!DNL Salesforce] objet

Lors de la recherche d’objets, vous pouvez saisir des mots de recherche individuels ou créer une requête plus complexe à l’aide de caractères génériques et d’opérateurs :

* Utilisez le caractère générique astérisque (\*) comme substitut à zéro ou plusieurs caractères. Par exemple, une recherche de Ca\* trouve des éléments qui commencent par Ca
* Utiliser un caractère générique de point d’interrogation (?) comme substitut à un seul caractère. Par exemple, une recherche sur Jo?n recherche des éléments avec le terme John ou Joan mais pas Jon.
* Utilisez l’opérateur de guillemets (&quot;&quot;) pour trouver une correspondance exacte avec l’expression. Par exemple : &quot;réunion du lundi&quot;

Pour plus d’informations sur les possibilités de recherche, voir [!DNL Salesforce] documentation destinée aux développeurs sur SOQL et SOSL.

## [!DNL Salesforce] modules et leurs champs

* [Triggers](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Triggers

* [[!UICONTROL Surveillance des enregistrements]](#watch-for-records)
* [[!UICONTROL Regarder les messages sortants]](#watch-outbound-messages)
* [[!UICONTROL Afficher un champ]](#watch-a-field)

#### [!UICONTROL Surveillance des enregistrements]

Ce module de déclenchement exécute un scénario lorsqu’un enregistrement d’un objet est créé ou mis à jour. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Sélectionnez le type de [!DNL Salesforce] enregistrement que vous souhaitez que le module regarde.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Champs D’Enregistrement]</td> 
   <td>Sélectionnez les champs que le module doit surveiller. Les champs disponibles dépendent du type d’enregistrement.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Déterminez si vous souhaitez que le scénario n’affiche que les nouveaux enregistrements du type que vous avez sélectionné ou les nouveaux enregistrements du type que vous avez sélectionné, ainsi que toutes les autres modifications apportées aux enregistrements de ce type.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder les messages sortants]

Ce module de déclenchement exécute un scénario lorsqu’une personne envoie un message. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Ce module nécessite une configuration supplémentaire :

1. Accédez au [!DNL Salesforce] page de configuration.

   Pour accéder à la page de configuration, recherchez et cliquez sur le bouton intitulé &quot;[!UICONTROL Configuration]&quot; dans le coin supérieur droit du [!DNL Salesforce] compte . Dans la [!DNL Salesforce] page de configuration, recherchez le[!UICONTROL Recherche/recherche rapide]&quot; à gauche. Recherchez &quot;[!UICONTROL Règles de workflow].&quot;

1. Cliquez sur **[!UICONTROL Règles de workflow]**.
1. Sur la page [!UICONTROL Règles de workflow] qui s’affiche, cliquez sur **[!UICONTROL Nouvelle règle]** et sélectionnez le type d’objet auquel la règle s’appliquera (par exemple, &quot;[!UICONTROL Opportunité]&quot; si vous surveillez les mises à jour des enregistrements d’opportunité).
1. Cliquez sur **[!UICONTROL Suivant]**.
1. Définissez un nom de règle, des critères d’évaluation et des critères de règle, puis cliquez sur **[!UICONTROL Enregistrer]** et **[!UICONTROL Suivant]**.

1. Cliquez sur **[!UICONTROL Terminé]**.
1. Dans la règle de workflow nouvellement créée, cliquez sur **[!UICONTROL Modifier]**.
1. Dans la **[!UICONTROL Ajouter une action de workflow]** liste déroulante, sélectionnez **[!UICONTROL Nouveau message sortant]**.

1. Indiquez le nom, la description, l’URL du point de fin et les champs que vous souhaitez inclure dans le nouveau message sortant, puis cliquez sur **[!UICONTROL Enregistrer]**.

   La variable **[!UICONTROL URL du point d’entrée]** contient l’URL fournie dans la variable [!DNL Salesforce] [!UICONTROL Message sortant] in [!DNL Workfront Fusion].

1. Configurez un scénario commençant par [!UICONTROL Message sortant] .

1. Cliquez sur le bouton **&lt;/>** en bas à droite et copiez l’URL fournie.
1. Revenez au **[!UICONTROL Règles de workflow]** recherchez la règle nouvellement créée, puis cliquez sur **[!UICONTROL Activer]**.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez le webhook que vous souhaitez utiliser pour surveiller les messages sortants. Pour ajouter un webhook, cliquez sur <strong>[!UICONTROL Ajouter]</strong> et saisissez le nom et la connexion du webhook.</p> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Sélectionnez le type de [!DNL Salesforce] enregistrement que vous souhaitez que le module surveille les messages sortants.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>Sélectionnez les champs que le module doit surveiller pour les messages sortants. Les champs disponibles dépendent du type d’enregistrement.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Afficher un champ]*

Ce module de déclenchement lance un scénario lorsqu’un champ est mis à jour dans [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Sélectionnez le type d’enregistrement qui contient le champ que le module doit surveiller. Vous devez choisir un type d’enregistrement pour lequel [!UICONTROL Field History] est activé. [!DNL Salesforce] configuration. Pour plus d’informations, voir <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Suivi de l’historique des champs</a> dans le [!DNL Salesforce] la documentation. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Sélectionnez les champs que le module doit surveiller pour les modifications.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de champs que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Création d’un enregistrement]](#create-a-record)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Suppression d’un enregistrement]](#delete-a-record)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Télécharger la pièce jointe/le document]](#upload-attachmentdocument)
* [[!UICONTROL Télécharger la pièce jointe/le document]](#download-attachmentdocument)

#### [!UICONTROL Création d’un enregistrement]

Ce module d’action crée un nouvel enregistrement dans un objet .

Le module vous permet de sélectionner les champs de l’objet disponibles dans le module . Cela réduit le nombre de champs que vous devez parcourir lors de la configuration du module.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Sélectionnez le type de [!DNL Salesforce] enregistrement que vous souhaitez que le module crée. Les champs deviennent disponibles en fonction du type d’enregistrement sélectionné dans le champ [!UICONTROL Record Type] . Ces champs reposent sur la variable [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sélectionner les champs à mapper]</td> 
   <td> <p>Sélectionnez les champs que le module doit configurer lors de la création du nouvel enregistrement. Les champs obligatoires se trouvent en haut de la liste. </p> <p>Les champs que vous sélectionnez s’ouvrent sous ce champ. Vous pouvez désormais saisir des valeurs dans ces champs.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit les données d’un seul objet dans [!DNL Salesforce].

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>Sélectionnez le type de [!DNL Salesforce] enregistrement que vous souhaitez que le module soit [action].read.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Champs D’Enregistrement]</td>
    <td>Sélectionnez les champs que le module doit lire. Vous devez sélectionner au moins un champ.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Saisissez ou mappez l’unique [!DNL Salesforce] Identifiant de l’enregistrement que vous souhaitez que le module lise.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Salesforce] dans votre navigateur et copiez le texte à la fin de l’URL après la dernière barre oblique (/). Par exemple : <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un enregistrement]

Ce module d’action supprime un enregistrement existant dans un objet.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Sélectionnez le type de [!DNL Salesforce] enregistrement que vous souhaitez supprimer du module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Saisissez ou mappez l’unique [!DNL Salesforce] Identifiant de l’enregistrement que vous souhaitez supprimer du module.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Salesforce] dans votre navigateur et copiez le texte à la fin de l’URL après la dernière barre oblique (/). Par exemple : <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Salesforce] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Salesforce] modules.

Le module renvoie les éléments suivants :

* **[!UICONTROL Code d’état]** (nombre) : indique la réussite ou l’échec de votre requête HTTP. Ce sont des codes standard que vous pouvez consulter sur Internet.
* **[!UICONTROL En-têtes]** (objet) : contexte plus détaillé pour le code de réponse/d’état qui ne se rapporte pas au corps de sortie. Tous les en-têtes qui apparaissent dans un en-tête de réponse ne sont pas des en-têtes de réponse. Certains peuvent donc ne pas vous être utiles.

  Les en-têtes de réponse dépendent de la requête HTTP que vous avez choisie lors de la configuration du module.

* **[!UICONTROL Corps]** (objet) : selon la requête HTTP que vous avez choisie lors de la configuration du module, vous pouvez recevoir des données en retour. Ces données, telles que les données d’une [!UICONTROL GET] est contenu dans cet objet.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Pour obtenir la liste des points de fin disponibles, reportez-vous à la section <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Guide du développeur de l’API REST Salesforce</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode [!UICONTROL]</p> </td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard. Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** L’appel API suivant renvoie la liste de tous les utilisateurs de votre [!DNL Salesforce] compte :
>
>* **URL**: `query`
>
>* **Méthode**: [!UICONTROL GET]
>
>* **Chaîne de requête**:
>
>* **Clé**: `q`
>
>* **Valeur**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Les correspondances de la recherche se trouvent dans la sortie du module sous **[!UICONTROL Bundle] > [!UICONTROL Corps] > [!UICONTROL records]**.
>
>Dans notre exemple, 6 utilisateurs ont été renvoyés :
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Télécharger la pièce jointe/le document]

Ce module d’action télécharge un fichier et l’associe à un enregistrement que vous spécifiez ou charge un document.

Le module renvoie l’identifiant de la pièce jointe ou du document et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type de téléchargement]</td> 
   <td>Indiquez si vous souhaitez que le module charge une pièce jointe ou un document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de l’objet auquel vous souhaitez charger une pièce jointe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Sélectionnez le dossier contenant le fichier que le module doit charger. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fichier source]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger la pièce jointe/le document]

Ce module d’action télécharge un document ou une pièce jointe à partir d’un enregistrement.

Vous indiquez l’identifiant de l’enregistrement et le type de téléchargement souhaité.

Le module renvoie l’identifiant de la pièce jointe ou du document et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Type de téléchargement]</td>
    <td> <p>Indiquez le type de fichier à télécharger à partir de Salesforce.</p> 
     <ul> 
      <li>[!UICONTROL Pièce jointe]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (il s’agit d’un document qui a été chargé dans une bibliothèque dans [!DNL Saleforce CRM Content] ou [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL ID de pièce jointe] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Saisissez ou mappez l’unique [!DNL Salesforce] Identifiant de l’enregistrement que vous souhaitez que le module télécharge.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Salesforce] dans votre navigateur et copiez le texte à la fin de l’URL après la dernière barre oblique (/). Par exemple : <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action modifie un enregistrement dans un objet .

Le module vous permet de sélectionner les champs de l’objet disponibles dans le module . Cela réduit le nombre de champs que vous devez parcourir lors de la configuration du module.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Sélectionnez le type de [!DNL Salesforce] enregistrement que vous souhaitez que le module soit mis à jour. Les champs deviennent disponibles en fonction du type d’enregistrement sélectionné dans le champ Type d’enregistrement . Ces champs reposent sur la variable [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sélectionner les champs à mapper]</td> 
   <td> <p>Sélectionnez les champs que le module doit configurer lors de la création du nouvel enregistrement. Les champs obligatoires se trouvent en haut de la liste. </p> <p>Les champs que vous sélectionnez s’ouvrent sous ce champ. Vous pouvez désormais saisir des valeurs dans ces champs.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Recherche avec requête]

Ce module de recherche recherche recherche des enregistrements dans un objet de la section [!DNL Salesforce] qui correspondent à la requête de recherche que vous spécifiez. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search Type]</td> 
   <td> <p>Sélectionnez le type de recherche que le module doit effectuer :</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL À L’Aide De SOSL (Langage De Recherche D’Objets Salesforce)]</p> </li> 
     <li> <p>[!UICONTROL À L’AIDE DE SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Si vous avez sélectionné le type de recherche Simple , choisissez le type de [!DNL Salesforce] enregistrement que vous souhaitez que le module recherche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>Saisissez la requête à rechercher.</p> <p>Pour plus d’informations sur SOSL, voir <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Langage de recherche d’objet Salesforce (SOSL)</a> dans le [!DNL Salesforce] la documentation.</p> <p>Pour plus d’informations sur SOQL, voir <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Langage de requête d’objet Salesforce (SOQL)</a> dans le [!DNL Salesforce] la documentation.</p> <p>Remarque : La valeur du paramètre <code>RETURNING </code>influence la sortie du module. Si vous utilisez <code>LIMIT</code>, [!DNL Fusion] ignore les paramètres du champ [!UICONTROL Nombre maximum d’enregistrements] . Si vous ne définissez aucune limite, Fusion insère la valeur [!UICONTROL LIMIT = Nombre maximum d’enregistrements].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher]

Ce module d&#39;action récupère tous les enregistrements répondant à un critère donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL Salesforce] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à[!DNL  Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Sélectionnez le type d’objet à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critères de recherche]</td> 
   <td>Sélectionnez le champ par lequel vous souhaitez effectuer une recherche, l’opérateur que vous souhaitez utiliser dans votre requête et la valeur que vous recherchez dans le champ. Vous pouvez connecter des requêtes à l’aide de AND ou OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Jeu de résultats]</td> 
   <td>Indiquez si vous souhaitez que le module renvoie tous les enregistrements correspondants ou uniquement le premier enregistrement correspondant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit récupérer au cours de chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>
