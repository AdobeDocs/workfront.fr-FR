---
title: Modules DocuSign
description: Les modules  [!DNL Adobe Workfront Fusion DocuSign]  vous permettent de surveiller et de récupérer l’état des enveloppes, de rechercher et de récupérer des enveloppes, ou de télécharger et d’envoyer un document pour vous connecter à votre compte  [!DNL DocuSign] .
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1946'
ht-degree: 21%

---

# Modules DocuSign

Les modules [!DNL Adobe Workfront Fusion] [!DNL DocuSign] vous permettent de surveiller et de récupérer l’état de l’enveloppe, de rechercher et de récupérer des enveloppes, ou de télécharger et d’envoyer un document pour vous connecter à votre compte [!DNL DocuSign].

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

Pour utiliser des modules [!DNL DocuSign], vous devez disposer d’un compte [!DNL DocuSign].

## Connecter [!DNL DocuSign] à [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Pour créer une connexion pour vos modules [!DNL DocuSign] :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone [!UICONTROL Connexion] lorsque vous commencez à configurer le premier module [!DNL DocuSign].
1. Saisissez les informations suivantes :

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>Saisissez un nom pour la nouvelle connexion [!DNL DocuSign].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Type de compte]</td> 
      <td>Indiquez si le compte auquel vous souhaitez vous connecter est un compte de production ou de démonstration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Continuez comme décrit dans [Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## Modules [!DNL DocuSign] et leurs champs

Lorsque vous configurez des modules [!DNL DocuSign], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL DocuSign] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)

### Déclencheurs

#### [!UICONTROL Surveiller les enveloppes]

Ce module de déclenchement lance un scénario lorsqu’une enveloppe est envoyée, diffusée, signée, terminée ou refusée.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit utiliser au cours de chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Télécharger un document]](#download-a-document)
* [[!UICONTROL Lire une enveloppe]](#read-an-envelope)
* [[!UICONTROL Télécharger un fichier vers une enveloppe]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Créer une enveloppe]](#create-a-new-envelope)
* [[!UICONTROL Ajouter un destinataire à l’enveloppe]](#add-recipient-to-envelope)
* [[!UICONTROL Ajouter un champ personnalisé]](#add-custom-field)
* [[!UICONTROL Modifier le champ personnalisé]](#modify-custom-field)
* [[!UICONTROL Envoi d’enveloppe]](#send-envelope)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compte]</td> 
   <td>Saisissez ou mappez le compte que vous souhaitez utiliser pour accéder à l'API [!DNL DocuSign].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Saisissez l’adresse sur le serveur web avec lequel le module doit interagir.</p> <p>Vous pouvez saisir une URL relative, ce qui signifie que vous n’avez pas à inclure le protocole (tel que <code>http://</code>) au début. Cela indique au serveur web que l’interaction se produit sur le serveur.</p> <p>Par exemple : <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Cela détermine le type de contenu de la requête.</p> <p>Par exemple,<code> {"Content-type":"application/json"}</code></p> <p>Remarque : si vous obtenez des erreurs et qu’il est difficile de déterminer leur origine, envisagez de modifier les en-têtes en fonction de la documentation [!DNL Workfront]. Si votre appel API personnalisé renvoie une erreur de requête HTTP 422, essayez d’utiliser un en-tête "Content-Type":"text/plain".</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal de résultats à utiliser au cours d’un cycle d’exécution.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Enveloppes de liste
>
>L’appel API suivant renvoie des enveloppes à partir de la date spécifiée dans votre compte [!DNL DocuSign] :
>
>**URL** : `/v2.1/accounts/{accountId}/envelopes/`
>
>**Méthode** : `GET`
>
>**Chaîne de requête** :
>
>* **Clé** : `from_date`
>
>* **Valeur** : `YYYY-MM-DD`
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

#### [!UICONTROL Télécharger un document]

Ce module d’action télécharge un seul document.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] à [!DNL Workfront Fusion]</a> de cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant le document que vous souhaitez télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de l’enveloppe que vous souhaitez télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Document ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du document que vous souhaitez télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificate]</td> 
   <td>Sélectionnez <strong>[!UICONTROL Oui]</strong> si vous souhaitez inclure le certificat de signature d’enveloppe dans le téléchargement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents by User ID]</td> 
   <td>Sélectionnez <strong>[!UICONTROL Oui]</strong> si vous souhaitez permettre aux destinataires de récupérer des documents par identifiant utilisateur. Par exemple, si un utilisateur est inclus dans deux commandes de routage différentes avec des visibilités différentes, l’utilisation de cette option renvoie tous les documents des deux routage.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chiffrer]</td> 
   <td>Sélectionnez <strong>[!UICONTROL Oui]</strong> si vous souhaitez que les octets de PDF renvoyés dans la réponse soient chiffrés pour tous les gestionnaires de clés configurés sur votre compte [!DNL DocuSign].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Sélectionnez la langue.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher les modifications]</td> 
   <td>Lorsque la valeur est définie sur <strong>[!UICONTROL Oui]</strong>, tous les champs modifiés du PDF renvoyé sont mis en surbrillance en jaune et les signatures ou initiales facultatives sont soulignées en rouge.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filigrane]</td> 
   <td> <p>Sélectionnez <strong>[!UICONTROL No]</strong> pour supprimer le filigrane des documents du PDF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire une enveloppe]

Ce module d’action lit des informations sur une enveloppe dans [!DNL DocuSign] à l’aide de l’ID d’enveloppe.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] à [!DNL Workfront Fusion]</a> de cet article.</p> </td>
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un fichier vers une enveloppe]

Ce module charge un fichier spécifié dans une enveloppe existante dans DocuSign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] à [!DNL Workfront Fusion]</a> de cet article.</p> </td>
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
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou saisissez le nom et les données du fichier source.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une enveloppe]

Ce module d’action crée une enveloppe à partir d’un modèle. Elle renvoie l’identifiant de la nouvelle enveloppe, ainsi que l’état de la nouvelle enveloppe.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>Pour plus d’informations sur la connexion de votre compte DocuSign à Workfront Fusion, voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l’application ou du service Web du module à Workfront Fusion</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans Adobe Workfront Fusion</a>.</p> </td> 
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
   <td> <p>Pour plus d’informations sur la connexion de votre compte DocuSign à Workfront Fusion, voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l’application ou du service Web du module à Workfront Fusion</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans Adobe Workfront Fusion</a>.</p> </td> 
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
   <td> <p>Saisissez ou mappez l'adresse email du destinataire à ajouter à l'enveloppe.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] à [!DNL Workfront Fusion]</a> de cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant le document dans lequel vous souhaitez ajouter un champ personnalisé.</p> </td> 
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

#### [!UICONTROL Modifier le champ personnalisé]

Ce module d’action modifie un champ personnalisé à l’aide du nom du champ.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] à [!DNL Workfront Fusion]</a> de cet article.</p> </td>
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL DocuSign] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connexion [!DNL DocuSign] à [!DNL Workfront Fusion]</a> de cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compte] </td> 
   <td> <p>Sélectionnez le compte contenant l’enveloppe préliminaire que vous souhaitez envoyer à ses destinataires.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’enveloppe]</td> 
   <td> <p> Saisissez ou mappez l'identifiant de l'enveloppe que vous souhaitez envoyer à ses destinataires.</p> </td> 
  </tr> 
 </tbody> 
</table>
