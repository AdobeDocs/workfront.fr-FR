---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP &gt; Lancer une demande d’autorisation de clé API
description: Ceci [!DNL Adobe Workfront Fusion] Le module d’action envoie une requête HTTPS à une URL spécifiée qui nécessite une autorisation API Key Auth et traite la réponse.
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 0%

---

# HTTP >[!UICONTROL Lancer une demande d’autorisation de clé API]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une [!DNL Adobe Workfront Fusion] en plus d’une licence Adobe Workfront.

Ceci [!DNL Adobe Workfront Fusion] Le module d’action envoie une requête HTTPS à une URL spécifiée qui nécessite une autorisation API Key Auth et traite la réponse.

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
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!UICONTROL Adobe Workfront Fusion] licences, voir [Licences Adobe Workfront Fusion](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Lancer une demande d’autorisation de clé API] configuration du module

Lorsque vous configurez la variable [!UICONTROL HTTP] >[!UICONTROL Lancer une demande d’autorisation de clé API] module, [!DNL Adobe Workfront Fusion] affiche les champs répertoriés ci-dessous. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credentials]</td> 
   <td> <p>Sélectionnez la clé contenant vos informations d’authentification de clé API. Pour ajouter une nouvelle clé, cliquez sur <strong>[!UICONTROL Ajouter]</strong> et configurez les informations suivantes :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom de la clé]</strong></p> <p>Saisissez un nom pour cet ensemble d’informations d’identification d’API.</p> </li> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Saisissez la clé API.</p> </li> 
     <li> <p><strong>[!UICONTROL Emplacement de la clé API]</strong> </p> <p>Indiquez si la clé API doit être placée dans l’en-tête ou dans la requête de l’appel API.</p> </li> 
     <li> <p><strong>[!UICONTROL Nom du paramètre de clé API]</strong> </p> <p>Saisissez le nom sous lequel l’appel API identifie la clé API, par exemple "apiKey" ou "X-API-Key". Vous trouverez ces informations dans la documentation du service Web auquel le module se connecte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Évaluer tous les états comme des erreurs (sauf 2xx et 3xx)] </td> 
   <td> <p>Utilisez cette option pour configurer la gestion des erreurs.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Gestion des erreurs dans Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Saisissez l’URL à laquelle vous souhaitez envoyer une requête, par exemple un point de terminaison API, un site web, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode [!UICONTROL]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Entrez les paires clé-valeur de requête souhaitées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type de corps]</p> </td> 
   <td> <p>Le corps HTTP est l’octet de données transmis dans un message de transaction HTTP immédiatement après les en-têtes s’il y a un élément à utiliser.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Le type de corps brut est généralement adapté à la plupart des requêtes de corps HTTP, même dans les cas où la documentation du développeur ne spécifie aucune donnée à envoyer.</p> <p>Spécifiez un formulaire d’analyse des données dans le champ [!UICONTROL Type de contenu] .</p> <p>Malgré le type de contenu sélectionné, le module saisit les données dans n’importe quel format requis par la documentation destinée aux développeurs.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Ce type de corps est destiné aux données [!UICONTROL POST] qui utilisent <code>application/x-www-form-urlencoded</code>.</p> <p>Pour <code>[!UICONTROL application/x-www-form-urlencoded]</code>, le corps du message HTTP envoyé au serveur est essentiellement une chaîne de requête. Les clés et les valeurs sont codées dans des paires clé-valeur séparées par <code>&amp;</code> et avec un <code>=</code> entre la clé et la valeur. </p> <p>Pour les données binaires, utilisez <code>[!UICONTROL multipart/form-data]</code> au lieu de .</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Exemple: </b></span></span> 
       <p>Exemple du format de requête HTTP obtenu :</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] est une requête HTTP multipart utilisée pour envoyer des fichiers et des données. Il est généralement utilisé pour charger des fichiers sur le serveur.</p> <p>Ajoutez les champs à envoyer dans la requête. Chaque champ doit contenir une paire clé-valeur.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Texte]</strong> </p> <p>Saisissez la clé et la valeur à envoyer dans le corps de la requête.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Saisissez la clé et indiquez le fichier source à envoyer dans le corps de la requête.</p> <p>Mappez le fichier que vous souhaitez charger à partir du module précédent (par exemple [!UICONTROL HTTP] &gt;[!UICONTROL Obtenir un fichier] ou [!UICONTROL Google Drive] &gt;[!UICONTROL Télécharger un fichier]), ou saisissez manuellement le nom du fichier et les données du fichier.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Réponse d’analyse]</p> </td> 
   <td> <p>Activez cette option pour analyser automatiquement les réponses et convertir les réponses JSON et XML afin que vous n’ayez pas à utiliser les modules [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] ou [!UICONTROL XML] &gt; [!UICONTROL Parse XML].</p> <p>Avant de pouvoir utiliser du contenu JSON ou XML analysé, exécutez le module une fois manuellement afin que le module puisse reconnaître le contenu de la réponse et vous permettre de le mapper dans les modules suivants.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Spécifiez le délai d’expiration de la requête en secondes (1 à 300). La valeur par défaut est de 40 secondes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partage de cookies avec d’autres modules HTTP]</td> 
   <td> <p> Activez cette option pour partager les cookies du serveur avec tous les modules HTTP de votre scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificat auto-signé]</td> 
   <td> <p> Téléchargez votre certificat si vous souhaitez utiliser TLS à l’aide de votre certificat auto-signé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rejeter les connexions qui utilisent des certificats non vérifiés (auto-signés)] </td> 
   <td> <p>Activez cette option pour rejeter les connexions qui utilisent des certificats TLS non vérifiés.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suivre la redirection]</td> 
   <td> <p> Activez cette option pour suivre les redirections d’URL avec les réponses 3xx.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suivre toutes les redirections] </td> 
   <td> <p>Activez cette option pour suivre les redirections d’URL avec tous les codes de réponse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Désactivation de la sérialisation de plusieurs mêmes clés de chaîne de requête en tant que tableaux]</p> </td> 
   <td> <p>Par défaut, [!DNL Workfront Fusion] gère plusieurs valeurs pour la même clé de paramètre de chaîne de requête d’URL que les tableaux. Par exemple : <code>www.test.com?foo=bar&amp;foo=baz</code> sera converti en <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Activez cette option pour désactiver cette fonction. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Demander du contenu compressé]</td> 
   <td> <p> Activez cette option pour demander une version compressée du site web.</p> <p>Ajoute un <code>[!UICONTROL Accept-Encoding]</code> pour demander du contenu compressé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Utiliser TLS Mutuel]</td> 
   <td> <p>Activez cette option pour utiliser le protocole TLS mutuel dans la requête HTTP.</p> <p>Pour plus d’informations sur le protocole TLS mutuel, voir <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Utilisation de TLS mutuel dans les modules HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
