---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Adobe Campaign Classic
description: Avec le [!DNL Adobe Campaign Classic] modules, vous pouvez lancer une [!DNL Adobe Workfront Fusion] selon les événements de votre [!DNL Adobe Campaign Classic] créer, lire ou mettre à jour des contrats et d’autres enregistrements, rechercher des enregistrements à l’aide de critères que vous définissez et télécharger des documents.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] modules

Avec le [!DNL Adobe Campaign Classic] modules, vous pouvez lancer une [!DNL Adobe Workfront Fusion] selon les événements de votre [!DNL Adobe Campaign Classic] créer, lire ou mettre à jour des enregistrements, rechercher des enregistrements à l’aide des critères que vous définissez et effectuer des appels API personnalisés.

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

## Connexion [!DNL Adobe Campaign Classic] to [!DNL Adobe Workfront Fusion]

1. Dans n’importe quel [!DNL Adobe Campaign Classic] module, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Entrez l’URL de base que vous utilisez pour vous connecter à votre [!DNL Adobe Campaign Classic] instance.
1. Saisissez votre nom d’utilisateur et votre mot de passe.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## [!DNL Adobe Campaign Classic] modules et leurs champs

Lorsque vous configurez [!DNL Adobe Campaign Classic] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Adobe Campaign Classic] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Triggers

#### [!UICONTROL Surveiller les enregistrements]

Ce module de déclenchement planifié lance un scénario lorsqu’un enregistrement change.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Indiquez si vous souhaitez rechercher de nouveaux enregistrements, des enregistrements mis à jour ou les deux.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez la ressource que vous souhaitez surveiller.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs à inclure en sortie]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs personnalisés à inclure en sortie]</td> 
   <td>Pour chaque champ personnalisé que vous souhaitez inclure dans la sortie, cliquez sur <b>[!UICONTROL Ajouter]</b> et saisissez le nom du champ personnalisé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de résultats renvoyés]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>


### Actions

* [[!UICONTROL Création d’un enregistrement]](#create-a-record)
* [[!UICONTROL Effectuer un appel API personnalisé]](#make-a-custom-api-call)
* [[!UICONTROL Suppression d’un enregistrement]](#delete-record)
* [[!UICONTROL Exécution d’une action]](#perform-an-action)
* [[!UICONTROL Lire un enregistrement]](#-read-a-record)
* [[!UICONTROL S’abonner ou se désabonner]](#subscribe-or-unsubscribe)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-record)

#### [!UICONTROL Création d’un enregistrement]

Ce module d’action crée un nouvel enregistrement dans [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type de [!DNL Adobe Campaign Classic] enregistrement que vous souhaitez créer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez définir des valeurs lors de la création de l’enregistrement, puis renseignez les valeurs de ces champs. Les champs varient en fonction du type d’enregistrement sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs personnalisés]</td> 
   <td> Pour chaque champ personnalisé à ajouter au nouvel enregistrement, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez ou mappez le nom et la valeur du champ. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API personnalisé]

Ce module effectue un appel API personnalisé à la fonction [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Sélectionnez l’action que vous souhaitez que l’appel API effectue.</p>
      <p>[!UICONTROL Exécuter la requête]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Obtenir l’entité si plus récente]</p>
      <p>[!UICONTROL Tout sélectionner]</p>
      <p>[!UICONTROL Événement Push]</p>
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
   <td> <p>Ajoutez le contenu du corps de l’appel API au format XML, sans l’élément session . </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Supprimer l’enregistrement]

Ce module d’action supprime un seul enregistrement de [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type de ressource à supprimer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la ressource que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Exécution d’une action]

Ce module d’action exécute une action sélectionnée sur un objet dans la variable [!DNL Adobe Campaign Classic] API.

Pour plus d’informations sur des actions et des champs spécifiques, voir [[!DNL Adobe Campaign] - Documentation de l’API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Sélectionnez l’action à effectuer sur l’objet.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Pour les champs disponibles, voir <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> dans cet article. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Pour les champs disponibles, voir <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> dans cet article. </p></li> 
   <li><p><b>[!UICONTROL Créer]</b></p><p> Pour les champs disponibles, voir <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Créer un enregistrement]</a> dans cet article. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Pour les champs disponibles, voir <a href="#update-record" class="MCXref xref" >[!UICONTROL Mettre à jour un enregistrement]</a> dans cet article. </p></li>
   <li><p><b>[!UICONTROL Supprimer]</b></p><p> Pour les champs disponibles, voir <a href="#delete-record" class="MCXref xref" >[!UICONTROL Supprimer un enregistrement]</a> dans cet article. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit un enregistrement à partir de [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type de [!DNL Adobe Campaign Classic] enregistrement que vous souhaitez lire.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Saisissez la carte de l’identifiant de l’enregistrement que vous souhaitez lire.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Champs à inclure en sortie] </td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs personnalisés à inclure en sortie]</td> 
   <td>Pour chaque champ personnalisé que vous souhaitez inclure dans la sortie, cliquez sur <b>[!UICONTROL Ajouter]</b> et saisissez le nom du champ personnalisé.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL S’abonner ou se désabonner]

Ce module d’action abonne un utilisateur à un service d’information ou le désabonne.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL S’abonner ou se désabonner]</td> 
   <td>Indiquez si vous souhaitez vous abonner ou vous désabonner au service d’information.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du service]</td> 
   <td>Sélectionnez le service auquel vous souhaitez vous abonner ou dont vous souhaitez vous désabonner.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adresse électronique du destinataire] </td> 
   <td>Saisissez ou mappez l’adresse email de l’utilisateur que vous souhaitez abonner ou désabonner au service d’information.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour l’enregistrement]

Ce module d’action met à jour un seul enregistrement dans [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type de [!DNL Adobe Campaign Classic] enregistrement que vous souhaitez créer.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Saisissez la carte de l’identifiant de l’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez mettre à jour les valeurs, puis renseignez les valeurs de ces champs. Les champs varient en fonction du type d’enregistrement sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs personnalisés]</td> 
   <td> Pour chaque champ personnalisé à mettre à jour, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez ou mappez le nom et la valeur du champ. </td> 
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
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign Classic], voir <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Créer une connexion à [!DNL Adobe Campaign Classic]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Sélectionnez le type de [!DNL Adobe Campaign Classic] enregistrement que vous souhaitez créer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>
