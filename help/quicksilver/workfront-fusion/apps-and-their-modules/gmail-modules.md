---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Gmail
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Gmail et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

# [!DNL Gmail] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Gmail], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Gmail] modules, vous devez disposer d’un [!DNL Gmail] compte .

## Connexion [!DNL Gmail] to [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connexion [!DNL Gmail] to [!DNL Workfront Fusion] Utilisation de [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connexion [!DNL Gmail] to [!DNL Workfront Fusion] using [!DNL gmail.com] ou [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connexion [!DNL Gmail] to [!DNL Workfront Fusion] using[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Pour obtenir des instructions sur la connexion à [!DNL G Suite] compte à [!UICONTROL Workfront Fusion], voir [Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) dans l’article [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connexion [!DNL Gmail] to [!DNL Workfront Fusion] using [!DNL gmail.com] ou [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Si vous êtes [!DNL @gmail.com] ou [!DNL @googlemail.com] vous devez créer un client OAuth sur [la valeur [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) pour obtenir un [!UICONTROL ID client] et [!UICONTROL Secret du client].

Pour obtenir des instructions détaillées sur la création du client OAuth et l’obtention d’un [!UICONTROL ID client] et [!UICONTROL Secret du client], voir [Connexion d’Adobe Workfront Fusion aux services Google à l’aide d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] modules et leurs champs

Lorsque vous configurez [!DNL Gmail] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Gmail] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Itérateurs](#iterators)

### Triggers

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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
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
     <li> <p> <strong>[!UICONTROL Filtre Gmail]</strong> </p> <p>Dans le champ [!UICONTROL Requête] , saisissez la requête que vous souhaitez utiliser pour filtrer les emails.</p> <p>Pour plus d’informations sur [!DNL Gmail] filtres, voir <a href="https://support.google.com/mail/answer/7190">Opérateurs de recherche</a> dans le [!DNL Gmail] documentation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Critères]</td> 
   <td>Choisissez si vous souhaitez consulter [!UICONTROL tout email], [!UICONTROL uniquement lire les emails] ou [!UICONTROL uniquement lire les emails non lus].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Adresse électronique de l’expéditeur]</td> 
   <td> <p> Saisissez une adresse email pour ne regarder que les emails envoyés depuis cette adresse.</p> </td> 
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
   <td> <p> Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Envoyer un email]](#send-an-email)
* [[!UICONTROL Création d’un brouillon]](#create-a-draft)
* [[!UICONTROL Marquer un email comme lu]](#mark-an-email-as-read)
* [[!UICONTROL Marquer un email comme non lu]](#mark-an-email-as-unread)
* [[!UICONTROL Déplacer un email]](#move-an-email)
* [[!UICONTROL Copier un email]](#copy-an-email)
* [[!UICONTROL Supprimer un email]](#delete-an-email)
* [[!UICONTROL Modification des libellés d’email]](#modify-email-labels)

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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL From]</td> 
   <td> <p>Saisissez ou mappez une adresse email de l'expéditeur.</p> <p>Remarque : Si vous saisissez une adresse email incorrecte, une erreur peut se produire lors de l’envoi d’un message, car votre compte peut ne pas être autorisé à envoyer des emails depuis une adresse différente de la vôtre.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL À] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l'adresse email de chaque destinataire.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Saisissez ou mappez l’objet du courrier électronique.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Saisissez ou mappez le contenu de l'email (corps du message). Les balises de HTML sont autorisées.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pièces jointes] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong> pour ajouter une pièce jointe. Vous pouvez mapper un fichier à partir des modules précédents.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copier les destinataires]</td> 
   <td> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse email de chaque destinataire de copie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinataires d’une copie aveugle]</td> 
   <td> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse électronique de chaque destinataire de copie aveugle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un brouillon]

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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez la [!DNL Gmail] dans lequel vous souhaitez créer un brouillon.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL À] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l'adresse email de chaque destinataire.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Saisissez ou mappez l’objet du courrier électronique.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Saisissez ou mappez le contenu de l'email (corps du message). Les balises de HTML sont autorisées.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pièces jointes] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong> pour ajouter une pièce jointe. Vous pouvez mapper un fichier à partir des modules précédents.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copier les destinataires]</td> 
   <td> <p> Cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez ou mappez l’adresse email de chaque destinataire de copie.</p> </td> 
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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez la [!DNL Gmail] qui contient l’email.</p> </td> 
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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez la [!DNL Gmail] qui contient l’email.</p> </td> 
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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez la [!DNL Gmail] dossier source contenant l’adresse électronique à déplacer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dossier de destination]</td> 
   <td> <p> Sélectionnez la [!DNL Gmail] dossier cible vers lequel vous souhaitez déplacer l’email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID d’adresse électronique (UID)]</td> 
   <td> <p> Saisissez ou mappez l’ID d’adresse électronique de l’adresse électronique que vous souhaitez déplacer.</p> </td> 
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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez la [!DNL Gmail] dossier source contenant l’email que vous souhaitez copier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dossier de destination]</td> 
   <td> <p>Sélectionnez la [!DNL Gmail] dossier cible vers lequel vous souhaitez copier l’email.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID d’adresse électronique (UID)]</td> 
   <td> <p>Saisissez ou mappez l’ID d’adresse électronique de l’adresse électronique que vous souhaitez copier.</p> </td> 
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
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID de message]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID d’adresse électronique de l’adresse électronique que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanemment] </td> 
   <td> <p>Activez cette option pour permettre au module de supprimer définitivement l’email au lieu de le déplacer vers le dossier de la corbeille.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modification des libellés d’email]

Ce module d&#39;action modifie le libellé d&#39;un email que vous spécifiez.

Le module renvoie l’identifiant de l’email et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion à [!DNL Gmail] compte à [!DNL Workfront Fusion], voir <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Gmail] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID de message]</td> 
   <td> <p> Saisissez ou mappez l’ID d’adresse électronique de l’adresse électronique que vous souhaitez supprimer.</p> </td> 
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
>[!UICONTROL Étiquette à ajouter] et [!UICONTROL Libellé à supprimer] ne chargent que les libellés créés par l’utilisateur.

### Itérateurs

#### [!UICONTROL Itérer les pièces jointes]

Vous pouvez itérer les pièces jointes aux emails. Chaque pièce jointe est un lot distinct dans la sortie du module. Pour plus d’informations, voir [Module d’itérateur dans Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Module source] </td> 
   <td> <p>Sélectionnez le module à partir duquel vous souhaitez itérer les pièces jointes. </p> </td> 
  </tr> 
 </tbody> 
</table>
