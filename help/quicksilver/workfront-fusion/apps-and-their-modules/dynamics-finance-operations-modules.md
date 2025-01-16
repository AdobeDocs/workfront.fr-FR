---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Finances et opérations de Microsoft Dynamics 365
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 19b00ee8-dc05-4cde-9a76-d857090fa543
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 31%

---

# [!DNL Microsoft Dynamics 365 Finance and Operations modules]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules Finances et opérations de Microsoft Dynamics 365](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/dynamics-finance-operations-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft Dynamics 365] et le connecter à plusieurs applications et services tiers.

>[!NOTE]
>
>Le connecteur [!DNL Microsoft Dynamics 365 Finance and Operations] ne prend pas en charge [!DNL Dynamics 365].
>
>Pour les modules Microsoft Dynamics 365, voir [[!DNL Microsoft Dynamics 365 modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Créer une connexion

Pour créer une connexion pour vos modules Finances et opérations Microsoft Dynamics 365 :

1. Dans un module Finances et opérations de Microsoft Dynamics 365, cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion.

1. Remplissez les champs suivants :

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Indiquez si vous créez une connexion Dynamics Finance and Operations standard ou une connexion à l’aide d’un code d’autorisation.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Saisissez un nom pour cette connexion.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre ID client Dynamics Finance and Operations [!UICONTROL].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre clé secrète client Dynamics Finance and Operations [!UICONTROL]. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Tenant ID]</td>
        <td>Saisissez votre ID client Dynamics Finance and Operations.</td>
        </tr>
        <tr>
        <td role="rowheader">Ressource</td>
        <td>Saisissez l’URL de votre compte Dynamics Finance and Operations (sans https://)</td>
        </tr>
      </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.



## Modules Finances et opérations de Microsoft Dynamics 365 et leurs champs

>[!IMPORTANT]
>
>Les entités de données disponibles via l’API Dynamics 365 F&amp;O peuvent varier par instance. Si vous ne savez pas quelles entités sont disponibles via l’API, il est utile de parcourir les entités de votre instance à l’aide du point d’entrée « data ». Le point d&#39;entrée « data » dans Dynamics 365 Finance and Operations est l&#39;URL racine pour accéder aux services OData. Ce point d’entrée vous permet d’interagir avec diverses entités de données exposées par le système à l’aide des protocoles OData standard.
>
>Vous pouvez récupérer ces entités à l’aide du module d’appel API personnalisé.
>
><!--For more information -->



### Créer un élément d’entité

Ce module d&#39;action crée un nouvel élément d&#39;entité dans Microsoft Dynamics 365 Finance and Operations.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Pour plus d’informations sur la connexion de Microsoft Dynamics 365 Finance and Operations à [!DNL Workfront Fusion], voir <a href="#create-a-connection" class="MCXref xref">Création d’une connexion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Saisissez ou mappez le type d'entité Dynamics Finance and Operations que vous souhaitez créer.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Saisissez ou mappez un corps JSON contenant les données que vous souhaitez inclure dans le nouvel élément d’entité.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Supprimer l’élément d’entité

Ce module d&#39;action supprime un élément d&#39;entité de Dynamics Finance and Operations. L’élément est identifié par ses champs de clé de Principal.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Pour plus d’informations sur la connexion de Microsoft Dynamics 365 Finance and Operations à [!DNL Workfront Fusion], voir <a href="#create-a-connection" class="MCXref xref">Création d’une connexion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Saisissez ou mappez le type d'entité Dynamics Finance and Operations que vous souhaitez supprimer.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Champs de clé de Principal]</td>
     <td> Les champs de clé de Principal identifient l’élément. Pour chaque champ de clé primaire que vous souhaitez fournir, cliquez sur <b>Ajouter un élément</b> et saisissez ou mappez la clé et la valeur uniques qui identifient cet élément. </td> 
  </tr> 
 </tbody> 
</table>

### Effectuer un appel API personnalisé.

Ce module d&#39;action effectue un appel personnalisé à l&#39;API Dynamics Finance and Operations.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>Pour plus d’informations sur la connexion de Microsoft Dynamics 365 Finance and Operations à [!DNL Workfront Fusion], voir <a href="#create-a-connection" class="MCXref xref">Création d’une connexion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Saisissez un chemin d’accès relatif à votre URL Dynamics Finance and Operations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Cela détermine le type de contenu de la requête.</p> <p>Par exemple,<code> {"Content-type":"application/json"}</code></p> <p>Note : si vous obtenez des erreurs et qu’il est difficile de déterminer leur origine, envisagez de modifier les en-têtes en fonction de la documentation [!DNL Workfront]. Si votre appel API personnalisé renvoie une erreur de requête HTTP 422, essayez d’utiliser un en-tête <code>"Content-Type":"text/plain"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chaîne de requête]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> <p>Conseil : nous vous recommandons d’envoyer des informations via le corps JSON plutôt que sous forme de paramètres de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Élément d’entité de lecture

Ce module d&#39;action renvoie les données d&#39;un élément d&#39;entité. L’élément est identifié par ses champs de clé de Principal.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Pour plus d’informations sur la connexion de Microsoft Dynamics 365 Finance and Operations à [!DNL Workfront Fusion], voir <a href="#create-a-connection" class="MCXref xref">Création d’une connexion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Saisissez ou mappez le type d'entité Dynamics Finance and Operations que vous souhaitez lire.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Champs de clé de Principal]</td>
     <td> Les champs de clé de Principal identifient l’élément. Pour chaque champ de clé primaire que vous souhaitez fournir, cliquez sur <b>Ajouter un élément</b> et saisissez ou mappez la clé et la valeur uniques qui identifient cet élément. </td> 
  </tr> 
 </tbody> 
</table>

### Mettre à jour l’élément d’entité

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Pour plus d’informations sur la connexion de Microsoft Dynamics 365 Finance and Operations à [!DNL Workfront Fusion], voir <a href="#create-a-connection" class="MCXref xref">Création d’une connexion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Saisissez ou mappez le type d'entité Dynamics Finance and Operations à mettre à jour.</td> 
  </tr>  
  <tr> 
    <td>[!UICONTROL Champs de clé de Principal]</td>
     <td> Les champs de clé de Principal identifient l’élément. Pour chaque champ de clé primaire que vous souhaitez fournir, cliquez sur <b>Ajouter un élément</b> et saisissez ou mappez la clé et la valeur uniques qui identifient cet élément. </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Saisissez ou mappez un corps JSON contenant les données que vous souhaitez inclure dans le nouvel élément d’entité.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherche

Ce module de recherche renvoie les résultats en fonction des critères que vous spécifiez.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], voir <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Workfront] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entity]</td> 
   <td>Saisissez ou mappez le type d'entité Dynamics Finance and Operations que vous souhaitez rechercher.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Renseignez le champ avec lequel vous souhaitez effectuer une recherche, l’opérateur que vous souhaitez utiliser dans votre requête et la valeur que vous recherchez dans le champ.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sort by]</td> 
   <td> <p>Saisissez ou mappez le champ selon lequel vous souhaitez trier les résultats.</p> </td> 
  </tr> 
 </tbody> 
</table>


<!--

### List All

This module lists all records for a given entity.  The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
     <td>Choose the Dynamics Finance and Operations entity type that you want the module to list.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
     <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Record

This trigger module starts a scenario when a record of the given type is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
