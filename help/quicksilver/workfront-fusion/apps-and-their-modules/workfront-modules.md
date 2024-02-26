---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Adobe Workfront
description: Vous pouvez utiliser le connecteur Adobe Workfront Fusion Adobe Workfront pour automatiser vos processus dans Workfront. Si vous disposez d’une licence Workfront Fusion for Work Automation and Integration , vous pouvez également l’utiliser pour vous connecter à des applications et services tiers.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 0558f72fb8a7fc52d06adc0421082e20520c0b8f
workflow-type: tm+mt
source-wordcount: '5935'
ht-degree: 2%

---

# [!DNL Adobe Workfront] modules

Vous pouvez utiliser la variable [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] connecteur pour automatiser vos processus dans [!DNL Workfront]. Si vous avez une [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] , vous pouvez également l’utiliser pour vous connecter à des applications et services tiers.

La variable [!DNL Workfront] Le connecteur ne compte pas par rapport au nombre d’applications actives disponibles pour votre organisation. Tous les scénarios, même s’ils utilisent uniquement la variable [!DNL Workfront] , ne comptez pas par rapport au nombre total de scénarios de votre entreprise.

Pour plus d’informations sur les applications et les scénarios disponibles de votre entreprise, voir [Organisations](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] organisations et équipes](../../workfront-fusion/organizations/organizations-and-teams.md).

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créez un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Exigences de licence actuelles : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de l’[!UICONTROL Select] ou de l’[!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connexion [!DNL Workfront] to [!DNL Workfront Fusion]

La variable [!DNL Workfront] Le connecteur utilise OAuth 2.0 pour se connecter à [!DNL Workfront].

Vous pouvez créer une connexion à votre [!DNL Workfront] compte directement depuis l’intérieur d’un [!DNL Workfront Fusion] module .

1. Dans un module Adobe Authenticator, cliquez sur **Ajouter** en regard du champ Connexion .
1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Nom de la connexion]</td>
        <td>
          <p>Saisissez le nom de la nouvelle connexion.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>
          <p>Indiquez si vous vous connectez à un environnement de production ou hors production.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type de connexion]</td>
        <td>
          <p>Choisissez si vous vous connectez à un compte de service ou à un compte personnel.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID client]</td>
        <td>Saisissez votre [!DNL Workfront] ID client. Vous pouvez le trouver dans la zone Applications OAuth2 de la zone Configuration de Workfront. Ouvrez l’application spécifique à laquelle vous vous connectez pour afficher l’identifiant du client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre [!DNL Workfront] ID client. Vous pouvez le trouver dans la zone Applications OAuth2 de la zone Configuration de Workfront. Ouvrez l’application spécifique à laquelle vous vous connectez pour afficher l’identifiant du client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>Cela peut rester la valeur par défaut ou vous pouvez saisir l’URL de votre instance Workfront, suivie de <code>/integrations/oauth2</code>. <p>Exemple : <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Préfixe d’hôte]</td>
        <td>Dans la plupart des cas, cette valeur doit être <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Si vous ne voyez pas de bouton de connexion SAML, votre entreprise n’a pas activé l’authentification unique (SSO). Vous pouvez vous connecter à l’aide de vos nom d’utilisateur et mot de passe.
>   
>   Pour plus d’informations sur SSO, voir [Présentation de la connexion unique [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* Connexions OAuth 2.0 à la [!DNL Workfront] L’API ne dépend plus des clés d’API.

## [!DNL Workfront] modules et leurs champs

Lorsque vous configurez [!DNL Workfront] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Workfront] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

>[!NOTE]
>
>Si vous ne voyez pas les champs les plus à jour dans un module Workfront, cela peut être dû à des problèmes de mise en cache. Patientez une heure et réessayez.

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Triggers

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Événements de contrôle]**

Ce module de déclenchement exécute un scénario en temps réel lorsque des objets d’un type spécifique sont ajoutés, mis à jour ou supprimés dans Workfront

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

1. Cliquez sur **[!UICONTROL Ajouter]** à droite du **Webhook** de la boîte.

1. Configurez le webhook dans la variable **[!UICONTROL Ajouter un crochet]** qui s’affiche.

   Lors de la configuration de ce module, les champs suivants s’affichent.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nom du webhook]</td> 
      <td>(Facultatif) Saisissez un nouveau nom pour le webhook.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez que le module regarde.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Indiquez si vous souhaitez consulter l’ancien état ou le nouvel état.<ul><li><p><b>[!UICONTROL Nouvel état]</b></p><p>Déclenchez un scénario lorsque l’enregistrement change <b>to</b> une valeur donnée.</p><p>Par exemple, si l’état est défini sur [!UICONTROL Nouvel état] et que le filtre est défini sur [!UICONTROL État] [!UICONTROL Égal à] [!UICONTROL En cours], le webhook déclenche un scénario lorsque l’[!UICONTROL État] passe à [!UICONTROL En cours], quel que soit l’état antérieur. </p></li><li><p><b>[!UICONTROL Ancien état]</b></p><p>Déclenchez un scénario lorsque l’enregistrement change <b>de</b> une valeur donnée.</p><p>Par exemple, si l’état est défini sur [!UICONTROL Ancien état] et que le filtre est défini sur [!UICONTROL État] [!UICONTROL Égal À] [!UICONTROL En cours], le webhook déclenche un scénario lorsqu’un [!UICONTROL État] , qui est actuellement [!UICONTROL En cours] passe à un autre état. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>Filtres [!UICONTROL Événements]</p> </td> 
      <td> <p>Vous pouvez définir des filtres pour ne surveiller que les enregistrements qui répondent aux critères sélectionnés.</p> <p>Pour chaque filtre, saisissez le champ que le filtre doit évaluer, l’opérateur et la valeur que le filtre doit autoriser. Vous pouvez utiliser plusieurs filtres en ajoutant des règles ET.</p> <p>Remarque : Vous ne pouvez pas modifier les filtres dans les [!DNL Workfront] webhooks. Pour configurer différents filtres pour [!DNL Workfront] abonnements aux événements, supprimez le webhook actuel et créez-en un nouveau.</p> <p>Pour plus d’informations sur les filtres d’événements, voir <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtres d’abonnement aux événements dans [!DNL Workfront] &gt; Modules [!UICONTROL Watch Events]</a> dans cet article.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclure les événements effectués par cette connexion</td> 
      <td>Activez cette option pour exclure les événements créés ou mis à jour à l’aide du même connecteur que celui utilisé par ce module de déclenchement. Cela peut empêcher qu’un scénario se déclenche lui-même, ce qui entraîne sa répétition dans une boucle sans fin.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Choisissez si vous souhaitez que le scénario soit regardé <strong>[!UICONTROL Nouveaux enregistrements uniquement]</strong>, <strong>[!UICONTROL Enregistrements mis à jour uniquement]</strong>, <strong>[!UICONTROL Enregistrements nouveaux et mis à jour]</strong>, ou <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Remarque : Si vous choisissez <strong>[!UICONTROL Enregistrements nouveaux et mis à jour]</strong>, la création du webhook crée 2 abonnements d’événement (pour la même adresse webhook).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Une fois le webhook créé, vous pouvez afficher l’adresse du point de terminaison auquel les événements sont envoyés.

Pour plus d’informations, voir la section [Exemples de payloads d’événement](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) dans le [!DNL Workfront] Article d’aide [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md).

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Champ de contrôle]**

Ce module de déclenchement exécute un scénario lorsqu’un champ que vous spécifiez est mis à jour. Le module renvoie l’ancienne et la nouvelle valeur du champ que vous spécifiez. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez que le module regarde.</p> <p>Par exemple, sélectionnez [!UICONTROL Tâche] si vous souhaitez commencer à exécuter le scénario chaque fois qu’un champ d’enregistrement est mis à jour dans une tâche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Sélectionnez le champ que le module doit surveiller pour les mises à jour. Ces champs reflètent les champs que votre [!DNL Workfront] a été configuré pour le suivi.</td> 
  </tr> 
  <tr> 
   <td>Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Surveiller les enregistrements]**

Ce module de déclenchement exécute un scénario lorsque des objets d’un type spécifique sont ajoutés, mis à jour ou les deux. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario. Dans la sortie, le module indique si chaque enregistrement est nouveau ou mis à jour.

Les enregistrements qui ont été ajoutés et mis à jour au cours de la période donnée sont renvoyés en tant que nouveaux enregistrements.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Choisissez si vous souhaitez que le scénario soit regardé <strong>[!UICONTROL Nouveaux enregistrements uniquement]</strong>, <strong>[!UICONTROL Enregistrements mis à jour uniquement]</strong>, ou <strong>[!UICONTROL Enregistrements nouveaux et mis à jour]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>(S’affiche une fois que vous avez sélectionné une <strong>Filtrer</strong>.) Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez que le module regarde.</p> <p>Par exemple, si vous souhaitez lancer le scénario chaque fois qu’un nouveau projet est créé, sélectionnez [!UICONTROL Projet].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtre facultatif]</td> 
   <td> <p>(Avancé) Saisissez une chaîne de code API pour définir des paramètres ou du code supplémentaires qui affineront vos critères. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++


### Actions

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL Conversion, objet]**

Ce module d’action effectue l’une des conversions suivantes :

* Convertir le problème en projet
* Convertir le problème en tâche
* Convertir la tâche en projet

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Type d’objet]</td> 
   <td> <p>Sélectionnez le type d’objet à convertir. Il s’agit du type dont dispose l’objet avant la conversion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convertir en]</td> 
   <td>Sélectionnez l’objet dans lequel vous souhaitez le convertir. Il s’agit du type de l’objet après la conversion.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>Saisissez l’identifiant de l’objet. </p> <p>Remarque : lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de modèle]</td> 
   <td> <p>Si vous effectuez une conversion vers un projet, sélectionnez l’ID de modèle à utiliser pour le projet.</p> <p>Remarque : lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Formulaires personnalisés]</td> 
   <td>Sélectionnez les formulaires personnalisés à ajouter à l’objet nouvellement converti, puis saisissez les valeurs des champs du formulaire personnalisé.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Options]</td> 
   <td> <p>Activez les options souhaitées lors de la conversion de l’objet. Des options sont disponibles selon l’objet que vous convertissez ou à partir duquel vous effectuez cette conversion.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer un enregistrement (joindre des formulaires personnalisés)]**

Ce module d’action crée un objet, tel qu’un projet, une tâche ou un problème dans [!DNL Workfront]et vous permet d’ajouter un formulaire personnalisé au nouvel objet. Le module vous permet de sélectionner les champs de l’objet disponibles dans le module .

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous pouvez utiliser ce module pour créer une tâche dans [!DNL Workfront] lorsqu’un client ajoute une nouvelle ligne dans une [!DNL Google Sheets] liste des tâches à effectuer.

Lors de la configuration de ce module, les champs suivants s’affichent.

Veillez à indiquer le nombre minimum de champs de saisie. Par exemple, si vous souhaitez créer un problème, vous devez fournir un ID de projet parent valide dans le champ ID de projet pour indiquer où le problème doit se trouver dans Workfront. Vous pouvez utiliser le panneau de mappage pour mapper ces informations à partir d’un autre module dans votre scénario, ou vous pouvez les saisir manuellement en saisissant le nom, puis en le sélectionnant dans la liste.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez que le module crée.</p> <p>Par exemple, si vous souhaitez créer un projet, sélectionnez [!UICONTROL Projet] dans la liste déroulante, puis assurez-vous que vous avez accès aux données (des modules précédents dans le scénario) qui vont compléter le projet.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sélectionner les champs à mapper]</td> 
   <td> <p>Sélectionnez les champs qui doivent être disponibles pour la saisie de données. Vous pouvez ainsi utiliser ces champs sans avoir à faire défiler ceux dont vous n’avez pas besoin.</p> <p>Pour les champs des formulaires personnalisés, utilisez la méthode <b>[!UICONTROL Joindre un formulaire personnalisé]</b> champ .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Joindre un formulaire personnalisé]</td> 
   <td>Sélectionnez les formulaires personnalisés à ajouter au nouvel objet, puis saisissez les valeurs de ces champs.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ .
>* Lors de la saisie du texte d’un champ personnalisé ou d’une [!UICONTROL Remarque] (Commentaire ou Réponse), vous pouvez utiliser des balises de HTML dans la variable [!UICONTROL Texte de la remarque] pour créer du texte enrichi, comme du texte en gras ou en italique.
>
>  Pour plus d’informations sur le texte enrichi dans les mises à jour, voir [Ajouter une mise à jour à un élément de travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Créer un enregistrement]**

Ce module d’action crée un objet, tel qu’un projet, une tâche ou un problème dans Workfront. Le module vous permet de sélectionner les champs de l’objet disponibles dans le module .

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous pouvez utiliser ce module pour créer une tâche dans [!DNL Workfront] lorsqu’un client ajoute une nouvelle ligne dans une liste de tâches à effectuer dans une feuille de calcul Google.

Lors de la configuration de ce module, les champs suivants s’affichent.

Veillez à indiquer le nombre minimum de champs de saisie. Par exemple, si vous souhaitez créer un problème, vous devez fournir un ID de projet parent valide dans le champ ID de projet pour indiquer où le problème doit se trouver dans Workfront. Vous pouvez utiliser le panneau de mappage pour mapper ces informations à partir d’un autre module dans votre scénario, ou vous pouvez les saisir manuellement en saisissant le nom, puis en le sélectionnant dans la liste.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez que le module crée.</p> <p>Par exemple, si vous souhaitez créer un projet, sélectionnez [!UICONTROL Projet] dans la liste déroulante, puis assurez-vous que vous avez accès aux données (des modules précédents dans le scénario) qui vont compléter le projet.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sélectionner les champs à mapper]</td> 
   <td>Sélectionnez les champs qui doivent être disponibles pour la saisie de données. Vous pouvez ainsi utiliser ces champs sans avoir à faire défiler ceux dont vous n’avez pas besoin.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ .
>* Lors de la saisie du texte d’un champ personnalisé ou d’une [!UICONTROL Remarque] (Commentaire ou Réponse), vous pouvez utiliser des balises de HTML dans la variable [!UICONTROL Texte de la remarque] pour créer du texte enrichi, comme du texte en gras ou en italique.
>
>  Pour plus d’informations sur le texte enrichi dans les mises à jour, voir [Ajouter une mise à jour à un élément de travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Appel API personnalisé]**

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Workfront] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Workfront] modules.

Le module renvoie les informations suivantes :

* **[!UICONTROL Code d’état]** (nombre) : indique la réussite ou l’échec de votre requête HTTP. Ce sont des codes standard que vous pouvez consulter sur Internet.
* **[!UICONTROL En-têtes]** (objet) : contexte plus détaillé pour le code de réponse/d’état qui ne se rapporte pas au corps de sortie. Tous les en-têtes qui apparaissent dans un en-tête de réponse ne sont pas des en-têtes de réponse. Certains peuvent donc ne pas vous être utiles.

  Les en-têtes de réponse dépendent de la requête HTTP que vous avez choisie lors de la configuration du module.

* **[!UICONTROL Corps]** (objet) : selon la requête HTTP que vous avez choisie lors de la configuration du module, vous pouvez recevoir des données en retour. Ces données, telles que les données d’une demande de GET, sont contenues dans cet objet.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Saisissez un chemin relatif à<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version de l’API]</td> 
   <td>Sélectionnez la version de la [!DNL Workfront] API que vous souhaitez que le module utilise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Cela détermine le type de contenu de la requête.</p> <p>Par exemple,<code> {"Content-type":"application/json"}</code></p> <p>Remarque : si vous obtenez des erreurs et qu’il est difficile de déterminer leur origine, envisagez de modifier les en-têtes en fonction de la variable [!DNL Workfront] la documentation. Si votre appel API personnalisé renvoie une erreur de requête HTTP 422, essayez d’utiliser une <code>"Content-Type":"text/plain"</code> en-tête .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> <p>Conseil : Nous vous recommandons d’envoyer des informations via le corps JSON plutôt que sous forme de paramètres de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Supprimer l’enregistrement]**

Ce module d’action supprime un objet, tel qu’un projet, une tâche ou un problème dans Workfront.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forcer la suppression]</td> 
   <td>Activez cette option pour vous assurer que l’enregistrement est supprimé, même si la variable [!DNL Workfront] L’interface utilisateur demande la confirmation de la suppression.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Saisissez l’unique [!DNL Workfront] Identifiant de l’enregistrement que vous souhaitez supprimer du module.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après "ID=." Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez supprimer du module.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>Nous vous recommandons de configurer le scénario suivant pour éviter que les enregistrements ne soient supprimés en raison d’opérations asynchrones.
>
>1. Supprimer l’enregistrement de manière synchrone.
>1. Ajoutez la gestion des erreurs au module Supprimer l’enregistrement pour ignorer l’erreur provoquée par le délai d’attente de 40 secondes.


+++

+++ **[!UICONTROL Télécharger le document]**

Ce module d’action télécharge un document à partir de Workfront.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie le contenu, le nom, l’extension et la taille de fichier du document. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID du document]</td> 
   <td> <p>Faire correspondre ou saisir manuellement l’unique [!DNL Workfront] ID du document que vous souhaitez que le module télécharge.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après "ID=." Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Diverses actions]**

Ce module d’action vous permet d’effectuer des actions sur l’API.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type de [!DNL Workfront] enregistrement avec lequel vous souhaitez que le module interagisse.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Sélectionnez l’action que le module doit exécuter.</p> <p>Vous devrez peut-être remplir des champs supplémentaires, en fonction du [!UICONTROL Type d’enregistrement] et de l’[!UICONTROL Action] que vous choisissez. Certaines combinaisons de ces deux paramètres peuvent ne nécessiter qu’un identifiant d’enregistrement, tandis que d’autres (telles que Projet pour la variable <strong>[!UICONTROL Record Type]</strong> et [!UICONTROL Modèle de pièce jointe] pour le <strong>[!UICONTROL Action]</strong>) requièrent des informations supplémentaires (comme un ID d’objet et un ID de modèle).</p> <p>Pour plus d’informations sur les champs individuels, voir <a href="http://developer.workfront.com/">Documentation destinée aux développeurs Workfront</a>. <p><strong>Remarque</strong>: le site de documentation destinée aux développeurs contient des informations uniquement via la version 14 de l’API, mais contient toujours des informations précieuses pour les appels API. </p> 
    <ol> 
     <li value="1"> <p>Sélectionnez le type d’enregistrement dans le volet de navigation de gauche du [!DNL Workfront] page de documentation destinée aux développeurs. Les types suivants possèdent leurs propres pages :</p> 
      <ul> 
       <li> <p>[!UICONTROL Projects]</p> </li> 
       <li> <p>[!UICONTROL Tâches]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>Utilisateurs [!UICONTROL]</p> </li> 
       <li> <p>[!UICONTROL Documents]</p> </li> 
      </ul> <p>Pour tous les autres types d’enregistrement, sélectionnez <b>[!UICONTROL Autres objets et points de fin]</b>et recherchez le type d’enregistrement sur les pages triées par ordre alphabétique.</p> </li> 
     <li value="2"> <p>Sur la page du type d’enregistrement approprié, recherchez l’action (Ctrl+F ou Cmd+F).</p> </li> 
     <li value="3"> <p>Affichez les descriptions des champs disponibles sous l’action sélectionnée.</p> </li> 
    </ol> <p>Remarque :  <p>Lors de la création d’un BAT via [!DNL Workfront] module [!UICONTROL Divers actes], la bonne pratique consiste à créer un BAT sans options avancées, puis à le mettre à jour à l’aide de la fonction [!DNL Workfront Proof] API SOAP.</p> <p>Pour plus d’informations sur la création d’un BAT avec la variable [!DNL Workfront] API (que ce module utilise), voir <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Ajoutez des options de vérification avancées lors de la création d’un BAT via la fonction [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’unique [!DNL Workfront] Identifiant de l’enregistrement avec lequel vous souhaitez que le module interagisse.<p>Pour obtenir l’identifiant, ouvrez le [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après "ID=." Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Lire un enregistrement]**

Ce module d’action récupère les données d’un seul enregistrement.

Vous spécifiez l’identifiant de l’enregistrement. Vous pouvez également spécifier les enregistrements associés que le module doit lire.

Par exemple, si l’enregistrement que le module est en train de lire est un projet, vous pouvez spécifier que vous souhaitez que les tâches du projet soient lues.

Le module renvoie un tableau de données des champs standard pour la sortie que vous avez spécifiée.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>

<td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>

<td>Choisissez la [!DNL Workfront] type d’objet que le module doit lire.</td> 
  </tr> 
  <tr> 
    <td>Sorties [!UICONTROL]</td>

<td> <p>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
    <td>Références [!UICONTROL]</td>
   <td>Sélectionnez les champs de référence que vous souhaitez inclure dans la sortie.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Collections]</td>
   <td>Sélectionnez les champs de référence que vous souhaitez inclure dans la sortie.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Saisissez l’unique [!DNL Workfront] Identifiant de l’enregistrement que vous souhaitez que le module lise.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après "ID=." Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Mettre à jour l’enregistrement]**

Ce module d’action met à jour un objet, tel qu’un projet, une tâche ou un problème. Le module vous permet de sélectionner les champs de l’objet disponibles dans le module .

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’objet et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Saisissez l’unique [!DNL Workfront] Identifiant de l’enregistrement que vous souhaitez que le module soit mis à jour.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après "ID=." Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez que le module soit mis à jour.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Sélectionnez les champs qui doivent être disponibles pour la saisie de données. Vous pouvez ainsi utiliser ces champs sans avoir à faire défiler ceux dont vous n’avez pas besoin.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ .
>* Lors de la saisie du texte d’un champ personnalisé ou d’une [!UICONTROL Remarque] (Commentaire ou Réponse), vous pouvez utiliser des balises de HTML dans la variable [!UICONTROL Texte de la remarque] pour créer du texte enrichi, comme du texte en gras ou en italique.
>
>  Pour plus d’informations sur le texte enrichi dans les mises à jour, voir [Ajouter une mise à jour à un élément de travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Télécharger le document]**

Ce module d’action télécharge un document vers un [!DNL Workfront] (projet, tâche ou problème, par exemple).

Indiquez l’emplacement du document, le fichier à charger et éventuellement un nouveau nom pour le fichier.

Le module renvoie l’identifiant du document et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Identifiant d’enregistrement associé]</td> 
   <td>Saisissez l’unique [!DNL Workfront] ID de l’enregistrement auquel vous souhaitez charger le document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>Sélectionnez le type de [!DNL Workfront] enregistrement de l’emplacement où vous souhaitez que le module charge le document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fichier source]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

### Recherches

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Lire les enregistrements associés]**

Ce module de recherche lit les enregistrements correspondant à la requête de recherche que vous spécifiez, dans un objet parent particulier.

Vous spécifiez les champs que vous souhaitez inclure dans la sortie. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement parent (objet Workfront) dont vous souhaitez lire les enregistrements associés.</p> <p>Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Parent Record ID]</td> 
   <td> <p>Saisissez ou mappez l'identifiant de l'enregistrement parent dont vous souhaitez lire les enregistrements associés.</p> <p>Pour obtenir l’identifiant, ouvrez le [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après "ID=." Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Sélectionnez ou mappez le type d’enregistrement enfant que vous souhaitez que le module lise.</td> 
  </tr> 
  <tr> 
   <td>Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Rechercher]**

Ce module de recherche recherche recherche des enregistrements dans un objet de la section [!DNL Workfront] qui correspondent à la requête de recherche que vous spécifiez.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Workfront] app to [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Workfront] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type de [!DNL Workfront] enregistrement que vous souhaitez que le module recherche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Sélectionnez une option pour indiquer si vous souhaitez que le module obtienne le premier résultat correspondant à vos critères de recherche ou tous les résultats qui correspondent.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Critères de recherche]</td> 
   <td> <p>Renseignez le champ par lequel vous souhaitez effectuer une recherche, l'opérateur que vous souhaitez utiliser dans votre requête et la valeur que vous recherchez dans le champ.</p> <p>Remarque : Ne pas utiliser <code>username </code>dans vos critères de recherche. Inclusion <code>username </code>dans une requête API à [!DNL Workfront] connecte l’utilisateur à Workfront, et la recherche échoue.</p> <p>Remarque : <code>In</code> et <code>NotIn</code>fonctionne avec des tableaux. Les entrées doivent être au format de tableau.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Sorties [!UICONTROL]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie de ce module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Références [!UICONTROL]</td> 
   <td>Sélectionnez les champs de référence à inclure dans la recherche.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Sélectionnez les collections à ajouter à la recherche.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des [!DNL Workfront] types d’objets pour lesquels vous pouvez utiliser ce module dans [[!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] types d’objet disponibles pour chaque [!DNL Workfront] module

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Types d’objet disponibles pour chaque [!DNL Workfront] module déclencheur**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Enregistrement de contrôle]</th> 
   <th>[!UICONTROL Champ de contrôle]</th> 
   <th>[!UICONTROL Événements de contrôle]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processus d'approbation</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Affectation</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Niveau de référence</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Enregistrement de facturation </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taux de facturation</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entreprise</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tableau de bord</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dossier de documents</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Demande de document</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Version du document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Frais</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Type de frais</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Groupe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Heure</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Type d’heure</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Itération</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fonction</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrée au journal</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Jalon</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Chemin jalonné</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Balise de note</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utilisateur du projet</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approbation d'épreuve</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Durée réservée* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapport</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risque</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type de risque</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approbateur d’étape</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modèle</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tâche de modèle</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Feuille de temps</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Types d’objet disponibles pour chaque [!DNL Workfront] module d&#39;action**

>[!NOTE]
>
>La variable [!UICONTROL Télécharger le document] n’est pas inclus dans ce tableau, car [!DNL Workfront] les types d’objets ne font pas partie de sa configuration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Créer un enregistrement]</th> 
   <th>[!UICONTROL Mettre à jour un enregistrement]</th> 
   <th>[!UICONTROL Supprimer un enregistrement]</th> 
   <th>[!UICONTROL Télécharger le document]</th> 
   <th>[!UICONTROL Lire un enregistrement]</th> 
   <th>[!UICONTROL Appel API personnalisé]</th> 
   <th>[!UICONTROL Diverses actions]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processus d'approbation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Affectation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Enregistrement de facturation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taux de facturation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entreprise</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dossier de documents</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Version du document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Frais</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Type de frais</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Groupe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Heure</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type d’heure</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Itération</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fonction</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrée au journal</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Jalon</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Chemin jalonné</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Balise de note</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utilisateur du projet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Durée réservée* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risque</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type de risque</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approbateur d’étape</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modèle</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tâche de modèle</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Feuille de temps</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Types d’objet disponibles pour chaque [!DNL Workfront] module de recherche**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Search]</th> 
   <th>[!UICONTROL Lire les enregistrements associés]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processus d'approbation</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Affectation</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Enregistrement de facturation</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taux de facturation</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entreprise</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dossier de documents</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Version du document</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Frais</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type de frais</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Groupe</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Heure</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type d’heure</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Itération</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fonction</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrée au journal</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Jalon</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Chemin jalonné</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Balise de note</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utilisateur du projet</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Durée réservée* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risque</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type de risque</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approbateur d’étape</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modèle</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tâche de modèle</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Feuille de temps</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Délégation d'utilisateur</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Nous vous recommandons de vérifier deux fois pour vous assurer que cela fonctionne comme prévu.

+++

## Filtres d’abonnement aux événements dans [!DNL Workfront] > [!UICONTROL Événements de contrôle] modules

>[!NOTE]
>
>Il est vivement recommandé d’utiliser des filtres d’abonnement aux événements dans votre [!UICONTROL Événements de contrôle] modules.

La variable [!DNL Workfront] [!UICONTROL Événements de contrôle] déclenche des scénarios basés sur un webhook qui crée un abonnement à un événement dans la variable [!DNL Workfront] API. L’abonnement à l’événement est un ensemble de données qui détermine les événements envoyés au webhook. Par exemple, si vous configurez une [!UICONTROL Événements de contrôle] qui recherche les problèmes, puis l’abonnement à l’événement envoie uniquement les événements liés aux problèmes.

En utilisant des filtres d’abonnement aux événements, les utilisateurs de Fusion peuvent créer des abonnements aux événements qui conviennent mieux à leurs cas d’utilisation. Par exemple, vous pouvez configurer un abonnement à un événement dans la variable [!DNL Workfront] API pour envoyer uniquement les problèmes qui se trouvent dans un projet spécifique au webhook, en veillant à ce que la variable [!UICONTROL Événements de contrôle] ne se déclenche que pour les problèmes de ce projet. La possibilité de créer des déclencheurs plus étroits améliore la conception des scénarios en réduisant le nombre de déclencheurs non pertinents.

Cela diffère de la configuration d’un filtre dans la variable [!DNL Workfront Fusion] . Sans filtre d’abonnement à un événement, votre webhook reçoit tous les événements liés au type d’objet sélectionné. La plupart de ces événements seraient hors de propos dans le scénario et doivent être filtrés avant que le scénario puisse continuer.

Les opérateurs suivants sont disponibles dans le filtre Workfront > Evénements de contrôle :

* Est égal à
* Non égal à
* Supérieur à
* Inférieur à
* Supérieur ou égal à
* Inférieur ou égal à
* Contient
* Existe
   * Cet opérateur ne nécessite pas de valeur et le champ de valeur est absent.
* N’existe pas
   * Cet opérateur ne nécessite pas de valeur et le champ de valeur est absent.
* Modifié
   * Cet opérateur ne nécessite pas de valeur et le champ de valeur est absent.
   * Cet opérateur ignore le champ Etat .
   * Lorsque vous utilisez `Changed`, sélectionnez **Événements mis à jour uniquement** dans le **Origine de l’enregistrement** champ .

>[!IMPORTANT]
>
>Vous ne pouvez pas modifier les filtres dans les [!DNL Workfront] webhooks. Pour configurer différents filtres pour [!DNL Workfront] abonnements aux événements, supprimez le webhook actuel et créez-en un nouveau.

>[!INFO]
>
>**Exemple :** Supposons que vous envisagiez de traiter de nouveaux problèmes affectés à un utilisateur spécifique, Ana.
>
>### Filtrage des événements à l’aide d’un filtre d’abonnement aux événements (recommandé)
>
>À l’aide du filtre d’événement, vous pouvez configurer le webhook pour déclencher le scénario lorsqu’un problème est affecté à Ana lors de la création du problème. Ana a l’ID utilisateur b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Si 100 problèmes sont créés en un jour, mais que deux d’entre eux seulement sont affectés à Ana, le scénario s’exécute deux fois.
>
>### Filtrage des événements dans le scénario (non recommandé)
>
>Pour filtrer les événements de sorte que seuls les problèmes affectés à Ana soient traités, vous pouvez créer un filtre après l’événement [!UICONTROL Événements de contrôle] module .
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Si 100 problèmes sont créés en un jour, mais que seuls deux d’entre eux sont affectés à Ana, le scénario s’exécute 100 fois. 98 des exécutions s’arrêteraient au filtre, mais le module déclencheur consomme toujours des données et effectue des opérations dans toutes les exécutions.

Pour plus d’informations sur les abonnements aux événements, voir [Questions fréquentes - Abonnements à un événement](../../wf-api/general/event-subs-faq.md).

Pour plus d’informations sur les webhooks, voir [Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Pour plus d’informations sur les filtres dans les scénarios, voir [Ajoutez un filtre à un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

