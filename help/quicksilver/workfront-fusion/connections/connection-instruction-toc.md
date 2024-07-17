---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: connections-annd-webhooks
title: Création de connexions dans  [!DNL Adobe Workfront Fusion]
description: Une connexion doit respecter les exigences définies par l’API de l’application ou du service Web auquel elle se connecte. Pour cette raison, les instructions de configuration d’une connexion varient en fonction de l’application ou du service Web. Cet article peut vous aider à identifier et à localiser les instructions pour se connecter  [!DNL Adobe Workfront Fusion] à l’application ou au service Web de votre choix.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 11%

---

# Création de connexions dans [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

Une connexion doit respecter les exigences définies par l’API de l’application ou du service Web auquel elle se connecte. Pour cette raison, les instructions de configuration d’une connexion varient en fonction de l’application ou du service Web. Cet article peut vous aider à identifier et à localiser les instructions pour connecter [!DNL Adobe Workfront Fusion] à l’application ou au service Web de votre choix.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>N’importe quelle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>  
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>  
   <td> 
   <p>Actuel : aucune exigence de licence [!DNL Workfront Fusion].</p> 
   <p>Ou</p> 
   <p>Hérité : Tout </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produit</td>  
   <td> 
   <p>Nouveau :</p> <ul><li>Formule [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront] : [!DNL Workfront Fusion] est inclus.</li></ul> 
   <p>Ou</p> 
   <p>Actuel : votre organisation doit acheter [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connexion à une application ou à un service web qui ne nécessite pas de configuration

Dans la plupart des cas, vous pouvez utiliser le module pour créer une connexion avec peu ou pas d’informations supplémentaires. [!DNL Workfront Fusion] gère automatiquement l’authentification.

Pour obtenir des instructions sur la création d’une connexion sans considérations spéciales, voir [Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Connexion à une application ou à un service Web [!DNL Microsoft]

La plupart des applications [!DNL Microsoft] de [!DNL Workfront Fusion] vous permettent de créer une connexion sans informations supplémentaires.

Les cas suivants nécessitent des étapes supplémentaires pour créer une connexion :

* Utilisation de [!DNL Microsoft Dynamics 365] modules.

  Pour obtenir des instructions, voir [[!DNL Microsoft Dynamics 365] modules](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Connexion à [!DNL Microsoft Graph API] à l’aide d’un module [!UICONTROL HTTP]

  Pour plus d’informations, voir [Appel de  [!DNL MS Graph REST API]  via le  [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL  Créer une requête OAuth 2.0] module](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Connexion à une application ou à un service Web [!DNL Google]

Le processus de connexion aux applications [!DNL Google] peut différer en fonction du type de compte [!DNL Google] que vous utilisez. En outre, les mesures de sécurité [!DNL Google] peuvent nécessiter une configuration supplémentaire lorsque vous vous connectez à [!DNL Workfront Fusion].

Pour plus d’informations, voir :

* [Connectez-vous  [!DNL Adobe Workfront Fusion] à  [!DNL Google Services] à l’aide d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Connectez-vous  [!DNL Adobe Workfront Fusion] à  [!DNL Google Services] avec des mesures de sécurité mises à jour](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Autres applications nécessitant une configuration supplémentaire

Les applications suivantes ne suivent pas la configuration de base pour les connexions [!DNL Workfront Fusion]. Vous trouverez des instructions pour la connexion de ces applications dans l’article correspondant à cette application.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>App / Web Service</th> 
   <th>Informations supplémentaires sur les connexions</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Adobe Workfront] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Allocadia] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] modules</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref"> Connectez-vous [!DNL AWS] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref"> Connectez-vous [!DNL Azure DevOps] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Bynder] à [!DNL Workfront Fusion] </a> dans <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] modules</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Cvent] à [!DNL Adobe Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Datadog] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL DocuSign] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>E-mail</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Connectez votre email à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref"> Connectez-vous [!DNL Gmail] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Jira Cloud] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref"> Connectez-vous [!DNL Jira Server] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL MariaDB] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Marketo] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Microsoft Dynamics 365] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Connexion de [!DNL Qualtrics] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL ServiceNow] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Connectez SFTP à [!DNL Workfront Fusion]</a> dans les modules <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL SharePoint] à [!DNL Workfront Fusion]</a> dans <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Split.io] à [!DNL Workfront Fusion] </a> dans <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Widen</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref"> Connectez-vous [!DNL Widen] à [!DNL Workfront Fusion] </a> dans <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] modules</a></td> 
  </tr> 
 </tbody> 
</table>
