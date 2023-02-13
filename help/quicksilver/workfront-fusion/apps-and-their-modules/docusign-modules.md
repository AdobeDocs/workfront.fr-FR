---
title: Modules DocuSign
description: Le [!DNL Adobe Workfront Fusion DocuSign] Les modules vous permettent de surveiller et de récupérer l’état des enveloppes, de rechercher et de récupérer des enveloppes, ou de télécharger et d’envoyer un document pour vous connecter. [!DNL DocuSign] compte .
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1911'
ht-degree: 0%

---

# Modules DocuSign

Le [!DNL Adobe Workfront Fusion] [!DNL DocuSign] Les modules vous permettent de surveiller et de récupérer l’état des enveloppes, de rechercher et de récupérer des enveloppes, ou de télécharger et d’envoyer un document pour vous connecter. [!DNL DocuSign] compte .

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Pour utiliser [!DNL DocuSign] modules, vous devez disposer d’un [!DNL DocuSign] compte .

## Connexion [!DNL DocuSign] to [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Pour créer une connexion pour votre [!DNL DocuSign] modules :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] lorsque vous commencez à configurer la première [!DNL DocuSign] module .
1. Saisissez les informations suivantes :

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nom de la connexion]</p> </td> 
      <td>Saisissez un nom pour la nouvelle [!DNL DocuSign] connection</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Type de compte]</td> 
      <td>Indiquez si le compte auquel vous souhaitez vous connecter est un compte de production ou de démonstration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Continuez comme décrit dans la section [Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] modules et leurs champs

Lorsque vous configurez [!DNL DocuSign] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL DocuSign] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)

### Triggers

#### [!UICONTROL Envois de montre]

Ce module de déclenchement lance un scénario lorsqu’une enveloppe est envoyée, diffusée, signée, terminée ou refusée.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte qui contient les enregistrements à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’événement]</td> 
   <td> <p> Sélectionnez le type d’événement à regarder.</p> 
    <ul> 
     <li>[!UICONTROL Document terminé]</li> 
     <li>[!UICONTROL Document décliné]</li> 
     <li>[!UICONTROL Document envoyé]</li> 
     <li>[!UICONTROL Document signé]</li> 
     <li>[!UICONTROL Nouveau document dans la boîte de réception]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Champs de sortie]</p> </td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit utiliser au cours de chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Téléchargement d’un document]](#download-a-document)
* [[!UICONTROL Lecture d’une enveloppe]](#read-an-envelope)
* [[!UICONTROL Transfert d’un fichier vers une enveloppe]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Création d’une enveloppe]](#create-a-new-envelope)
* [[!UICONTROL Ajouter un destinataire à l’enveloppe]](#add-recipient-to-envelope)
* [[!UICONTROL Ajouter un champ personnalisé]](#add-custom-field)
* [[!UICONTROL Modifier un champ personnalisé]](#modify-custom-field)
* [[!UICONTROL Envoi d’enveloppe]](#send-envelope)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compte]</td> 
   <td>Saisissez ou mappez le compte que vous souhaitez utiliser pour accéder au [!DNL DocuSign] API.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Saisissez l’adresse sur le serveur web avec lequel le module doit interagir.</p> <p>Vous pouvez saisir une URL relative, ce qui signifie que vous n’avez pas besoin d’inclure le protocole (tel que <code>http://</code>) au début. Cela indique au serveur web que l’interaction se produit sur le serveur.</p> <p>Par exemple : <code>[!DNL /api/conversations].create</code></p> <p>Conseil : Pour obtenir la liste des points de fin disponibles, voir <a href="https://developers.docusign.com/esign-rest-api/reference">[!DNL DocuSign] Référence d’API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Méthode [!UICONTROL]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Cela détermine le type de contenu de la requête.</p> <p>Par exemple,<code> {"Content-type":"application/json"}</code></p> <p>Remarque : Si vous rencontrez des erreurs et qu’il est difficile de déterminer leur origine, envisagez de modifier les en-têtes en fonction de la variable [!DNL Workfront] documentation. Si votre appel API personnalisé renvoie une erreur de requête HTTP 422, essayez d’utiliser un en-tête "Content-Type":"text/plain".</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Saisissez ou mappez le nombre maximal de résultats à utiliser au cours d’un cycle d’exécution.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Enveloppes de liste
>
>L’appel API suivant renvoie des enveloppes à partir de la date spécifiée dans votre [!DNL DocuSign] compte :
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**Méthode**: `GET`
>
>**Chaîne de requête**:
>
>* **Clé**: `from_date`
>
>* **Valeur**: `YYYY-MM-DD`
>
>Indique le moment où la requête commence à vérifier les modifications d’état des enveloppes du compte.
>
>![](assets/example-docusign-setup-350x770.png)
>
>Le résultat se trouve dans la sortie du module sous Bundle > Body > enveloppes.
>
>Dans notre exemple, 6 enveloppes ont été renvoyées :
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL Téléchargement d’un document]

Ce module d’action télécharge un seul document.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant le document à télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de l’enveloppe que vous souhaitez télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID du document]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du document que vous souhaitez télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificate]</td> 
   <td>Sélectionner <strong>[!UICONTROL Oui]</strong> si vous souhaitez inclure le certificat de signature d’enveloppe dans le téléchargement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents by User ID]</td> 
   <td>Sélectionner <strong>[!UICONTROL Oui]</strong> si vous souhaitez permettre aux destinataires de récupérer des documents par identifiant utilisateur. Par exemple, si un utilisateur est inclus dans deux commandes de routage différentes avec des visibilités différentes, l’utilisation de cette option renvoie tous les documents des deux routage.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chiffrer]</td> 
   <td>Sélectionner <strong>[!UICONTROL Oui]</strong> si vous souhaitez que les octets de PDF renvoyés dans la réponse soient chiffrés pour tous les gestionnaires de clés configurés sur votre [!DNL DocuSign] compte .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Sélectionnez la langue.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher les modifications]</td> 
   <td>Lorsque la variable est définie sur <strong>[!UICONTROL Oui]</strong>, les champs modifiés du PDF renvoyé sont mis en surbrillance en jaune et les signatures ou initiales facultatives sont indiquées en rouge.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filigrane]</td> 
   <td> <p>Sélectionner <strong>[!UICONTROL No]</strong> pour supprimer le filigrane des documents du PDF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lecture d’une enveloppe]

Ce module d’action lit des informations sur une enveloppe dans [!DNL DocuSign] à l’aide de l’ID d’enveloppe.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant le document à partir duquel vous souhaitez lire les informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l’identifiant avec le document à partir duquel vous souhaitez lire les informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Transfert d’un fichier vers une enveloppe]

Ce module charge un fichier spécifié dans une enveloppe existante dans DocuSign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant l’enveloppe dans laquelle vous souhaitez transférer un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de l’enveloppe dans laquelle vous souhaitez charger un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fichier source]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou saisissez le nom et les données du fichier source.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’une enveloppe]

Ce module d’action crée une enveloppe à partir d’un modèle. Elle renvoie l’identifiant de la nouvelle enveloppe, ainsi que l’état de la nouvelle enveloppe.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>Pour plus d’informations sur la connexion de votre compte DocuSign à Workfront Fusion, voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service Web du module à Workfront Fusion</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Compte] </td>
   <td> <p>Sélectionnez le compte contenant l’enveloppe dans laquelle vous souhaitez transférer un fichier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template]</td>
   <td> <p> Sélectionnez le modèle à partir duquel vous souhaitez créer la nouvelle enveloppe. Les modèles sont disponibles en fonction du [!UICONTROL Compte] que vous avez sélectionné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL Après la création]
   </td> 
   <td> <p>Indiquez si vous souhaitez enregistrer l’enveloppe en tant que brouillon ou l’envoyer pour signature.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Destinataires des modèles]</td>
    <td>Sélectionner le destinataire de cette enveloppe</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter un destinataire à l’enveloppe]

Ce module d’action ajoute un ou plusieurs destinataires à une enveloppe existante. Si l&#39;enveloppe a déjà été envoyée, le destinataire reçoit un email. Ce module n’est pas valide pour les enveloppes déjà terminées.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Pour plus d’informations sur la connexion de votre compte DocuSign à Workfront Fusion, voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service Web du module à Workfront Fusion</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Compte] </td>
   <td> <p>Sélectionnez le compte contenant l'enveloppe dans laquelle vous souhaitez ajouter des destinataires.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID d’enveloppe]</td>
    <td>Sélectionnez le ou mappez l'identifiant de l'enveloppe dans laquelle vous souhaitez ajouter le destinataire.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Type de destinataire]</td>
   <td> <p> Sélectionnez le type de destinataire à ajouter à l'enveloppe.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Carbon copy]</p> </li> 
     <li> <p>[!UICONTROL Diffusion certifiée]</p> </li> 
     <li> <p>[!UICONTROL Signataire en personne]</p> </li> 
     <li> <p>[!UICONTROL Intermédiaire]</p> </li> 
     <li> <p>[!UICONTROL Signer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Email]</td>
   <td> <p>Saisissez ou mappez l'adresse email du destinataire que vous souhaitez ajouter à l'enveloppe.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Name]</td>
   <td>Saisissez ou mappez le nom du destinataire à ajouter à l'enveloppe.</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Ordre de routage]</td>
   <td> <p>Saisissez ou mappez le numéro de routage du destinataire. Le numéro de routage détermine l’ordre dans lequel les destinataires reçoivent et signent vos documents.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Corps de l’email]</td>
   <td>Saisissez ou mappez le corps (contenu) de l'email envoyé au destinataire.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Objet de l’email]</td>
   <td>Saisissez ou mappez l'objet de l'email envoyé au destinataire.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Message privé]</td>
   <td> <li> <p>Seul le destinataire sélectionné voit le message privé, ainsi que le message général. Le message privé est limité à 1 000 caractères.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Authentication]</td> 
   <td> <p>Sélectionnez la méthode d'authentification à utiliser pour confirmer l'identité du destinataire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Aucun]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Code d’accès]</strong> </p> <p>Saisissez ou mappez le code d’accès.</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>Saisie ou mappage du numéro de téléphone</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>Saisie ou mappage du numéro de téléphone</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter un champ personnalisé]

Ce module d’action ajoute un champ personnalisé au document.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant le document auquel vous souhaitez ajouter un champ personnalisé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de l’enveloppe qui contient le document dans lequel vous souhaitez ajouter un champ personnalisé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du champ]</td> 
   <td>Saisissez ou mappez un nom pour le nouveau champ à ajouter.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obligatoire]</td> 
   <td>Activez cette option si vous souhaitez que le champ ajouté soit un champ obligatoire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher le champ]</td> 
   <td>Activez cette option si vous souhaitez que le champ soit visible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Saisissez ou mappez la valeur (contenu) du champ ajouté. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modifier un champ personnalisé]

Ce module d’action modifie un champ personnalisé à l’aide du nom du champ.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant le document dans lequel vous souhaitez modifier un champ personnalisé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de l’enveloppe qui contient le document dans lequel vous souhaitez modifier un champ personnalisé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field ID]</td> 
   <td>Saisissez ou mappez l’identifiant du champ à modifier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du champ]</td> 
   <td>Saisissez ou mappez le nom du champ à modifier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obligatoire]</td> 
   <td>Activez cette option si vous souhaitez que le champ modifié soit un champ obligatoire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher le champ]</td> 
   <td>Activez cette option si vous souhaitez que le champ soit visible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Saisissez ou mappez la valeur (contenu) du champ modifié. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Envoi d’enveloppe]

Ce module d’action envoie une enveloppe de brouillon à ses destinataires.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL DocuSign] compte à [!DNL Workfront Fusion], voir <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant l'enveloppe de brouillon que vous souhaitez envoyer à ses destinataires.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l'identifiant de l'enveloppe que vous souhaitez envoyer à ses destinataires.</p> </td> 
  </tr> 
 </tbody> 
</table>
