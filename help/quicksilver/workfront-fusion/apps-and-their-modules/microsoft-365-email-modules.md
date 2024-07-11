---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: E-mail Microsoft Office 365
description: Dans un [!DNL Adobe Workfront Fusion] vous pouvez automatiser les workflows qui utilisent Microsoft Office 365 Email, et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: a09116572d4f9101740fa976f1d334e99fac3010
workflow-type: tm+mt
source-wordcount: '2699'
ht-degree: 13%

---

# Modules [!DNL Microsoft Office 365 Email]

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!UICONTROL Microsoft Office 365 Email], ainsi que de la connecter à plusieurs applications et services tiers.

Pour utiliser [!UICONTROL Office 365 Email] avec [!DNL Adobe Workfront Fusion], une [!UICONTROL Compte Office 365]. Vous pouvez en créer un à l’adresse www.office.com.

Pour obtenir des instructions sur la connexion à [!UICONTROL Office 365] compte à [!DNL Workfront Fusion], voir [Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

Une fois le consentement accordé, vous êtes redirigé vers le [!UICONTROL Workfront Fusion] page d’administration où vous pouvez continuer à créer votre scénario.

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

Pour utiliser des modules [!DNL Microsoft Office 365 Email], vous devez disposer d’un compte [!DNL Microsoft Office 365 Email].



## Connexion de la variable [!DNL Office 365 Email] service à [!DNL Workfront Fusion]

Pour obtenir des instructions sur la connexion à [!DNL Office 365 Email] compte à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations utilisateur individuelles. Par conséquent, lors de la création d’une connexion, l’écran de consentement des autorisations affiche les autorisations qui ont été accordées à la connexion de cet utilisateur, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur dispose d’autorisations &quot;Lecture de tableau&quot; accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les emails, l’écran de consentement des autorisations affiche à la fois l’autorisation &quot;Lecture de tableau&quot; déjà accordée et l’autorisation &quot;Ecriture d’email&quot; nouvellement requise.

## Modules [!DNL Microsoft Office 365 Email] et leurs champs

Lorsque vous configurez des modules [!DNL Microsoft Office 365 Email], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Microsoft Office 365 Email] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Message](#message)
* [Brouillon du message](#draft-message)
* [Pièce jointe](#attachment)
* [Autre](#other)

### Message

* [[!UICONTROL Création et envoi d’un message (hérité)]](#create-and-send-a-message)
* [[!UICONTROL Suppression d’un message]](#delete-a-message)
* [[!UICONTROL Obtention d’un message]](#get-a-message)
* [[!UICONTROL Déplacer un message]](#move-a-message)
* [[!UICONTROL Messages de recherche]](#search-messages)
* [[!UICONTROL Regarder les messages]](#watch-messages)



#### [!UICONTROL Création et envoi d’un message (hérité)]

Crée et envoie un message électronique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez ou mappez l’objet du message.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Indiquez si le contenu du corps du message est HTML ou Texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du corps]</td> 
   <td> <p>Saisissez ou mappez le texte du corps du message de l'email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionner l'importance de l'email</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aux Destinataires]</p> </td> 
   <td> <p>Ajoutez l'adresse email à laquelle vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinataires CC]</p> </td> 
   <td> <p>Ajoutez les destinataires que vous souhaitez recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinataires Cci]</p> </td> 
   <td> <p>Ajoutez les destinataires que vous souhaitez copier dans le message, sans permettre à d'autres destinataires de voir leurs noms ou adresses email :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajoutez les pièces jointes au courrier électronique :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom du fichier]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou mappez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL En-têtes de message Internet]</td> 
   <td> <p>Ajoutez les en-têtes de message pour l’email.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom de l’en-tête.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez une valeur pour l’en-tête .</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création et envoi d’un message]

Crée et envoie un message électronique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez ou mappez l’objet du message.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Indiquez si le contenu du corps du message est HTML ou Texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du corps]</td> 
   <td> <p>Saisissez ou mappez le texte du corps du message de l'email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionner l'importance de l'email</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aux Destinataires]</p> </td> 
   <td> <p>Ajoutez l'adresse email à laquelle vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinataires CC]</p> </td> 
   <td> <p>Ajoutez les destinataires que vous souhaitez recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinataires Cci]</p> </td> 
   <td> <p>Ajoutez les destinataires que vous souhaitez copier dans le message, sans permettre à d'autres destinataires de voir leurs noms ou adresses email :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajoutez les pièces jointes au courrier électronique :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom du fichier]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou mappez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL En-têtes de message Internet]</td> 
   <td> <p>Ajoutez les en-têtes de message pour l’email.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom de l’en-tête.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez une valeur pour l’en-tête .</p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un message]

Supprime un message électronique existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID de message]</td> 
   <td> <p> Sélectionnez ou mappez l’identifiant du message que vous souhaitez supprimer.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un message]

Obtient les métadonnées d’un message spécifique

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de message]</td> 
   <td> <p> Sélectionnez ou mappez l’identifiant du message pour lequel vous souhaitez récupérer des métadonnées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtention du contenu MIME]</td> 
   <td>Activez cette option pour récupérer les données sur le contenu MIME du message. Le contenu [!UICONTROL MIME] peut inclure des images, du contenu audio, vidéo ou d’autres types de fichiers.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un message]

Déplace un message électronique vers un dossier sélectionné de la boîte aux lettres.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de message]</td> 
   <td> <p> Sélectionnez ou mappez l’identifiant du message que vous souhaitez déplacer vers un autre dossier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder] </td> 
   <td> <p>Sélectionnez ou mappez l’identifiant du dossier dans lequel vous souhaitez déplacer le message.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Messages de recherche]

Recherche des messages selon des critères spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Sélectionnez le dossier contenant les messages à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Entrez votre requête de recherche. Pour plus d’informations sur l’écriture d’une requête de recherche, voir [!DNL Microsoft] article du support <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Recherche dans les courriers électroniques et les personnes dans [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordre par]</td> 
   <td> <p>Sélectionnez le mode de commande des résultats :</p> 
    <ul> 
     <li>[!UICONTROL Objet (ascendant ou descendant)]</li> 
     <li>[!UICONTROL Heure de la date de création (ascendante ou descendante)]</li> 
     <li>[!UICONTROL Dernière heure de modification (ascendante ou descendante)]</li> 
     <li>[!UICONTROL Heure de la date de réception (ascendante ou descendante)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Entrer le nombre maximum de messages [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder les messages]

Déclenche lorsqu’un nouveau message électronique est envoyé ou reçu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Messages De Contrôle]</p> </td> 
   <td> <p>Sélectionnez les messages à regarder :</p> 
    <ul> 
     <li>[!UICONTROL Seulement Non Lu]</li> 
     <li>[!UICONTROL Lecture seule]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Sélectionnez le dossier contenant les messages que vous souhaitez voir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Entrez votre requête de recherche. Pour plus d’informations sur l’écriture d’une requête de recherche, voir [!DNL Microsoft] article du support <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Recherche dans les courriers électroniques et les personnes dans [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Entrer le nombre maximum de messages [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Brouillon du message

* [Création d’un brouillon de message](#create-a-draft-message)
* [Envoyer un brouillon de message](#send-a-draft-message)
* [Mettre à jour un message](#update-a-message)

#### [!UICONTROL Création d’un brouillon de message]

Crée un message électronique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez l’objet du message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Indiquez si le contenu du corps du message est HTML ou Texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du corps]</td> 
   <td> <p>Entrez le texte du corps du message de l’email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionner l'importance de l'email</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aux Destinataires]</p> </td> 
   <td> <p>Ajoutez les destinataires auxquels vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinataires CC]</p> </td> 
   <td> <p>Ajoutez les destinataires. Vous souhaitez recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>Nom</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>Adresse électronique</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinataires Cci</p> </td> 
   <td> <p>Ajoutez les destinataires que vous souhaitez copier dans le message, sans permettre à d'autres destinataires de voir leurs noms ou adresses email :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajoutez les pièces jointes au courrier électronique :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom du fichier]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou mappez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Envoyer un brouillon de message]

Envoie un message électronique qui est actuellement en version préliminaire.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saisissez un ID de message]</td> 
   <td> <p>Sélectionnez le mode d'identification du message à mettre à jour :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée Manuelle]</strong> </p> <p>Saisissez ou mappez l’identifiant du message.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le dossier contenant le message à mettre à jour, puis sélectionnez le message.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez l’objet du message.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du corps]</td> 
   <td> <p>Entrez le texte du corps du message de l’email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionner l'importance de l'email</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aux Destinataires]</p> </td> 
   <td> <p>Ajoutez l'adresse email à laquelle vous souhaitez envoyer les messages :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinataires CC]</p> </td> 
   <td> <p>Ajoutez les destinataires. Vous souhaitez recevoir une copie du message :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinataires Cci]</p> </td> 
   <td> <p>Ajoutez les destinataires que vous souhaitez copier dans le message, sans permettre à d'autres destinataires de voir leurs noms ou adresses email :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du contact.</p> </li> 
     <li> <p><strong>[!UICONTROL Adresse électronique]</strong> </p> <p>Saisissez l'adresse email du contact.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pièces jointes]</p> </td> 
   <td> <p>Ajoutez les pièces jointes au courrier électronique :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom du fichier]</strong> </p> <p>Saisissez le nom du fichier. Exemple : <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Saisissez les données du fichier dans le champ ou mappez la source du fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marquer comme lu]</td> 
   <td>Activez cette option pour marquer le message mis à jour comme lu.</td> 
  </tr> 
 </tbody> 
</table>

### Pièce jointe

* [[!UICONTROL Téléchargement d’une pièce jointe]](#download-an-attachment)
* [[!UICONTROL Lister des pièces jointes]](#list-attachments)

#### [!UICONTROL Téléchargement d’une pièce jointe]

Ce module télécharge la pièce jointe spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID de message]</td> 
   <td> <p> Sélectionnez ou mappez l’identifiant du message qui contient la pièce jointe que vous souhaitez télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de pièce jointe]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la pièce jointe à télécharger.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister des pièces jointes]

Ce module récupère une liste de pièces jointes appartenant au message spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de message]</td> 
   <td> <p> Sélectionnez ou mappez l’identifiant du message à partir duquel vous souhaitez récupérer les pièces jointes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de pièces jointes que le module doit renvoyer lors de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Ajout d’une pièce jointe]](#add-an-attachment)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL Ajout d’une pièce jointe]

Ce module ajoute un grand attachement à un message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À partir de l’adresse électronique]</td> 
   <td> <p> Pour utiliser une adresse email partagée, saisissez l'adresse ici. L’utilisateur dont les informations d’identification sont utilisées dans la connexion utilisée pour ce module doit avoir accès au dossier partagé.<p>Laissez ce champ vide pour utiliser l’adresse électronique du propriétaire de la connexion.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de message]</td> 
   <td> <p> Sélectionnez ou mappez l’identifiant du message auquel vous souhaitez ajouter une pièce jointe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
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
