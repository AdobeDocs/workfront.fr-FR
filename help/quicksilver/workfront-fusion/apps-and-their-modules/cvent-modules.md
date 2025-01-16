---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Cvent
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 89%

---

# Modules [!DNL Cvent]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules Cvent](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/cvent-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Cvent] et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Pour utiliser les modules [!DNL Cvent], vous devez disposer d’un compte [!DNL Cvent].

## Informations sur l’API Cent

Le connecteur Cvent utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> V200611.ASMX </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.7.14</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>Les modules [!DNL Cvent] fonctionnent par l’intermédiaire d’une API [!UICONTROL SOAP]. Pour créer une connexion à [!DNL Cvent], vous devez vous assurer des points suivants :
>
>* Vous avez un accès [!UICONTROL SOAP] à l’API [!DNL Cvent].
>* Les adresses IP [!DNL Workfront Fusion] ont été ajoutées à la liste d’autorisation de votre organisation.
>
>  Pour obtenir une liste des adresses IP de [!DNL Workfront Fusion], voir [Adresses IP pour l’accès à  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md).


Vous pouvez créer une connexion à votre compte [!DNL Cvent] directement à partir d’un module [!DNL Cvent].

1. Dans n’importe quel module [!DNL Cvent], cliquez sur **[!UICONTROL Ajouter]** à côté du champ [!UICONTROL Connexion].
1. Sélectionnez la zone géographique à laquelle vous souhaitez vous connecter.

   * [!UICONTROL Amérique du Nord]
   * [!UICONTROL Europe]
   * [!UICONTROL Sandbox]

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Cvent] et leurs champs

Lorsque vous configurez les modules [!DNL Cvent], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Cvent] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez la section [Mappage des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)

### Actions

* [[!UICONTROL Personnaliser un appel API]](#create-meeting-request)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Enregistrer une personne invitée]](#register-invitee)
* [[!UICONTROL Ajouter une personne invitée]](#add-invitee)
* [[!UICONTROL Supprimer un contact]](#delete-contact)
* [[!UICONTROL Mettre à jour un contact]](#update-contact)
* [[!UICONTROL Créer une demande de réunion]](#create-meeting-request)

#### [!UICONTROL Personnaliser un appel API]

Ce module d’action vous permet d’effectuer un appel personnalisé et authentifié à l’API [!DNL Cvent]. Cela vous permet de créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Cvent].

Lorsque vous configurez ce module, les champs suivants s’affichent.

Le module renvoie le code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opération</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corps (XML)</td> 
   <td> <p>Saisissez ou mappez le corps de l’appel API. Il ne doit comprendre que le XML. Le module inclura automatiquement les en-têtes d’authentification. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action permet de lire les informations relatives à un enregistrement spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td>Sélectionnez le type d’élément de l’enregistrement que vous souhaitez lire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Event] / [!UICONTROL Invitee ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’élément que vous souhaitez lire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module. Les champs sont disponibles en fonction du type d’élément que vous avez sélectionné.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enregistrer une personne invitée]

Ce module d’action enregistre une personne invitée à un événement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Identifiant de personne invitée</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant de la personne invitée que vous souhaitez inscrire à un événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Identifiant d’événement</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’événement auquel vous souhaitez inscrire la personne invitée.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une personne invitée]

Ce module d’action invite un contact à un événement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du contact que vous souhaitez ajouter à un événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’événement auquel vous souhaitez ajouter le contact.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un contact]

Ce module d’action supprime un seul contact dans Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du contact que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un contact]

Ce module d’action met à jour un contact existant en utilisant son identifiant.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du contact que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Sélectionnez les champs pour lesquels vous souhaitez saisir des informations, puis remplissez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> <p>Sélectionnez les champs pour lesquels vous souhaitez saisir des informations, puis remplissez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une demande de réunion]

Ce module d’action ajoute une demande de réunion à votre compte.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Form ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du formulaire que vous souhaitez utiliser pour créer la demande de réunion.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Meeting Request Fields]</td> 
   <td> <p>Sélectionnez les champs de la demande de réunion pour lesquels vous souhaitez saisir des informations, puis indiquez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Request Fields]</td> 
   <td> <p>Sélectionnez les champs de demande d’événement pour lesquels vous souhaitez saisir des informations, puis renseignez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
   <td> <p>Sélectionnez les champs de l’appel d’offres pour lesquels vous souhaitez saisir des informations, puis indiquez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Répertorier des enregistrements]

Ce module de recherche permet d’obtenir des informations sur tous les enregistrements d’un type spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez répertorier.</p> 
    <ul> 
     <li> <p>Tous les événements de votre compte [!DNL Cvent]</p> </li> 
     <li> <p>Toutes les sessions d’un événement</p> </li> 
     <li> <p>Toutes les personnes invitées à un événement</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Si vous répertoriez des personnes invitées ou des sessions, saisissez ou mappez l’identifiant de l’événement auquel ces personnes invitées ou sessions sont associées.</p> </td> 
  </tr> 
 </tbody> 
</table>
