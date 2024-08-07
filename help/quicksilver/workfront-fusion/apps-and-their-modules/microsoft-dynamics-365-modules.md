---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Microsoft Dynamics 365
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Microsoft Dynamics 365, et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 37%

---

# [!DNL Microsoft Dynamics 365 modules]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft Dynamics 365] et les connecter à plusieurs applications et services tiers.

>[!NOTE]
>
>Le connecteur [!DNL Microsoft Dynamics 365] ne prend pas en charge [!DNL Dynamics Finance and Operations].

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

Pour utiliser [!DNL Microsoft Dynamics] 365, vous devez disposer d&#39;un compte [!DNL Microsoft Dynamics 365].

## Connexion de Microsoft Dynamics 365 à Workfront Fusion

Vous pouvez créer une connexion à votre compte [!DNL Microsoft Dynamics 365] directement depuis un module [!DNL Microsoft Dynamics 365].

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations utilisateur individuelles. Par conséquent, lors de la création d’une connexion, l’écran de consentement des autorisations affiche les autorisations qui ont été accordées à la connexion de cet utilisateur, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur dispose d’autorisations &quot;Lecture de tableau&quot; accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les emails, l’écran de consentement des autorisations affiche à la fois l’autorisation &quot;Lecture de tableau&quot; déjà accordée et l’autorisation &quot;Ecriture d’email&quot; nouvellement requise.

1. Dans un module [!DNL Microsoft Dynamics 365], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Saisissez le nom de la connexion.
1. Dans le champ **[!UICONTROL Resource]** , saisissez l’adresse de votre compte [!DNL Dynamics 365], sans `https://`.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

>[!NOTE]
>
>Lors de l’enregistrement de [!DNL Workfront Fusion] sur votre portail [!DNL Microsoft Azure], utilisez l’URI de redirection suivant :
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## Modules [!DNL Microsoft Dynamics 365] et leurs champs

Lorsque vous configurez des modules [!DNL Microsoft Dynamics 365], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Microsoft Dynamics 365] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Surveiller les enregistrements (planifiés)]](#watch-records-scheduled)
* [[!UICONTROL Surveiller les enregistrements (temps réel)]](#watch-records-real-time)
* [[!UICONTROL Créer un enregistrement]](#create-record)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)
* [[!UICONTROL Supprimer l’enregistrement]](#delete-record)
* [[!UICONTROL Lecture d’enregistrements]](#read-records)
* [[!UICONTROL Mettre à jour l’enregistrement]](#update-record)
* [[!UICONTROL Enregistrements de recherche]](#search-records)

### [!UICONTROL Surveiller les enregistrements (planifiés)]

Ce module de déclenchement planifié exécute un scénario lorsqu’un enregistrement dans l’objet que vous spécifiez est créé ou mis à jour après la dernière exécution planifiée dans [!DNL Dynamics 365].

La sortie du module indique si l’enregistrement trouvé est nouveau ou mis à jour (s’il a été ajouté et mis à jour au cours de la période, il est marqué comme nouveau). Vous pouvez mapper ces informations dans les modules suivants du scénario.

Cela se produit dans un intervalle régulièrement planifié que vous spécifiez.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Indiquez si vous souhaitez que le module surveille <strong>[!UICONTROL Uniquement les nouveaux enregistrements]</strong>, <strong>[!UICONTROL Enregistrements mis à jour uniquement]</strong> ou <strong>[!UICONTROL Nouveaux enregistrements et modifications]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’enregistrement [!UICONTROL Microsoft Dynamics 365] que vous souhaitez voir dans le scénario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nb max. d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Surveiller les enregistrements (temps réel)]

Ce module de déclenchement instantané exécute un scénario lorsqu’un enregistrement (objet) que vous spécifiez est créé ou mis à jour dans [!DNL Dynamics 365].

Un webhook est requis dans ce module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez le webhook que vous souhaitez utiliser pour ce module. </p> <p>Pour ajouter un nouveau webhook :</p> 
    <ol> 
     <li value="1"> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong> à droite du champ Webhook.</p> </li> 
     <li value="2"> <p>Dans le champ de nom <strong>[!UICONTROL Webhook]</strong>, saisissez un nom explicite pour le webhook.</p> </li> 
     <li value="3"> <p>Dans le champ <strong>[!UICONTROL Connection]</strong> , sélectionnez la connexion que vous souhaitez utiliser</p> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </li> 
     <li value="4"> <p>Cliquez sur <strong>[!UICONTROL Enregistrer]</strong> pour enregistrer votre webhook et revenir au module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Créer un enregistrement]

Ce module d’action crée une entité, telle qu’un rendez-vous ou une tâche.

Vous spécifiez des informations sur l’entité que vous souhaitez créer.

Le module renvoie l’identifiant de la nouvelle entité et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’entité que vous souhaitez que le module crée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner les champs à mapper]</td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez inclure des valeurs lors de la création de l’enregistrement. Les champs disponibles dépendent du type d’entité.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Champs de propriété]</td> 
   <td> Il s’agit des champs que vous avez sélectionnés. Saisissez la valeur que l’enregistrement doit avoir pour une propriété donnée. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Microsoft Dynamics 365]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Microsoft Dynamics 365].

Le module renvoie des informations sur le code d’état, les en-têtes et le corps. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Pour en savoir plus, consultez la documentation [!DNL Microsoft] sur l’utilisation de [!DNL Dynamics 365 Customer Engagement Web API].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin relatif à <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> <p>Pour en savoir plus, voir</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
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

### [!UICONTROL Supprimer l’enregistrement]

Ce module d’action supprime une entité.

Vous spécifiez l’identifiant de l’entité.

Le module renvoie l’identifiant de l’entité et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td> <p>Sélectionnez le type d’entité que vous souhaitez que le module supprime.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant unique [!DNL Microsoft Dynamics 365] de l’enregistrement que vous souhaitez que le module supprime.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lecture d’enregistrements]

Ce module d’action lit les données d’une seule entité dans [!DNL Microsoft Dynamics 365].

Vous spécifiez l’identifiant de l’entité.

Le module renvoie l’identifiant de l’entité et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’entité que vous souhaitez que le module lise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant unique [!DNL Microsoft Dynamics 365] de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour l’enregistrement]

Ce module d’action met à jour une entité.

Vous spécifiez l’identifiant de l’entité.

Le module renvoie l’identifiant de l’enregistrement mis à jour et les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’entité que le module doit mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner les champs à mapper]</td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez inclure des valeurs lors de la création de l’enregistrement. Les champs disponibles dépendent du type d’entité.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Champs de propriété]</td> 
   <td>Il s’agit des champs que vous avez sélectionnés. Saisissez la valeur que l’enregistrement doit avoir pour une propriété donnée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l'identifiant unique [!DNL Microsoft Dynamics] 365 de l'enregistrement que vous souhaitez que le module soit mis à jour.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Enregistrements de recherche]

Ce module de recherche recherche recherche des enregistrements dans un objet de [!DNL Microsoft Dynamics 365] correspondant à la requête de recherche que vous spécifiez. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connexion [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’entité]</td> 
   <td>Sélectionnez le type d’entité que le module doit mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtres]</td> 
   <td> <p>Sélectionnez le filtre à utiliser pour cette recherche.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtres standard]</strong> </p> <p>Configurez le filtre en sélectionnant un champ et un opérateur, puis en saisissant ou en associant la valeur à rechercher. Vous pouvez utiliser des règles ET ou OU pour votre filtre.</p> </li> 
     <li> <p><strong>[!UICONTROL Fonctions De Requête]</strong> </p> <p>Saisissez la fonction de requête de l’API web [!DNL Dynamics 365] que vous souhaitez utiliser pour la recherche. </p> <p>Pour plus d’informations sur les fonctions de requête, consultez la <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">référence sur les fonctions de requête de l’API web</a> dans la documentation [!DNL Microsoft].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>Indiquez l’ordre dans lequel les éléments sont renvoyés. Vous pouvez ajouter plusieurs types.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Indiquez le champ de tri des résultats.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Définissez la direction du tri (ascendant ou descendant).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nb max. d’enregistrements]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
 </tbody> 
</table>
