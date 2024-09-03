---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Messagerie e-mail Microsoft Office 365
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent la messagerie e-mail Microsoft Office 365, ainsi que la connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: a09116572d4f9101740fa976f1d334e99fac3010
workflow-type: tm+mt
source-wordcount: '2699'
ht-degree: 82%

---

# Modules [!DNL Microsoft Office 365 Email]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent la [!UICONTROL messagerie e-mail Microsoft Office 365], ainsi que la connecter à plusieurs applications et services tiers.

Pour utiliser la [!UICONTROL messagerie e-mail Microsoft Office 365] avec [!DNL Adobe Workfront Fusion], il est nécessaire de disposer d’un [!UICONTROL compte Office 365]. Rendez-vous sur www.office.com pour en créer un.

Pour savoir comment connecter votre compte [!UICONTROL Office 365] à [!DNL Workfront Fusion], consultez la section [Créer une connexion à  [!DNL Adobe Workfront Fusion]  - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md).

Après avoir donné votre accord, vous faites l’objet d’une redirection vers la page d’administration de [!UICONTROL Workfront Fusion] où vous pouvez continuer l’élaboration de votre scénario.

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
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Microsoft Office 365 Email], vous devez disposer d’un compte [!DNL Microsoft Office 365 Email].



## Connexion du service [!DNL Office 365 Email] à [!DNL Workfront Fusion].

Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365 Email] à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] : instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations d’utilisateur ou d’utilisatrice. Ainsi, lors de la création d’une connexion, l’écran de consentement aux autorisations affiche les autorisations précédemment accordées à la connexion de cet utilisateur ou de cette utilisatrice, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur ou une utilisatrice dispose d’autorisations « Lire le tableau » accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les e-mails, l’écran de consentement aux autorisations affiche à la fois l’autorisation « Lire le tableau » déjà accordée et l’autorisation « Écrire des e-mails » nouvellement requise.

## Modules [!DNL Microsoft Office 365 Email] et leurs champs

Lorsque vous configurez les modules [!DNL Microsoft Office 365 Email], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Microsoft Office 365 Email] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez la section [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Message](#message)
* [Brouillon de message](#draft-message)
* [Pièce jointe](#attachment)
* [Autre](#other)

### Message

* [[!UICONTROL Créer et envoyer un message (hérité)]](#create-and-send-a-message)
* [[!UICONTROL Supprimer un message]](#delete-a-message)
* [[!UICONTROL Recevoir un message]](#get-a-message)
* [[!UICONTROL Déplacer un message]](#move-a-message)
* [[!UICONTROL Rechercher des messages]](#search-messages)
* [[!UICONTROL Surveiller les messages]](#watch-messages)



#### [!UICONTROL Créer et envoyer un message (hérité)]

Crée et envoie un e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez ou mappez l’objet du message.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Choisissez le format du corps du message : HTML ou texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Saisissez ou mappez le texte du corps de l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionnez l’importance de l’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Ajoutez l’adresse e-mail à laquelle vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires qui doivent recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires que vous souhaitez mettre en copie du message, dont l’adresse e-mail sera masquée des autres personnes destinataires :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Ajoutez les pièces jointes à l’e-mail :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou indiquez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>Ajouter les en-têtes du message.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisir le nom de l’en-tête</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez une valeur pour l’en-tête.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer et envoyer un message]

Crée et envoie un e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez ou mappez l’objet du message.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Choisissez le format du corps du message : HTML ou texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Saisissez ou mappez le texte du corps de l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionnez l’importance de l’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Ajoutez l’adresse e-mail à laquelle vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires qui doivent recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires que vous souhaitez mettre en copie du message, dont l’adresse e-mail sera masquée des autres personnes destinataires :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Ajoutez les pièces jointes à l’e-mail :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou indiquez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>Ajouter les en-têtes du message.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisir le nom de l’en-tête</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez une valeur pour l’en-tête.</p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un message]

Supprime un e-mail existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Sélectionnez ou mappez l’ID du message que vous souhaitez supprimer.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Recevoir un message]

Obtient les métadonnées d’un message spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Sélectionnez ou mappez l’ID du message pour lequel vous souhaitez récupérer les métadonnées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get MIME contents]</td> 
   <td>Activez cette option pour récupérer des données sur le contenu MIME du message. Le contenu [!UICONTROL MIME] peut comprendre des images, des fichiers audio et vidéo ou d’autres types de fichiers.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un message]

Déplace un e-mail vers un dossier sélectionné de la boîte de réception.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Sélectionnez ou mappez l’ID du message que vous souhaitez déplacer vers un autre dossier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder] </td> 
   <td> <p>Sélectionnez ou mappez l’ID du dossier dans lequel vous souhaitez déplacer le message.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des messages]

Permet de rechercher des messages sur la base de critères spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Sélectionnez le dossier qui contient les messages dans lesquels effectuer la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Saisissez votre requête de recherche. Pour plus d’informations sur la manière d’écrire une requête de recherche, voir l’article de support [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Rechercher des courriers et des personnes dans [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>Sélectionnez la façon dont vous souhaitez classer les résultats :</p> 
    <ul> 
     <li>[!UICONTROL Subject (Ascending or descending)]</li> 
     <li>[!UICONTROL Created Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Last Modified Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Received Date Time (Ascending or descending)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez le nombre maximum de messages que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les messages]

Se déclenche lors de la réception ou de l’envoi d’un e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Watch Messages]</p> </td> 
   <td> <p>Sélectionnez les messages que vous souhaitez surveiller :</p> 
    <ul> 
     <li>[!UICONTROL Only Unread]</li> 
     <li>[!UICONTROL Only read]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Sélectionnez le dossier qui contient les messages que vous voulez surveiller.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Saisissez votre requête de recherche. Pour plus d’informations sur la manière d’écrire une requête de recherche, voir l’article de support [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Rechercher des courriers et des personnes dans [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Saisissez le nombre maximum de messages que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Brouillon de message

* [Créer un brouillon de message](#create-a-draft-message)
* [Envoyer un brouillon de message](#send-a-draft-message)
* [Mettre à jour un message](#update-a-message)

#### [!UICONTROL Créer un brouillon de message]

Permet de créer un e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez l’objet du message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Choisissez le format du corps du message : HTML ou texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Saisissez le texte du corps du message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionnez l’importance de l’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires auxquelles vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires qui doivent recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>Nom</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>Adresse e-mail</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinataires Cci</p> </td> 
   <td> <p>Ajoutez les personnes destinataires que vous souhaitez mettre en copie du message, dont l’adresse e-mail sera masquée des autres personnes destinataires :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Ajoutez les pièces jointes à l’e-mail :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou indiquez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Envoyer un brouillon de message]

Envoie un brouillon d’e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Draft Message ID]</td> 
   <td> <p> Sélectionnez ou mappez l’ID de message du brouillon que vous souhaitez envoyer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un message]

Met à jour un message existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a message ID]</td> 
   <td> <p>Sélectionnez la manière dont vous souhaitez identifier le message à mettre à jour :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter Manually]</strong> </p> <p>Saisissez ou mappez l’ID du message.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Sélectionnez le dossier qui contient le message que vous souhaitez mettre à jour, puis sélectionnez le message.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez l’objet du message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Saisissez le texte du corps du message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionnez l’importance de l’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Ajoutez l’adresse e-mail à laquelle vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires qui doivent recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>Ajoutez les personnes destinataires que vous souhaitez mettre en copie du message, dont l’adresse e-mail sera masquée des autres personnes destinataires :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Saisissez l’adresse e-mail du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Ajoutez les pièces jointes à l’e-mail :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou indiquez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark it as Read]</td> 
   <td>Activez cette option pour marquer le message mis à jour comme lu.</td> 
  </tr> 
 </tbody> 
</table>

### Pièce jointe

* [[!UICONTROL Télécharger une pièce jointe]](#download-an-attachment)
* [[!UICONTROL Répertorier les pièces jointes]](#list-attachments)

#### [!UICONTROL Télécharger une pièce jointe]

Ce module télécharge la pièce jointe spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Sélectionnez ou mappez l’ID du message qui contient la pièce jointe que vous souhaitez télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment ID]</td> 
   <td> <p>Saisissez ou mappez l’ID de la pièce jointe que vous souhaitez télécharger.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier les pièces jointes]

Ce module permet de récupérer une liste de pièces jointes appartenant au message spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Sélectionnez ou mappez l’ID du message dont vous souhaitez récupérer les pièces jointes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum de pièces jointes que vous souhaitez que le module renvoie au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Ajouter une pièce jointe]](#add-an-attachment)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL Ajouter une pièce jointe]

Ce module permet d’ajouter une pièce jointe volumineuse à un message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Sélectionnez ou mappez l’ID du message auquel vous souhaitez ajouter une pièce jointe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour les instructions concernant la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à <code>https://graph.microsoft.com</code>. Exemple :<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
