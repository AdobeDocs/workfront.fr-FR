---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules email
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez connecter votre compte de messagerie à plusieurs applications et services tiers. Cela vous permet de télécharger des emails via IMAP, d’envoyer des emails via SMTP, de créer des brouillons, de déplacer et de copier des emails d’un dossier vers un autre, de marquer les emails comme lus ou non lus et de supprimer des emails.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: ea19c2a58bac322c804fca3f6bb7d7147efa4d9a
workflow-type: tm+mt
source-wordcount: '2578'
ht-degree: 0%

---

# Modules email

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez connecter votre compte de messagerie à plusieurs applications et services tiers. Cela vous permet de télécharger des emails via IMAP, d’envoyer des emails via SMTP, de créer des brouillons, de déplacer et de copier des emails d’un dossier vers un autre, de marquer les emails comme lus ou non lus et de supprimer des emails.

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

## Connexion de votre email à Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Connexion à Google](#connect-to-google)
* [Connexion à d’autres services de messagerie électronique (SMAP)](#connect-to-other-email-services-smap)

### Se connecter à [!DNL Google]

Utilisez cette option pour créer des scénarios avec des modules de messagerie qui nécessitent une connexion à votre [!DNL Google] compte . Il s’agit d’un compte avec des portées restreintes.

Vous pouvez créer une connexion à votre [!DNL Google] compte directement depuis un module Email.

1. Dans n’importe quel module Email, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Sélectionner **[!DNL Google]** comme type de connexion.
1. Saisissez le nom de la connexion.
1. (Facultatif) Saisissez votre [!UICONTROL [!DNL Google] ID client] et [!UICONTROL Secret du client].
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

### Connexion à d’autres services de messagerie électronique (SMAP)

La connexion SMAP permet d&#39;accéder à distance à votre boîte mail et de lire ou manipuler les messages de votre boîte mail. La connexion SMAP est utilisée par la plupart des modules de messagerie.

1. Dans n’importe quel module Email, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Sélectionner **[!UICONTROL Autres (SMTP)]** comme type de connexion.
1. Saisissez un **[!UICONTROL Nom]** pour la connexion.
1. Sélectionnez votre **[!UICONTROL Fournisseur de messagerie]** dans la liste. Si votre fournisseur de messagerie n’est pas dans la liste, sélectionnez Autre.
1. Saisissez votre **[!UICONTROL Adresse électronique]**, **[!UICONTROL Votre nom complet]**, votre **[!UICONTROL Nom d’utilisateur]**, et **[!UICONTROL Mot de passe]**.
1. (Conditionnel) Si votre fournisseur ne figure pas dans la liste, saisissez votre **[!UICONTROL Serveur SMTP]** et **[!UICONTROL Port]**, puis indiquez si vous souhaitez **[!UICONTROL Utiliser une connexion sécurisée (TLS)]**. Pour trouver ces informations, cochez la case [!UICONTROL Aide] pour votre boîte aux lettres. Si vous ne disposez pas de ces informations, contactez votre fournisseur de services de messagerie.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## [!UICONTROL Email] modules et leurs champs

Lorsque vous configurez [!UICONTROL Email] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, des champs supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Certains champs d&#39;email peuvent déjà contenir des données, car vous les avez utilisées dans un autre module dans le scénario. Consultez la documentation d’aide par courrier électronique si vous avez besoin d’informations à leur sujet.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>L’ID d’adresse électronique unique connu sous le nom de &quot;&quot;[!UICONTROL ID de message électronique (UID)]&#39; est l’identifiant de l’email. L’ID d’adresse électronique est spécifique à chacun des dossiers de l’adresse électronique.

* [Triggers](#triggers)
* [Actions](#actions)
* [Itérateurs](#iterators)

### Triggers

#### [!UICONTROL Regarder les emails]

Déclenche lorsqu’un nouvel email est reçu pour traitement selon des critères spécifiés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier contenant les emails que vous souhaitez voir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Critères]</p> </td> 
   <td> <p>Sélectionnez les critères selon lesquels vous souhaitez voir les emails :</p> 
    <ul> 
     <li>[!UICONTROL Tous les emails]</li> 
     <li>[!UICONTROL Lecture Seule Des Emails]</li> 
     <li>[!UICONTROL Uniquement Les Emails Non Lus]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adresse électronique de l’expéditeur] </td> 
   <td> <p>Saisissez l'adresse email de l'expéditeur dont vous souhaitez consulter les emails.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Adresse électronique du destinataire]</td> 
   <td> <p> Saisissez l'adresse email du destinataire dont vous souhaitez consulter les emails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Saisissez l’objet de l’email que vous souhaitez regarder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Entrez des mots-clés pour ne regarder que les emails contenant des expressions spécifiques.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marquer le ou les messages comme lus lors de la récupération]</td> 
   <td> <p>Activez cette option pour marquer l’email non lu comme lu après avoir récupéré les détails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de résultats]</td> 
   <td> <p> Nombre maximal d’emails [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Envoyer un courrier électronique]](#send-an-email)
* [[!UICONTROL Création d’un brouillon]](#create-a-draft)
* [[!UICONTROL Marquage d’un email comme lu]](#mark-an-email-as-read)
* [[!UICONTROL Marquage d’un email comme non lu]](#mark-an-email-as-unread)
* [[!UICONTROL Déplacer un email]](#move-an-email)
* [[!UICONTROL Copier un courrier électronique]](#copy-an-email)
* [[!UICONTROL Suppression d’un courrier électronique]](#delete-an-email)
* [[!UICONTROL Obtenir des emails]](#get-emails)

#### [!UICONTROL Envoyer un courrier électronique]

Envoie un nouvel email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte de messagerie à [!DNL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enregistrer le message après l’envoi]</td> 
   <td>Une fois le message électronique envoyé, il sera enregistré dans votre boîte aux lettres. Activez cette option si vous souhaitez enregistrer les emails envoyés à l’aide de [!DNL Workfront Fusion] au <i>[!UICONTROL Envoyé du courrier]</i> ou un autre dossier de votre boîte aux lettres. Certains services de messagerie, tels que [!DNL Gmail], enregistrez automatiquement les messages envoyés.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À] </td> 
   <td> <p>Ajoutez les adresses électroniques auxquelles vous souhaitez envoyer l’email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Saisissez ou mappez l’objet du courrier électronique.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>Sélectionnez le type [!UICONTROL content] de l'email :</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Saisissez ou mappez le contenu de l'email au format HTML à l'aide de balises de HTML, ou en texte brut, selon ce que vous avez choisi dans le champ [!UICONTROL Type de contenu] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajouter une pièce jointe :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom du fichier]</strong> </p> <p>Saisissez le nom du fichier. Par exemple, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez le chemin d’accès au dossier où télécharger la pièce jointe.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Saisissez l’[!UICONTROL ID de contenu] pour insérer la pièce jointe (image) dans le contenu.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copier le destinataire] </td> 
   <td> <p>Saisissez ou mappez une ou plusieurs adresses électroniques auxquelles vous souhaitez envoyer une copie de cet email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinataire de la copie aveugle]</td> 
   <td> <p> Saisissez ou mappez une ou plusieurs adresses électroniques auxquelles vous souhaitez envoyer une copie de cet email sans que l’adresse email apparaisse dans l’email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>Entrez ou mappez l’adresse électronique (et le nom, le cas échéant) qui apparaît dans le champ [!UICONTROL À partir de] de l’adresse électronique. </p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Remarque : Normalement, [!DNL Workfront Fusion] utilise l’adresse électronique que vous avez saisie lors de la création de la connexion en tant qu’adresse d’expéditeur. Si vous saisissez une autre adresse électronique, une erreur peut se produire lors de l’envoi d’un message, car votre compte peut ne pas être autorisé à envoyer des emails depuis une autre adresse que la vôtre. Par exemple : <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Entrez ou mappez l’adresse électronique qui apparaît dans le champ [!UICONTROL Expéditeur] de l’adresse électronique.</p> <p>Conseil : Si vous ne savez pas si ce champ doit être utilisé ou le champ De , il est recommandé de choisir le champ De .</p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Réponse]</td> 
   <td> <p> Si vous souhaitez que les réponses à cet email soient envoyées à une adresse différente de celle de l’adresse "expéditeur", saisissez l’adresse email à laquelle vous souhaitez que les réponses à cet email soient envoyées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL En Réponse]</td> 
   <td> <p> Si vous répondez à un email spécifique, saisissez ou mappez l’identifiant de l’email auquel vous répondez.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Références [!UICONTROL] </td> 
   <td> <p>Saisissez les ID de message de toutes les réponses du thread.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Sélectionnez la priorité de l'email :</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Ajoutez les en-têtes :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Ajoutez la clé. Par exemple, [!UICONTROL Expéditeur], [!UICONTROL Date], [!UICONTROL À], etc.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Saisissez la valeur de la clé.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un brouillon]

Crée et ajoute un nouveau brouillon à un dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Sélectionnez le dossier dans lequel vous souhaitez créer le brouillon du courrier électronique.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À] </td> 
   <td> <p>Saisissez ou mappez l'adresse email à laquelle vous souhaitez envoyer l'email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Saisissez ou mappez l’objet du courrier électronique.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>Sélectionnez le type de contenu de l'email :</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Texte brut]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Saisissez ou mappez le contenu de l'email au format HTML à l'aide de balises de HTML, ou en texte brut, selon ce que vous avez choisi dans le champ [!UICONTROL Type de contenu] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajouter une pièce jointe :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom du fichier]</strong> </p> <p>Saisissez le nom du fichier. Par exemple, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez le chemin d’accès au dossier où télécharger la pièce jointe.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Saisissez l'identifiant du contenu pour insérer la pièce jointe (image) dans le contenu.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copier le destinataire] </td> 
   <td> <p>Saisissez ou mappez une ou plusieurs adresses électroniques auxquelles vous souhaitez envoyer une copie de cet email. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinataire de la copie aveugle]</td> 
   <td> <p> Saisissez ou mappez une ou plusieurs adresses électroniques auxquelles vous souhaitez envoyer une copie de cet email sans que l’adresse email apparaisse dans l’email.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>Entrez ou mappez l’adresse électronique (et le nom, le cas échéant) qui apparaît dans le champ [!UICONTROL À partir de] de l’adresse électronique. </p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Remarque : Normalement, [!DNL Workfront Fusion] utilise l’adresse électronique que vous avez saisie lors de la création de la connexion en tant qu’adresse d’expéditeur. Si vous saisissez une autre adresse électronique, une erreur peut se produire lors de l’envoi d’un message, car votre compte peut ne pas être autorisé à envoyer des emails depuis une autre adresse que la vôtre. Par exemple : <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Entrez ou mappez l’adresse électronique qui apparaît dans le champ [!UICONTROL Expéditeur] de l’adresse électronique.</p> <p>Conseil : Si vous ne savez pas si ce champ doit être utilisé ou le champ De , il est recommandé de choisir le champ De .</p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Réponse]</td> 
   <td> <p> Si vous souhaitez que les réponses à cet email soient envoyées à une adresse différente de l’adresse "[!UICONTROL de]", saisissez l’adresse email à laquelle vous souhaitez que les réponses à cet email soient envoyées.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL En Réponse]</td> 
   <td> <p> Si vous répondez à un email spécifique, saisissez ou mappez l’identifiant de l’email auquel vous répondez.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Références [!UICONTROL] </td> 
   <td> <p>Saisissez les ID de message de toutes les réponses du thread.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Sélectionnez la priorité de l'email :</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Ajoutez les en-têtes :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Ajoutez la clé. Par exemple, Expéditeur, Date, A, etc.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Saisissez la valeur de la clé.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marquage d’un email comme lu]

Marque un courrier électronique ou un brouillon dans un dossier sélectionné comme lu en définissant la variable [!UICONTROL Lecture] Indicateur.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Sélectionnez le dossier de l'email que vous souhaitez marquer comme lu. Exemple : Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’adresse électronique (UID)]</p> </td> 
   <td> <p>Saisissez l'UID de l'email que vous souhaitez marquer comme lu.</p> <p>Vous pouvez obtenir l’UID de l’email à l’aide du module [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou du module [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marquage d’un email comme non lu]

Marque un courrier électronique ou un brouillon dans un dossier sélectionné comme non lu en définissant l’indicateur Non lu .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Sélectionnez le dossier de l'email que vous souhaitez marquer comme non lu. Exemple : Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’adresse électronique (UID)]</p> </td> 
   <td> <p>Saisissez l'UID de l'email que vous souhaitez marquer comme non lu.</p> <p>Vous pouvez obtenir l’UID de l’email à l’aide du module [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou du module [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un email]

Déplace un email ou un brouillon sélectionné vers un dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Sélectionnez le dossier contenant l'email à partir duquel vous souhaitez déplacer l'email. Exemple : Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> Sélectionnez le dossier auquel vous souhaitez ajouter l'email. Exemple : Travail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’adresse électronique (UID)]</p> </td> 
   <td> <p>Saisissez l'UID de l'email que vous souhaitez déplacer vers le dossier de destination.</p> <p>Vous pouvez obtenir l’UID de l’email à l’aide du module [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou du module [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier un courrier électronique]

Copie un courrier électronique ou un brouillon dans un dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Sélectionnez le dossier dans lequel vous souhaitez copier l'email. Exemple : Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> Sélectionnez le dossier dans lequel vous souhaitez copier l'email. Exemple : Travail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’adresse électronique (UID)]</p> </td> 
   <td> <p>Saisissez l'UID de l'email que vous souhaitez copier dans le dossier de destination.</p> <p>Vous pouvez obtenir l’UID de l’email à l’aide du module [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou du module [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un courrier électronique]

Supprime un courrier électronique ou un brouillon du dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Sélectionnez le dossier de l'email que vous souhaitez supprimer. Exemple : Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’adresse électronique (UID)]</p> </td> 
   <td> <p>Saisissez l'UID de l'email que vous souhaitez supprimer.</p> <p>Vous pouvez obtenir l’UID de l’email à l’aide du module [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou du module [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>Activez cette option pour permettre au module de supprimer définitivement tous les messages marqués comme [!UICONTROL Supprimés] dans la boîte aux lettres ouverte.</p> <p>Remarque : Dans [!DNL Gmail], ce comportement est piloté par le paramètre de la section [!UICONTROL Paramètres] &gt;[!UICONTROL Transfert POP/IMAP dans l’accès IMAP] .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des emails]

Renvoie les courriers électroniques qui correspondent aux critères spécifiés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connectez votre email à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier contenant les emails que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marquer le ou les messages comme lus lors de la récupération] </td> 
   <td> <p>Activez cette option si vous souhaitez marquer l’email non lu comme lu après avoir récupéré les détails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Critères]</p> </td> 
   <td> <p>Sélectionnez les critères des emails que vous souhaitez récupérer :</p> 
    <ul> 
     <li>[!UICONTROL Tous les emails]</li> 
     <li>[!UICONTROL Lecture Seule Des Emails]</li> 
     <li>[!UICONTROL Uniquement Les Emails Non Lus]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adresse électronique de l’expéditeur] </td> 
   <td> <p>Saisissez ou mappez l'adresse email de l'expéditeur dont vous souhaitez récupérer les emails.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Adresse électronique du destinataire]</td> 
   <td> <p> Saisissez ou mappez l'adresse email du destinataire dont vous souhaitez récupérer les emails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de la date] </td> 
   <td> <p>Saisissez ou mappez la date pour récupérer les emails traités à la date spécifiée ou après cette date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Avant la date]</td> 
   <td> <p> Saisissez ou mappez la date pour récupérer les emails traités à la date spécifiée ou avant.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Saisissez ou mappez l’objet de l’email que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Saisissez ou mappez des mots-clés pour récupérer uniquement les emails contenant des expressions spécifiques.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’adresse électronique (UID)]</td> 
   <td> <p> Saisissez l’ ID d’adresse électronique (UID) de l’adresse électronique dont vous souhaitez récupérer les détails.</p> <p>Vous pouvez obtenir l’UID de l’email en utilisant [!DNL Workfront Fusion]Module s[!UICONTROL Watch Email] ou module [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de résultats]</td> 
   <td> <p> Nombre maximal d’emails [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Poursuivre l’exécution de l’itinéraire même si le module ne renvoie aucun résultat]</td> 
   <td> <p> Sélectionnez cette option si vous souhaitez continuer à exécuter le module même si aucun résultat n’est renvoyé.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Itérateurs

#### [!UICONTROL Itérer les pièces jointes]

Itère une par une les pièces jointes reçues.

Le module d&#39;itérateur d&#39;email permet de gérer séparément les pièces jointes aux emails. Vous pouvez, par exemple, configurer pour qu’il consulte les emails afin qu’ils soient traités avec des pièces jointes et qu’ils reçoivent des alertes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module source]</td> 
   <td> <p>Sélectionnez le module qui génère l’email avec les pièces jointes que vous souhaitez itérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur les itérateurs, voir [Module d’itérateur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
