---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules AWS S3
description: Le [!DNL Adobe Workfront Fusion AWS] Les modules S3 vous permettent d’effectuer des opérations sur vos compartiments S3.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# Modules AWS S3

Le [!DNL Adobe Workfront Fusion AWS] Les modules S3 vous permettent d’effectuer des opérations sur vos compartiments S3.

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

Pour utiliser [!UICONTROL AWS S3] modules, vous devez disposer d’un [!DNL Amazon Web Service] compte .

## Connexion [!DNL AWS] to [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Pour se connecter [!DNL AWS S3] to [!DNL Workfront Fusion] vous devez connecter votre [!DNL AWS] compte à [!DNL Workfront Fusion]. Pour ce faire, vous devez d’abord créer un utilisateur API dans [!DNL AWS] [!UICONTROL IAM].

1. Connectez-vous à [!DNL AWS] [!UICONTROL IAM] compte .
1. Accédez à **[!UICONTROL Gestion des identités et des accès]** > **[!UICONTROL Gestion des accès]** > **[!UICONTROL Utilisateurs]**.

1. Cliquez sur **[!UICONTROL Ajouter un utilisateur]**.
1. Saisissez le nom du nouvel utilisateur et sélectionnez l’option **[!UICONTROL Accès programmatique]** dans le [!UICONTROL Type d’accès] .
1. Cliquez sur **[!UICONTROL Association directe des stratégies existantes]**, puis recherchez **[!UICONTROL AmazonS3FullAccess]** dans la barre de recherche. Cliquez dessus lorsqu’il apparaît, puis cliquez sur **[!UICONTROL Suivant]**.

1. Passez aux autres écrans de la boîte de dialogue, puis cliquez sur **[!UICONTROL Créer un utilisateur]**.
1. Copiez le **[!UICONTROL Accès à l’ID de clé]** et **[!UICONTROL Clé d’accès secrète]**.

1. Accédez à [!DNL Workfront Fusion] et ouvrez le [!DNL AWS S3] du module **[!UICONTROL Création d’une connexion]** boîte de dialogue.
1. Saisissez le [!UICONTROL Accès à l’ID de clé] et [!UICONTROL Clé d’accès secrète] de l’étape 7 aux champs respectifs, puis cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

## [!DNL AWS S3] modules et leurs champs

Lorsque vous configurez [!DNL AWS S3] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL AWS S3] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)

### Actions

* [[!UICONTROL Créer un compartiment]](#create-bucket)
* [[!UICONTROL Obtenir le fichier]](#get-file)
* [[!UICONTROL Télécharger fichier]](#upload-file)
* [[!UICONTROL Lancer un appel API]](#make-an-api-call)

#### [!UICONTROL Créer un compartiment]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL AWS] compte à [!DNL Workfront Fusion], voir <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez le nom du nouveau compartiment.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans la documentation AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir le fichier]

Télécharge un fichier depuis un compartiment.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL AWS] compte à [!DNL Workfront Fusion], voir <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans le [!DNL AWS] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartiment] </td> 
   <td> <p>Sélectionnez le compartiment à partir duquel vous souhaitez télécharger le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Saisissez le chemin d’accès au fichier. Exemple: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger fichier]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL AWS] compte à [!DNL Workfront Fusion], voir <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans le [!DNL AWS] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (facultatif) </p> </td> 
   <td> <p>Indiquez le dossier cible vers lequel vous souhaitez charger un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fichier source]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL En-têtes] (facultatif)</p> </td> 
   <td> <p> Insérez des en-têtes de requête. Les en-têtes disponibles se trouvent dans la <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] documentation - objet [!UICONTROL PUT]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lancer un appel API]

Pour une discussion détaillée de la variable [!DNL Amazon S3] API, voir [[!DNL Amazon S3] [!UICONTROL REST] Présentation des API](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL AWS] compte à [!DNL Workfront Fusion], voir <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans le [!DNL AWS] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Saisissez une URL hôte. Le chemin doit être relatif à<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Méthode [!UICONTROL]</td> 
   <td> <p>Sélectionnez la méthode de requête [!UICONTROL HTTP] dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête [!UICONTROL HTTP] dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez un en-tête de requête. Vous pouvez utiliser les en-têtes de requête courants suivants. Pour plus d’en-têtes de requête, reportez-vous à la section <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] Documentation API</a>.</p> <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Nom de l’en-tête</th> 
       <th> <p> Description</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>Longueur du message (sans en-têtes) conformément à la norme RFC 2616. Cet en-tête est requis pour les opérations et les opérations [!UICONTROL PUT] qui chargent du code XML, telles que la journalisation et les listes de contrôle d’accès.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>Type de contenu de la ressource, au cas où le contenu de la requête se trouverait dans le corps. Exemple: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Résumé MD5 128 bits encodé en base64 du message (sans en-têtes), selon la RFC 1864. Cet en-tête peut être utilisé comme contrôle d’intégrité du message pour vérifier que les données sont les mêmes données que celles envoyées initialement. Bien qu’il soit facultatif, nous vous recommandons d’utiliser le mécanisme [!UICONTROL Content-MD5] comme contrôle d’intégrité de bout en bout. Pour plus d’informations sur l’authentification des requêtes [!UICONTROL REST], voir <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">Authentification [!UICONTROL REST]</a> dans le <i>[!DNL Amazon] Guide du développeur du service de stockage simple</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>Date et heure actuelles en fonction du demandeur. Exemple: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Lorsque vous spécifiez la variable <code>Authorization </code>en-tête , vous devez spécifier l’une des options suivantes : <code>x-amz-date</code> ou le <code>Date </code>en-tête .</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Attendez]</p> </td> 
       <td> <p>Lorsque votre application utilise [!UICONTROL 100-continue], elle n’envoie pas le corps de la requête tant qu’elle n’a pas reçu d’accusé de réception. Si le message est rejeté en fonction des en-têtes, le corps du message n’est pas envoyé. Cet en-tête ne peut être utilisé que si vous envoyez un corps.</p> <p>Valeurs valides : [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Pour les requêtes de style chemin, la valeur est <code>s3.amazonaws.com</code>. Pour les requêtes de style virtuel, la valeur est <code>BucketName.s3.amazonaws.com</code>. Pour plus d’informations, voir <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Hébergement virtuel</a> dans le <i>[!DNL Amazon] Guide du développeur du service de stockage simple</i>.</p> <p>Cet en-tête est requis pour HTTP 1.1 (la plupart des kits d’outils ajoutent cet en-tête automatiquement) ; facultatif pour les requêtes HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Lorsque vous utilisez la version 4 de signature pour authentifier la requête, cet en-tête fournit un hachage de la payload de la requête. Lors du téléchargement d’un objet en blocs, définissez la valeur sur <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> pour indiquer que la signature couvre uniquement les en-têtes et qu’il n’y a aucune charge utile. Pour plus d’informations, voir <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Calculs de signatures pour l’en-tête d’autorisation : Transfert de la charge utile en plusieurs blocs (transfert fragmenté) ([!DNL AWS] Signature version 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>Date et heure actuelles en fonction du demandeur. Exemple: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Lorsque vous spécifiez la variable <code>Authorization </code>en-tête , vous devez spécifier l’une des options suivantes : <code>x-amz-date</code> ou le <code>Date </code>en-tête . Si vous spécifiez les deux, la valeur spécifiée pour la variable <code>x-amz-date</code> L’en-tête est prioritaire.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Cet en-tête peut être utilisé dans les scénarios suivants :</p> 
        <ul> 
         <li>Fournir des jetons de sécurité pour [!DNL Amazon DevPay] opérations. Chaque requête qui utilise [!DNL Amazon DevPay] require2 <code>x-amz-security-token</code> headers : un pour le jeton de produit et un pour le jeton utilisateur. When [!DNL Amazon S3] reçoit une requête authentifiée, elle compare la signature calculée à la signature fournie. Les en-têtes à plusieurs valeurs mal formatés utilisés pour calculer une signature peuvent entraîner des problèmes d’authentification.</li> 
         <li>Fournissez un jeton de sécurité lors de l’utilisation d’informations d’identification de sécurité temporaires. Lors de l’exécution de requêtes à l’aide d’informations d’identification de sécurité temporaires obtenues auprès d’IAM, vous devez fournir un jeton de sécurité à l’aide de cet en-tête. Pour en savoir plus sur les informations d’identification de sécurité temporaires, voir Lancement de requêtes .</li> 
        </ul> <p>Cet en-tête est requis pour les requêtes qui utilisent [!DNL Amazon DevPay] et les demandes signées à l’aide d’informations d’identification de sécurité temporaires.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez les chaînes de requête souhaitées, telles que des paramètres ou des champs de formulaire.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:   <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Fichiers de liste]](#list-files)
* [[!UICONTROL Dossiers de liste]](#list-folders)

#### [!UICONTROL Fichiers de liste]

Renvoie une liste de fichiers à partir d’un emplacement spécifié.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL AWS] compte à [!DNL Workfront Fusion], voir <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans le [!DNL AWS] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartiment] </td> 
   <td> <p>Sélectionnez la [!DNL Amazon S3] pour rechercher des fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (facultatif)</p> </td> 
   <td> <p> Chemin d’accès à un dossier dans lequel rechercher des fichiers, par exemple <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dossiers de liste]

Renvoie une liste de dossiers à partir d’un emplacement spécifié.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL AWS] compte à [!DNL Workfront Fusion], voir <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans la documentation AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartiment] </td> 
   <td> <p>Sélectionnez la [!DNL Amazon S3] pour rechercher des dossiers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (facultatif)</p> </td> 
   <td> <p> Chemin d’accès à un dossier dans lequel rechercher des dossiers, par exemple <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
