---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Marketo
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2136'
ht-degree: 94%

---

# Modules [!DNL Marketo]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules Marketo](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-marketo-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Marketo] et le connecter à plusieurs applications et services tiers.

Pour une vidéo d’introduction au connecteur Marketo, voir :

* [Marketo](https://video.tv.adobe.com/v/3427026/){target=_blank}

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Marketo], vous devez disposer d’un compte [!DNL Marketo].

## Informations sur l’API Marketo

Le connecteur Marketo utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.14.19</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!DNL Marketo] à Workfront Fusion {#connect-marketo-to-workfront-fusion}

Vous pouvez créer une connexion à votre compte [!DNL Marketo] directement depuis le module [!DNL Marketo].

1. Dans n’importe quel module [!DNL Marketo], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Saisissez votre ID de compte [!DNL Marketo] ou votre ID [!DNL Marketo] [!UICONTROL Munchkin]. Il s’agit de la partie unique de l’URL de base ou du point d’entrée affecté à votre compte, que vous utilisez pour accéder à [!DNL Marketo] via son API [!UICONTROL REST]. Pour plus d’informations sur sa localisation, voir [URL de base](https://developers.marketo.com/rest-api/base-url/) dans la documentation [!DNL Marketo].
1. Saisissez votre [!UICONTROL ID client ou cliente] et [!UICONTROL secret client ou cliente]. Pour obtenir des instructions sur la localisation de ces éléments, voir [Authentification](https://developers.marketo.com/rest-api/authentication/) dans la documentation [!DNL Marketo].
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenez au module.

## Modules [!DNL Marketo] et leurs champs

Lorsque vous configurez les modules [!DNL Marketo], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Marketo] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

* [[!UICONTROL Regarder des événements (instantané)]](#watch-events-instant)
* [[!UICONTROL Surveiller les enregistrements]](#watch-records)

#### [!UICONTROL Regarder des événements (instantané)]

Ce module de déclenchement lance un scénario lorsqu’un enregistrement est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Saisissez le webhook que le module doit utiliser.</p> <p>Pour plus d’informations sur les webhooks, voir <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder des enregistrements]

Ce module de déclenchement lance un scénario lorsqu’un enregistrement est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Activity]</strong> </p> <p>Sélectionnez le type d’activité que vous souhaitez regarder. </p> <p>Le module ne recherche que les nouvelles activités.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Sélectionnez si vous souhaitez regarder les nouveaux enregistrements, les enregistrements mis à jour, les deux ou les mises à jour de champs spécifiques. Si vous choisissez de regarder les mises à jour de champs spécifiques, sélectionnez le champ que le module doit rechercher.</p> </li> 
     <li> <p><strong>[!UICONTROL Program]</strong> </p> <p>Sélectionnez si vous souhaitez regarder les nouveaux enregistrements, les enregistrements mis à jour ou les deux.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Ajouter des leads à une liste]](#add-leads-to-a-list)
* [[!UICONTROL Cloner un programme]](#clone-a-program)
* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Télécharger un fichier]](#download-a-file)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Supprimer des leads d’une liste]](#remove-leads-from-a-list)
* [[!UICONTROL Planifier une campagne]](#schedule-a-campaign)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Charger un fichier]](#upload-a-file)

#### [!UICONTROL Ajouter des leads à une liste]

Ce module d’action ajoute un ou plusieurs leads à une liste, à l’aide de leur identifiant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la liste dans laquelle vous souhaitez ajouter des leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>Pour chaque lead à ajouter à la liste, cliquez sur <b>[!UICONTROL Add]</b>, puis saisissez ou mappez l’ID du lead à ajouter. Vous pouvez ajouter jusqu’à 300 leads pour que le module les ajoute à la liste.</p> <p>Cliquez sur le bouton Mapper pour mapper une collection existante de leads que vous souhaitez ajouter à la liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cloner un programme]

Ce module d’action effectue une copie d’un programme à l’aide de l’ID du programme existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Existing Program ID]</td> 
   <td>Saisissez ou mappez l’ID du programme que vous souhaitez copier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL New Program Name]</p> </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouveau programme.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Saisissez ou mappez l’ID du dossier dans lequel vous souhaitez que le nouveau programme soit situé.</td> 
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
   <td> <p>Pour savoir comment connecter votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
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
   <td>Si vous créez une entreprise ou un lead, sélectionnez les champs pour lesquels vous souhaitez définir des valeurs lors de la création du nouvel enregistrement, puis saisissez des valeurs pour ces champs.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Type]</td> 
   <td>Si vous créez un programme, sélectionnez le type de programme que vous souhaitez créer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Channel] </td> 
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
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>Si vous créez un programme, ajoutez des coûts.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Si vous créez un programme, ajoutez des balises.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel personnalisé et authentifié vers l’API [!DNL Marketo]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], consultez la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin d’accès relatif à <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, placez des guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que vous souhaitez que le module utilise lors de chaque cycle d’exécution du scénario.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Mappez l’identifiant du fichier que vous souhaitez télécharger.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit des informations concernant un enregistrement à l’aide de son identifiant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
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
   <td>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.
Les champs sont disponibles en fonction du [!UICONTROL Record Type] que vous avez sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Object&gt; ID]</td> 
   <td>Saisissez ou mappez l’identifiant de l’objet dont vous souhaitez récupérer les informations.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer des leads d’une liste]

Ce module d’action supprime un ou plusieurs leads d’une liste à l’aide de l’ID de lead.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Saisissez ou mappez l’ID de la liste dans laquelle vous souhaitez supprimer des leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>Pour chaque lead à supprimer de la liste, cliquez sur <b>[!UICONTROL Add]</b>, puis saisissez ou mappez l’ID du lead à supprimer. Vous pouvez ajouter jusqu’à 300 leads pour que le module les supprime de la liste. </p> <p>Cliquez sur le bouton Mapper pour mapper une collection de leads existante à supprimer de la liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Planifier une campagne]

Ce module d’action planifie une campagne existante pour une certaine date.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Saisissez ou mappez l’ID de la campagne que vous souhaitez planifer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Schedule for Date]</p> </td> 
   <td>Sélectionnez la date d’exécution de la campagne. Si ce champ n’est pas renseigné, la campagne s’exécute cinq minutes après le début du scénario.</td> 
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
   <td> <p>Pour savoir comment connecter votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL Program ID]</td> 
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
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>Si vous mettez à jour un programme, saisissez ou mappez une nouvelle date de début pour le programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>Si vous mettez à jour un programme, saisissez ou mappez une nouvelle date de fin pour le programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>Si vous mettez à jour un programme, ajoutez des frais.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Si vous mettez à jour un programme, ajoutez des balises.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Charger un fichier]

Ce module d’action charge un nouveau fichier vers [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir la section <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Saisissez ou mappez l’identifiant du dossier dans lequel vous souhaitez que le nouveau fichier se trouve.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez une description pour le fichier chargé.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Répertorier des enregistrements]](#list-records)
* [[!UICONTROL Rechercher des enregistrements]](#update-a-record)

#### [!UICONTROL Répertorier des enregistrements]

Ce module d’action récupère tous les enregistrements d’un type spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez répertorier.</p> 
    <ul> 
     <li> <p>[!UICONTROL Read all campaigns]</p> </li> 
     <li> <p>[!UICONTROL Read all programs]</p> </li> 
     <li> <p>[!UICONTROL Read all leads] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>Si vous avez choisi de récupérer des leads, choisissez si vous souhaitez récupérer des leads à partir d’une liste ou d’un programme.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.
Les champs sont disponibles en fonction du [!UICONTROL Record Type] que vous avez sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des enregistrements]

Ce module de recherche récupère une liste d’enregistrements correspondant à des critères de recherche spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Marketo] à [!DNL Workfront Fusion], voir <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement à rechercher.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaigns]</p> </li> 
     <li> <p>[!UICONTROL Leads]</p> </li> 
     <li> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Field]</p> </td> 
   <td> <p>Indiquez si vous souhaitez effectuer une recherche par nom, nom de programme ou nom d’espace de travail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td>Pour chaque valeur à rechercher, cliquez sur <b>[!UICONTROL Add item]</b> et saisissez la valeur.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>
