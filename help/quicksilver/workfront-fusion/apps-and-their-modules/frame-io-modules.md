---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Frame.io
description: Le [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] compte .
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 0%

---

# [!DNL Frame.io] modules

Le [!DNL Adobe Workfront Fusion] [!DNL Frame.io] Les modules vous permettent de surveiller, créer, mettre à jour, récupérer ou supprimer des ressources et des commentaires dans vos [!DNL Frame.io] compte .

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

Pour utiliser [!DNL Frame.io] modules, vous devez disposer d’un [!DNL Frame.io] account

## Connexion [!DNL Frame.io] to [!UICONTROL Adobe Workfront Fusion]

Vous pouvez vous connecter à [!DNL Frame.io] à l’aide d’un jeton API ou d’OAuth 2.0.

[Se connecter à [!DNL Frame.io] utilisation d’un jeton API](#connect-to-frameio-using-an-api-token)

[Se connecter à [!DNL Frame.io] utilisation d’OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### Se connecter à [!DNL Frame.io] utilisation d’un jeton API

Pour connecter votre [!DNL Frame.io] compte à [!DNL Workfront Fusion] à l’aide d’un jeton API, vous devez créer le jeton API dans votre [!DNL Frame.io] et insérez-le dans le [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Création d’une connexion] boîte de dialogue.

1. Connectez-vous à [!DNL Frame.io] compte .
1. Accédez au **[!UICONTROL Jetons]** dans la [!DNL Frame.io] Développeur.
1. Cliquez sur **[!UICONTROL Nouveau]**.
1. Saisissez le nom du jeton, sélectionnez les portées à utiliser, puis cliquez sur **[!UICONTROL Créer]**.
1. Copiez le jeton fourni.
1. Accédez à [!DNL Workfront Fusion] et ouvrez le [!DNL Frame.io] du module **[!UICONTROL Création d’une connexion]** boîte de dialogue.
1. Dans le **[!UICONTROL Type de connexion]** champ, sélectionnez **[!DNL Frame.io]**.
1. Saisissez le jeton copié à l’étape 5 dans la **[!UICONTROL Votre [!DNL Frame.io] Clé API]** champ et clic **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

### Se connecter à [!DNL Frame.io] utilisation d’OAuth 2.0 PKCE

Vous pouvez créer une connexion à [!DNL Frame.io] utilisation d’OAuth 2.0 PKCE avec un identifiant client facultatif. Si vous souhaitez inclure un ID client dans votre connexion, vous devez créer une application OAuth 2.0 dans votre [!DNL Frame.io] compte .

* [Se connecter à [!DNL Frame.io] utilisation d’OAuth 2.0 PKCE (sans identifiant client)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Se connecter à [!DNL Frame.io] utilisation d’OAuth 2.0 PKCE (avec identifiant client)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Se connecter à [!DNL Frame.io] utilisation d’OAuth 2.0 PKCE (sans identifiant client)

1. Accédez à [!DNL Workfront Fusion] et ouvrez le [!DNL Frame.io] du module **[!UICONTROL Création d’une connexion]** boîte de dialogue.
1. Dans le **[!UICONTROL Type de connexion]** champ, sélectionnez **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Saisissez le nom de la nouvelle connexion dans la **[!UICONTROL Nom de la connexion]** champ .
1. Cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

#### Se connecter à [!DNL Frame.io] utilisation d’OAuth 2.0 PKCE (avec identifiant client)

1. Création d’une application OAuth 2.0 dans [!DNL Frame.io]. Pour obtenir des instructions, voir [!DNL Frame.io] documentation sur [!UICONTROL Flux d’autorisation du code OAuth 2.0].

   >[!IMPORTANT]
   >
   >Lors de la création de l’application OAuth 2.0 dans [!DNL Frame.io]:
   >
   >* Saisissez l’URI de redirection suivant :
   >   
   >  Amériques/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Activez l’option PCKE .



1. Copiez le `client_id`.
1. Accédez à [!DNL Workfront Fusion] et ouvrez le [!DNL Frame.io] du module **[!UICONTROL Création d’une connexion]** boîte de dialogue.
1. Dans le **[!UICONTROL Type de connexion]** champ, sélectionnez **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Saisissez le nom de la nouvelle connexion dans la **[!UICONTROL Nom de la connexion]** champ .
1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
1. Saisissez le `client_id` vous avez copié à l’étape 2 dans la fonction **[!UICONTROL ID client]** champ .
1. Cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

La connexion a été établie. Vous pouvez poursuivre la configuration du module.

## [!DNL Frame.io] modules et leurs champs

Lorsque vous configurez [!DNL Frame.io] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Frame.io] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ressources](#assets)
* [Commentaires](#comments)
* [Projets](#projects)
* [Autre](#other)

### Ressources

* [[!UICONTROL Création d’une ressource]](#create-an-asset)
* [[!UICONTROL Suppression d’une ressource]](#delete-an-asset)
* [[!UICONTROL Obtention d’une ressource]](#get-an-asset)
* [[!UICONTROL Liste des ressources]](#list-assets)
* [[!UICONTROL Mise à jour d’une ressource]](#update-an-asset)
* [[!UICONTROL Regarder la ressource supprimée]](#watch-asset-deleted)
* [[!UICONTROL Étiquette de ressource de contrôle mise à jour]](#watch-asset-label-updated)
* [[!UICONTROL Regarder une nouvelle ressource]](#watch-new-asset)

#### [!UICONTROL Création d’une ressource]

Ce module d’action crée une ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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

#### [!UICONTROL Suppression d’une ressource]

Ce module d’action supprime une ressource spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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

#### [!UICONTROL Obtention d’une ressource]

Ce module d’action récupère les détails de la ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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

#### [!UICONTROL Liste des ressources]

Ce module de recherche récupère toutes les ressources dans le dossier du projet spécifié.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Définition du nombre maximal de ressources [!DNL Workfront Fusion] renverra pendant un cycle d'exécution.</p> </td> 
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
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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
   <td role="rowheader">[!UICONTROL Nom du webhook]</td> 
   <td> <p> Saisissez le nom du webhook, par exemple Ressource supprimée.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Étiquette de ressource de contrôle mise à jour]

Ce module de déclenchement lance un scénario lorsque l’état d’une ressource est défini, modifié ou supprimé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du webhook]</td> 
   <td> <p> Saisissez le nom du webhook, par exemple le statut de la ressource mis à jour.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder une nouvelle ressource]

Ce module de déclenchement lance un scénario lorsqu’une nouvelle ressource est créée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du webhook]</td> 
   <td> <p> Saisissez le nom du webhook, par exemple Ressource créée.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez l’équipe pour laquelle ce webhook est créé.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Commentaires

* [[!UICONTROL Créer un commentaire]](#create-a-comment)
* [[!UICONTROL Suppression d’un commentaire]](#delete-a-comment)
* [[!UICONTROL Obtention d’un commentaire]](#get-a-comment)
* [[!UICONTROL Lister des commentaires]](#list-comments)
* [[!UICONTROL Mettre à jour un commentaire]](#update-a-comment)
* [[!UICONTROL Commentaire de l’observation mis à jour]](#watch-comment-updated)
* [[!UICONTROL Regarder le nouveau commentaire]](#watch-new-comment)

#### [!UICONTROL Créer un commentaire]

Ce module d’action ajoute un nouveau commentaire ou une nouvelle réponse à la ressource.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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

#### [!UICONTROL Suppression d’un commentaire]

Ce module d’action supprime un commentaire existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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
   <td> <p> Sélectionnez le dossier contenant la ressource dont vous souhaitez supprimer un commentaire.</p> </td> 
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

#### [!UICONTROL Obtention d’un commentaire]

Ce module d’action récupère les détails du commentaire spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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

#### [!UICONTROL Lister des commentaires]

Ce module de recherche récupère tous les commentaires de la ressource spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Définir le nombre maximal de commentaires [!DNL Workfront Fusion] renverra pendant un cycle d'exécution.</p> </td> 
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
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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

#### [!UICONTROL Commentaire de l’observation mis à jour]

Ce module de déclenchement lance un scénario lorsqu’un commentaire est modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du webhook] </td> 
   <td> <p>Saisissez le nom du webhook, par exemple Comment modifié.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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
   <td role="rowheader">[!UICONTROL Nom du webhook] </td> 
   <td> <p>Saisissez le nom du webhook, par exemple New Comment.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
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
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’équipe] </td> 
   <td> <p>Sélectionnez ou mappez l’équipe pour laquelle vous souhaitez récupérer les projets.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Définition du nombre maximal de projets [!DNL Workfront Fusion] renverra pendant un cycle d'exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### [!UICONTROL Lancer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Frame.io], voir <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à <code>https://api.frame.io</code>. Exemple: <code> /v2/teams</code></p> <p>Remarque : Pour obtenir la liste des points de fin disponibles, reportez-vous à la section [!DNL Frame.io] Référence de l’API.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode [!UICONTROL]</p> </td> 
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** L’appel API suivant renvoie toutes les équipes et les détails de cet appel dans votre [!DNL Frame.io] compte :

URL: `/v2/teams`

Méthode: `GET`

![](assets/api-call-example.png)

Le résultat se trouve dans la sortie du module sous Bundle > Body.

Dans notre exemple, les détails de 1 équipe ont été renvoyés :

![](assets/api-call-output.png)
