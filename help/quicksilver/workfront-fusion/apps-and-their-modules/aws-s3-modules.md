---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules AWS S3
description: Les modules  [!DNL Adobe Workfront Fusion AWS] S3 vous permettent d’effectuer des opérations sur vos compartiments S3.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 21%

---

# Modules AWS S3

Les modules S3 [!DNL Adobe Workfront Fusion AWS] vous permettent d’effectuer des opérations sur vos compartiments S3.

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

Pour utiliser les modules [!UICONTROL AWS S3], vous devez disposer d’un compte [!DNL Amazon Web Service].

## Connecter [!DNL AWS] à [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Pour connecter [!DNL AWS S3] à [!DNL Workfront Fusion], vous devez connecter votre compte [!DNL AWS] à [!DNL Workfront Fusion]. Pour ce faire, vous devez d’abord créer un utilisateur API dans [!DNL AWS] [!UICONTROL IAM].

1. Connectez-vous à votre compte [!DNL AWS] [!UICONTROL IAM].
1. Accédez à **[!UICONTROL Gestion des identités et des accès]** > **[!UICONTROL Gestion des accès]** > **[!UICONTROL Utilisateurs]**.

1. Cliquez sur **[!UICONTROL Ajouter un utilisateur]**.
1. Saisissez le nom du nouvel utilisateur et sélectionnez l&#39;option **[!UICONTROL Accès programmatique]** dans la section [!UICONTROL Type d&#39;accès] .
1. Cliquez sur **[!UICONTROL Joindre directement les stratégies existantes]**, puis recherchez **[!UICONTROL AmazonS3FullAccess]** dans la barre de recherche. Cliquez dessus lorsqu’il apparaît, puis cliquez sur **[!UICONTROL Suivant]**.

1. Passez aux autres écrans de la boîte de dialogue, puis cliquez sur **[!UICONTROL Créer un utilisateur]**.
1. Copiez l&#39;**[!UICONTROL ID de clé d&#39;accès]** et la **[!UICONTROL clé d&#39;accès secrète]** fournis.

1. Accédez à [!DNL Workfront Fusion] et ouvrez la boîte de dialogue **[!UICONTROL Créer une connexion]** du module [!DNL AWS S3].
1. Saisissez les [!UICONTROL ID de la clé d&#39;accès] et [!UICONTROL Clé d&#39;accès secrète] de l&#39;étape 7 aux champs respectifs et cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

## Modules [!DNL AWS S3] et leurs champs

Lorsque vous configurez des modules [!DNL AWS S3], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL AWS S3] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)

### Actions

* [[!UICONTROL Créer un compartiment]](#create-bucket)
* [[!UICONTROL Obtenir un fichier]](#get-file)
* [[!UICONTROL Télécharger le fichier]](#upload-file)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL Créer un compartiment]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL AWS] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez le nom du nouveau compartiment.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur les <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans la documentation AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un fichier]

Télécharge un fichier depuis un compartiment.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL AWS] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur les <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points d’entrée régionaux</a> dans la documentation [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartiment] </td> 
   <td> <p>Sélectionnez le compartiment à partir duquel vous souhaitez télécharger le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Saisissez le chemin d’accès au fichier. Exemple : <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger le fichier]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL AWS] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur les <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points d’entrée régionaux</a> dans la documentation [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (facultatif) </p> </td> 
   <td> <p>Indiquez le dossier cible vers lequel vous souhaitez charger un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL En-têtes] (facultatif)</p> </td> 
   <td> <p> Insérez des en-têtes de requête. Les en-têtes disponibles se trouvent dans la documentation <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] - Objet [!UICONTROL PUT]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Pour une discussion détaillée sur l’API [!DNL Amazon S3], voir [[!DNL Amazon S3] [!UICONTROL REST] API Introduction](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL AWS] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur les <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points d’entrée régionaux</a> dans la documentation [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Saisissez une URL hôte. Le chemin doit être relatif à<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête [!UICONTROL HTTP] dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir les méthodes de requête <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez un en-tête de requête. Vous pouvez utiliser les en-têtes de requête courants suivants. Pour plus d’en-têtes de requête, reportez-vous à la <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] documentation de l’API</a>.</p> <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation.</p> 
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
       <td> <p>Type de contenu de la ressource, au cas où le contenu de la requête se trouverait dans le corps. Exemple : <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Résumé MD5 128 bits encodé en base64 du message (sans en-têtes), selon la RFC 1864. Cet en-tête peut être utilisé comme contrôle d’intégrité du message pour vérifier que les données sont les mêmes données que celles envoyées initialement. Bien qu’il soit facultatif, nous vous recommandons d’utiliser le mécanisme [!UICONTROL Content-MD5] comme contrôle d’intégrité de bout en bout. Pour plus d’informations sur l’'authentification de requête [!UICONTROL REST], consultez la page <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] Authentication</a> du <i>[!DNL Amazon] Guide du développeur de services de stockage simple</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>Date et heure actuelles en fonction du demandeur. Exemple : <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Lorsque vous spécifiez l'en-tête <code>Authorization </code>, vous devez spécifier l'en-tête <code>x-amz-date</code> ou <code>Date </code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Attendez]</p> </td> 
       <td> <p>Lorsque votre application utilise [!UICONTROL 100-continue], elle n’envoie pas le corps de la requête tant qu’elle n’a pas reçu d’accusé de réception. Si le message est rejeté en fonction des en-têtes, le corps du message n’est pas envoyé. Cet en-tête ne peut être utilisé que si vous envoyez un corps.</p> <p>Valeurs valides : [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Pour les demandes de style de chemin d’accès, la valeur est <code>s3.amazonaws.com</code>. Pour les demandes de style virtuel, la valeur est <code>BucketName.s3.amazonaws.com</code>. Pour plus d’informations, voir <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Hébergement virtuel</a> dans le <i>[!DNL Amazon] Simple Storage Service Developer Guide</i>.</p> <p>Cet en-tête est requis pour HTTP 1.1 (la plupart des kits d’outils ajoutent cet en-tête automatiquement) ; facultatif pour les requêtes HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Lorsque vous utilisez la version 4 de signature pour authentifier la requête, cet en-tête fournit un hachage de la payload de la requête. Lors du chargement d’un objet en blocs, définissez la valeur sur <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> pour indiquer que la signature couvre uniquement les en-têtes et qu’il n’y a pas de charge utile. Pour plus d’informations, voir <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Calculs de signature pour l’en-tête d’autorisation : transfert de charge utile en plusieurs blocs (téléchargement fragmenté) ([!DNL AWS] Signature version 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>Date et heure actuelles en fonction du demandeur. Exemple : <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Lorsque vous spécifiez l'en-tête <code>Authorization </code>, vous devez spécifier l'en-tête <code>x-amz-date</code> ou <code>Date </code>. Si vous spécifiez les deux, la valeur spécifiée pour l’en-tête <code>x-amz-date</code> est prioritaire.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Cet en-tête peut être utilisé dans les scénarios suivants :</p> 
        <ul> 
         <li>Fournissez des jetons de sécurité pour les opérations [!DNL Amazon DevPay]. Chaque requête qui utilise [!DNL Amazon DevPay] nécessite deux en-têtes <code>x-amz-security-token</code> : un pour le jeton de produit et un autre pour le jeton utilisateur. Lorsque [!DNL Amazon S3] reçoit une requête authentifiée, il compare la signature calculée à la signature fournie. Les en-têtes à plusieurs valeurs mal formatés utilisés pour calculer une signature peuvent entraîner des problèmes d’authentification.</li> 
         <li>Fournissez un jeton de sécurité lors de l’utilisation d’informations d’identification de sécurité temporaires. Lors de l’exécution de requêtes à l’aide d’informations d’identification de sécurité temporaires obtenues auprès d’IAM, vous devez fournir un jeton de sécurité à l’aide de cet en-tête. Pour en savoir plus sur les informations d’identification de sécurité temporaires, voir Lancement de requêtes .</li> 
        </ul> <p>Cet en-tête est requis pour les requêtes qui utilisent [!DNL Amazon DevPay] et les requêtes signées à l’aide d’informations d’identification de sécurité temporaires.</p> </td> 
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :   <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL AWS] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur les <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points d’entrée régionaux</a> dans la documentation [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartiment] </td> 
   <td> <p>Sélectionnez le compartiment [!DNL Amazon S3] à rechercher dans les fichiers.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL AWS] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connexion [!DNL AWS] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Sélectionnez votre point de terminaison régional. Pour plus d’informations, voir la discussion sur les <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">points de terminaison régionaux</a> dans la documentation AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartiment] </td> 
   <td> <p>Sélectionnez le compartiment [!DNL Amazon S3] que vous souhaitez rechercher dans les dossiers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (facultatif)</p> </td> 
   <td> <p> Chemin d’accès à un dossier dans lequel rechercher des dossiers, par exemple <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
