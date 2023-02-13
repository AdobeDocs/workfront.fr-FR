---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Connexion [!DNL Adobe Workfront Fusion] to [!DNL Google Services] avec des mesures de sécurité mises à jour
description: Google a récemment introduit des restrictions sur la manière dont les utilisateurs peuvent utiliser leur API. Cet article décrit comment se connecter [!DNL Adobe Workfront Fusion] à Google, en tenant compte de ces mises à jour des mesures de sécurité.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Connexion [!DNL Adobe Workfront Fusion] to [!DNL Google Services] avec des mesures de sécurité mises à jour

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrictions

[!DNL Google] introduction de restrictions sur l’utilisation de l’API par les utilisateurs à partir du 1er juin 2020. Ces mesures de sécurité protègent [!DNL Google] les utilisateurs de fuites ou d’abus de leurs données personnelles sur [!DNL Google]. Les restrictions sont liées au [!DNL Gmail] et [!DNL Google Drive] applications. Pour plus d’informations sur ces restrictions, voir &quot;Conditions supplémentaires pour les portées d’API spécifiques&quot; dans la section [[!DNL Google] Stratégie de données utilisateur des services d’API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Pour accéder aux portées restreintes, le service connecté ([!DNL Adobe Workfront Fusion] ou tout autre service qui souhaite accéder aux données de l’utilisateur via l’API) doit être vérifié et doit comporter une lettre d’évaluation afin de prouver que le service est sécurisé et transparent sur sa manière d’utiliser les données. [!DNL Workfront Fusion] est conforme à tous les [!DNL Google]Conditions requises pour l’accès aux portées restreintes. Cependant, la plupart des services connectés tiers dans [!DNL Workfront Fusion] ne pas avoir la lettre d&#39;évaluation et ne pas respecter [!DNL Google] termes. A cause de cela, [!DNL Workfront Fusion] n’est pas autorisée à envoyer des données à ces services.

## Exceptions aux [!DNL Google Services] restrictions

Il existe quelques exceptions qui permettent d’envoyer des données à un service tiers non approuvé qui ne possède pas de lettre d’évaluation sans enfreindre aucune des nouvelles restrictions. Ils diffèrent en fonction des [!DNL G Suite] avec le [!DNL Workfront Fusion] client OAuth, [!DNL G Suite] avec un autre client OAuth, ou [!DNL @gmail.com] et [!DNL @google.mail.com].

* [[!DNL G Suite] avec [!DNL Workfront Fusion] Client OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G Suite] avec un autre client OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] et [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] avec [!DNL Workfront Fusion] Client OAuth

[!DNL Workfront Fusion] utilise la variable [!UICONTROL Installation à l’échelle du domaine] exception. L’installation à l’échelle du domaine est adaptée aux [!DNL G Suite] et permet aux utilisateurs d’intégrer des services non approuvés sans aucune restriction. Si vous utilisez la suite G, vous n’avez pas à effectuer d’étapes supplémentaires et pouvez vous connecter directement aux services non approuvés.

### [!DNL G suite] avec un autre client OAuth

[!DNL G Suite] les utilisateurs qui préfèrent utiliser leur propre client OAuth au lieu d’utiliser la variable [!DNL Workfront Fusion] Le client OAuth peut se connecter à [!DNL Google Services] via la [!UICONTROL Interne] Utilisez l’approche . Cette option est destinée aux utilisateurs avancés. Pour obtenir des instructions, voir [Connexion [!DNL Adobe Workfront Fusion] to [!DNL Google Services] utilisation d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] et [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Utilisateur ayant accès à [!DNL Google Services] through [!DNL @gmail.com] ou [!DNL @googlemail.com] peut se connecter à [!DNL Google Services] par le biais de l’approche Utilisation personnelle. Cette option est destinée aux utilisateurs avancés. Pour obtenir des instructions, voir [Connexion [!DNL Adobe Workfront Fusion] to [!DNL Google Services] utilisation d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [Applications dans [!DNL Adobe Workfront Fusion] sont affectées ?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Ai-je un compte [!DNL G Suite] ?](#do-i-have-a-g-suite-account)
* [Que devrais-je faire si je suis [!DNL @gmail.com] ou [!DNL @googlemail.com] utilisateur ?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Que dois-je faire si je suis un utilisateur de [!DNL G Suite] ?](#what-should-i-do-if-im-a-g-suite-user)

### Applications dans [!DNL Adobe Workfront Fusion] sont affectées ? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]et Email (connecté à [!DNL Gmail] ).

### Ai-je une [!DNL G Suite] compte ? {#do-i-have-a-g-suite-account}

Si votre adresse électronique se termine par [!DNL @gmail.com] ou [!DNL @googlemail.com] votre compte n’est pas un [!DNL G Suite] compte . Si votre [!DNL Google] Le compte se termine par un domaine personnalisé tel que @my-company.com alors il s’agit d’un [!DNL G Suite] compte .

### Que devrais-je faire si je suis [!DNL @gmail.com] ou [!DNL @googlemail.com] utilisateur ? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Ces nouvelles restrictions ne s’appliquent que si vous intégrez [!DNL Google Drive] ou [!DNL Gmail]. Si vous souhaitez vous connecter à [!DNL Google Drive] ou [!DNL Gmail], vous pouvez

* Basculer vers [!DNL G Suite]

   ou

* Créez un client OAuth personnalisé. Cette option est destinée aux utilisateurs avancés.

   Pour obtenir des instructions, voir [Connexion [!DNL Adobe Workfront Fusion] to [!DNL Google Services] utilisation d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Si vous souhaitez intégrer un autre service que [!DNL Google Drive] ou [!DNL Gmail], ces restrictions ne s’appliquent pas.

Pour obtenir des instructions sur la connexion à d’autres [!DNL Google Services] to [!DNL Workfront Fusion], voir [Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) dans l’article [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Que dois-je faire si je suis un [!DNL G Suite] utilisateur ? {#what-should-i-do-if-im-a-g-suite-user}

Aucune action n’est requise.
