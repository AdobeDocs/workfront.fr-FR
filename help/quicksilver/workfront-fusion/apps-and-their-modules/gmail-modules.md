---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Gmail
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Gmail et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 23%

---

# Modules [!DNL Gmail]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Gmail] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez la section [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Pour utiliser des modules [!DNL Gmail], vous devez disposer d’un compte [!DNL Gmail].

## Connecter [!DNL Gmail] à [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connectez-vous  [!DNL Gmail]  à  [!DNL Workfront Fusion] en utilisant [!DNL Google Workspace]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connectez-vous [!DNL Gmail]  à  [!DNL Workfront Fusion] en utilisant [!DNL gmail.com] ou [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connectez [!DNL Gmail] à [!DNL Workfront Fusion] en utilisant [!DNL  Google Workspace] {#connect-gmail-to-workfront-fusion-using-g-suite}

Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Workspace] à [!UICONTROL Workfront Fusion], reportez-vous à la section [Connexion de l’application ou du service Web du module à [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) dans l’article [Créer un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connectez [!DNL Gmail] à [!DNL Workfront Fusion] en utilisant [!DNL gmail.com] ou [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Si vous êtes un utilisateur [!DNL @gmail.com] ou [!DNL @googlemail.com], vous devez créer un client OAuth sur [le  [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) afin d&#39;obtenir un [!UICONTROL identifiant client] et un [!UICONTROL secret client].

Pour obtenir des instructions détaillées sur la création du client OAuth et l’obtention d’un [!UICONTROL identifiant client] et d’un [!UICONTROL secret client], voir [Connexion d’Adobe Workfront Fusion aux services Google à l’aide d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Modules [!DNL Gmail] et leurs champs

Lorsque vous configurez des modules [!DNL Gmail], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Gmail] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Itérateurs](#iterators)

### Déclencheurs

#### [!UICONTROL Regarder les emails]

Ce module de déclenchement exécute un scénario lorsqu’un nouvel email est reçu pour être traité.

Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier de courrier électronique à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type de filtre] </td> 
   <td> <p>Sélectionnez le type de filtre à utiliser pour regarder les emails.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtre simple]</strong> </p> <p>Renseignez les champs [!UICONTROL Critères], [!UICONTROL Adresse électronique de l’expéditeur], [!UICONTROL Objet] et [!UICONTROL Phrase de recherche].</p> </li> 
     <li> <p> <strong>[!UICONTROL Filtre Gmail]</strong> </p> <p>Dans le champ [!UICONTROL Requête] , saisissez la requête que vous souhaitez utiliser pour filtrer les emails.</p> <p>Pour plus d'informations sur les filtres [!DNL Gmail], voir <a href="https://support.google.com/mail/answer/7190">Opérateurs de recherche</a> dans la documentation [!DNL Gmail].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Critères]</td> 
   <td>Choisissez si vous souhaitez consulter [!UICONTROL tout email], [!UICONTROL uniquement lire les emails] ou [!UICONTROL uniquement lire les emails non lus].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Adresse électronique de l’expéditeur]</td> 
   <td> <p> Saisissez une adresse email pour ne regarder que les emails envoyés à partir de cette adresse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Entrez une chaîne de texte pour n’afficher que les emails dont l’objet contient cette chaîne de texte.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Expression de recherche]</td> 
   <td>Entrez une chaîne de texte pour afficher uniquement les courriers électroniques qui contiennent cette chaîne de texte n’importe où dans l’email.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Marquer le ou les emails comme lus lors de la récupération]</td> 
   <td> <p> Activez cette option pour marquer les emails récupérés comme lus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de résultats]</td> 
   <td> <p> Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Envoyer un email]](#send-an-email)
* [[!UICONTROL Créer un brouillon]](#create-a-draft)
* [[!UICONTROL Marquer un email comme lu]](#mark-an-email-as-read)
* [[!UICONTROL Marquer un email comme non lu]](#mark-an-email-as-unread)
* [[!UICONTROL Déplacer un email]](#move-an-email)
* [[!UICONTROL Copier un email]](#copy-an-email)
* [[!UICONTROL Supprimer un email]](#delete-an-email)
* [[!UICONTROL  Modifier les étiquettes des emails ]](#modify-email-labels)

#### [!UICONTROL Envoyer un email]

Ce module d’action envoie un nouvel email.

Vous indiquez le destinataire de l’email.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL From]</td> 
   <td> <p>Saisissez ou mappez une adresse email de l'expéditeur.</p> <p>Remarque : si vous saisissez une adresse électronique incorrecte, une erreur peut se produire lors de l’envoi d’un message, car votre compte peut ne pas être autorisé à envoyer des emails à partir d’une adresse différente de la vôtre.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL À] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse électronique de chaque destinataire.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Saisissez ou mappez l’objet du courrier électronique.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Saisissez ou mappez le contenu de l'email (corps du message). Les balises d’HTML sont autorisées.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pièces jointes] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong> pour ajouter une pièce jointe. Vous pouvez mapper un fichier à partir des modules précédents.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copier les destinataires]</td> 
   <td> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse électronique de chaque destinataire de copie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinataires d’une copie aveugle]</td> 
   <td> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse électronique de chaque destinataire de copie aveugle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un brouillon]

Ce module d’action crée un brouillon de courrier électronique et l’ajoute à un dossier que vous spécifiez.

Vous spécifiez le dossier dans lequel vous souhaitez créer un brouillon.

Le module renvoie l’identifiant du brouillon d’email et les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier [!DNL Gmail] dans lequel vous souhaitez créer un brouillon.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL À] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse électronique de chaque destinataire.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Saisissez ou mappez l’objet du courrier électronique.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Saisissez ou mappez le contenu de l'email (corps du message). Les balises d’HTML sont autorisées.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pièces jointes] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong> pour ajouter une pièce jointe. Vous pouvez mapper un fichier à partir des modules précédents.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copier les destinataires]</td> 
   <td> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse électronique de chaque destinataire de copie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinataires d’une copie aveugle]</td> 
   <td> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse électronique de chaque destinataire de copie aveugle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marquer un email comme lu]

Ce module d’action marque un email comme lu.

Vous indiquez l&#39;identifiant de l&#39;email et de son dossier.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier [!DNL Gmail] contenant l'email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID d’adresse électronique (UID)]</td> 
   <td> <p> Saisissez ou mappez l’ID de courrier électronique.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marquer un email comme non lu]

Ce module d’action marque un courrier électronique ou un brouillon de courrier électronique comme non lu.

Vous indiquez l&#39;identifiant de l&#39;email et de son dossier.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier [!DNL Gmail] contenant l'email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID d’adresse électronique (UID)] </td> 
   <td> <p>Saisissez ou mappez l’ID d’email que vous souhaitez marquer comme non lu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un email]

Ce module d’action déplace un courrier électronique ou un brouillon de courrier électronique vers un dossier que vous spécifiez.

Vous indiquez le dossier, le dossier de destination et l’identifiant de l’email.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier source [!DNL Gmail] contenant l'email que vous souhaitez déplacer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dossier de destination]</td> 
   <td> <p> Sélectionnez le dossier cible vers lequel vous souhaitez déplacer l'email.[!DNL Gmail]</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID d’adresse électronique (UID)]</td> 
   <td> <p> Saisissez ou mappez l’ID de l’email que vous souhaitez déplacer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier un email]

Ce module d’action copie un courrier électronique ou un brouillon de courrier électronique dans un dossier que vous spécifiez.

Vous indiquez le dossier, le dossier de destination et l’identifiant de l’email.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier source [!DNL Gmail] contenant l'email que vous souhaitez copier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dossier de destination]</td> 
   <td> <p>Sélectionnez le dossier cible dans lequel vous souhaitez copier l’email.[!DNL Gmail]</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID d’adresse électronique (UID)]</td> 
   <td> <p>Saisissez ou mappez l’ID de l’email que vous souhaitez copier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un email]

Ce module d’action supprime un courrier électronique ou un brouillon de courrier électronique d’un dossier que vous spécifiez.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID de message]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID de l’email que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanemment] </td> 
   <td> <p>Activez cette option pour permettre au module de supprimer définitivement l’email, au lieu de le déplacer vers le dossier de la corbeille.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL  Modifier les étiquettes des emails ]

Ce module d&#39;action modifie le libellé d&#39;un email que vous spécifiez.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Gmail] à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID de message]</td> 
   <td> <p> Saisissez ou mappez l’ID de l’email que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Étiquettes à ajouter]</p> </td> 
   <td> <p>Sélectionnez ou mappez le libellé à ajouter au message électronique sélectionné.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Étiquettes à supprimer]</td> 
   <td> <p> Sélectionnez ou mappez le libellé à supprimer du message électronique sélectionné.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Étiquette à ajouter] et [!UICONTROL Étiquette à supprimer] pour charger uniquement les étiquettes créées par l’utilisateur.

### Itérateurs

#### [!UICONTROL Itérer les pièces jointes]

Vous pouvez itérer les pièces jointes aux emails. Chaque pièce jointe est un lot distinct dans la sortie du module. Pour plus d’informations, voir [Module d’itérateur dans Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Module [!UICONTROL Source] </td> 
   <td> <p>Sélectionnez le module à partir duquel vous souhaitez itérer les pièces jointes. </p> </td> 
  </tr> 
 </tbody> 
</table>
