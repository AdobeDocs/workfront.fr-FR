---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules d’événement
description: Dans un [!DNL Adobe Workfront Fusion] vous pouvez automatiser les workflows qui utilisent Cvent et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 1%

---

# [!DNL Cvent] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Cvent], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Pour utiliser [!DNL Cvent] modules, vous devez disposer d’un [!DNL Cvent] compte .

## Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>Le [!DNL Cvent] les modules fonctionnent par le biais d’une [!UICONTROL SOAP] API. Pour créer une connexion à [!DNL Cvent], vous devez vous assurer que :
>
>* Vous avez [!UICONTROL SOAP] accès au [!DNL Cvent] API.
>* Le [!DNL Workfront Fusion] Des adresses IP ont été ajoutées à la liste autorisée de votre entreprise.
>
>  Pour une liste de [!DNL Workfront Fusion] Adresses IP, voir [Adresses IP pour l’accès [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Vous pouvez créer une connexion à votre [!DNL Cvent] compte directement depuis l’intérieur d’un [!DNL Cvent] module .

1. Dans n’importe quel [!DNL Cvent] module, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Sélectionnez la région à laquelle vous souhaitez vous connecter.

   * [!UICONTROL Amérique du Nord]
   * [!UICONTROL Europe]
   * [!UICONTROL Sandbox]

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## [!DNL Cvent] modules et leurs champs

Lorsque vous configurez [!DNL Cvent] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Cvent] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)

### Actions

* [[!UICONTROL Appel API personnalisé]](#create-meeting-request)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Enregistrer l’invitation]](#register-invitee)
* [[!UICONTROL Ajouter une invitation]](#add-invitee)
* [[!UICONTROL Supprimer contact]](#delete-contact)
* [[!UICONTROL Mettre à jour le contact]](#update-contact)
* [[!UICONTROL Créer une demande de réunion]](#create-meeting-request)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Cvent] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Cvent] modules.

Lors de la configuration de ce module, les champs suivants s’affichent.

Le module renvoie un code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opération</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body (XML)</td> 
   <td> <p>Saisissez ou mappez le corps de l’appel API. Cela ne doit inclure que le code XML. Le module inclut automatiquement des en-têtes d’authentification. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit des informations sur un enregistrement spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type d’enregistrement]</p> </td> 
   <td>Sélectionnez le type d’élément de l’enregistrement que vous souhaitez lire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Événement] / [!UICONTROL ID d’invité]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’élément que vous souhaitez lire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module. Les champs sont disponibles en fonction du type d’élément sélectionné.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enregistrer l’invitation]

Ce module d’action enregistre un invité pour un événement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Identifiant d’invité</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’invité que vous souhaitez enregistrer pour un événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Identifiant d’événement</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’événement pour lequel vous souhaitez enregistrer l’invitation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une invitation]

Ce module d’action invite un contact à un événement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de contact]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du contact que vous souhaitez ajouter à un événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’événement auquel vous souhaitez ajouter le contact.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer contact]

Ce module d’action supprime un seul contact dans Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de contact]</td> 
   <td> <p>Saisissez ou mappez l'identifiant du contact que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour le contact]

Ce module d’action met à jour un contact existant à l’aide de son identifiant.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de contact]</p> </td> 
   <td> <p>Saisissez ou mappez l'identifiant du contact que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Sélectionnez les champs pour lesquels vous souhaitez saisir des informations, puis indiquez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs personnalisés]</td> 
   <td> <p>Sélectionnez les champs pour lesquels vous souhaitez saisir des informations, puis indiquez les valeurs souhaitées pour ces champs.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de formulaire]</p> </td> 
   <td> <p>Saisissez ou mappez l'identifiant du formulaire que vous souhaitez utiliser pour créer la demande de réunion.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs De Demande De Réunion]</td> 
   <td> <p>Sélectionnez les champs de demande de réunion pour lesquels vous souhaitez saisir des informations, puis indiquez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs de requête d’événement]</td> 
   <td> <p>Sélectionnez les champs de requête d’événement pour lesquels vous souhaitez saisir des informations, puis indiquez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Champs De Requête RFP]</td> 
   <td> <p>Sélectionnez les champs de demande de proposition pour lesquels vous souhaitez saisir des informations, puis indiquez les valeurs souhaitées pour ces champs.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Lister des enregistrements]

Ce module de recherche récupère des informations sur tous les enregistrements d’un type spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Cvent] compte à [!DNL Workfront Fusion], voir <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type d’enregistrement]</p> </td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez répertorier.</p> 
    <ul> 
     <li> <p>Tous les événements de votre [!DNL Cvent] account</p> </li> 
     <li> <p>Toutes les sessions pour un événement</p> </li> 
     <li> <p>Toutes les invitations pour un événement</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Si vous répertoriez des invités ou des sessions, saisissez ou mappez l’identifiant de l’événement auquel ces invités ou sessions sont associés.</p> </td> 
  </tr> 
 </tbody> 
</table>
