---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Module SOAP
description: Vous pouvez utiliser le module SOAP pour vous connecter aux API SOAP dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 94%

---

# Module [!UICONTROL SOAP]

Vous pouvez utiliser le module [!UICONTROL SOAP] pour vous connecter aux API [!UICONTROL SOAP] dans [!UICONTROL Adobe Workfront Fusion].

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
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Restrictions du module [!UICONTROL SOAP]

>[!NOTE]
>
>Les redirections sont désactivées pendant le chargement du WDSL. Il s’agit d’une fonctionnalité de sécurité, mais cela peut signifier que les redirections non vérifiées sont bloquées lors de l’exécution du module.

Le module [!UICONTROL SOAP] est actuellement en version Beta et ne prend pas en charge :

* les éléments de redéfinition ;
* les restrictions relatives aux chiffres des fractions ;
* les restrictions relatives aux chiffres totaux ;
* les restrictions relatives aux espaces blancs ;
* plusieurs parties dans les messages d’entrée et de sortie, seuls les messages en une seule partie sont pris en charge ;
* les éléments de schéma XML personnalisés définis à l’aide des schémas et éléments d’[[!UICONTROL encodage] SOAP](https://schemas.xmlsoap.org).

>[!INFO]
>
>**Exemple :**
>  
>Les éléments suivants ne sont pas correctement reconnus par [!UICONTROL Workfront Fusion] :
>
>```
><complexType name="ArrayOfFloat">
>     <complexContent>
>           <restriction base="soapenc:Array">
>                 <attribute ref="soapenc:arrayType"
>                       wsdl:arrayType="xsd:integer[]"/>
>           </restriction>
>     </complexContent>
></complexType>
>```
>
>Cet exemple inclut les références `soapenc:Array`, `soapenc:arrayType` et `wsdl:arrayType` qui ne sont pas encore prises en charge dans [!UICONTROL Workfront Fusion].

## Solution de contournement

Si le module [!UICONTROL SOAP] refuse de traiter le fichier WSDL ou renvoie diverses erreurs dans la configuration du module, vous pouvez essayer d’utiliser le module universel **[!UICONTROL HTTP] > [!UICONTROL Effectuer une requête]** à la place :

1. Dans [!DNL Workfront Fusion], créez un scénario.
1. Insérez le module **[!UICONTROL HTTP] > [!UICONTROL Effectuer une requête]** dans le scénario.
1. Ouvrez la configuration du module et renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL Enabled]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Ouvrez une nouvelle fenêtre ou un nouvel onglet du navigateur web.
1. Collez l’URL WSDL dans la barre d’adresse du navigateur web et récupérez le fichier XML.

   L’URL WSDL se termine généralement par `?wsdl`, mais pas nécessairement, par exemple `http://voip.ms/api/v1/server.wsdl`.

1. Si le fichier WSDL ne s’affiche pas directement dans le navigateur web, ouvrez le fichier téléchargé dans un éditeur de texte.
1. Recherchez la balise `<service>` ou `<wsdl:service>` :

   ![](assets/service-350x65.png)

1. Une fois localisée, copiez l’URL à partir de l’attribut `location`.
1. Dans [!DNL Workfront Fusion], collez l’URL dans le champ URL du module HTTP.
1. Ouvrez le [Client [!UICONTROL SOAP] en ligne](https://wsdlbrowser.com/) dans une nouvelle fenêtre ou un nouvel onglet du navigateur web.
1. Collez l’URL WSDL dans le champ URL WSDL.
1. Cliquez sur **[!UICONTROL Parcourir]**.
1. Faites votre choix dans la liste des fonctions située à gauche, par exemple `getLanguages`.
1. Copiez le contenu de la zone de texte [!UICONTROL Requête XML].
1. Dans [!UICONTROL Workfront Fusion], collez le contenu copié dans le champ URL du module.
1. Indiquez des valeurs pour les paramètres sélectionnés en remplaçant les points d’interrogation par des valeurs réelles :

   ![](assets/request-xml-350x172.png)

1. Fermez la configuration du module en cliquant sur **[!UICONTROL OK]**.
1. Exécutez le scénario ou le module.
