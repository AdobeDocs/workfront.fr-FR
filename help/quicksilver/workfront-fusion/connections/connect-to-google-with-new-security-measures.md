---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: connections-annd-webhooks
title: Connecter  [!DNL Adobe Workfront Fusion]  à  [!DNL Google Services]  avec des mesures de sécurité mises à jour
description: Google a récemment ajouté des restrictions sur la manière dont les utilisateurs et les utilisatrices peuvent utiliser leur API. Cet article décrit comment connecter  [!DNL Adobe Workfront Fusion]  à Google, en tenant compte de ces nouvelles mesures de sécurité.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 94%

---

# Connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services] conformément aux nouvelles mesures de sécurité

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
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Restrictions [!DNL Google Services]

[!DNL Google] a ajouté des restrictions sur l’utilisation de l’API par les utilisateurs et les utilisatrices à partir du 1er juin 2020. Ces mesures de sécurité protègent les utilisateurs et les utilisatrices de [!DNL Google] de fuites ou d’abus quant à leurs données personnelles sur [!DNL Google]. Les restrictions sont liées à aux applications [!DNL Gmail] et [!DNL Google Drive]. Pour plus d’informations sur ces restrictions, voir « Conditions supplémentaires pour les portées d’API spécifiques » dans la [[!DNL Google] Politique de données utilisateur des services d’API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes).

Pour accéder aux portées restreintes, le service connecté ([!DNL Adobe Workfront Fusion] ou tout autre service qui souhaite accéder aux données de l’utilisateur ou de l’utilisatrice via l’API) doit être vérifié et doit comporter une lettre d’évaluation afin de prouver que le service est sécurisé et transparent sur l’utilisation des données. [!DNL Workfront Fusion] est conforme à toutes les conditions requises de [!DNL Google] pour l’accès aux portées restreintes. Cependant, la plupart des services connectés tiers dans [!DNL Workfront Fusion] ne disposent pas de la lettre d’évaluation et ne respectent pas les conditions de [!DNL Google]. Pour cette raison, [!DNL Workfront Fusion] n’est pas autorisé à envoyer des données à ces services.

## Exceptions aux restrictions de [!DNL Google Services]

Il existe quelques exceptions qui permettent d’envoyer des données à un service tiers non approuvé qui ne possède pas de lettre d’évaluation sans enfreindre aucune des nouvelles restrictions. Elles diffèrent en fonction de [!DNL Google Workspace] avec le client OAuth [!DNL Workfront Fusion], [!DNL Google Workspace] avec un autre client OAuth, ou [!DNL @gmail.com] et [!DNL @google.mail.com].

* [[!DNL Google Workspace] avec  [!DNL Workfront Fusion] client OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] avec un autre client OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] et  [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] avec client OAuth [!DNL Workfront Fusion]

[!DNL Workfront Fusion] utilise l’exception [!UICONTROL Installation à l’échelle du domaine]. L’installation à l’échelle du domaine est adaptée aux utilisateurs et aux utilisatrices de [!DNL Google Workspace] et permet d’intégrer des services non approuvés sans aucune restriction. Si vous utilisez Google Workspace, vous n’avez pas à effectuer d’étapes supplémentaires et pouvez vous connecter directement aux services non approuvés.

### [!DNL Google Workspace] avec un autre client OAuth

Les utilisateurs et les utilisatrices de [!DNL Google Workspace] qui préfèrent utiliser leur propre client OAuth au lieu d’utiliser le client OAuth [!DNL Workfront Fusion] pour se connecter à [!DNL Google Services] par le biais de l’approche [!UICONTROL interne]. Cette option est destinée aux utilisateurs et aux utilisatrices avancés. Pour obtenir des instructions, consultez [Connnecter  [!DNL Adobe Workfront Fusion]  à  [!DNL Google Services]  avec un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] et [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Utilisateur ou utilisatrice ayant accès à [!DNL Google Services] par le biais de [!DNL @gmail.com] ou [!DNL @googlemail.com] peut se connecter à [!DNL Google Services] via l’approche d’utilisation personnelle. Cette option est destinée aux utilisateurs et aux utilisatrices avancés. Pour obtenir des instructions, consultez [Connnecter  [!DNL Adobe Workfront Fusion]  à  [!DNL Google Services]  avec un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Questions fréquentes

* [Quelles applications dans  [!DNL Adobe Workfront Fusion]  ont été affectées ?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Ai-je un compte  [!DNL Google Workspace] ?](#do-i-have-a-g-suite-account)
* [Que dois-je faire si je suis un utilisateur ou une utilisatrice de  [!DNL @gmail.com]  ou  [!DNL @googlemail.com]  ?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Que dois-je faire si je suis un utilisateur de  [!DNL Google Workspace]  ?](#what-should-i-do-if-im-a-g-suite-user)

### Quelles applications dans [!DNL Adobe Workfront Fusion] ont été affectées ? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] et E-mail (connecté au compte [!DNL Gmail]).

### Ai-je un compte [!DNL Google Workspace] ? {#do-i-have-a-g-suite-account}

Si votre adresse e-mail se termine par [!DNL @gmail.com] ou [!DNL @googlemail.com], votre compte n’est pas un compte [!DNL Google Workspace]. Si votre compte [!DNL Google] se termine par un domaine personnalisé tel que @mon-entreprise.com alors il s’agit d’un compte [!DNL Google Workspace].

### Que dois-je faire si je suis un utilisateur ou une utilisatrice de [!DNL @gmail.com] ou [!DNL @googlemail.com] ? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Ces nouvelles restrictions s’appliquent uniquement si vous intégrez [!DNL Google Drive] ou [!DNL Gmail]. Si vous souhaitez vous connecter à [!DNL Google Drive] ou [!DNL Gmail], vous pouvez

* basculer vers [!DNL Google Workspace]

  ou

* créer un client OAuth personnalisé. Cette option est destinée aux utilisateurs et aux utilisatrices avancés.

  Pour obtenir des instructions, consultez [Connecter  [!DNL Adobe Workfront Fusion]  à  [!DNL Google Services]  avec un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Si vous souhaitez intégrer un autre service que [!DNL Google Drive] ou [!DNL Gmail], ces restrictions ne s’appliquent pas.

Pour obtenir des instructions sur la connexion d’autres [!DNL Google Services] à [!DNL Workfront Fusion], consultez [Connecter l’application ou le service Web du module à  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) dans l’article [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Que dois-je faire si je suis un utilisateur ou une utilisatrice [!DNL Google Workspace] ? {#what-should-i-do-if-im-a-g-suite-user}

Aucune action n’est requise.
