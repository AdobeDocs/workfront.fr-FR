---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Frame.io
description: Le compte  [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] .
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 15%

---

# Modules [!DNL Frame.io]

Les modules [!DNL Adobe Workfront Fusion] [!DNL Frame.io] vous permettent de surveiller, créer, mettre à jour, récupérer ou supprimer des ressources et des commentaires dans votre compte [!DNL Frame.io].

Pour une présentation vidéo du connecteur Frame.io, voir :

* [Frame.io](https://video.tv.adobe.com/v/3427032/){target=_blank}

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

Pour utiliser les modules [!DNL Frame.io], vous devez avoir un compte [!DNL Frame.io]

## Connectez [!DNL Frame.io] à [!UICONTROL Adobe Workfront Fusion]

Vous pouvez vous connecter à [!DNL Frame.io] à l’aide d’un jeton API ou à l’aide d’OAuth 2.0.

[Connexion à  [!DNL Frame.io]  à l’aide d’un jeton API](#connect-to-frameio-using-an-api-token)

[Connexion à  [!DNL Frame.io] à l’aide d’OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### Connexion à [!DNL Frame.io] à l’aide d’un jeton API

Pour connecter votre compte [!DNL Frame.io] à [!DNL Workfront Fusion] à l’aide d’un jeton API, vous devez créer le jeton API dans votre compte [!DNL Frame.io] et l’insérer dans la boîte de dialogue [!DNL Workfront Fusion] [!DNL Frame.io]  Créer une connexion .

1. Connectez-vous à votre compte [!DNL Frame.io].
1. Accédez à la page **[!UICONTROL Tokens]** du développeur [!DNL Frame.io].
1. Cliquez sur **[!UICONTROL New]**.
1. Saisissez le nom du jeton, sélectionnez les portées à utiliser, puis cliquez sur **[!UICONTROL Créer]**.
1. Copiez le jeton fourni.
1. Accédez à [!DNL Workfront Fusion] et ouvrez la boîte de dialogue **[!UICONTROL Créer une connexion]** du module [!DNL Frame.io].
1. Dans le champ **[!UICONTROL Type de connexion]**, sélectionnez **[!DNL Frame.io]**.
1. Saisissez le jeton que vous avez copié à l’étape 5 dans le champ **[!UICONTROL Votre [!DNL Frame.io] clé API]** et cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

### Connexion à [!DNL Frame.io] à l’aide d’OAuth 2.0 PKCE

Vous pouvez créer une connexion à [!DNL Frame.io] à l’aide de OAuth 2.0 PKCE avec un identifiant client facultatif. Si vous souhaitez inclure un ID client dans votre connexion, vous devez créer une application OAuth 2.0 dans votre compte [!DNL Frame.io].

* [Connexion à  [!DNL Frame.io] à l’aide d’OAuth 2.0 PKCE (sans identifiant client)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Connexion à  [!DNL Frame.io] à l’aide d’OAuth 2.0 PKCE (avec identifiant client)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Connexion à [!DNL Frame.io] à l’aide d’OAuth 2.0 PKCE (sans identifiant client)

1. Accédez à [!DNL Workfront Fusion] et ouvrez la boîte de dialogue **[!UICONTROL Créer une connexion]** du module [!DNL Frame.io].
1. Dans le champ **[!UICONTROL Connection type]** , sélectionnez **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Saisissez un nom pour la nouvelle connexion dans le champ **[!UICONTROL Nom de la connexion]**.
1. Cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

#### Connexion à [!DNL Frame.io] à l’aide d’OAuth 2.0 PKCE (avec identifiant client)

1. Créez une application OAuth 2.0 dans [!DNL Frame.io]. Pour obtenir des instructions, consultez la documentation [!DNL Frame.io] sur le [!UICONTROL flux d’autorisation de code OAuth 2.0].

   >[!IMPORTANT]
   >
   >Lors de la création de l’application OAuth 2.0 dans [!DNL Frame.io] :
   >
   >* Saisissez l’URI de redirection suivant :
   >   
   >  Amériques/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Activez l’option PCKE .


1. Copiez le `client_id` fourni.
1. Accédez à [!DNL Workfront Fusion] et ouvrez la boîte de dialogue **[!UICONTROL Créer une connexion]** du module [!DNL Frame.io].
1. Dans le champ **[!UICONTROL Connection type]** , sélectionnez **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Saisissez un nom pour la nouvelle connexion dans le champ **[!UICONTROL Nom de la connexion]**.
1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
1. Saisissez le `client_id` que vous avez copié à l’étape 2 dans le champ **[!UICONTROL ID client]** .
1. Cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

## Modules [!DNL Frame.io] et leurs champs

Lorsque vous configurez des modules [!DNL Frame.io], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Frame.io] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ressources](#assets)
* [Commentaires](#comments)
* [Projets](#projects)
* [Autre](#other)

### Ressources

* [[!UICONTROL Créer une ressource]](#create-an-asset)
* [[!UICONTROL Supprimer une ressource]](#delete-an-asset)
* [[!UICONTROL Obtenir une ressource]](#get-an-asset)
* [[!UICONTROL Lister Assets]](#list-assets)
* [[!UICONTROL Mettre à jour une ressource]](#update-an-asset)
* [[!UICONTROL Regarder la ressource supprimée]](#watch-asset-deleted)
* [[!UICONTROL Regarder l’étiquette de la ressource mise à jour]](#watch-asset-label-updated)
* [[!UICONTROL Watch New Asset]](#watch-new-asset)

#### [!UICONTROL Créer une ressource]

Ce module d’action crée une ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet pour lequel vous souhaitez créer une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet] </td> 
   <td> <p>Sélectionnez le projet ou mappez l’identifiant du projet pour lequel vous souhaitez créer une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier ou mappez l’identifiant du dossier dans lequel vous souhaitez créer une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Indiquez si vous souhaitez créer un dossier ou un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez le nom du nouveau fichier ou dossier.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source URL] </td> 
   <td> <p>Saisissez l’URL du fichier que vous souhaitez charger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>Saisissez une brève description de la ressource.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une ressource]

Ce module d’action supprime une ressource spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet qui contient la ressource à supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet]</td> 
   <td> <p> Sélectionnez le projet ou qui contient la ressource à supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier contenant la ressource à supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource] </td> 
   <td> <p>Sélectionnez ou mappez la ressource à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une ressource]

Ce module d’action récupère les détails de la ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet qui contient la ressource dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet]</td> 
   <td> <p> Sélectionnez le projet qui contient la ressource dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier contenant la ressource dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource] </td> 
   <td> <p>Sélectionnez la ressource ou mappez l’identifiant de la ressource dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister Assets]

Ce module de recherche récupère toutes les ressources dans le dossier du projet spécifié.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet contenant le dossier duquel vous souhaitez récupérer les ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet]</td> 
   <td> <p> Sélectionnez le projet contenant le dossier duquel vous souhaitez récupérer les ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier à partir duquel vous souhaitez répertorier les ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre maximal de ressources que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

Ce module d’action vous permet de mettre à jour le nom, la description ou les champs personnalisés d’une ressource existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet pour lequel vous souhaitez mettre à jour une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet] </td> 
   <td> <p>Sélectionnez le projet ou mappez l’identifiant du projet pour lequel vous souhaitez mettre à jour une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier ou mappez l’identifiant du dossier dans lequel vous souhaitez mettre à jour une ressource.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez le nom du fichier mis à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>Entrez une brève description de la ressource mise à jour.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder la ressource supprimée]

Ce module de déclenchement lance un scénario lorsqu’une ressource est supprimée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Saisissez le nom du webhook, par exemple Ressource supprimée.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder l’étiquette de la ressource mise à jour]

Ce module de déclenchement lance un scénario lorsque l’état d’une ressource est défini, modifié ou supprimé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Saisissez le nom du webhook, par exemple le statut de la ressource mis à jour.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch New Asset]

Ce module de déclenchement lance un scénario lorsqu’une nouvelle ressource est créée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Saisissez le nom du webhook, par exemple Ressource créée.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Commentaires

* [[!UICONTROL Créer un commentaire]](#create-a-comment)
* [[!UICONTROL Supprimer un commentaire]](#delete-a-comment)
* [[!UICONTROL Obtenir un commentaire]](#get-a-comment)
* [[!UICONTROL Liste des commentaires]](#list-comments)
* [[!UICONTROL Mettre à jour un commentaire]](#update-a-comment)
* [[!UICONTROL Commentaire de contrôle mis à jour]](#watch-comment-updated)
* [[!UICONTROL Regarder le nouveau commentaire]](#watch-new-comment)

#### [!UICONTROL Créer un commentaire]

Ce module d’action ajoute un nouveau commentaire ou une nouvelle réponse à la ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Indiquez si vous souhaitez créer un commentaire ou répondre à un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet contenant la ressource à laquelle vous souhaitez ajouter un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet] </td> 
   <td> <p>Sélectionnez le projet ou mappez l’identifiant du projet qui contient la ressource à laquelle vous souhaitez ajouter un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier ou mappez l’identifiant du dossier contenant la ressource à laquelle vous souhaitez ajouter un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource] </td> 
   <td> <p>Sélectionnez ou mappez la ressource à laquelle vous souhaitez ajouter un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de commentaire] </td> 
   <td> <p>Sélectionnez ou mappez le commentaire auquel vous souhaitez ajouter une réponse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texte]</td> 
   <td> <p> Saisissez le contenu textuel du commentaire ou de la réponse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Horodatage] </td> 
   <td> <p>Saisissez le numéro de l’image dans la vidéo à laquelle le commentaire doit être lié.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un commentaire]

Ce module d’action supprime un commentaire existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe]</td> 
   <td> <p> Sélectionnez ou mappez l’équipe propriétaire du projet qui contient la ressource dont vous souhaitez supprimer un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet]</td> 
   <td> <p> Sélectionnez le projet ou mappez l’identifiant du projet qui contient la ressource dont vous souhaitez supprimer un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier]</td> 
   <td> <p> Sélectionnez le dossier contenant la ressource à partir de laquelle vous souhaitez supprimer un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource] </td> 
   <td> <p>Sélectionnez la ressource contenant le commentaire à supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de commentaire] </td> 
   <td> <p>Sélectionnez le commentaire à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un commentaire]

Ce module d’action récupère les détails du commentaire spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet qui contient le dossier duquel vous souhaitez récupérer les ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet] </td> 
   <td> <p>Sélectionnez le projet contenant le dossier duquel vous souhaitez récupérer les ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier à partir duquel vous souhaitez répertorier les ressources.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource] </td> 
   <td> <p>Sélectionnez la ressource contenant le commentaire que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de commentaire] </td> 
   <td> <p>Sélectionnez le commentaire dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Liste des commentaires]

Ce module de recherche récupère tous les commentaires de la ressource spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet qui contient le dossier duquel vous souhaitez récupérer les commentaires.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet] </td> 
   <td> <p>Sélectionnez le projet contenant le dossier duquel vous souhaitez récupérer les commentaires.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier contenant la ressource à partir de laquelle vous souhaitez répertorier les commentaires.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource] </td> 
   <td> <p>Sélectionnez la ressource pour laquelle vous souhaitez répertorier les commentaires.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre maximal de commentaires [!DNL Workfront Fusion] qui seront renvoyés au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un commentaire]

Ce module d’action modifie un commentaire existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe propriétaire du projet qui contient la ressource sur laquelle vous souhaitez mettre à jour un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet] </td> 
   <td> <p>Sélectionnez le projet \ qui contient la ressource sur laquelle vous souhaitez mettre à jour un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td> <p>Sélectionnez le dossier contenant la ressource sur laquelle vous souhaitez mettre à jour un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de ressource] </td> 
   <td> <p>Sélectionnez la ressource sur laquelle vous souhaitez mettre à jour un commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de commentaire] </td> 
   <td> <p>Sélectionnez le commentaire à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texte]</td> 
   <td> <p> Saisissez le contenu textuel du commentaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Horodatage] </td> 
   <td> <p>Saisissez le numéro de l’image dans la vidéo à laquelle le commentaire est lié.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Commentaire de contrôle mis à jour]

Ce module de déclenchement lance un scénario lorsqu’un commentaire est modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Saisissez le nom du webhook, par exemple Comment modifié.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder le nouveau commentaire]

Ce module de déclenchement lance un scénario lorsqu’un nouveau commentaire ou une nouvelle réponse est créé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Saisissez le nom du webhook, par exemple : Nouveau commentaire.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Projets

#### [!UICONTROL Liste des projets]

Ce module de recherche récupère tous les projets pour l’équipe spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe pour laquelle vous souhaitez récupérer les projets.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre maximal de projets [!DNL Workfront Fusion] qui seront renvoyés au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### [!UICONTROL Effectuer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour plus d'informations sur la création d'une connexion à [!DNL Frame.io], reportez-vous à la section <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] à [!DNL Adobe Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à <code>https://api.frame.io</code>. Exemple : <code> /v2/teams</code></p> <p>Remarque : Pour obtenir la liste des points de terminaison disponibles, reportez-vous à la référence de l’API [!DNL Frame.io].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Saisissez la chaîne de requête de requête de requête. Pour chaque paramètre à inclure dans la chaîne de requête, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez le nom du champ et la valeur souhaitée.</p> </td> 
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

**Exemple :** L’appel API suivant renvoie toutes les équipes et les détails de l’appel dans votre compte [!DNL Frame.io] :

URL : `/v2/teams`

Méthode : `GET`

![](assets/api-call-example.png)

Le résultat se trouve dans la sortie du module sous Bundle > Body.

Dans notre exemple, les détails de 1 équipe ont été renvoyés :

![](assets/api-call-output.png)
