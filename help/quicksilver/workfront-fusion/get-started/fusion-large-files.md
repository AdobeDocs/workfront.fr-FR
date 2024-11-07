---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Utilisation de fichiers volumineux dans Adobe Workfront Fusion
description: La prise en charge des fichiers volumineux est actuellement disponible pour les connecteurs Workfront et HTTP.
author: Becky
feature: Workfront Fusion
source-git-commit: d9f7f1b9a97faf767965abce4f64c62cb9aad8d2
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 6%

---

# Utilisation de fichiers volumineux dans Adobe Workfront Fusion

Des fonctionnalités améliorées de transfert de données sont désormais disponibles dans Workfront Fusion, ce qui permet à des scénarios de traiter des fichiers beaucoup plus volumineux.

La fonctionnalité de fichiers volumineux n’est disponible que pour les clients Workfront Ultimate.

Pour gérer les fichiers plus volumineux, vos scénarios doivent être mis à jour.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>
   <td> <p>Nouveau : Ultmate</p> <p>Ou</p> <p>Actuel : non disponible</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuel : non disponible</p> </td> 
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
   <p>Nouveau : [!DNL Workfront Fusion] est inclus dans le plan Workfront Ultimate.</p> <p>Ou</p>
   <p>Actuel : non disponible</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Connecteurs prenant en charge les fichiers volumineux

Pour la version initiale, les connecteurs suivants prennent en charge les fichiers volumineux.

* Workfront > Télécharger le document
* Adobe Experience Manager Assets > Télécharger le document
* HTTP

D’autres connecteurs seront pris en charge dans les prochaines versions.

## Mise à jour de vos scénarios pour la gestion des fichiers volumineux

Le module Workfront > Télécharger le document a été modifié pour gérer les fichiers plus volumineux. L’ancienne version de ce module affiche désormais `(Legacy)` ajouté au nom du module. Dans la plupart des cas, le module hérité continuera à fonctionner.

Si vous envisagez d’utiliser des fichiers plus volumineux, nous vous recommandons de remplacer le module hérité par le nouveau module Télécharger le document . Le nouveau module Télécharger le document empêche les dépassements de délai et d’autres erreurs.

![Charger un document](assets/new-upload-document.png)

## Questions fréquentes

### Quelle est la nouvelle limite de taille de fichier ?

Les utilisateurs peuvent désormais traiter des fichiers dépassant la limite précédente de 1 Go, ce qui améliore l’efficacité et la productivité.  Bien que la plateforme puisse prendre en charge des fichiers individuels allant jusqu’à 15 Go pour une seule action (par exemple le téléchargement d’un fichier), d’autres facteurs affectent le transfert des données. La limite de taille de fichier d’une action unique dépend finalement du service Web auquel Fusion se connecte. Le transfert de données est le traitement total d’une seule exécution. Cela signifie que plusieurs actions d’une seule exécution contribuent au transfert total des données.

Fusion traite les fichiers jusqu&#39;à ce que la limite d&#39;exécution de 40 minutes soit atteinte. Dans votre scénario Fusion, le chargement, le téléchargement ou le traitement de fichiers volumineux peuvent prendre du temps. Bien qu’il n’existe aucune limite concernant la taille de fichier, la durée d’exécution du scénario est limitée à 40 minutes. Par conséquent, si l’exécution prend plus de 40 minutes avec des fichiers volumineux, le scénario échoue. Le temps d’exécution du scénario peut également être affecté par la taille du scénario, la complexité du module et la vitesse du réseau. Par conséquent, nous vous recommandons de tenir compte de ces aspects de vos scénarios lors de l’utilisation de fichiers volumineux.

### Comment fonctionne le nouveau transfert de fichier de Fusion ?

Lorsque Fusion traite les fichiers, les fichiers plus volumineux sont ajoutés au stockage persistant (compartiment S3 ou stockage Azure Blob). Lorsqu’un module Fusion exécute une action de fichier, comme télécharger ou télécharger, Fusion utilise le fichier dans le stockage persistant comme source plutôt que comme mémoire active.

### Puis-je travailler avec des fichiers plus volumineux à l’aide d’exécutions incomplètes ?

Oui, Fusion prend en charge les exécutions incomplètes avec des fichiers plus volumineux. Notez que les exécutions incomplètes sont de taille limitée pour une organisation et doivent être gérées activement.

### Puis-je utiliser des fichiers plus volumineux avec n’importe quel connecteur ?

Chaque connecteur Fusion doit être mis à jour pour prendre en charge les fichiers plus volumineux. Les connecteurs pris en charge sont Workfront, HTTP et AEM Assets. Les connecteurs de fusion sont toujours limités par la taille de fichier prise en charge par le service Web. Les limites de taille de fichier sont généralement incluses dans la documentation de l’API pour les points de terminaison de service Web qui téléchargent et chargent des fichiers.

### Cela a-t-il une incidence sur les opérations ?

Non, le nombre d&#39;opérations exécutées par un module est le même.

### Quand l’interface utilisateur de Fusion sera-t-elle mise à jour pour afficher les données de transfert de fichier ?

Nous travaillons activement à des mises à jour de l’interface utilisateur de Fusion pour le transfert de fichiers sur le tableau de bord et la page des détails de l’exécution du scénario, avec une version ciblée au 1er trimestre 2025.

### Quelles sont les façons de penser aux nouvelles limites de traitement des fichiers qui m’aideront à concevoir des scénarios ?

Concevoir un scénario pour qu’il fonctionne dans la limite d’exécution de 40 minutes peut sembler compliqué. Nous vous recommandons de garder à l’esprit les éléments suivants lors de la conception d’un scénario :

* **Comprendre les besoins de votre entreprise en termes de temps d’exécution** : la limite de plateforme de Fusion pour le temps d’exécution est de 40 minutes, mais la plupart des automatisations de processus d’entreprise sont censées s’exécuter beaucoup plus rapidement. Par exemple, les automatisations initiées par l’utilisateur avec poursuite dépendante des résultats devraient se terminer bien en dessous de la limite de 40 minutes.
* **Tenez compte du temps d’exécution lors de la conception de** : lors de la conception de votre scénario, il est essentiel de comprendre le temps d’exécution du module pour les actions de fichiers individuelles, telles que les chargements et les téléchargements. Ces connaissances vous aident à planifier des scénarios qui impliquent plusieurs actions de fichier.  Pour garantir la précision de votre conception, nous vous recommandons d’arrondir le délai d’exécution du module afin d’inclure une mémoire tampon.
Par exemple, si Fusion télécharge un document en 144 secondes (2,4 minutes), vous pouvez vous attendre à ce qu’une seule exécution puisse effectuer des actions similaires plusieurs fois. Dans cet exemple, l’exécution du module prend 144 secondes et vous devez prévoir 3 minutes d’exécution pour le téléchargement. Si vos besoins incluent à la fois un téléchargement et un téléchargement, le temps d’exécution prévu est d’environ 6 minutes. Notez que les temps d’exécution de fusion sont plafonnés à 40 minutes.

* **Consolidation des actions de fichier** : l’exemple le plus courant d’actions de fichier dans un scénario Fusion est un téléchargement et un chargement. La plupart des scénarios comportant uniquement ces deux actions s’exécuteront dans quelques minutes. Lorsque cela est possible, les concepteurs de Fusion doivent limiter leurs scénarios à un téléchargement et un chargement.

* **Calculez la taille à l’aide du panneau de mappage** : Workfront et d’autres services Web incluent la taille de fichier d’un fichier dans la sortie du module de téléchargement. Vous pouvez utiliser ces données pour filtrer les fichiers trop volumineux pour un chargement de module ou trop volumineux pour le temps d’exécution du scénario.

* **Isolez les actions de fichier dans leur propre scénario lors de l’utilisation de plusieurs fichiers** : les concepteurs de fusion doivent envisager d’isoler les actions de fichier dans des scénarios distincts. Par exemple, un scénario de fusion déclenché par une nouvelle requête Workfront avec plusieurs fichiers joints peut nécessiter une capacité de 30 fichiers au maximum. Étant donné que le chargement et le téléchargement de chaque fichier peuvent prendre jusqu’à 3 minutes, le traitement de tous les fichiers en une seule exécution dépasserait la limite d’exécution de 40 minutes de Fusion. La solution consiste à créer un scénario d’actions de fichier dédié à la gestion du téléchargement et du téléchargement de fichiers individuels. Le scénario déclenché par la requête effectue une itération sur les fichiers joints, en appelant le scénario d’actions de fichier pour chaque fichier à l’aide du module HTTP. Cette approche garantit que chaque fichier est traité dans les limites du temps d’exécution.

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




