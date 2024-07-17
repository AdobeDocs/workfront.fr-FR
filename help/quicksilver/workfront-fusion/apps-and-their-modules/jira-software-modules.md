---
title: Modules du logiciel Jira
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les processus qui utilisent le  [!DNL Jira] logiciel, et le connecter à plusieurs applications et services tiers.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 36%

---

# Modules [!DNL Jira Software]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Jira Software] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Jira], vous devez disposer d&#39;un compte [!DNL Jira].

## Connecter [!DNL Jira Software] à [!DNL Workfront Fusion]

Votre méthode de connexion est basée sur l’utilisation de [!DNL Jira Cloud] ou [!DNL Jira Server].

* [Connexion de  [!DNL Jira Cloud]  à Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Se connecter [!DNL Jira Server] à [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connecter [!DNL Jira Cloud] à [!DNL Workfront Fusion]

Connecter [!DNL Jira Cloud] à [!DNL Workfront Fusion]

Pour vous connecter [!DNL Jira Software] à [!DNL Workfront Fusion], vous devez créer un jeton API et l&#39;insérer avec votre URL de service et votre nom d&#39;utilisateur dans le champ [!UICONTROL Créer une connexion] dans [!DNL Workfront Fusion].

#### Création d’un jeton API dans [!DNL Jira]

1. Accédez à [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) et connectez-vous.
1. Cliquez sur **[!UICONTROL Créer un jeton API]**.
1. Saisissez le nom du jeton, par exemple *Workfront Fusion*.
1. Copiez le jeton à l’aide du bouton **[!UICONTROL Copier dans le presse-papiers]** .

   >[!IMPORTANT]
   >
   >Vous ne pouvez plus afficher le jeton après avoir fermé cette boîte de dialogue.
1. Stockez le jeton généré en lieu sûr.
1. Passez à [Configuration du jeton d’API [!DNL Jira]  dans [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configuration du jeton d’API [!DNL Jira] dans [!DNL Workfront Fusion]

1. Dans [!DNL Workfront Fusion], ajoutez un module [!DNL Jira] à un scénario pour ouvrir la boîte **[!UICONTROL Créer une connexion]**.
1. Indiquez les informations suivantes :

   * **[!UICONTROL URL du service]**
   * **[!UICONTROL Nom d’utilisateur]**
   * **[!UICONTROL Jeton API] :** Il s’agit du jeton API que vous avez créé dans la section [Créer un jeton API dans [!DNL Jira]](#create-an-api-token-in-jira) de cet article.

1. Cliquez sur [!UICONTROL Continuer] pour créer la connexion et revenir au module.

### Connecter [!DNL Jira Server] à [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Pour autoriser une connexion entre [!DNL Workfront Fusion] et [!DNL Jira Server], vous avez besoin de votre clé de consommateur, de votre clé privée et de votre URL de service. Vous devrez peut-être contacter votre administrateur [!DNL Jira] pour obtenir ces informations.

* [Générer des clés publiques et privées pour votre connexion  [!DNL Jira] ](#generate-public-and-private-keys-for-your-jira-connection)
* [Configuration de l’application cliente en tant que consommateur dans [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Créez une connexion à [!DNL Jira] Serveur ou Jira Data Center dans [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Générer des clés publiques et privées pour votre connexion [!DNL Jira]

Pour acquérir une clé privée pour votre connexion [!DNL Workfront Fusion Jira], vous devez générer des clés publique et privée.

1. Dans votre terminal, exécutez les commandes `openssl` suivantes.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Cette commande génère une clé privée 1024 bits.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Cette commande crée un certificat X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Cette commande extrait la clé privée (format PKCS8) vers le `jira_privatekey.pcks8`
fichier .

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Cette commande extrait la clé publique du certificat vers le fichier `jira_publickey.pem`.

     >[!NOTE]
     >
     >Si vous utilisez Windows, vous devrez peut-être enregistrer manuellement la clé publique dans le fichier `jira_publickey.pem` :
     >
     >1. Dans votre terminal, exécutez la commande suivante :
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Copiez la sortie du terminal (y compris `-------BEGIN PUBLIC KEY--------` et `-------END PUBLIC KEY--------`
     >   
     >1. Collez la sortie du terminal dans un fichier nommé `jira_publickey.pem`.


1. Passez à [Configuration de l’application cliente en tant que consommateur dans [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configuration de l’application cliente en tant que consommateur dans [!DNL Jira]

1. Connectez-vous à votre instance [!DNL Jira].
1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL [!DNL Jira]Paramètres]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Applications]**> ****.
1. Dans le champ **[!UICONTROL Entrez l&#39;URL de l&#39;application que vous souhaitez lier]** , saisissez

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Cliquez sur **[!UICONTROL Créer un lien]**. Ignorez le message d’erreur &quot;Aucune réponse n’a été reçue de l’URL que vous avez saisie&quot;.
1. Dans la fenêtre **[!UICONTROL Lier les applications]** , saisissez des valeurs dans les champs **[!UICONTROL Clé du client]** et **[!UICONTROL Secret partagé]** .

   Vous pouvez choisir les valeurs de ces champs.

1. Copiez les valeurs des champs **[!UICONTROL Consumer key]** et **[!UICONTROL Shared secret]** vers un emplacement sécurisé.

   Vous aurez besoin de ces valeurs plus tard dans le processus de configuration.

1. Renseignez les champs URL comme suit :

   | champ | Description |
   |---|---|
   | [!UICONTROL URL du jeton de demande] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL d’autorisation] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL du jeton d’accès] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Cochez la case **[!UICONTROL Créer un lien entrant]** .
1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre **[!UICONTROL Lier des applications]** , renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> Collez la clé du consommateur que vous avez copiée vers un emplacement sécurisé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom du consommateur]</td> 
      <td>Saisissez le nom de votre choix. Ce nom est à titre de référence.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clé publique]</td> 
      <td>Collez la clé publique à partir de votre fichier <code>[!DNL jira_publickey.pem]</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Passez à [Créer une connexion à [!DNL Jira Server] ou [!DNL Jira Data Center] dans [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Créez une connexion à [!DNL Jira Server] ou [!DNL Jira Data Center] dans [!DNL Workfront Fusion]

>[!NOTE]
>
>Utilisez l’application [!DNL Jira Server] pour vous connecter à [!DNL Jira Server] ou [!DNL Jira Data Center].
1. Dans n&#39;importe quel module [!DNL Jira Server] de [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL connexion] .
1. Dans le panneau [!UICONTROL Créer une connexion] , renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Saisissez un nom pour la connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>Collez la clé du client que vous avez copiée vers un emplacement sécurisé dans <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configurez l’application cliente en tant que consommateur dans [!DNL Jira]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Collez la clé privée à partir du fichier <code>[!DNL jira_privatekey.pcks8]</code> que vous avez créé dans <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Générer des clés publiques et privées pour votre [!DNL Jira] connexion</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Saisissez l’URL de votre instance [!DNL Jira]. </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Jira Software] et leurs champs

Lorsque vous configurez des modules [!DNL Jira Software], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Jira Software] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement lance un scénario lorsqu’un enregistrement est ajouté, mis à jour ou supprimé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez le webhook que vous souhaitez utiliser pour rechercher des enregistrements. </p> <p>Pour ajouter un nouveau webhook :</p> 
    <ol> 
     <li value="1">Cliquez sur <strong>[!UICONTROL Ajouter]</strong></li> 
     <li value="2">Saisissez le nom du webhook.</li> 
     <li value="3"> <p>Sélectionnez la connexion que vous souhaitez utiliser pour votre webhook. </p> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </li> 
     <li value="4"> <p>Sélectionnez le type d’enregistrement que le logiciel doit surveiller :</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL Problème]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Ajouter un problème au sprint]](#add-issue-to-sprint)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)
* [[!UICONTROL Télécharger une pièce jointe]](#download-an-attachment)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)

#### [!UICONTROL Ajouter un problème au sprint]

Ce module d’action ajoute un ou plusieurs problèmes à un sprint.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Saisissez ou mappez l’ID d’impression du sprint auquel vous souhaitez ajouter un problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou clés de problème]</td> 
   <td>Ajoutez un ID ou une clé de problème pour chaque problème que vous souhaitez ajouter au sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un nouvel enregistrement dans Jira.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que le module doit créer. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module .</p> 
    <ul> 
     <li>[!UICONTROL Pièce jointe]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Problème]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Jira Software]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Jira Software].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un enregistrement particulier.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que le module doit supprimer. </p> 
    <ul> 
     <li>[!UICONTROL Pièce jointe]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Problème]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou clé]</td> 
   <td>Saisissez ou mappez l’identifiant ou la clé de l’enregistrement que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger une pièce jointe]

Ce module d’action télécharge une pièce jointe particulière.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la pièce jointe à télécharger.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit les données d’un seul enregistrement dans [!DNL Jira Software].

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Jira] que le module doit lire.</p> 
    <ul> 
     <li>[!UICONTROL Pièce jointe]</li> 
     <li>[!UICONTROL Problème]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les sorties que vous souhaitez recevoir. Les options de sortie sont disponibles en fonction du type d’enregistrement sélectionné dans le champ "[!UICONTROL Record Type]".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant unique [!DNL Jira Software] de l’enregistrement que vous souhaitez que le module lise.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un enregistrement existant, tel qu’un problème ou un projet.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que le module doit mettre à jour. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module .</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Problème]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Problème de transition]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID ou clé]</td> 
   <td>Saisissez ou mappez l’identifiant ou la clé de l’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Répertorier les enregistrements]](#list-records)
* [[!UICONTROL Rechercher des enregistrements]](#search-for-records)

#### [!UICONTROL Répertorier les enregistrements]

Ce module de recherche récupère tous les éléments d’un type spécifique correspondant à votre requête de recherche.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que le module doit répertorier. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module .</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Problème]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Problème Sprint]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Résultats max.]</p> </td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit récupérer au cours de chaque cycle d'exécution de scénario.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des enregistrements]

Ce module de recherche recherche des enregistrements d’un objet dans [!DNL Jira Software] qui correspondent à la requête de recherche que vous avez spécifiée.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Jira Software] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL Jira Software] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que le module doit rechercher. Lorsque vous sélectionnez un type d’enregistrement, d’autres champs spécifiques à ce type d’enregistrement apparaissent dans le module .</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Language)] </p> <p>Pour plus d’informations sur JQL, voir <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> sur le site d’aide d’Atlassian. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Projet par numéro]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
