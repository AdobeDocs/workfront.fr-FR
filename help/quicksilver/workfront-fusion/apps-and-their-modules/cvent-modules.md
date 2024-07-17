---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Cvent
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Cvent et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 34%

---

# Modules [!DNL Cvent]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Cvent] et les connecter à plusieurs applications et services tiers.

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

Pour utiliser des modules [!DNL Cvent], vous devez disposer d’un compte [!DNL Cvent].

## Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>Les modules [!DNL Cvent] fonctionnent avec une API [!UICONTROL SOAP]. Pour créer une connexion à [!DNL Cvent], vous devez vous assurer que :
>
>* Vous avez [!UICONTROL SOAP] accès à l’API [!DNL Cvent].
>* Les adresses IP [!DNL Workfront Fusion] ont été ajoutées à la liste autorisée de votre entreprise.
>
>  Pour obtenir la liste de [!DNL Workfront Fusion] adresses IP, voir [Adresses IP pour l’accès à [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Vous pouvez créer une connexion à votre compte [!DNL Cvent] directement à partir de l’intérieur d’un module [!DNL Cvent].

1. Dans un module [!DNL Cvent], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Sélectionnez la région à laquelle vous souhaitez vous connecter.

   * [!UICONTROL Amérique du Nord]
   * [!UICONTROL Europe]
   * [!UICONTROL Sandbox]

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Cvent] et leurs champs

Lorsque vous configurez des modules [!DNL Cvent], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Cvent] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)

### Actions

* [[!UICONTROL Appel API personnalisé]](#create-meeting-request)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Enregistrer l’invitation]](#register-invitee)
* [[!UICONTROL Ajouter une invitation]](#add-invitee)
* [[!UICONTROL Supprimer le contact]](#delete-contact)
* [[!UICONTROL Mettre à jour le contact]](#update-contact)
* [[!UICONTROL Créer une demande de réunion]](#create-meeting-request)

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Cvent]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Cvent].

Lors de la configuration de ce module, les champs suivants s’affichent.

Le module renvoie un code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Outputs]</td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
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

#### [!UICONTROL Supprimer le contact]

Ce module d’action supprime un seul contact dans Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
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

#### [!UICONTROL Répertorier les enregistrements]

Ce module de recherche récupère des informations sur tous les enregistrements d’un type spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Cvent] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connexion [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type d’enregistrement]</p> </td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez répertorier.</p> 
    <ul> 
     <li> <p>Tous les événements de votre compte [!DNL Cvent]</p> </li> 
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
