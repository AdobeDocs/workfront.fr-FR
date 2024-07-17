---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Marketo
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Marketo] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2068'
ht-degree: 30%

---

# Modules [!DNL Marketo]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Marketo] et les connecter à plusieurs applications et services tiers.

Pour une vidéo d’introduction au connecteur Marketo, voir :

* [Marketo](https://video.tv.adobe.com/v/3427026/){target=_blank}

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

Pour utiliser des modules [!DNL Marketo], vous devez disposer d’un compte [!DNL Marketo].

## Connexion de [!DNL Marketo] à Workfront Fusion {#connect-marketo-to-workfront-fusion}

Vous pouvez créer une connexion à votre compte [!DNL Marketo] directement depuis le module [!DNL Marketo].

1. Dans un module [!DNL Marketo], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Saisissez votre compte [!DNL Marketo] ou l&#39;ID [!DNL Marketo] [!UICONTROL Munchkin]. Il s’agit de la partie unique de l’URL de base ou du point de terminaison affecté à votre compte, que vous utilisez pour accéder à [!DNL Marketo] via son API [!UICONTROL REST]. Pour plus d’informations sur la localisation de ce problème, voir [URL de base](https://developers.marketo.com/rest-api/base-url/) dans la documentation [!DNL Marketo].
1. Saisissez votre [!UICONTROL ID client] et votre [!UICONTROL Secret client]. Pour obtenir des instructions sur la localisation de ces fichiers, voir [Authentification](https://developers.marketo.com/rest-api/authentication/) dans la documentation [!DNL Marketo].
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## [!DNL Marketo] Modules et leurs champs

Lorsque vous configurez des modules [!DNL Marketo], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Marketo] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

* [[!UICONTROL Surveiller les enregistrements]](#watch-records)
* [[!UICONTROL Surveiller les événements (instantanés)]](#watch-events-instant)

#### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement lance un scénario lorsqu’un enregistrement est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Activité]</strong> </p> <p>Sélectionnez le type d’activité que vous souhaitez voir. </p> <p>Le module n’observe que les nouvelles activités.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Indiquez si vous souhaitez rechercher de nouveaux enregistrements, des enregistrements mis à jour, des enregistrements nouveaux et mis à jour ou des mises à jour de champs spécifiques. Si vous choisissez de regarder les mises à jour de champs spécifiques, sélectionnez le champ que le module doit surveiller.</p> </li> 
     <li> <p><strong>[!UICONTROL Program]</strong> </p> <p>Indiquez si vous souhaitez rechercher de nouveaux enregistrements, des enregistrements mis à jour ou des enregistrements nouveaux et mis à jour.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les événements (instantanés)]

Ce module de déclenchement lance un scénario lorsqu’un enregistrement est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Saisissez le webhook que le module doit utiliser.</p> <p>Pour plus d’informations sur les webhooks, voir <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant Triggers (webhooks) dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Télécharger un fichier]](#download-a-file)
* [[!UICONTROL Charger un fichier]](#upload-a-file)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Ajouter des pistes à une liste]](#add-leads-to-a-list)
* [[!UICONTROL Supprimer des pistes d’une liste]](#remove-leads-from-a-list)
* [[!UICONTROL Planifier une campagne]](#schedule-a-campaign)
* [[!UICONTROL Copier un programme]](#copy-a-program)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Marketo]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit utiliser au cours de chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un nouvel enregistrement dans [!DNL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Folder]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
   <td>Si vous créez une société ou un prospect, sélectionnez les champs pour lesquels vous souhaitez définir des valeurs lors de la création du nouvel enregistrement, puis saisissez des valeurs pour ces champs.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de programme]</td> 
   <td>Si vous créez un programme, sélectionnez le type de programme que vous souhaitez créer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Canal de programme] </td> 
   <td>Si vous créez un programme, sélectionnez le canal du programme dans lequel vous souhaitez créer le programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Program Name]</td> 
   <td>Si vous créez un dossier ou un programme, saisissez ou mappez un nom pour le nouvel enregistrement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>Si vous créez un dossier ou un programme, saisissez ou mappez une description pour le nouvel enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID]</td> 
   <td>Si vous créez un dossier ou un programme, saisissez ou mappez l’identifiant du dossier parent dans lequel vous souhaitez créer le nouvel enregistrement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Coûts]</td> 
   <td>Si vous créez un programme, ajoutez des coûts.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Si vous créez un programme, ajoutez des balises.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un enregistrement existant à l’aide de son identifiant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entreprise] / [!UICONTROL Piste] / [!UICONTROL ID de programme]</td> 
   <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
   <td>Si vous mettez à jour une société ou un prospect, sélectionnez les champs pour lesquels vous souhaitez mettre à jour les valeurs, puis saisissez les valeurs de ces champs.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Name]</td> 
   <td>Si vous mettez à jour un programme, saisissez ou mappez un nouveau nom pour le programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>Si vous mettez à jour un programme, saisissez ou mappez une nouvelle description du programme.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date de début]</td> 
   <td>Si vous mettez à jour un programme, saisissez ou mappez une nouvelle date de début pour le programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date de fin]</td> 
   <td>Si vous mettez à jour un programme, saisissez ou mappez une nouvelle date de fin pour le programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Coûts]</td> 
   <td>Si vous mettez à jour un programme, ajoutez des frais.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Si vous mettez à jour un programme, ajoutez des balises.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un fichier]

Ce module d’action télécharge un fichier à l’aide de l’identifiant de fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de fichier]</td> 
   <td>Mappez l’identifiant du fichier que vous souhaitez télécharger.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Charger un fichier]

Ce module d’action télécharge un nouveau fichier vers [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier]</td> 
   <td>Saisissez ou mappez l’identifiant du dossier dans lequel vous souhaitez que le nouveau fichier soit situé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez une description pour le fichier téléchargé.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit des informations sur un enregistrement à l’aide de son identifiant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL List]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module. Les champs sont disponibles en fonction du [!UICONTROL Type d’enregistrement] que vous avez sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Object&gt; ID]</td> 
   <td>Saisissez ou mappez l’identifiant de l’objet dont vous souhaitez récupérer les informations.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter des pistes à une liste]

Ce module d’action ajoute une ou plusieurs pistes à une liste, à l’aide de l’identifiant de piste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la liste dans laquelle vous souhaitez ajouter des pistes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de piste]</td> 
   <td> <p>Pour chaque piste à ajouter à la liste, cliquez sur <b>[!UICONTROL Ajouter]</b>, puis saisissez ou mappez l’identifiant de la piste à ajouter. Vous pouvez ajouter jusqu’à 300 pistes pour que le module soit ajouté à la liste.</p> <p>Cliquez sur le bouton d’activation/désactivation de la carte pour mapper une collection existante de pistes que vous souhaitez ajouter à la liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer des pistes d’une liste]

Ce module d’action supprime une ou plusieurs pistes d’une liste à l’aide de l’identifiant de piste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la liste dans laquelle vous souhaitez supprimer des pistes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de piste]</td> 
   <td> <p>Pour chaque piste à supprimer de la liste, cliquez sur <b>[!UICONTROL Ajouter]</b>, puis saisissez ou mappez l’identifiant de la piste à supprimer. Vous pouvez ajouter jusqu’à 300 pistes pour que le module soit supprimé de la liste. </p> <p>Cliquez sur le bouton bascule de la carte pour mapper une collection de pistes existante à supprimer de la liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Planifier une campagne]

Ce module d’action planifie une opération existante pour une certaine date.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de campagne]</td> 
   <td>Saisissez ou mappez l'identifiant de la campagne que vous souhaitez programmer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Planification de la date]</p> </td> 
   <td>Sélectionnez la date d'exécution de la campagne. Si ce champ n’est pas renseigné, la campagne s’exécute cinq minutes après le début du scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier un programme]

Ce module d’action effectue une copie d’un programme à l’aide de l’identifiant du programme existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de programme existant]</td> 
   <td>Saisissez ou mappez l’identifiant du programme que vous souhaitez copier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nouveau nom du programme]</p> </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouveau programme.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier]</td> 
   <td>Saisissez ou mappez l’identifiant du dossier dans lequel vous souhaitez que le nouveau programme soit situé.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Répertorier les enregistrements]](#list-records)
* [[!UICONTROL Enregistrements de recherche]](#update-a-record)

#### [!UICONTROL Répertorier les enregistrements]

Ce module d’action récupère tous les enregistrements d’un type spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez répertorier.</p> 
    <ul> 
     <li> <p>[!UICONTROL Lire toutes les campagnes]</p> </li> 
     <li> <p>[!UICONTROL Lire tous les programmes]</p> </li> 
     <li> <p>[!UICONTROL Lire toutes les pistes] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>Si vous avez choisi de récupérer des pistes, choisissez si vous souhaitez récupérer des pistes à partir d’une liste ou d’un programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module. Les champs sont disponibles en fonction du [!UICONTROL Type d’enregistrement] que vous avez sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enregistrements de recherche]

Ce module de recherche récupère une liste d’enregistrements correspondant à des critères de recherche spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Sélectionnez le type d’enregistrement à rechercher.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campagnes]</p> </li> 
     <li> <p>[!UICONTROL Leads]</p> </li> 
     <li> <p>[!UICONTROL Programmes]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Field]</p> </td> 
   <td> <p>Indiquez si vous souhaitez effectuer une recherche par nom, nom du programme ou nom de l’espace de travail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td>Pour chaque valeur à rechercher, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez la valeur.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>
