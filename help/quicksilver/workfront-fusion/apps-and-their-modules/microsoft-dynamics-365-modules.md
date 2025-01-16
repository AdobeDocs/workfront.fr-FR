---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Microsoft Dynamics 365
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 93%

---

# [!DNL Microsoft Dynamics 365 modules]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules Microsoft Dynamics 365](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-dynamics-365-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft Dynamics 365] et le connecter à plusieurs applications et services tiers.

>[!NOTE]
>
>Le connecteur [!DNL Microsoft Dynamics 365] ne prend pas en charge [!DNL Dynamics Finance and Operations].
>
>Pour les modules Finances et opérations de Microsoft Dynamics 365, voir [[!DNL Microsoft Dynamics 365 Finance and Operations modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/dynamics-finance-operations-modules.md).

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Pour utiliser [!DNL Microsoft Dynamics] 365, vous devez avoir un compte [!DNL Microsoft Dynamics 365].

## Connecter Microsoft Dynamics 365 à Workfront Fusion

Vous pouvez créer une connexion à votre compte [!DNL Microsoft Dynamics 365] directement à partir d’un module [!DNL Microsoft Dynamics 365].

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations d’utilisateur ou d’utilisatrice. Ainsi, lors de la création d’une connexion, l’écran de consentement aux autorisations affiche les autorisations précédemment accordées à la connexion de cet utilisateur ou de cette utilisatrice, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur ou une utilisatrice dispose d’autorisations « Lire le tableau » accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les e-mails, l’écran de consentement aux autorisations affiche à la fois l’autorisation « Lire le tableau » déjà accordée et l’autorisation « Écrire des e-mails » nouvellement requise.

1. Dans un module [!DNL Microsoft Dynamics 365], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Saisissez un nom pour la connexion.
1. Dans le champ **[!UICONTROL Ressource]**, saisissez l’adresse de votre compte [!DNL Dynamics 365], sans `https://`.
1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module.

>[!NOTE]
>
>Lors de l’enregistrement de [!DNL Workfront Fusion] dans votre portail [!DNL Microsoft Azure], utilisez l’URI de redirection suivant :
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## Modules [!DNL Microsoft Dynamics 365] et leurs champs

Lorsque vous configurez les modules [!DNL Microsoft Dynamics 365], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Microsoft Dynamics 365] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Surveiller des enregistrements (prévus)]](#watch-records-scheduled)
* [[!UICONTROL Surveillee des enregistrements (temps réel)]](#watch-records-real-time)
* [[!UICONTROL Créer un enregistrement]](#create-record)
* [[!UICONTROL Lancer un appel API]](#make-an-api-call)
* [[!UICONTROL Supprimer un enregistrement]](#delete-record)
* [[!UICONTROL Lire des enregistrements]](#read-records)
* [[!UICONTROL Mettre à jour des enregistrements]](#update-record)
* [[!UICONTROL Rechercher des enregistrements]](#search-records)

### [!UICONTROL Surveiller des enregistrements (prévus)]

Ce module de déclenchement prévu exécute un scénario lorsqu’un enregistrement dans l’objet que vous spécifiez est créé ou mis à jour après la dernière exécution prévue dans [!DNL Dynamics 365].

La sortie du module indique si l’enregistrement trouvé est nouveau ou mis à jour (s’il a été ajouté et mis à jour au cours de la période, il est marqué comme nouveau). Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Cela se produit à un intervalle planifié régulier que vous spécifiez.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour savoir comment connecter votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], consultez la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Sélectionnez si le module doit surveiller <strong>[!UICONTROL Only new records]</strong>, <strong>[!UICONTROL Updated records only]</strong> ou <strong>[!UICONTROL New records and all changes]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Sélectionnez le type d’enregistrement [!UICONTROL Microsoft Dynamics 365] que vous souhaitez que le scénario surveille.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Surveiller des enregistrements (en temps réel)]

Ce module de déclenchement instantané exécute un scénario lorsqu’un enregistrement (objet) que vous spécifiez est créé ou mis à jour dans [!DNL Dynamics 365].

Un webhook est nécessaire pour ce module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez le webhook que vous souhaitez utiliser pour ce module. </p> <p>Pour ajouter un nouveau webhook :</p> 
    <ol> 
     <li value="1"> <p>Cliquez sur <strong>[!UICONTROL Add]</strong> à droite du champ Webhook.</p> </li> 
     <li value="2"> <p>Dans le champ Nom du <strong>[!UICONTROL Webhook]</strong>, saisissez un nom explicite pour le webhook.</p> </li> 
     <li value="3"> <p>Dans le champ <strong>[!UICONTROL Connection]</strong>, sélectionnez la connexion que vous souhaitez utiliser.</p> <p>Pour savoir comment connecter votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], voir <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans cet article. </p> </li> 
     <li value="4"> <p>Cliquez sur <strong>[!UICONTROL Save]</strong> pour enregistrer votre webhook et revenir au module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Créer un enregistrement]

Ce module d’action crée une entité, telle qu’un rendez-vous ou une tâche.

Vous spécifiez des informations sur l’entité que vous souhaitez créer.

Le module renvoie l’ID de la nouvelle entité et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], voir <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Sélectionnez le type d’entité que vous souhaitez que le module crée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select Fields to Map]</td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez inclure des valeurs lors de la création de l’enregistrement. Les champs disponibles dépendent du type d’entité.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td> Il s’agit des champs que vous avez sélectionnés. Saisissez la valeur que vous souhaitez donner à l’enregistrement pour une propriété donnée. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Réaliser un appel API]

Ce module d’action permet d’effectuer un appel authentifié personnalisé vers l’API [!DNL Microsoft Dynamics 365]. De cette façon, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Microsoft Dynamics 365].

Le module renvoie des informations sur le code d’état, les en-têtes et le corps. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Pour en savoir plus, consultez la documentation [!DNL Microsoft] sur l’utilisation de [!DNL Dynamics 365 Customer Engagement Web API].

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], consultez la section <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin d’accès relatif à <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> <p>Pour en savoir plus, voir</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer l’enregistrement]

Ce module d’action supprime une entité.

Vous spécifiez l’identifiant de l’entité.

Le module renvoie l’identifiant de l’entité et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], voir <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>Sélectionnez le type d’entité que vous souhaitez que le module supprime.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant [!DNL Microsoft Dynamics 365] unique de l’enregistrement que vous souhaitez que le module supprime.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lire les enregistrements]

Ce module d’action lit les données d’une seule entité dans [!DNL Microsoft Dynamics 365].

Vous spécifiez l’identifiant de l’entité.

Le module renvoie l’identifiant de l’entité et tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], voir <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Sélectionnez le type d’entité que vous souhaitez que le module lise.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant [!DNL Microsoft Dynamics 365] unique de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour une entité.

Vous spécifiez l’identifiant de l’entité.

Le module renvoie l’identifiant de l’enregistrement mis à jour et les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], voir <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans cet article. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Sélectionnez le type d’entité que le module doit mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select Fields to Map]</td> 
   <td>Sélectionnez les champs pour lesquels vous souhaitez inclure des valeurs lors de la création de l’enregistrement. Les champs disponibles dépendent du type d’entité.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>Il s’agit des champs que vous avez sélectionnés. Saisissez la valeur que vous souhaitez donner à l’enregistrement pour une propriété donnée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant unique [!DNL Microsoft Dynamics] 365 de l’enregistrement que le module doit mettre à jour.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Rechercher des enregistrements]

Ce module de recherche trouve des enregistrements dans un objet de [!DNL Microsoft Dynamics 365] qui correspondent à la requête que vous spécifiez. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion], voir <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans cet article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Sélectionnez le type d’entité que le module doit mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>Sélectionnez le filtre à utiliser pour cette recherche.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standard Filters]</strong> </p> <p>Configurez le filtre en sélectionnant un champ et un opérateur, puis en saisissant ou en mappant la valeur à rechercher. Vous pouvez utiliser des règles AND ou OR pour votre filtre.</p> </li> 
     <li> <p><strong>[!UICONTROL Query Functions]</strong> </p> <p>Saisissez la fonction de requête de l’API web [!DNL Dynamics 365] que vous souhaitez utiliser pour la recherche. </p> <p>Pour plus d’informations sur les fonctions de requête, voir <a href="https://docs.microsoft.com/fr-fr/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Référence de fonction de requête d’API Web</a> dans la documentation [!DNL Microsoft].</p> </li> 
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
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
 </tbody> 
</table>
