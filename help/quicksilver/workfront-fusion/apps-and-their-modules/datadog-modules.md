---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Datadog
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent la fonctionnalité Datadog et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 42%

---

# Modules [!DNL Datadog]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Datadog] et les connecter à plusieurs applications et services tiers.

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

Pour utiliser des modules [!DNL Datadog], vous devez disposer d’un compte [!DNL Datadog].

## Connecter [!DNL Datadog] à [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Récupération de votre clé API et de votre clé d’application {#retrieve-your-api-key-and-application-key}

Pour connecter votre compte [!DNL Datadog] à [!DNL Workfront Fusion], vous devez récupérer une clé API et une clé d’application à partir de votre compte [!DNL Datadog].

1. Connectez-vous à votre compte [!DNL Datadog].
1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Intégrations]**, puis sur **[!UICONTROL APIs]**.
1. Sur l’écran principal, cliquez sur **[!UICONTROL API Keys]**.
1. Passez la souris sur la barre violette pour afficher la clé API.
1. Copiez la clé API vers un emplacement sécurisé.
1. Sur l’écran principal, cliquez sur **[!UICONTROL Clés d’application]**.
1. Pointez sur la barre violette pour afficher la clé de l’application.
1. Copiez la clé de l’application dans un emplacement sécurisé.

### Créer une connexion à [!DNL Datadog] dans [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL Datadog] directement depuis un module [!UICONTROL Datadog].

1. Dans un module [!UICONTROL Datadog], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Renseignez les champs du module comme suit :

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection Type]</td> 
      <td> <p> Sélectionnez l’option [!UICONTROL [!DNL Datadog] Application] pour obtenir un accès complet à l’API [!DNL Datadog].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection Name]</td> 
      <td> <p> Saisissez le nom de la connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>Sélectionnez le domaine auquel vous souhaitez vous connecter (États-Unis ou UE).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clé API]</td> 
      <td> <p> Entrez votre clé d’API [!DNL Datadog]. </p> <p>Pour plus d'informations sur la récupération de la clé API, reportez-vous à la section <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Récupération de votre clé API et de votre clé d'application</a> de cet article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clé D’Application]</td> 
      <td> <p> Entrez votre clé d’application [!DNL Datadog]. </p> <p>Pour plus d'informations sur la récupération de la clé de l'application, reportez-vous à la section <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Récupération de votre clé d'API et de votre clé d'application</a> de cet article.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Datadog] et leurs champs

Lorsque vous configurez des modules [!DNL Datadog], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Datadog] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Actions

* [[!UICONTROL  Points de série chronologique Post]](#post-timeseries-points)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL  Points de série chronologique Post]

Le module vous permet de publier des données de série temporelle qui peuvent être présentées dans des graphiques sur les tableaux de bord de [!DNL Datadog].

La limite pour les charges utiles compressées est de 3,2 mégaoctets (3200000) et de 62 mégaoctets (62914560) pour les charges utiles décompressées.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Datadog] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Datadog] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Ajoutez la série temporelle à envoyer à [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metric]</strong> </p> <p>Saisissez le nom des horodatages.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>Sélectionnez le type de mesure.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> Si le type de mesure est rate ou count, définissez l’intervalle correspondant.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>Ajoutez des points relatifs à une mesure.</p> <p>Il s’agit d’un tableau JSON de points. Chaque point a le format suivant : <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Remarque :  <p>L’horodatage doit être exprimé en secondes.</p> <p>L’horodatage doit être en cours. Current est défini comme ne dépassant pas 10 minutes dans le futur ou plus d’une heure dans le passé.</p> <p> Le format de la valeur numérique doit être une valeur en virgule flottante.</p> </p> <p>Ce champ doit contenir au moins 1 élément.</p> </li> 
     <li> <p><strong>[!UICONTROL Hôte]</strong> </p> <p>Entrez le nom de l’hôte qui a produit la mesure.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Datadog] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Datadog] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://api.datadoghq.com/api/</code>. Exemple :<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
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
 </tbody> 
</table>

**Exemple :** L’appel API suivant renvoie tous les tableaux de bord de votre compte [!DNL Datadog] :

URL : `/v1/dashboard`

Méthode : `GET`

![](assets/datadog-api-example.png)

Le résultat se trouve dans la sortie du module sous Bundle > Body > dashboard.

Dans notre exemple, 3 tableaux de bord ont été renvoyés :

![](assets/datadog-api-response-example.png)
