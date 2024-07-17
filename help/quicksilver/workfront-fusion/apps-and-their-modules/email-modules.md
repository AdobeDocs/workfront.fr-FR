---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules d’e-mail
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez connecter votre compte de messagerie à plusieurs applications et services tiers. Cela vous permet de télécharger des emails via IMAP, d’envoyer des emails via SMTP, de créer des brouillons, de déplacer et de copier des emails d’un dossier vers un autre, de marquer les emails comme lus ou non lus et de supprimer des emails.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2626'
ht-degree: 8%

---

# Modules d’e-mail

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez connecter votre compte de messagerie à plusieurs applications et services tiers. Cela vous permet de télécharger des emails via IMAP, d’envoyer des emails via SMTP, de créer des brouillons, de déplacer et de copier des emails d’un dossier vers un autre, de marquer les emails comme lus ou non lus et de supprimer des emails.

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

## Connexion de votre courrier électronique à Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Connexion à Google](#connect-to-google)
* [Connexion à d’autres services de messagerie électronique (SMAP)](#connect-to-other-email-services-smap)

### Connexion à [!DNL Google]

Utilisez cette option pour créer des scénarios avec des modules de messagerie qui nécessitent une connexion à votre compte [!DNL Google]. Il s’agit d’un compte avec des portées restreintes.

Vous pouvez créer une connexion à votre compte [!DNL Google] directement depuis un module de messagerie.

1. Dans n&#39;importe quel module de messagerie, cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion] .
1. Sélectionnez **[!DNL Google]** comme type de connexion.
1. Saisissez le nom de la connexion.
1. (Facultatif) Saisissez votre [!UICONTROL [!DNL Google] ID client] et votre [!UICONTROL Secret client].
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

### Connexion à d’autres services de messagerie électronique (SMAP)

La connexion SMAP permet d&#39;accéder à distance à votre boîte mail et de lire ou manipuler les messages de votre boîte mail. La connexion SMAP est utilisée par la plupart des modules de messagerie.

1. Dans n&#39;importe quel module de messagerie, cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion] .
1. Sélectionnez **[!UICONTROL Autres (SMTP)]** comme type de connexion.
1. Saisissez un **[!UICONTROL Nom]** pour la connexion.
1. Sélectionnez votre **[!UICONTROL fournisseur de messagerie]** dans la liste. Si votre fournisseur de messagerie n’est pas dans la liste, sélectionnez Autre.
1. Saisissez votre **[!UICONTROL Adresse électronique]**, **[!UICONTROL votre nom complet]**, votre **[!UICONTROL nom d’utilisateur]** et votre **[!UICONTROL mot de passe]**.
1. (Conditionnel) Si votre fournisseur ne figure pas dans la liste, saisissez vos **[!UICONTROL serveur SMTP]** et **[!UICONTROL port]**, et indiquez si vous souhaitez **[!UICONTROL utiliser une connexion sécurisée (TLS)]**. Pour trouver ces informations, consultez la section [!UICONTROL Aide] de votre boîte aux lettres. Si vous ne disposez pas de ces informations, contactez votre fournisseur de services de messagerie.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!UICONTROL Email] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Email], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, des champs supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Certains champs d&#39;email peuvent déjà contenir des données, car vous les avez utilisées dans un autre module dans le scénario. Consultez la documentation d’aide par courrier électronique si vous avez besoin d’informations à leur sujet.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>L’ID d’adresse électronique unique appelé &quot;[!UICONTROL ID d’adresse électronique (UID)]&quot; est l’identifiant de l’adresse électronique. L’ID de message électronique est spécifique à chacun des dossiers de l’email.

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Itérateurs](#iterators)

### Déclencheurs

#### [!UICONTROL Watch Emails]

Déclenche lorsqu’un nouvel email est reçu pour traitement selon des critères spécifiés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td> 
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
   <td> <p> Le nombre maximal de messages électroniques [!DNL Workfront Fusion] doit être renvoyé au cours d’un cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Envoyer un courrier électronique]](#send-an-email)
* [[!UICONTROL Créer un brouillon]](#create-a-draft)
* [[!UICONTROL Marquer un email comme lu]](#mark-an-email-as-read)
* [[!UICONTROL Marquer un email comme non lu]](#mark-an-email-as-unread)
* [[!UICONTROL Déplacer un email]](#move-an-email)
* [[!UICONTROL Copier un email]](#copy-an-email)
* [[!UICONTROL Supprimer un email]](#delete-an-email)
* [[!UICONTROL Obtenir des emails]](#get-emails)

#### [!UICONTROL Envoyer un courrier électronique]

Envoie un nouvel email.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!DNL Workfront Fusion], voir <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enregistrer le message après l’envoi]</td> 
   <td>Une fois le message électronique envoyé, il sera enregistré dans votre boîte aux lettres. Activez cette option si vous souhaitez enregistrer les emails envoyés à l’aide de [!DNL Workfront Fusion] dans le dossier <i>[!UICONTROL Envoyé]</i> ou dans un autre dossier de votre boîte aux lettres. Certains services de messagerie, tels que [!DNL Gmail], enregistrent automatiquement les messages envoyés.</td> 
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
   <td> <p>Saisissez ou mappez le contenu de l'email au format HTML à l'aide de balises d'HTML, ou en texte brut, selon ce que vous avez choisi dans le champ [!UICONTROL Type de contenu] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajouter une pièce jointe :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom de fichier]</strong> </p> <p>Saisissez le nom du fichier. Par exemple, sample.doc.</p> </li> 
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
   <td> <p>Entrez ou mappez l’adresse électronique (et le nom, le cas échéant) qui apparaît dans le champ [!UICONTROL À partir de] de l’adresse électronique. </p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Remarque : En règle générale, [!DNL Workfront Fusion] utilise l’adresse électronique que vous avez saisie lors de la création de la connexion comme adresse d’expéditeur. Si vous saisissez une autre adresse électronique, une erreur peut se produire lors de l’envoi d’un message, car votre compte peut ne pas être autorisé à envoyer des emails depuis une autre adresse que la vôtre. Par exemple, <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Entrez ou mappez l’adresse électronique qui apparaît dans le champ [!UICONTROL Expéditeur] de l’adresse électronique.</p> <p>Conseil : Si vous n’êtes pas sûr d’utiliser ce champ ou le champ De , il est recommandé de choisir le champ De .</p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
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
   <td role="rowheader">[!UICONTROL References] </td> 
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

#### [!UICONTROL Créer un brouillon]

Crée et ajoute un nouveau brouillon à un dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td>
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
   <td> <p>Saisissez ou mappez le contenu de l'email au format HTML à l'aide de balises d'HTML, ou en texte brut, selon ce que vous avez choisi dans le champ [!UICONTROL Type de contenu] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajouter une pièce jointe :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom de fichier]</strong> </p> <p>Saisissez le nom du fichier. Par exemple, sample.doc.</p> </li> 
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
   <td> <p>Entrez ou mappez l’adresse électronique (et le nom, le cas échéant) qui apparaît dans le champ [!UICONTROL À partir de] de l’adresse électronique. </p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code>.</p> <p>Remarque : En règle générale, [!DNL Workfront Fusion] utilise l’adresse électronique que vous avez saisie lors de la création de la connexion comme adresse d’expéditeur. Si vous saisissez une autre adresse électronique, une erreur peut se produire lors de l’envoi d’un message, car votre compte peut ne pas être autorisé à envoyer des emails depuis une autre adresse que la vôtre. Par exemple, <code>test@mail.com</code> ou "<code>John Bush" test@email.com</code>".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Entrez ou mappez l’adresse électronique qui apparaît dans le champ [!UICONTROL Expéditeur] de l’adresse électronique.</p> <p>Conseil : Si vous n’êtes pas sûr d’utiliser ce champ ou le champ De , il est recommandé de choisir le champ De .</p> <p>Important : Utilisez la syntaxe correcte : <code>name@email.com</code> ou <code>"Name" name@email.com</code></p> </td> 
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
   <td role="rowheader">[!UICONTROL References] </td> 
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

#### [!UICONTROL Marquer un email comme lu]

Marque un courrier électronique ou un brouillon dans un dossier sélectionné comme lu en définissant l’indicateur [!UICONTROL Lecture] .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td>
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

#### [!UICONTROL Marquer un email comme non lu]

Marque un courrier électronique ou un brouillon dans un dossier sélectionné comme non lu en définissant l’indicateur Non lu .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td>
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
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Sélectionnez le dossier contenant l'email à partir duquel vous souhaitez déplacer l'email. Exemple : Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> Sélectionnez le dossier auquel vous souhaitez ajouter l'email. Exemple : travail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’adresse électronique (UID)]</p> </td> 
   <td> <p>Saisissez l'UID de l'email que vous souhaitez déplacer vers le dossier de destination.</p> <p>Vous pouvez obtenir l’UID de l’email à l’aide du module [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou du module [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier un email]

Copie un courrier électronique ou un brouillon dans un dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Sélectionnez le dossier dans lequel vous souhaitez copier l'email. Exemple : Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> Sélectionnez le dossier dans lequel vous souhaitez copier l'email. Exemple : travail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’adresse électronique (UID)]</p> </td> 
   <td> <p>Saisissez l'UID de l'email que vous souhaitez copier dans le dossier de destination.</p> <p>Vous pouvez obtenir l’UID de l’email à l’aide du module [!UICONTROL Email] &gt;[!UICONTROL Watch Email] ou du module [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un email]

Supprime un courrier électronique ou un brouillon du dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td>
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
   <td> <p>Pour plus d’informations sur la connexion de votre compte de messagerie à [!UICONTROL Workfront Fusion], reportez-vous à la section <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Connexion de votre adresse électronique à [!UICONTROL Workfront Fusion]</a> de cet article.</p> </td>
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
   <td> <p> Saisissez l’ ID d’adresse électronique (UID) de l’adresse électronique dont vous souhaitez récupérer les détails.</p> <p>Vous pouvez obtenir l’UID de l’email en utilisant le module [!UICONTROL Email] de [!DNL Workfront Fusion] ou le module [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de résultats]</td> 
   <td> <p> Le nombre maximal de messages électroniques [!DNL Workfront Fusion] doit être renvoyé au cours d’un cycle d’exécution de scénario.</p> </td> 
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
   <td role="rowheader">Module [!UICONTROL Source]</td> 
   <td> <p>Sélectionnez le module qui génère l’email avec les pièces jointes que vous souhaitez itérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur les itérateurs, voir [Module d’itérateur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
