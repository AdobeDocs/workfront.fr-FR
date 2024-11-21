---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Campaign v7/v8
description: Avec les modules  [!DNL Adobe Campaign] , vous pouvez lancer un scènario  [!DNL Adobe Workfront Fusion]  selon les événements de votre compte  [!DNL Adobe Campaign] , créer, lire ou mettre à jour des contrats et d’autres enregistrements, rechercher des enregistrements à l’aide de critères que vous définissez et charger des documents.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 97%

---

# Modules [!DNL Adobe Campaign]

Avec les modules [!DNL Adobe Campaign], vous pouvez démarrer un scénario [!DNL Adobe Workfront Fusion] selon les événements de votre compte [!DNL Adobe Campaign v7/v8], créer, lire ou mettre à jour des enregistrements, rechercher des enregistrements à l’aide des critères que vous définissez et effectuer des appels API personnalisés.

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
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Vous devez ajouter les adresses IP Fusion à [!DNL Adobe Campaign].

* Pour plus d’informations sur l’ajout d’adresses IP à votre liste autorisée Campaign, voir [Ajouter des adresses IP à la liste autorisée](https://experienceleague.adobe.com/fr/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) dans la documentation Adobe Campaign.
* Pour obtenir la liste des adresses IP à ajouter à la liste autorisée, voir [Adresses IP pour accéder à Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## Informations sur l’API Adobe Campaign

Le connecteur Adobe Campaign utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.7.22</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!DNL Adobe Campaign] à [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Il est vivement recommandé de créer une connexion serveur à serveur. Adobe Campaign a mis à jour son API pour n’accepter que les connexions de serveur à serveur. Si vous vous connectez à la version 8 ou ultérieure de Campaign, vous **devez** créez une connexion serveur à serveur.
>
>Pour plus d’informations sur les nouvelles exigences de connexion de Campaign, voir [Migration des opérateurs techniques Campaign vers Adobe Developer Console](https://experienceleague.adobe.com/fr/docs/campaign/technotes-ac/tn-new/ims-migration) dans la documentation de Campaign.

1. Dans n’importe quel module [!DNL Adobe Campaign], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Remplissez les champs suivants :
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection type]</td>
          <td>
            <p>Indiquez si vous créez une connexion de base ou une connexion serveur à serveur.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Saisissez un nom pour cette connexion.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Base URL]</td>
          <td>Saisissez l’URL de base que vous utilisez pour vous connecter à votre instance [!DNL Adobe Campaign].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Username]</td>
          <td>Si vous créez une connexion de base, saisissez votre nom d’utilisateur ou d’utilisatrice Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Password]</td>
          <td>Si vous créez une connexion de base, saisissez votre mot de passe Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Si vous créez une connexion serveur à serveur, saisissez votre [!UICONTROL Client ID] [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] d’[!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Si vous créez une connexion serveur à serveur, saisissez votre [!UICONTROL Client Secret] [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>Indiquez si votre connexion est établie à un environnement de production ou hors production.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>Indiquez si vous vous connectez à un compte de service ou à un compte personnel.
        </tr>
   </tbody>
    </table>
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenez au module.

## Modules [!DNL Adobe Campaign] et leurs champs

Lorsque vous configurez les modules [!DNL Adobe Campaign], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Adobe Campaign] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement planifié lance un scénario lorsqu’un enregistrement change.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Indiquez si vous souhaitez surveiller les nouveaux enregistrements, les enregistrements mis à jour ou les deux.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez la ressource que vous souhaitez surveiller.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>Pour chaque champ personnalisé à inclure dans la sortie, cliquez sur <b>[!UICONTROL Add]</b> et saisissez le nom du champ personnalisé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>


### Actions

* [[!UICONTROL Créer un enregistrement]](#create-a-record)
* [[!UICONTROL Effectuer un appel API personnalisé]](#make-a-custom-api-call)
* [[!UICONTROL Supprimer un enregistrement]](#delete-record)
* [[!UICONTROL Exécuter une action]](#perform-an-action)
* [[!UICONTROL Lire un enregistrement]](#-read-a-record)
* [[!UICONTROL S’abonner ou se désabonner]](#subscribe-or-unsubscribe)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-record)

#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un enregistrement dans [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Adobe Campaign] à créer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez définir des valeurs lors de la création de l’enregistrement, puis renseignez les valeurs de ces champs. Les champs varient en fonction du type d’enregistrement sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> Pour chaque champ personnalisé à ajouter au nouvel enregistrement, cliquez sur <b>[!UICONTROL Add item]</b> et saisissez ou mappez le nom et la valeur du champ. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API personnalisé]

Ce module effectue un appel API personnalisé à l’API [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Sélectionnez l’action que vous souhaitez que l’appel API effectue.</p>
      <p>[!UICONTROL Execute query]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Get entity if more recent]</p>
      <p>[!UICONTROL Select all]</p>
      <p>[!UICONTROL Push event]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] ajoute automatiquement l’en-tête du jeton [!UICONTROL x-security].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API au format XML, sans l’élément de session. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Supprimer l’enregistrement]

Ce module d’action supprime un seul enregistrement d’[!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type de ressource à supprimer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’ID de la ressource que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Exécuter une action]

Ce module d’action exécute une action sélectionnée sur un objet dans l’API [!DNL Adobe Campaign].

Pour plus d’informations sur des actions et des champs spécifiques, voir Documentation de l’API [[!DNL Adobe Campaign] ](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html?lang=fr).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Sélectionnez l’action à effectuer sur l’objet.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Pour les champs disponibles, voir <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> dans cet article. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Pour les champs disponibles, voir <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> dans cet article. </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> Pour les champs disponibles, voir <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Create a record]</a> dans cet article. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Pour les champs disponibles, voir <a href="#update-record" class="MCXref xref" >[!UICONTROL Update a record]</a> dans cet article. </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> Pour les champs disponibles, voir <a href="#delete-record" class="MCXref xref" >[!UICONTROL Delete a record]</a> dans cet article. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit un enregistrement à partir d’[!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Adobe Campaign] que vous souhaitez lire.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Saisissez ou mapper l’ID de l’enregistrement que vous souhaitez lire.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output] </td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>Pour chaque champ personnalisé à inclure dans la sortie, cliquez sur <b>[!UICONTROL Add]</b> et saisissez le nom du champ personnalisé.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Abonner ou désabonner]

Ce module d’action abonne une personne à un service d’information ou la désabonne.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe or unsubscribe]</td> 
   <td>Indiquez si vous souhaitez vous abonner au service d’information ou vous en désabonner.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>Sélectionnez le service auquel vous souhaitez vous abonner ou dont vous souhaitez vous désabonner.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient email address] </td> 
   <td>Saisissez ou mappez l’adresse e-mail de la personne que vous souhaitez abonner au service d’information ou que vous souhaitez désabonner de ce service.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour l’enregistrement]

Ce module d’action met à jour un seul enregistrement dans [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Adobe Campaign] à créer.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Saisissez ou mappez l’ID de l’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez mettre à jour les valeurs, puis renseignez les valeurs de ces champs. Les champs varient en fonction du type d’enregistrement sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> Pour chaque champ personnalisé à mettre à jour, cliquez sur <b>[!UICONTROL Add item]</b> et saisissez ou mappez le nom et la valeur du champ. </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Rechercher]

Ce module de recherche renvoie des enregistrements en fonction des critères spécifiés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Adobe Campaign] à créer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>
