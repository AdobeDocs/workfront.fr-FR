---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Utilisation de fichiers volumineux dans Adobe Workfront Fusion
description: La prise en charge des fichiers volumineux est actuellement disponible pour les connecteurs Workfront et HTTP.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: 630467ca64281df0b257dae8cc5c6edc55ae56ad
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# Utilisation de fichiers volumineux dans Adobe Workfront Fusion

Certains connecteurs Fusion peuvent prendre en charge un fichier dont la taille est supérieure à la limite de 1 Go.

## Connecteurs prenant en charge les fichiers volumineux

La prise en charge des fichiers volumineux est actuellement disponible pour les connecteurs suivants :

* Workfront
* HTTP

## Effet de grande taille de fichier sur le temps d’exécution du scénario

Dans votre scénario Fusion, le chargement, le téléchargement ou le traitement de fichiers volumineux peuvent prendre du temps. Bien qu’il n’y ait aucune limite sur la taille du fichier, la durée d’exécution du scénario est limitée à 40 minutes. Par conséquent, si l’exécution prend plus de 40 minutes avec des fichiers volumineux, le scénario échoue.

Le temps d’exécution du scénario peut également être affecté par la taille du scénario, la complexité du module et la vitesse du réseau. Par conséquent, nous vous recommandons de tenir compte de ces aspects de vos scénarios lors de l’utilisation de fichiers volumineux.


<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom









If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->