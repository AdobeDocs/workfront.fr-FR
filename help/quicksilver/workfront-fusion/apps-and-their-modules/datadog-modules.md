---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules de données
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Datadog et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# [!DNL Datadog] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Datadog], ainsi que de la connecter à plusieurs applications et services tiers.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Datadog] modules, vous devez disposer d’un [!DNL Datadog] compte .

## Connexion [!DNL Datadog] to [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Récupération de votre clé API et de votre clé d’application {#retrieve-your-api-key-and-application-key}

Pour connecter votre [!DNL Datadog] compte à [!DNL Workfront Fusion] vous devez récupérer une clé API et une clé d’application à partir de votre [!DNL Datadog] compte .

1. Connectez-vous à [!DNL Datadog] compte .
1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Intégrations]**, puis cliquez sur **[!UICONTROL API]**.
1. Sur l’écran principal, cliquez sur **[!UICONTROL Clés API]**.
1. Passez la souris sur la barre violette pour afficher la clé API.
1. Copiez la clé API vers un emplacement sécurisé.
1. Sur l’écran principal, cliquez sur **[!UICONTROL Clés d’application]**.
1. Pointez sur la barre violette pour afficher la clé de l’application.
1. Copiez la clé de l’application dans un emplacement sécurisé.

### Créer une connexion à [!DNL Datadog] in [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre [!DNL Datadog] compte directement depuis l’intérieur d’un [!UICONTROL Datadog] module .

1. Dans n’importe quel [!UICONTROL Datadog] module, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Renseignez les champs du module comme suit :

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection Type]</td> 
      <td> <p> Sélectionnez l’[!UICONTROL [!DNL Datadog] Option de l’application pour obtenir un accès complet à [!DNL Datadog] API.</p> </td> 
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
      <td> <p> Saisissez votre [!DNL Datadog] Clé API. </p> <p>Pour plus d’informations sur la récupération de la clé API, voir <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Récupération de votre clé API et de votre clé d’application</a> dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clé D’Application]</td> 
      <td> <p> Saisissez votre [!DNL Datadog] clé de l’application. </p> <p>Pour plus d’informations sur la récupération de la clé de l’application, voir <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Récupération de votre clé API et de votre clé d’application</a> dans cet article.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## [!DNL Datadog] modules et leurs champs

Lorsque vous configurez [!DNL Datadog] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Datadog] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Actions

* [[!UICONTROL Points des séries de dates de publication]](#post-timeseries-points)
* [[!UICONTROL Lancer un appel API]](#make-an-api-call)

#### [!UICONTROL Points des séries de dates de publication]

Le module vous permet de publier des données de série temporelle qui peuvent être présentées sous forme de graphique sur [!DNL Datadog]des tableaux de bord de .

La limite pour les charges utiles compressées est de 3,2 mégaoctets (3200000) et de 62 mégaoctets (62914560) pour les charges utiles décompressées.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Datadog] compte à [!DNL Workfront Fusion], voir <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Datadog] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Ajout de séries temporelles à envoyer [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mesure]</strong> </p> <p>Saisissez le nom des horodatages.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>Sélectionnez le type de mesure.</p> </li> 
     <li> <p><strong>[!UICONTROL Intervalle]</strong> </p> <p> Si le type de mesure est rate ou count, définissez l’intervalle correspondant.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>Ajoutez des points relatifs à une mesure.</p> <p>Il s’agit d’un tableau JSON de points. Chaque point a le format suivant : <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Note:  <p>L’horodatage doit être exprimé en secondes.</p> <p>L’horodatage doit être en cours. Current est défini comme ne dépassant pas 10 minutes dans le futur ou plus d’une heure dans le passé.</p> <p> Le format de la valeur numérique doit être une valeur en virgule flottante.</p> </p> <p>Ce champ doit contenir au moins 1 élément.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Entrez le nom de l’hôte qui a produit la mesure.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lancer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Datadog] compte à [!DNL Workfront Fusion], voir <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Datadog] to [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://api.datadoghq.com/api/</code>. Exemple:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** L’appel API suivant renvoie tous les tableaux de bord de votre [!DNL Datadog] compte :

URL: `/v1/dashboard`

Méthode: `GET`

![](assets/datadog-api-example.png)

Le résultat se trouve dans la sortie du module sous Bundle > Body > dashboard.

Dans notre exemple, 3 tableaux de bord ont été renvoyés :

![](assets/datadog-api-response-example.png)
