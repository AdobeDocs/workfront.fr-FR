---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: http-modules
title: Utiliser TLS mutuel dans les modules HTTP d’Adobe Workfront Fusion
description: Vous pouvez utiliser le protocole TLS mutuel dans vos modules HTTP Fusion Adobe Workfront, ce qui permet aux deux côtés de la transaction d’information de vérifier l’identité de l’autre.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: d2baef04d0a02a2a73dbe1dd4c46cb49a75a0d5e
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 18%

---

# Utilisation de TLS mutuel dans les modules HTTP dans [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une licence Adobe Workfront.

## Présentation de TLS mutuel

Lorsque vous envoyez des données sur Internet, il est important de vous assurer qu’elles arrivent ou qu’elles proviennent du bon emplacement et que seul le destinataire prévu peut les lire. Lorsque TLS est activé, le client (ordinateur demandant des informations) utilise des certificats pour vérifier l’identité du serveur (ordinateur fournissant des informations). Cela permet de sécuriser les connexions HTTP.

TLS mutuel permet à cette confirmation d’identité de se dérouler dans les deux sens. Lorsque le serveur envoie son certificat pour vérifier son identité au client, il demande également le certificat du client. Cela permet de s’assurer que le serveur n’envoie pas d’informations à un site ou à un utilisateur qui en ferait un mauvais usage.

>[!INFO]
>
>**Exemple :**
>
>* **TLS** : lorsqu’une personne tape &quot;MyGreatBank.com&quot; dans un navigateur, elle veut s’assurer qu’elle se rend sur My Great Bank, et non sur un site web qui risque d’abuser ou de vendre ses informations bancaires. Ils veulent aussi s&#39;assurer que les informations de leur compte bancaire sont cryptées.
>
>   Lorsque le navigateur (le client) se connecte à MyGreatBank.com (le serveur), TLS nécessite un certificat de MyGreatBank.com pour vérifier son identité. Le certificat est fourni par une autorité de certification telle que [!DNL DigiCert] ou [!DNL Thawte]. Comme le navigateur fait confiance à l’autorité de certification, il autorise la connexion.
>
>* **TLS mutuel** : MySoftware.com est un client logiciel qui a besoin d’informations de l’API MyGreatBank.com. MyGreatBank permet uniquement aux clients de confiance de se connecter à leurs serveurs. Ainsi, en plus du protocole TLS standard qui vérifie l’identité de MyGreatBank.com, le processus d’autorité de certification TLS/certificate vérifie également la demande de MySoftware.com.

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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

&#42;&#42; Pour plus d’informations sur les [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Fournir votre certificat public [!DNL Workfront Fusion]


Lorsque vous vous connectez à un service Web avec une requête HTTP, le service Web requiert généralement un certificat public [!DNL Workfront Fusion] pour vérification. Cela permet au service Web de comparer le certificat présenté dans la requête HTTP à celui du fichier, afin de s’assurer que le certificat se trouve sur la liste autorisée du service Web.

Pour obtenir des instructions sur le téléchargement du certificat public [!DNL Adobe Workfront Fusion] vers un service Web, consultez la documentation du service Web.

>[!NOTE]
>
>Vous devrez peut-être fournir d’autres informations en plus du certificat. Pour plus d’informations sur les exigences d’un service Web, consultez la documentation de l’API du service Web.

Vous pouvez utiliser les liens suivants pour télécharger les certificats publics Workfront Fusion :

### Certificats du 23 avril 2023 au 7 mai 2024

>[!IMPORTANT]
>
>* Ces [!DNL Workfront Fusion] certificats publics expirent le 7 mai 2025. Une fois le vôtre arrivé à expiration, vous devrez charger un nouveau certificat vers le service Web. Nous vous recommandons :
>
>   * Notez la date d’expiration et définissez un rappel pour que vous puissiez télécharger le certificat vers votre service Web.
>   * Mettez cette page en signet pour trouver facilement les nouveaux certificats.
>
>* Il s’agit de certificats mTLS non génériques.

* [Télécharger [!DNL Workfront Fusion] Certificat 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-us-mtls-certificate.pem)
* [Télécharger [!DNL Workfront Fusion] Certificat UE 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

  À utiliser dans l’UE

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## Activation du protocole TLS mutuel dans les modules HTTP [!DNL Workfront Fusion]

Tous les modules de requête [!DNL Workfront Fusion] [!UICONTROL HTTP] ont la possibilité d’activer le protocole TLS mutuel.

Pour activer le protocole TLS mutuel dans un module de requête [!UICONTROL HTTP] :

1. Ajoutez un module de requête [!UICONTROL HTTP] à votre scénario.
1. Commencez à configurer le module.

   Pour plus d’informations sur la configuration d’un module de requête [!UICONTROL HTTP], reportez-vous à l’article approprié sous [[!UICONTROL modules HTTP]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Activez l’option **[!UICONTROL Afficher les paramètres avancés]** près du bas du module.
1. Activez **[!UICONTROL Utiliser TLS Mutuel]**.
