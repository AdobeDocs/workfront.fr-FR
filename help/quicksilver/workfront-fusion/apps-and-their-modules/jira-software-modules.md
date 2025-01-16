---
title: Modules de Jira Software
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2165'
ht-degree: 93%

---

# Modules [!DNL Jira Software]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules logiciels Jira](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Jira Software] et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Jira], vous devez disposer d’un compte [!DNL Jira].

## Informations sur l’API Jira

Le connecteur Jira utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"></td> 
   <td> Jira Cloud</td> 
   <td> Serveur Jira</td> 
  </tr> 
  <tr> 
   <td role="rowheader">apiVersion</td> 
   <td> 2</td> 
   <td> 2</td> 
  </tr> 
  <tr> 
   <td role="rowheader">apiVersionAgile</td> 
   <td> 1,0 </td> 
   <td> 1,0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>1,7,29</td> 
   <td>1,0,19</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]

La méthode de connexion dépend de si vous utilisez [!DNL Jira Cloud] ou [!DNL Jira Server].

* [Connecter  [!DNL Jira Cloud]  à Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connecter  [!DNL Jira Server]  à  [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connecter [!DNL Jira Cloud] à [!DNL Workfront Fusion]

Connecter [!DNL Jira Cloud] à [!DNL Workfront Fusion]

Pour connecter [!DNL Jira Software] à [!DNL Workfront Fusion], vous devez créer un jeton d’API et l’insérer avec votre URL de service et votre nom d’utilisateur ou d’utilisatrice dans le champ [!UICONTROL Créer une connexion] dans [!DNL Workfront Fusion].

#### Créer un jeton d’API dans [!DNL Jira]

1. Accédez à [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) et connectez-vous.
1. Cliquez sur **[!UICONTROL Créer un jeton d’API]**.
1. Saisissez un nom pour le jeton, par exemple *Workfront Fusion*.
1. Copiez le jeton à l’aide du bouton **[!UICONTROL Copier dans le presse-papiers]**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez plus visualiser le jeton après avoir fermé cette boîte de dialogue.
1. Conservez le jeton généré en lieu sûr.
1. Continuez avec [Configurer le jeton d’API  [!DNL Jira]  dans  [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configurer le jeton d’API [!DNL Jira] dans [!DNL Workfront Fusion]

1. Dans [!DNL Workfront Fusion], ajoutez un module [!DNL Jira] à un scénario pour ouvrir la boîte de dialogue **[!UICONTROL Créer une connexion]**.
1. Indiquez les informations suivantes :

   * **[!UICONTROL URL du service] :** il s’agit de l’URL de base que vous utilisez pour accéder à votre compte Jira. Exemple : `yourorganization.atlassian.net`
   * **[!UICONTROL Le nom d’utilisateur ou d’utilisatrice]**
   * **[!UICONTROL Le jeton d’API] :** il s’agit du jeton d’API que vous avez créé dans la section [Créer un jeton d’API dans [!DNL Jira]](#create-an-api-token-in-jira) de cet article.

1. Cliquez sur [!UICONTROL Continuer] pour créer la connexion et revenir au module.

### Connecter [!DNL Jira Server] à [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Pour autoriser une connexion entre [!DNL Workfront Fusion] et [!DNL Jira Server], vous avez besoin de votre clé de consommateur ou consommatrice, de votre clé privée et de l’URL du service. Vous devrez peut-être contacter votre administrateur ou administratrice [!DNL Jira] pour obtenir ces informations.

* [Générer des clés publiques et privées pour votre connexion  [!DNL Jira] ](#generate-public-and-private-keys-for-your-jira-connection)
* [Configurer l’application cliente en tant que consommatrice dans  [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Créer une connexion au serveur  [!DNL Jira]  ou au centre de données Jira dans  [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Générer des clés publiques et privées pour votre connexion [!DNL Jira]

Pour obtenir une clé privée pour votre connexion [!DNL Workfront Fusion Jira], vous devez générer des clés publiques et privées.

1. Dans votre terminal, exécutez les commandes `openssl` suivantes.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Cette commande génère une clé privée de 1 024 bits.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Cette commande crée un certificat X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Cette commande extrait la clé privée (format PKCS8) dans le fichier `jira_privatekey.pcks8`.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Cette commande permet d’extraire la clé publique du certificat dans le fichier `jira_publickey.pem`.

     >[!NOTE]
     >
     >Si vous utilisez Windows, vous devrez peut-être enregistrer manuellement la clé publique dans le fichier `jira_publickey.pem` :
     >
     >1. Dans votre terminal, exécutez la commande suivante :
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Copiez la sortie du terminal (y compris `-------BEGIN PUBLIC KEY--------` et `-------END PUBLIC KEY--------`).
     >   
     >1. Collez la sortie du terminal dans un fichier nommé `jira_publickey.pem`.


1. Continuez à [configurer l’application cliente en tant que consommatrice dans  [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira).

#### Configurez l’application cliente en tant que consommatrice dans [!DNL Jira].

1. Connectez-vous à votre instance [!DNL Jira].
1. Dans le panneau de navigation de gauche, cliquez sur Paramètres **[!UICONTROL [!DNL Jira]]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Applications]** > **[!UICONTROL Liens d’application]**.
1. Dans le champ **[!UICONTROL Entrer l’URL de l’application que vous voulez lier]**, entrez :

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Cliquez sur **[!UICONTROL Créer un lien]**. Ignorez le message d’erreur « Aucune réponse n’a été reçue de l’URL que vous avez saisie ».
1. Dans la fenêtre **[!UICONTROL Lier les applications]**, entrez des valeurs dans les champs **[!UICONTROL Clé de consommateur ou consommatrice]** et **[!UICONTROL Secret partagé]**.

   Vous pouvez choisir les valeurs de ces champs.

1. Copiez les valeurs des champs **[!UICONTROL Clé de consommateur ou consommatrice]** et **[!UICONTROL Secret partagé]** dans un endroit sûr.

   Vous aurez besoin de ces valeurs plus tard dans le processus de configuration.

1. Remplissez les champs de l’URL comme suit :

   | champ | Description |
   |---|---|
   | [!UICONTROL URL du jeton de demande] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL d’autorisation] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL du jeton d’accès] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Cochez la case **[!UICONTROL Créer un lien entrant]**.
1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre **[!UICONTROL Lier les applications]**, remplissez les champs suivants :

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> Collez la clé de consommateur que vous avez copiée dans un endroit sûr.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer name]</td> 
      <td>Saisissez le nom de votre choix. Ce nom est destiné à vous servir de référence.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public key]</td> 
      <td>Collez la clé publique de votre fichier <code>[!DNL jira_publickey.pem]</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Continuez vers [Créer une connexion à  [!DNL Jira Server]  ou  [!DNL Jira Data Center]  dans  [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion).

#### Créer une connexion à [!DNL Jira Server] ou [!DNL Jira Data Center] dans [!DNL Workfront Fusion]

>[!NOTE]
>
>Utilisez l’application [!DNL Jira Server] pour vous connecter à [!DNL Jira Server] ou [!DNL Jira Data Center].

1. Dans n’importe quel module [!DNL Jira Server] de [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Ajouter]** à côté du champ [!UICONTROL connexion].
1. Dans le panneau [!UICONTROL Créer une connexion], remplissez les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Saisir le nom de la connexion</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>Collez la clé de consommateur que vous avez copiée dans un endroit sûr dans <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configurer l’application client en tant que consommatrice dans [!DNL Jira]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Collez la clé privée du fichier <code>[!DNL jira_privatekey.pcks8]</code> que vous avez créé dans <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Générer des clés publiques et privées pour votre connexion [!DNL Jira]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Saisissez l’URL de votre instance [!DNL Jira]. Exemple : <code>yourorganization.atlassian.net</code></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Jira Software] et leurs champs

Lorsque vous configurez les modules [!DNL Jira Software], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Jira Software] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### [!UICONTROL Surveiller des enregistrements]

Ce module déclencheur lance un scénario lorsqu’un enregistrement est ajouté, mis à jour ou supprimé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez le webhook que vous souhaitez utiliser pour surveiller les enregistrements. </p> <p>Pour ajouter un nouveau webhook :</p> 
    <ol> 
     <li value="1">Cliquez sur <strong>[!UICONTROL Add]</strong>.</li> 
     <li value="2">Saisissez un nom pour le webhook.</li> 
     <li value="3"> <p>Sélectionnez la connexion que vous souhaitez utiliser pour votre webhook. </p> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], consultez l’article <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a>.</p> </li> 
     <li value="4"> <p>Sélectionnez le type d’enregistrement que vous souhaitez que le logiciel surveille :</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL Issue]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Ajouter un problème au sprint]](#add-issue-to-sprint)
* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)
* [[!UICONTROL Télécharger une pièce jointe]](#download-an-attachment)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)

#### [!UICONTROL Ajouter un problème au sprint]

Ce module d’action ajoute un ou plusieurs problèmes à un sprint.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], consultez l’article <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Saisissez ou mappez l’ID du sprint auquel vous souhaitez ajouter un problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue ID or Keys]</td> 
   <td>Ajoutez un ID ou une clé de problème pour chaque problème que vous souhaitez ajouter au sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un nouvel enregistrement dans Jira.

Le module renvoie tous les champs standard associés à l’enregistrement, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], voir <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez que le module crée. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel personnalisé et authentifié à l’API [!DNL Jira Software]. Cela vous permet de créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Jira Software].

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], consultez la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisir un chemin relatif à<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <img src="assets/quotes-in-json-350x120.png">  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un enregistrement particulier.

Vous indiquez l’ID de l’enregistrement.

Le module renvoie l’ID de l’enregistrement et tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], voir <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez que le module supprime. </p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>Saisissez ou mappez l’ID ou la clé de l’enregistrement que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger une pièce jointe]

Ce module d’action télécharge une pièce jointe particulière.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], voir <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’ID de la pièce jointe que vous souhaitez télécharger.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit les données d’un seul enregistrement dans [!DNL Jira Software].

Vous indiquez l’ID de l’enregistrement.

Le module renvoie tous les champs standard associés à l’enregistrement, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], voir <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Jira] que vous souhaitez que le module lise.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les sorties que vous souhaitez recevoir. Les options de sortie sont disponibles en fonction du type d’enregistrement sélectionné dans le champ [!UICONTROL Record Type].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant unique [!DNL Jira Software] de l’enregistrement que vous souhaitez que le module lise.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action met à jour un enregistrement existant, tel qu’une question ou un projet.

Vous indiquez l’ID de l’enregistrement.

Le module renvoie l’ID de l’enregistrement et tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], voir <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez que le module mette à jour. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Transition issue]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>Saisissez ou mettez en correspondance l’ID ou la clé de l’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Liste des enregistrements]](#list-records)
* [[!UICONTROL Rechercher des enregistrements]](#search-for-records)

#### [!UICONTROL Liste des enregistrements]

Ce module de recherche permet de retrouver tous les éléments d’un type spécifique qui correspondent à votre requête de recherche.

Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], voir <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez voir figurer dans le module. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint issue]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que vous souhaitez que le module récupère au cours de chaque cycle d’exécution du scénario.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des enregistrements]

Ce module de recherche recherche les enregistrements d’un objet dans [!DNL Jira Software] qui correspondent à la requête de recherche que vous avez spécifiée.

Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], voir <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez que le module recherche. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module.</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Lanuguage)] </p> <p>Pour plus d’informations sur JQL, consultez l’article <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> sur le site d’aide d’Atlassian. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Project by issue]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
