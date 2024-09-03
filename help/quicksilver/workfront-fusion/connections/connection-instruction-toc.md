---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: connections-annd-webhooks
title: Créer des connexions dans  [!DNL Adobe Workfront Fusion]
description: Une connexion doit respecter les exigences définies par l’API de l’application ou du service web auquel elle se connecte. Pour cette raison, les instructions de configuration d’une connexion varient en fonction de l’application ou du service web. Cet article peut vous aider à identifier et à localiser les instructions pour connecter  [!DNL Adobe Workfront Fusion]  à l’application ou au service web de votre choix.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 100%

---

# Créer des connexions dans [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

Une connexion doit respecter les exigences définies par l’API de l’application ou du service web auquel elle se connecte. Pour cette raison, les instructions de configuration d’une connexion varient en fonction de l’application ou du service web. Cet article peut vous aider à identifier et à localiser les instructions pour connecter [!DNL Adobe Workfront Fusion] à l’application ou au service web de votre choix.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Tous</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>  
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>  
   <td> 
   <p>Actuelle : aucune exigence de licence [!DNL Workfront Fusion] requise.</p> 
   <p>Ou</p> 
   <p>Héritée : n’importe laquelle. </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produit</td>  
   <td> 
   <p>Nouveau :</p> <ul><li>Forfait [!DNL Workfront] [!UICONTROL Select] ou [!UICONTROL Prime] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Forfait [!DNL Workfront] [!UICONTROL Ultimate] : [!DNL Workfront Fusion] est inclus.</li></ul> 
   <p>Ou</p> 
   <p>Actuel : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Se connecter à une application ou à un service web qui ne nécessite pas de configuration.

Dans la plupart des cas, vous pouvez utiliser le module pour créer une connexion avec peu ou pas d’informations supplémentaires. [!DNL Workfront Fusion] gère automatiquement l’authentification.

Pour plus d’informations sur la création d’une connexion sans considérations spéciales, voir [Créer une connexion à  [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Se connecter à une application ou service web [!DNL Microsoft]

La plupart des applications [!DNL Microsoft] dans [!DNL Workfront Fusion] vous permettent de créer une connexion sans informations supplémentaires.

Dans les cas suivants, la création de la connexion requiert des étapes supplémentaires :

* L’utilisation de modules [!DNL Microsoft Dynamics 365].

  Pour obtenir des instructions, voir Modules [[!DNL Microsoft Dynamics 365] ](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* La connexion à l’[!DNL Microsoft Graph API] avec un module [!UICONTROL HTTP].

  Pour obtenir des instructions, voir [Appelez l’ [!DNL MS Graph REST API]  via le module  [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Se connecter à une application ou un service web [!DNL Google]

Le processus pour se connecter à des applications [!DNL Google] peut varier en fonction du type compte [!DNL Google] que vous utilisez. En outre, les mesures de sécurité [!DNL Google] peuvent nécessiter une configuration supplémentaire lorsque vous vous connectez à [!DNL Workfront Fusion].

Pour plus d’informations, voir ce qui suit :

* [Connecter  [!DNL Adobe Workfront Fusion]  à  [!DNL Google Services]  avec un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Connecter  [!DNL Adobe Workfront Fusion]  à  [!DNL Google Services]  avec des mesures de sécurité mises à jour](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Autres applications nécessitant une configuration supplémentaire

Les applications suivantes ne suivent pas la configuration de base des connexions [!DNL Workfront Fusion]. Vous trouverez des instructions pour la connexion de ces applications dans l’article correspondant à cette application.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Application/service web</th> 
   <th>Informations supplémentaires sur les connexions</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Connecter [!DNL Adobe Workfront] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Connecter [!DNL Allocadia] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Connecter [!DNL AWS] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Connecter [!DNL Azure DevOps] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Connecter [!DNL Bynder] à [!DNL Workfront Fusion] </a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Connecter [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Connecter [!DNL Datadog] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Connecter [!DNL DocuSign] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>E-mail</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Connectez votre adresse e-mail à [!DNL Workfront Fusion]</a> dans les modules [!UICONTROL Email]<a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref"></a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Connecter [!DNL Gmail] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Connecter [!DNL Jira Cloud] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Connecter [!DNL Jira Server] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Connecter [!DNL MariaDB] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Connecter [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Connecter [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Connecter [!DNL Qualtrics] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Connecter [!DNL ServiceNow] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Connecter SFTP à [!DNL Workfront Fusion]</a> dans les modules [!UICONTROL SFTP]<a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref"></a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Connecter [!DNL SharePoint] à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Connecter [!DNL Split.io] à [!DNL Workfront Fusion] </a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Widen</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Connecter [!DNL Widen] à [!DNL Workfront Fusion] </a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen]</a></td> 
  </tr> 
 </tbody> 
</table>
