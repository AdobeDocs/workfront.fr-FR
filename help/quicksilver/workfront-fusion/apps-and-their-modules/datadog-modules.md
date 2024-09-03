---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Datadog
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Datadog, ainsi que le connecter à de multiples applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 100%

---

# Modules [!DNL Datadog]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Datadog] et le connecter à plusieurs applications et services tiers.

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
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Datadog], vous devez disposer d’un compte [!DNL Datadog].

## Connecter [!DNL Datadog] à [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Récupérer votre clé d’API et clé d’application {#retrieve-your-api-key-and-application-key}

Pour connecter votre compte [!DNL Datadog] à [!DNL Workfront Fusion], vous devez récupérer une clé d’API et une clé d’application depuis votre compte [!DNL Datadog].

1. Connectez-vous à votre compte [!DNL Datadog].
1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Intégrations]**, puis sur **[!UICONTROL API]**.
1. Dans l’écran principal, cliquez sur **[!UICONTROL Clés d’API]**.
1. Pointez sur la barre violette pour faire apparaître la clé d’API.
1. Copiez la clé d’API dans un emplacement sécurisé.
1. Dans l’écran principal, cliquez sur **[!UICONTROL Clés d’application]**.
1. Pointez sur la barre violette pour faire apparaître la clé d’application.
1. Copiez la clé d’application dans un emplacement sécurisé.

### Créer une connexion à [!DNL Datadog] dans [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL Datadog] directement à partir d’un module [!UICONTROL Datadog].

1. Dans n’importe quel module [!UICONTROL Datadog], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Remplissez les champs du module comme suit :

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
      <td> <p> Saisissez un nom pour la connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>Sélectionnez le domaine auquel vous souhaitez vous connecter (US ou UE).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td> <p> Saisissez votre clé d’API [!DNL Datadog]. </p> <p>Pour obtenir des instructions sur la récupération de la clé d’API, consultez <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Récupérer votre clé d’API et votre clé d’application</a> dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application Key]</td> 
      <td> <p> Saisissez votre clé d’application [!DNL Datadog]. </p> <p>Pour savoir comment récupérer la clé d’application, voir <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Récupérer votre clé d’API et votre clé d’application</a> dans cet article.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Datadog] et leurs champs

Lorsque vous configurez les modules [!DNL Datadog], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Datadog] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez la section [Mappage des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Actions

* [[!UICONTROL Publier les points de la série chronologique]](#post-timeseries-points)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL Publier les points de la série chronologique]

Le module vous permet d’afficher des données de séries chronologiques qui peuvent être représentées sur les tableaux de bord de [!DNL Datadog].

La limite pour les payloads compressées est de 3,2 mégaoctets (3 200 000), et de 62 mégaoctets (62 914 560) pour les payloads décompressées.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Datadog] à [!DNL Workfront Fusion], voir <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Datadog] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Ajoutez les séries temporelles que vous souhaitez soumettre à [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metric]</strong> </p> <p>Entrez le nom de la série temporelle.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>Sélectionnez le type de mesure.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> Si le type de mesure est un taux ou un comptage, définissez l’intervalle correspondant.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>Ajoutez des points relatifs à une mesure.</p> <p>Il s’agit d’un tableau de points JSON. Chaque point a le format suivant : <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Note :  <p>L’horodatage doit être exprimé en secondes.</p> <p>L’horodatage doit être actuel. Le paramètre Actuel est défini sous forme de période n’allant pas au-delà de 10 minutes dans le futur ou d’une heure dans le passé.</p> <p> Le format de la valeur numérique doit être une valeur flottante.</p> </p> <p>Ce champ doit contenir au moins 1 élément.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Entrez le nom de l’hôte qui a produit la mesure.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Datadog] à [!DNL Workfront Fusion], consultez la section <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Datadog] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin d’accès relatif à <code>https://api.datadoghq.com/api/</code>. Exemple :<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, mettez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** l’appel API suivant renvoie tous les tableaux de bord de votre compte [!DNL Datadog] :

URL : `/v1/dashboard`

Méthode : `GET`

![](assets/datadog-api-example.png)

Le résultat se trouve dans la sortie du module sous Bundle > Body > dashboards.

Dans notre exemple, 3 tableaux de bord ont été renvoyés :

![](assets/datadog-api-response-example.png)
