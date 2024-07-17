---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Workfront
description: Vous pouvez utiliser le connecteur Adobe Workfront Fusion pour automatiser vos processus dans Workfront. Si vous disposez d’une licence Workfront Fusion pour l’automatisation du travail et l’intégration, vous pouvez également l’utiliser pour vous connecter à des applications et services tiers.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: f8abe5240f163693c30dc1bd6cf77e4cad5ea476
workflow-type: tm+mt
source-wordcount: '6259'
ht-degree: 99%

---

# Modules [!DNL Adobe Workfront]

Utilisez le connecteur [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] pour automatiser vos processus dans [!DNL Workfront]. Si vous disposez d’une licence [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail et l’intégration], vous pouvez également l’utiliser pour vous connecter à des applications et services tiers.

Le connecteur [!DNL Workfront] n’est pas pris en compte dans le nombre d’applications actives disponibles pour votre organisation. Tous les scénarios, même s’ils utilisent uniquement l’application [!DNL Workfront], ne sont pas pris en compte dans le nombre total de scénarios de votre entreprise.

Pour plus d’informations sur les applications et les scénarios disponibles pour votre entreprise, consultez [Organisations](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) dans [[!DNL Adobe Workfront Fusion] Organisations et équipes](../../workfront-fusion/organizations/organizations-and-teams.md).

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Connecter [!DNL Workfront] à [!DNL Workfront Fusion]

Le connecteur [!DNL Workfront] utilise OAuth 2.0 pour se connecter à [!DNL Workfront].

Vous pouvez créer une connexion à votre compte [!DNL Workfront] directement à partir de l’intérieur d’un module [!DNL Workfront Fusion].

1. Dans un module Adobe Workfront, cliquez sur **Ajouter** en regard du champ Connexion.
1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Saisissez un nom pour la nouvelle connexion.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>
          <p>Indiquez si vous vous connectez à un environnement de production ou hors production.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Choisissez si vous vous connectez à un compte de service ou à un compte personnel.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre ID client [!DNL Workfront]. Vous pouvez le trouver dans la zone Applications OAuth2 de la configuration de Workfront. Ouvrez l’application spécifique à laquelle vous vous connectez pour afficher l’ID client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre ID client [!DNL Workfront]. Vous pouvez le trouver dans la zone Applications OAuth2 de la configuration de Workfront. Ouvrez l’application spécifique à laquelle vous vous connectez pour afficher l’ID client.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>Vous pouvez conserver la valeur par défaut ou saisir l’URL de votre instance Workfront, suivie de <code>/integrations/oauth2</code>. <p>Exemple : <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Host prefix]</td>
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
>* Si vous ne voyez pas de bouton de connexion SAML, votre entreprise n’a pas activé l’authentification unique (SSO). Vous pouvez vous connecter à l’aide de votre nom d’utilisateur ou d’utilisatrice et mot de passe.
>   
>   Pour plus d’informations sur la SSO, consultez [Vue d’ensemble de l’authentification unique dans  [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).
>   
>* Les connexions OAuth 2.0 à l’API [!DNL Workfront] ne dépendent plus des clés d’API.

## Modules [!DNL Workfront] et leurs champs

Lorsque vous configurez des modules [!DNL Workfront], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Workfront] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

>[!NOTE]
>
>Si vous ne voyez pas les champs les plus à jour dans un module Workfront, cela peut être dû à des problèmes de cache. Patientez une heure et réessayez.

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Événements de contrôle]**

Ce module de déclenchement exécute un scénario en temps réel lorsque des objets d’un type spécifique sont ajoutés, mis à jour ou supprimés dans Workfront.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone **Webhook**.

1. Configurez le webhook dans la zone **[!UICONTROL Ajouter un webhook]** qui s’affiche.

   Lors de la configuration de ce module, les champs suivants s’affichent.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Facultatif) Donnez un autre nom au webhook.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>Sélectionnez le type d’enregistrement [!DNL Workfront] que le module doit surveiller.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Indiquez si vous souhaitez surveiller l’ancien ou le nouveau statut.<ul><li><p><b>[!UICONTROL New state]</b></p><p>Déclenchez un scénario lorsque l’enregistrement change <b>vers</b> une valeur donnée.</p><p>Par exemple, si le statut est défini sur [!UICONTROL New State] et que le filtre est défini sur [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress], le webhook déclenche un scénario lorsque le [!UICONTROL Status] passe à [!UICONTROL In Progress], quel que soit le statut antérieur. </p></li><li><p><b>[!UICONTROL Old state]</b></p><p>Déclenchez un scénario lorsque l’enregistrement change <b>à partir d’</b>une valeur donnée.</p><p>Par exemple, si le statut est défini sur [!UICONTROL Old State] et que le filtre est défini sur [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress], le webhook déclenche un scénario lorsqu’un [!UICONTROL Status] [!UICONTROL In Progress] passe à un autre statut. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>Vous pouvez définir des filtres pour ne surveiller que les enregistrements qui répondent aux critères sélectionnés.</p> <p>Pour chaque filtre, saisissez le champ que le filtre doit évaluer, l’opérateur et la valeur que le filtre doit autoriser. Vous pouvez utiliser plusieurs filtres en ajoutant des règles ET.</p> <p>Remarque : vous ne pouvez pas modifier les filtres dans les webhooks [!DNL Workfront] existants. Pour configurer différents filtres pour les abonnements aux événements [!DNL Workfront], supprimez le webhook actuel et créez-en un nouveau.</p> <p>Pour plus d’informations sur les filtres d’événements, consultez <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtres d’abonnement aux événements dans [!DNL Workfront] &gt; Modules [!UICONTROL Watch Events]</a> dans cet article.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclure les événements créés par cette connexion</td> 
      <td>Activez cette option pour exclure les événements créés ou mis à jour à l’aide du même connecteur que celui utilisé par ce module de déclenchement. Cela peut empêcher qu’un scénario se déclenche lui-même et se répète en une boucle sans fin.<p><b>REMARQUE</b> : le type d’enregistrement Affectation n’inclut pas cette option.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Choisissez si vous souhaitez que le scénario surveille les <strong>[!UICONTROL New Records Only]</strong>, les <strong>[!UICONTROL Updated Records Only]</strong>, les <strong>[!UICONTROL New and Updated Records]</strong> ou les <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Remarque : si vous choisissez les <strong>[!UICONTROL New and Updated Records]</strong>, la création du webhook crée 2 abonnements d’événement (pour la même adresse de webhook).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Une fois le webhook créé, vous pouvez afficher l’adresse du point d’entrée auquel les événements sont envoyés.

Pour plus d’informations, consultez la section [Exemples de payloads d’événement](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) dans l’article d’aide de [!DNL Workfront] [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md).

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Workfront] que vous souhaitez que le module surveille.</p> <p>Par exemple, sélectionnez [!UICONTROL Task] si vous souhaitez commencer à exécuter le scénario chaque fois qu’un champ d’enregistrement est mis à jour dans une tâche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Sélectionnez le champ que le module doit surveiller pour les mises à jour. Ces champs reflètent ceux que votre administrateur ou administratrice [!DNL Workfront] a configurés pour le suivi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Enregistrement de contrôle]**

Ce module de déclenchement exécute un scénario lorsque des objets d’un type spécifique sont ajoutés, mis à jour ou les deux. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario. Dans la sortie, le module indique si chaque enregistrement est nouveau ou mis à jour.

Les enregistrements qui ont été ajoutés et mis à jour au cours de la période donnée sont renvoyés en tant que nouveaux enregistrements.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de l’application [!DNL Workfront] à [!DNL Workfront Fusion], consultez la section <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Choisissez si vous souhaitez que le scénario surveille les <strong>[!UICONTROL New Records Only]</strong>, les <strong>[!UICONTROL Updated Records Only]</strong> ou les <strong>[!UICONTROL New and Updated Records]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>(S’affiche une fois que vous avez sélectionné un <strong>Filtre</strong>.) Sélectionnez le type d’enregistrement [!DNL Workfront] que le module doit surveiller.</p> <p>Par exemple, si vous souhaitez lancer le scénario chaque fois qu’un nouveau projet est créé, sélectionnez [!UICONTROL Project].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optional Filter]</td> 
   <td> <p>(Avancé) Saisissez une chaîne de code API pour définir des paramètres ou du code supplémentaires qui affineront vos critères. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

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

+++ **[!UICONTROL Convertir un objet]**

Ce module d’action effectue l’une des conversions suivantes :

* Convertir un problème en projet
* Convertir un problème en tâche
* Convertir une tâche en projet

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], consultez la section <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Object type]</td> 
   <td> <p>Sélectionnez le type d’objet à convertir. Il s’agit du type dont dispose l’objet avant la conversion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convert to]</td> 
   <td>Sélectionnez l’objet vers lequel vous souhaitez le convertir. Il s’agit du type de l’objet après la conversion.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;Object&gt; ID]</td> 
   <td> <p>Saisissez l’identifiant de l’objet. </p> <p>Remarque : lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Template ID]</td> 
   <td> <p>Si vous effectuez une conversion vers un projet, sélectionnez l’ID de modèle à utiliser pour le projet.</p> <p>Remarque : lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom forms]</td> 
   <td>Sélectionnez les formulaires personnalisés à ajouter à l’objet nouvellement converti, puis saisissez les valeurs des champs du formulaire personnalisé.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Options]</td> 
   <td> <p>Activez les options souhaitées lors de la conversion de l’objet. Des options sont disponibles selon l’objet que vous convertissez ou à partir duquel vous effectuez cette conversion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copier des champs natifs]</td> 
   <td> <p>Activez cette option pour copier les champs natifs de l’objet d’origine vers le nouvel objet.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copier des formulaires personnalisés]</td> 
   <td> <p>Activez cette option pour copier les champs natifs de l’objet d’origine vers le nouvel objet.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer un enregistrement (joindre des formulaires personnalisés)]**

Ce module d’action crée un objet, tel qu’un projet, une tâche ou un problème dans [!DNL Workfront] et vous permet d’ajouter un formulaire personnalisé au nouvel objet. Le module vous permet de sélectionner les champs de l’objet disponibles dans le module.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous pouvez utiliser ce module pour créer une tâche dans [!DNL Workfront] lorsqu’un client ou une cliente ajoute une nouvelle ligne dans une liste de tâches [!DNL Google Sheets] à effectuer.

Lors de la configuration de ce module, les champs suivants s’affichent.

Veillez à indiquer le nombre minimum de champs de saisie. Par exemple, si vous souhaitez créer un problème, vous devez fournir un ID de projet parent valide dans le champ ID de projet pour indiquer l’emplacement du problème dans Workfront. Vous pouvez utiliser le panneau de mappage pour mapper ces informations à partir d’un autre module dans votre scénario, ou vous pouvez les saisir manuellement en saisissant le nom, puis en le sélectionnant dans la liste.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Workfront] que vous souhaitez que le module crée.</p> <p>Par exemple, si vous souhaitez créer un projet, sélectionnez [!UICONTROL Project] dans la liste déroulante, puis assurez-vous que vous avez accès aux données (depuis les modules précédents dans le scénario) qui alimenteront le projet.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Sélectionnez les champs qui doivent être disponibles pour la saisie de données. Vous pouvez ainsi utiliser ces champs sans avoir à faire défiler ceux dont vous n’avez pas besoin.</p> <p>Pour les champs des formulaires personnalisés, utilisez le champ <b>[!UICONTROL Attach Custom Form]</b>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Attach Custom Form]</td> 
   <td>Sélectionnez les formulaires personnalisés à ajouter au nouvel objet, puis saisissez les valeurs de ces champs.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ.
>* Lors de la saisie du texte d’un champ personnalisé ou d’un objet [!UICONTROL Note] (Commentaire ou Réponse), vous pouvez utiliser des balises HTML dans le champ [!UICONTROL Texte de la note] pour créer du texte enrichi, comme du texte en gras ou en italique.
>
>  Pour plus d’informations sur le texte enrichi dans les mises à jour, voir [Ajouter une mise à jour à un élément de travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) dans [Mettre à jour le travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Créer un enregistrement]**

Ce module d’action crée un objet, tel qu’un projet, une tâche ou un problème dans Workfront. Le module vous permet de sélectionner les champs de l’objet disponibles dans le module.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous pouvez utiliser ce module pour créer une tâche dans [!DNL Workfront] lorsqu’une personne ajoute une nouvelle ligne dans une liste de tâches Google Sheets à faire.

Lors de la configuration de ce module, les champs suivants s’affichent.

Veillez à indiquer le nombre minimum de champs de saisie. Par exemple, si vous souhaitez créer un problème, vous devez fournir un ID de projet parent valide dans le champ ID de projet pour indiquer l’emplacement du problème dans Workfront. Vous pouvez utiliser le panneau de mappage pour mapper ces informations à partir d’un autre module dans votre scénario, ou vous pouvez les saisir manuellement en saisissant le nom, puis en le sélectionnant dans la liste.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Workfront] que vous souhaitez que le module crée.</p> <p>Par exemple, si vous souhaitez créer un projet, sélectionnez [!UICONTROL Project] dans la liste déroulante, puis assurez-vous que vous avez accès aux données (depuis les modules précédents dans le scénario) qui alimenteront le projet.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td>Sélectionnez les champs qui doivent être disponibles pour la saisie de données. Vous pouvez ainsi utiliser ces champs sans avoir à faire défiler ceux dont vous n’avez pas besoin.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ.
>* Lors de la saisie du texte d’un champ personnalisé ou d’un objet [!UICONTROL Note] (Commentaire ou Réponse), vous pouvez utiliser des balises HTML dans le champ [!UICONTROL Texte de la note] pour créer du texte enrichi, comme du texte en gras ou en italique.
>
>  Pour plus d’informations sur le texte enrichi dans les mises à jour, voir [Ajouter une mise à jour à un élément de travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) dans [Mettre à jour le travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Appel API personnalisé]**

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Workfront]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Workfront].

Le module renvoie les informations suivantes :

* **[!UICONTROL Code d’état]** (nombre) : indique la réussite ou l’échec de votre requête HTTP. Ce sont des codes standard que vous pouvez consulter sur Internet.
* **[!UICONTROL En-têtes]** (objet) : contexte plus détaillé pour le code de réponse/d’état qui ne se rapporte pas au corps de sortie. Tous les en-têtes qui apparaissent dans un en-tête de réponse ne sont pas des en-têtes de réponse. Certains peuvent donc ne pas vous être utiles.

  Les en-têtes de réponse dépendent de la requête HTTP que vous avez choisie lors de la configuration du module.

* **[!UICONTROL Corps]** (objet) : selon la requête HTTP que vous avez choisie lors de la configuration du module, vous pouvez recevoir des données en retour. Ces données, telles que les données d’une requête GET, sont contenues dans cet objet.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Saisissez un chemin relatif à <code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Sélectionnez la version de l’API [!DNL Workfront] que vous souhaitez que le module utilise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Cela détermine le type de contenu de la requête.</p> <p>Par exemple,<code> {"Content-type":"application/json"}</code></p> <p>Remarque : si vous obtenez des erreurs et qu’il est difficile de déterminer leur origine, envisagez de modifier les en-têtes en fonction de la documentation [!DNL Workfront]. Si votre appel API personnalisé renvoie une erreur de requête HTTP 422, essayez d’utiliser un en-tête <code>"Content-Type":"text/plain"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> <p>Conseil : nous vous recommandons d’envoyer des informations via le corps JSON plutôt que sous forme de paramètres de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les [[!DNL Workfront] types d’objets disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Force delete]</td> 
   <td>Activez cette option pour vous assurer que l’enregistrement est supprimé, même si l’IU de [!DNL Workfront] demande la confirmation de la suppression.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Saisissez l’identifiant [!DNL Workfront] unique de l’enregistrement que lem odule doit supprimer.</p> <p>Pour obtenir l’ID, ouvrez l’objet [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après « ID= .». Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Workfront] que le module doit supprimer.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les [[!DNL Workfront] types d’objet disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>Nous vous recommandons de configurer le scénario suivant pour éviter que les enregistrements ne soient supprimés en raison d’opérations asynchrones.
>
>1. Supprimez l’enregistrement de manière synchrone.
>1. Ajoutez la gestion des erreurs au module Supprimer l’enregistrement pour ignorer l’erreur provoquée par le délai d’expiration de 40 secondes.


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
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document ID]</td> 
   <td> <p>Faites correspondre ou saisissez manuellement l’ID [!DNL Workfront] unique du document que le module doit télécharger.</p> <p>Pour obtenir l’ID, ouvrez l’objet [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après « ID= .». Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les [[!DNL Workfront] types d’objet disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Actions diverses]**

Ce module d’action vous permet d’effectuer des actions sur l’API.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Workfront] avec lequel vous souhaitez que le module interagisse.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Sélectionnez l’action que le module doit exécuter.</p> <p>Vous devrez peut-être remplir des champs supplémentaires, en fonction du [!UICONTROL Record Type] et de l’[!UICONTROL Action] que vous choisissez. Certaines combinaisons de ces deux paramètres peuvent ne nécessiter qu’un identifiant d’enregistrement, tandis que d’autres (telles que Projet pour le <strong>[!UICONTROL Record Type]</strong> et le [!UICONTROL Attach Template] pour l’<strong>[!UICONTROL Action]</strong>) requièrent des informations supplémentaires (comme un ID d’objet et un ID de modèle).</p> <p>Pour plus d’informations sur les champs individuels, voir <a href="http://developer.workfront.com/">Documentation destinée à l’équipe de développement pour Workfront</a>. <p><strong>Remarque</strong> : le site de documentation destinée à l’équipe de développement contient des informations uniquement jusqu’à la version 14 de l’API, mais contient toujours des informations précieuses pour les appels API. </p> 
    <ol> 
     <li value="1"> <p>Sélectionnez le type d’enregistrement dans le volet de navigation de gauche de la page de documentation destinée à l’équipe de développement pour [!DNL Workfront]. Les types suivants possèdent leurs propres pages :</p> 
      <ul> 
       <li> <p>[!UICONTROL Projects]</p> </li> 
       <li> <p>[!UICONTROL Tasks]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>[!UICONTROL Users]</p> </li> 
       <li> <p>[!UICONTROL Documents]</p> </li> 
      </ul> <p>Pour tous les autres types d’enregistrement, sélectionnez <b>[!UICONTROL Other objects and endpoints]</b>, et recherchez le type d’enregistrement sur les pages triées par ordre alphabétique.</p> </li> 
     <li value="2"> <p>Sur la page du type d’enregistrement approprié, recherchez l’action (Ctrl+F ou Cmd+F).</p> </li> 
     <li value="3"> <p>Affichez les descriptions des champs disponibles sous l’action sélectionnée.</p> </li> 
    </ol> <p>Remarque :  <p>Lors de la création d’une épreuve via le module [!UICONTROL Misc Action] de [!DNL Workfront], la bonne pratique consiste à créer une épreuve sans options avancées, puis à la mettre à jour à l’aide de l’API SOAP [!DNL Workfront Proof].</p> <p>Pour plus d’informations sur la création d’une épreuve avec l’API [!DNL Workfront] (que ce module utilise), voir <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Ajouter des options de relecture avancées lors de la création d’une épreuve via l’API [!DNL Adobe Workfront]</a>.</p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’ID [!DNL Workfront] unique de l’enregistrement avec lequel vous souhaitez que le module interagisse.<p>Pour obtenir l’ID, ouvrez l’objet [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après « ID= ». Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

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

<td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>

<td>Choisissez le type d’objet [!DNL Workfront] que le module doit lire.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>

<td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL References]</td>
   <td>Sélectionnez les champs de référence que vous souhaitez inclure dans la sortie.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Collections]</td>
   <td>Sélectionnez les champs de référence que vous souhaitez inclure dans la sortie.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Saisissez l’ID [!DNL Workfront] unique de l’enregistrement que le module doit lire.</p> <p>Pour obtenir l’ID, ouvrez l’objet [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après « ID= ». Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les [[!DNL Workfront] types d’objet disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Mettre à jour l’enregistrement]**

Ce module d’action met à jour un objet, tel qu’un projet, une tâche ou un problème. Le module vous permet de sélectionner les champs de l’objet disponibles dans le module.

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’ID de l’objet et de tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Saisissez l’ID [!DNL Workfront] unique de l’enregistrement que le module doit mettre à jour.</p> <p>Pour obtenir l’ID, ouvrez l’objet [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après « ID= ». Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Workfront] que le module doit mettre à jour.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Sélectionnez les champs qui doivent être disponibles pour la saisie de données. Vous pouvez ainsi utiliser ces champs sans avoir à faire défiler ceux dont vous n’avez pas besoin.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Lorsque vous saisissez l’identifiant d’un objet, vous pouvez commencer à saisir son nom, puis le sélectionner dans la liste. Le module saisit ensuite l’identifiant approprié dans le champ.
>* Lors de la saisie du texte d’un champ personnalisé ou d’un objet [!UICONTROL Note] (Commentaire ou Réponse), vous pouvez utiliser des balises HTML dans le champ [!UICONTROL Texte de la note] pour créer du texte enrichi, comme du texte en gras ou en italique.
>
>  Pour plus d’informations sur le texte enrichi dans les mises à jour, voir [Ajouter une mise à jour à un élément de travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) dans [Mettre à jour le travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Charger le document]**

Ce module d’action charge un document vers un objet [!DNL Workfront] (projet, tâche ou problème, par exemple).

Indiquez l’emplacement du document, le fichier à charger et éventuellement un nouveau nom pour le fichier.

Le module renvoie l’ID du document et des champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Saisissez l’ID [!DNL Workfront] unique de l’enregistrement dans lequel charger le document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Workfront] où le module doit charger le document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les [[!DNL Workfront] types d’objet disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

+++

### Recherches

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Lire les enregistrements associés]**

Ce module de recherche lit les enregistrements correspondant à la requête de recherche que vous spécifiez, dans un objet parent particulier.

Vous spécifiez les champs à inclure dans la sortie. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement parent (objet Workfront) dont vous souhaitez lire les enregistrements associés.</p> <p>Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] disponibles pour chaque module [!DNL Workfront]</a> dans cet article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Parent Record ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’enregistrement parent dont vous souhaitez lire les enregistrements associés.</p> <p>Pour obtenir l’identifiant, ouvrez l’objet [!DNL Workfront] dans votre navigateur et copiez le texte à la fin de l’URL après « ID= ». Par exemple : https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Sélectionnez ou mappez le type d’enregistrement enfant que le module doit lire.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Rechercher]**

Ce module de recherche recherche des enregistrements d’un objet dans [!DNL Workfront] qui correspondent à la requête de recherche que vous avez spécifiée.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Workfront] que le module doit rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Sélectionnez une option pour indiquer si vous souhaitez que le module obtienne le premier résultat correspondant à vos critères de recherche ou tous les résultats correspondants.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria fields]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez utiliser pour vos critères de recherche. Ces champs seront ensuite disponibles dans la liste déroulante Critères de recherche.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Renseignez le champ avec lequel vous souhaitez effectuer une recherche, l’opérateur que vous souhaitez utiliser dans votre requête et la valeur que vous recherchez dans le champ.</p> <p>Remarque : n’utilisez pas <code>username </code> dans vos critères de recherche. L’inclusion de <code>username </code> dans une requête API à [!DNL Workfront] connecte l’utilisateur ou l’utilisatrice à Workfront, et la recherche échoue.</p> <p>Remarque : <code>In</code> et <code>NotIn</code> fonctionnent avec des tableaux. Les entrées doivent être au format de tableau.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie de ce module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL References]</td> 
   <td>Sélectionnez les champs de référence à inclure dans la recherche.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Sélectionnez les collections à ajouter à la recherche.</td> 
  </tr> 
 </tbody> 
</table>
+++

+++ **[!UICONTROL Recherche (hérité)]**

Ce module de recherche recherche des enregistrements d’un objet dans [!DNL Workfront] qui correspondent à la requête de recherche que vous avez spécifiée.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement [!DNL Workfront] que le module doit rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Sélectionnez une option pour indiquer si vous souhaitez que le module obtienne le premier résultat correspondant à vos critères de recherche ou tous les résultats correspondants.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Renseignez le champ avec lequel vous souhaitez effectuer une recherche, l’opérateur que vous souhaitez utiliser dans votre requête et la valeur que vous recherchez dans le champ.</p> <p>Remarque : n’utilisez pas <code>username </code> dans vos critères de recherche. L’inclusion de <code>username </code> dans une requête API à [!DNL Workfront] connecte l’utilisateur ou l’utilisatrice à Workfront, et la recherche échoue.</p> <p>Remarque : <code>In</code> et <code>NotIn</code> fonctionnent avec des tableaux. Les entrées doivent être au format de tableau.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les champs que vous souhaitez inclure dans la sortie de ce module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL References]</td> 
   <td>Sélectionnez les champs de référence à inclure dans la recherche.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Sélectionnez les collections à ajouter à la recherche.</td> 
  </tr> 
 </tbody> 
</table>

Consultez la liste des types d’objets [!DNL Workfront] pour lesquels vous pouvez utiliser ce module dans les types d’objet [[!DNL Workfront]  disponibles pour chaque module  [!DNL Workfront] ](#workfront-object-types-available-for-each-workfront-module).

+++

## Types d’objet [!DNL Workfront] disponibles pour chaque module [!DNL Workfront]

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Types d’objet disponibles pour chaque module déclencheur [!DNL Workfront]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Watch Record]</th> 
   <th>[!UICONTROL Watch Field]</th> 
   <th>[!UICONTROL Watch Events]</th> 
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
   <td>Temps réservé* </td> 
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
   <td>Approbateur ou approbatrice d’étape</td> 
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

+++**Types d’objets disponibles pour chaque module d’action [!DNL Workfront]**

>[!NOTE]
>
>Le module [!UICONTROL Télécharger un document] n’est pas inclus dans ce tableau, car les types d’objets [!DNL Workfront] ne font pas partie de sa configuration.

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
   <th>[!UICONTROL Create a record]</th> 
   <th>[!UICONTROL Update a record]</th> 
   <th>[!UICONTROL Delete a record]</th> 
   <th>[!UICONTROL Upload Document]</th> 
   <th>[!UICONTROL Read a record]</th> 
   <th>[!UICONTROL Custom API Call]</th> 
   <th>[!UICONTROL Misc Action]</th> 
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
   <td>Niveau de référence</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Taux de change</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td>Document externe</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
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
   <td>Temps réservé* </td> 
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
   <td>Approbateur ou approbatrice d’étape</td> 
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
   <td> </td> 
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

+++**Types d’objets disponibles pour chaque module de recherche [!DNL Workfront]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Search]</th> 
   <th>[!UICONTROL Read Related Records]</th> 
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
   <td>Temps réservé* </td> 
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
   <td>Approbateur ou approbatrice d’étape</td> 
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

Nous vous recommandons de vérifier à nouveau que cela fonctionne comme vous l’attendez.

+++

## Filtres d’abonnement aux événements dans les modules [!DNL Workfront] > [!UICONTROL Événements de contrôle] 

>[!NOTE]
>
>Nous vous recommandons vivement d’utiliser des filtres d’abonnement aux événements dans vos modules [!UICONTROL Événements de contrôle].

Le module [!UICONTROL Événements de contrôle] [!DNL Workfront] déclenche des scénarios basés sur un webhook qui crée un abonnement à un événement dans l’API [!DNL Workfront]. L’abonnement à un événement est un ensemble de données qui détermine quels événements sont envoyés au webhook. Par exemple, si vous configurez un module [!UICONTROL Événements de contrôle] qui surveille les problèmes, l’abonnement aux événements n’envoie que les événements liés aux problèmes.

En utilisant des filtres d’abonnement aux événements, les utilisateurs et utilisatrices de Fusion peuvent créer des abonnements aux événements qui correspondent mieux à leurs cas d’utilisation. Par exemple, vous pouvez configurer un abonnement à un événement dans l’API [!DNL Workfront] pour n’envoyer au webhook que les problèmes qui se trouvent dans un projet spécifique, ce qui garantit que le module [!UICONTROL Événements de contrôle] ne se déclenchera que pour les problèmes de ce projet. La possibilité de créer des déclencheurs plus étroits améliore la conception des scénarios en réduisant le nombre de déclencheurs non pertinents.

Cela diffère de la mise en place d’un filtre dans le scénario [!DNL Workfront Fusion]. Sans filtre d’abonnement aux événements, votre webhook reçoit tous les événements liés au type d’objet que vous avez sélectionné. La plupart de ces événements ne sont pas pertinents pour le scénario et doivent être éliminés avant que le scénario ne puisse se poursuivre.

Les opérateurs suivants sont disponibles dans le filtre Workfront > Événements de contrôle :

* Est égal à
* N’est pas égal à
* Supérieur à
* Inférieur à
* Supérieur ou égal à
* Inférieur ou égal à
* Contient
* Existe
   * Cet opérateur ne nécessite pas de valeur et le champ de la valeur est absent.
* N’existe pas
   * Cet opérateur ne nécessite pas de valeur et le champ de la valeur est absent.
* Modifié
   * Cet opérateur ne nécessite pas de valeur et le champ de la valeur est absent.
   * Cet opérateur ne tient pas compte du champ État.
   * Si vous utilisez `Changed`, sélectionnez **Événements mis en jour uniquement** dans le champ **Origine de l’enregistrement**.

>[!IMPORTANT]
>
>Vous ne pouvez pas modifier les filtres dans les webhooks [!DNL Workfront] existants. Pour définir différents filtres pour les abonnements aux événements [!DNL Workfront], supprimez le webhook actuel et créez-en un nouveau.

>[!INFO]
>
>**Exemple :** prenons l’exemple d’un scénario qui traite les nouveaux problèmes affectés à une utilisatrice spécifique, Ana.
>
>### Filtrer les événements à l’aide d’un filtre d’abonnement aux événements (recommandé)
>
>En utilisant le filtre d’événement, vous pouvez configurer le webhook pour déclencher le scénario lorsqu’un problème est assigné à Ana lors de la création du problème. L’identifiant d’utilisatrice d’Ana est b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Si 100 problèmes sont créés en une journée, mais que seuls deux d’entre eux sont affectés à Ana, le scénario s’exécutera deux fois.
>
>### Filtrer les événements à l’intérieur du scénario (non recommandé)
>
>Pour filtrer les événements afin que seuls les problèmes attribués à Ana soient traités, vous pouvez créer un filtre après le module [!UICONTROL Événements de contrôle].
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Si 100 problèmes sont créés en une journée, mais que seuls deux d’entre eux sont affectés à Ana, le scénario s’exécutera 100 fois. 98 des exécutions s’arrêteraient au niveau du filtre, mais le module déclencheur continue à consommer des données et à effectuer des opérations dans toutes les exécutions.

Pour plus d’informations sur les abonnements aux événements, voir [Questions fréquentes - Abonnements aux événements](../../wf-api/general/event-subs-faq.md).

Pour plus d’informations sur les webhooks, voir [Déclencheurs instantanés (webhooks) dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

Pour plus d’informations sur les filtres dans les scénarios, voir [Ajouter un filtre à un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

