---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Salesforce
description: Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent Salesforce et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2740'
ht-degree: 31%

---

# Modules [!DNL Salesforce]

Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent [!DNL Salesforce] et les connecter à plusieurs applications et services tiers.

Pour une vidéo d’introduction au connecteur Salesforce, voir :

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Toutes les éditions de [!DNL Salesforce] n’ont pas accès à l’API. Pour plus d’informations, consultez les informations sur les éditions [!DNL Salesforce] avec accès à l’API sur le site de la communauté [!DNL Salesforce].
>* Pour plus d’informations sur les erreurs spécifiques renvoyées par l’API [!DNL Salesforce], consultez la documentation de l’API [!DNL Salesforce]. Vous pouvez également vérifier l’état de l’API [!DNL Salesforce] pour toute interruption de service possible.
>

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

Pour utiliser des modules [!DNL Salesforce], vous devez disposer d’un compte [!DNL Salesforce].

## À propos de la recherche d’objets [!DNL Salesforce]

Lors de la recherche d’objets, vous pouvez saisir des mots de recherche individuels ou créer une requête plus complexe à l’aide de caractères génériques et d’opérateurs :

* Utilisez le caractère générique astérisque (\*) comme substitut à zéro ou plusieurs caractères. Par exemple, une recherche de Ca\* trouve des éléments qui commencent par Ca
* Utiliser un caractère générique de point d’interrogation (?) comme substitut à un seul caractère. Par exemple, une recherche sur Jo?n recherche des éléments avec le terme John ou Joan mais pas Jon.
* Utilisez l’opérateur de guillemets (&quot;&quot;) pour trouver une correspondance exacte avec l’expression. Par exemple : &quot;réunion du lundi&quot;

Pour plus d’informations sur les possibilités de recherche, consultez la documentation destinée aux développeurs [!DNL Salesforce] sur SOQL et SOSL.

## Modules [!DNL Salesforce] et leurs champs

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

* [[!UICONTROL Surveiller les enregistrements]](#watch-for-records)
* [[!UICONTROL Regarder les messages sortants]](#watch-outbound-messages)
* [[!UICONTROL  Afficher un champ]](#watch-a-field)

#### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement exécute un scénario lorsqu’un enregistrement d’un objet est créé ou mis à jour. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Salesforce] que le module doit surveiller.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Champs D’Enregistrement]</td> 
   <td>Sélectionnez les champs que le module doit surveiller. Les champs disponibles dépendent du type d’enregistrement.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
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

1. Accédez à la page de configuration [!DNL Salesforce].

   Pour accéder à la page de configuration, recherchez et cliquez sur le bouton intitulé &quot;[!UICONTROL Setup]&quot; dans le coin supérieur droit du compte [!DNL Salesforce]. Sur la page de configuration de [!DNL Salesforce], recherchez la barre &quot;[!UICONTROL Recherche/recherche rapide]&quot; sur la gauche. Recherchez &quot;[!UICONTROL Règles de workflow]&quot;.

1. Cliquez sur **[!UICONTROL Règles de workflow]**.
1. Sur la page [!UICONTROL Règles de workflow] qui s’affiche, cliquez sur **[!UICONTROL Nouvelle règle]** et sélectionnez le type d’objet auquel la règle s’appliquera (par exemple &quot;[!UICONTROL Opportunity]&quot; si vous surveillez les mises à jour des enregistrements d’opportunité).
1. Cliquez sur **[!UICONTROL Suivant]**.
1. Définissez un nom de règle, des critères d’évaluation et des critères de règle, puis cliquez sur **[!UICONTROL Enregistrer]** et **[!UICONTROL Suivant]**.

1. Cliquez sur **[!UICONTROL Terminé]**.
1. Dans la règle Workflow nouvellement créée, cliquez sur **[!UICONTROL Modifier]**.
1. Dans la liste déroulante **[!UICONTROL Ajouter une action de workflow]** , sélectionnez **[!UICONTROL Nouveau message sortant]**.

1. Indiquez le nom, la description, l’URL du point d’entrée et les champs que vous souhaitez inclure dans le nouveau message sortant, puis cliquez sur **[!UICONTROL Enregistrer]**.

   Le champ **[!UICONTROL URL du point d’entrée]** contient l’URL fournie sur le [!DNL Salesforce]  [!DNL Workfront Fusion].

1. Configurez un scénario commençant par l’événement [!UICONTROL Message sortant].

1. Cliquez sur l’icône **&lt;/>** en bas à droite et copiez l’URL fournie.
1. Revenez à la page **[!UICONTROL Règles de workflow]**, recherchez la règle nouvellement créée, puis cliquez sur **[!UICONTROL Activer]**.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez le webhook que vous souhaitez utiliser pour surveiller les messages sortants. Pour ajouter un webhook, cliquez sur <strong>[!UICONTROL Ajouter]</strong> et saisissez le nom et la connexion du webhook.</p> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Salesforce] que le module doit surveiller pour les messages sortants.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Sélectionnez le type d’enregistrement qui contient le champ que le module doit surveiller. Vous devez choisir un type d’enregistrement pour lequel [!UICONTROL Field History] est activé dans la configuration de [!DNL Salesforce]. Pour plus d’informations, voir <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Field History Tracking</a> dans la documentation [!DNL Salesforce]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Sélectionnez les champs que le module doit surveiller pour les modifications.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de champs que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Télécharger la pièce jointe/le document]](#upload-attachmentdocument)
* [[!UICONTROL Télécharger la pièce jointe/le document]](#download-attachmentdocument)

#### [!UICONTROL Créer un enregistrement]

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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Salesforce] que le module doit créer. Les champs deviennent disponibles en fonction du type d’enregistrement sélectionné dans le champ [!UICONTROL Record Type] . Ces champs sont basés sur l’API [!DNL Salesforce].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>Sélectionnez le type d’enregistrement [!DNL Salesforce] que vous souhaitez que le module soit [action].read.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Champs D’Enregistrement]</td>
    <td>Sélectionnez les champs que le module doit lire. Vous devez sélectionner au moins un champ.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Saisissez ou mappez l’identifiant unique [!DNL Salesforce] de l’enregistrement que vous souhaitez que le module lise.</p> <p>Pour obtenir l’ID, ouvrez l’objet [!DNL Salesforce] dans votre navigateur et copiez le texte à la fin de l’URL après la dernière barre oblique (/). Par exemple : <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un enregistrement]

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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Salesforce] que le module doit supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant unique [!DNL Salesforce] de l’enregistrement que vous souhaitez que le module supprime.</p> <p>Pour obtenir l’ID, ouvrez l’objet [!DNL Salesforce] dans votre navigateur et copiez le texte à la fin de l’URL après la dernière barre oblique (/). Par exemple : <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Salesforce]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Salesforce].

Le module renvoie les éléments suivants :

* **[!UICONTROL Code d’état]** (nombre) : indique la réussite ou l’échec de votre requête HTTP. Ce sont des codes standard que vous pouvez consulter sur Internet.
* **[!UICONTROL En-têtes]** (objet) : contexte plus détaillé pour le code de réponse/d’état qui ne se rapporte pas au corps de sortie. Tous les en-têtes qui apparaissent dans un en-tête de réponse ne sont pas des en-têtes de réponse. Certains peuvent donc ne pas vous être utiles.

  Les en-têtes de réponse dépendent de la requête HTTP que vous avez choisie lors de la configuration du module.

* **[!UICONTROL Corps]** (objet) : selon la requête HTTP que vous avez choisie lors de la configuration du module, vous pouvez recevoir des données en retour. Ces données, telles que les données d’une requête [!UICONTROL GET], sont contenues dans cet objet.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à <code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Pour obtenir la liste des points de terminaison disponibles, reportez-vous au <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Guide du développeur de l’API REST Salesforce</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple, <code>{"Content-type":"application/json"}</code>. Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard. Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**Exemple :** L’appel API suivant renvoie la liste de tous les utilisateurs de votre compte [!DNL Salesforce] :
>
>* **URL** : `query`
>
>* **Méthode** : [!UICONTROL GET]
>
>* **Chaîne de requête** :
>
>* **Clé** : `q`
>
>* **Valeur** : `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Les correspondances de la recherche se trouvent dans la sortie du module sous **[!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL records]**.
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td>[!UICONTROL Source File]</td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Type de téléchargement]</td>
    <td> <p>Indiquez le type de fichier à télécharger à partir de Salesforce.</p> 
     <ul> 
      <li>[!UICONTROL Pièce jointe]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (il s’agit d’un document qui a été téléchargé vers une bibliothèque dans [!DNL Saleforce CRM Content] ou [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL ID de pièce jointe] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Saisissez ou mappez l’identifiant unique [!DNL Salesforce] de l’enregistrement que vous souhaitez que le module télécharge.</p> <p>Pour obtenir l’ID, ouvrez l’objet [!DNL Salesforce] dans votre navigateur et copiez le texte à la fin de l’URL après la dernière barre oblique (/). Par exemple : <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Salesforce] que le module doit mettre à jour. Les champs deviennent disponibles en fonction du type d’enregistrement sélectionné dans le champ Type d’enregistrement . Ces champs sont basés sur l’API [!DNL Salesforce].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Sélectionnez les champs que le module doit configurer lors de la création du nouvel enregistrement. Les champs obligatoires se trouvent en haut de la liste. </p> <p>Les champs que vous sélectionnez s’ouvrent sous ce champ. Vous pouvez désormais saisir des valeurs dans ces champs.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Recherche avec requête]

Ce module de recherche recherche recherche des enregistrements dans un objet de [!DNL Salesforce] correspondant à la requête de recherche que vous spécifiez. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Si vous avez sélectionné le type de recherche Simple , choisissez le type d’enregistrement [!DNL Salesforce] que le module doit rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>Saisissez la requête à rechercher.</p> <p>Pour plus d’informations sur SOSL, voir <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce Object Search Language (SOSL)</a> dans la documentation [!DNL Salesforce].</p> <p>Pour plus d’informations sur SOQL, voir <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language (SOQL)</a> dans la documentation [!DNL Salesforce].</p> <p>Remarque : Notez que la valeur du paramètre <code>RETURNING </code> influence la sortie du module. Si vous utilisez <code>LIMIT</code>, [!DNL Fusion] ignorera les paramètres du champ [!UICONTROL Nombre maximum d'enregistrements]. Si vous ne définissez aucune limite, Fusion insère la valeur [!UICONTROL LIMIT = Nombre maximum d’enregistrements].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
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
   <td>Pour plus d’informations sur la connexion de votre compte [!DNL Salesforce] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à[!DNL  Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Sélectionnez le type d’objet à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>Sélectionnez le champ par lequel vous souhaitez effectuer une recherche, l’opérateur que vous souhaitez utiliser dans votre requête et la valeur que vous recherchez dans le champ. Vous pouvez connecter des requêtes à l’aide de AND ou OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
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
