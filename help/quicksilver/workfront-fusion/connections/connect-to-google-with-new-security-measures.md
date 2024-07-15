---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: connections-annd-webhooks
title: Connectez-vous  [!DNL Adobe Workfront Fusion] à  [!DNL Google Services] avec des mesures de sécurité mises à jour
description: Google a récemment introduit des restrictions sur la manière dont les utilisateurs peuvent utiliser leur API. Cet article décrit comment se connecter  [!DNL Adobe Workfront Fusion] à Google, en tenant compte de ces mesures de sécurité de mise à jour.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 18%

---

# Connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services] avec des mesures de sécurité mises à jour

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

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrictions

[!DNL Google] a introduit des restrictions sur la manière dont les utilisateurs peuvent utiliser leur API à compter du 1er juin 2020. Ces mesures de sécurité protègent les utilisateurs de [!DNL Google] contre les fuites ou l&#39;utilisation abusive de leurs données personnelles sur [!DNL Google]. Les restrictions sont liées aux applications [!DNL Gmail] et [!DNL Google Drive]. Pour plus d’informations sur ces restrictions, voir &quot;Exigences supplémentaires pour les portées d’API spécifiques&quot; dans la [[!DNL Google] stratégie de données utilisateur des services d’API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Pour accéder aux portées restreintes, le service connecté ([!DNL Adobe Workfront Fusion] ou tout autre service qui souhaite accéder aux données de l’utilisateur via l’API) doit être vérifié et doit disposer d’une lettre d’évaluation pour prouver que le service est sécurisé et transparent sur la manière dont il utilise les données. [!DNL Workfront Fusion] est conforme à toutes les exigences de [!DNL Google] pour l’accès aux portées restreintes. Cependant, la plupart des services tiers connectés dans [!DNL Workfront Fusion] ne possèdent pas la lettre d’évaluation et ne respectent donc pas les termes de [!DNL Google]. Pour cette raison, [!DNL Workfront Fusion] n’est pas autorisé à envoyer des données à ces services.

## Exceptions aux restrictions [!DNL Google Services]

Il existe quelques exceptions qui permettent d’envoyer des données à un service tiers non approuvé qui ne possède pas de lettre d’évaluation sans enfreindre aucune des nouvelles restrictions. Ils diffèrent selon [!DNL Google Workspace] avec le client [!DNL Workfront Fusion] OAuth, [!DNL Google Workspace] avec un autre client OAuth, ou [!DNL @gmail.com] et [!DNL @google.mail.com].

* [[!DNL Google Workspace] avec  [!DNL Workfront Fusion] client OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] avec un autre client OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] et [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] avec [!DNL Workfront Fusion] client OAuth

[!DNL Workfront Fusion] utilise l’exception [!UICONTROL Installation à l’échelle du domaine]. L’installation à l’échelle du domaine est adaptée aux utilisateurs de [!DNL Google Workspace] et permet aux utilisateurs d’intégrer des services non approuvés sans limites. Si vous utilisez Google Workspace, vous n’avez pas à effectuer d’étapes supplémentaires et pouvez vous connecter directement aux services non approuvés.

### [!DNL Google Workspace] avec un autre client OAuth

Les utilisateurs de [!DNL Google Workspace] qui préfèrent utiliser leur propre client OAuth au lieu d&#39;utiliser le client OAuth [!DNL Workfront Fusion] peuvent se connecter à [!DNL Google Services] par l&#39;intermédiaire de l&#39;approche d&#39;utilisation [!UICONTROL Interne]. Cette option est destinée aux utilisateurs avancés. Pour obtenir des instructions, reportez-vous à la section [Se connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services]  à l’aide d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] et [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Les utilisateurs qui accèdent à [!DNL Google Services] par [!DNL @gmail.com] ou [!DNL @googlemail.com] peuvent se connecter à [!DNL Google Services] par le biais de l’approche à usage personnel. Cette option est destinée aux utilisateurs avancés. Pour obtenir des instructions, reportez-vous à la section [Se connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services]  à l’aide d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Questions fréquentes

* [Quelles applications de  [!DNL Adobe Workfront Fusion] sont affectées ?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Ai-je un compte  [!DNL Google Workspace] ?](#do-i-have-a-g-suite-account)
* [Que dois-je faire si je suis un utilisateur de  [!DNL @gmail.com] ou de [!DNL @googlemail.com]  ?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Que dois-je faire si je suis un utilisateur de  [!DNL Google Workspace]  ?](#what-should-i-do-if-im-a-g-suite-user)

### Quelles applications dans [!DNL Adobe Workfront Fusion] sont affectées ? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] et Courrier électronique (connecté à un compte [!DNL Gmail]).

### Ai-je un compte [!DNL Google Workspace] ? {#do-i-have-a-g-suite-account}

Si votre adresse électronique se termine par [!DNL @gmail.com] ou [!DNL @googlemail.com], votre compte n’est pas un compte [!DNL Google Workspace]. Si votre compte [!DNL Google] se termine par un domaine personnalisé tel que @my-company.com, il s’agit alors d’un compte [!DNL Google Workspace].

### Que dois-je faire si je suis un utilisateur [!DNL @gmail.com] ou [!DNL @googlemail.com] ? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Ces nouvelles restrictions ne s’appliquent que si vous intégrez [!DNL Google Drive] ou [!DNL Gmail]. Si vous souhaitez vous connecter à [!DNL Google Drive] ou [!DNL Gmail], vous pouvez

* Passer à [!DNL Google Workspace]

  ou

* Créez un client OAuth personnalisé. Cette option est destinée aux utilisateurs avancés.

  Pour obtenir des instructions, reportez-vous à la section [Se connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services]  à l’aide d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Si vous souhaitez intégrer un autre service que [!DNL Google Drive] ou [!DNL Gmail], ces restrictions ne s’appliquent pas.

Pour plus d&#39;informations sur la connexion d&#39;autres [!DNL Google Services] à [!DNL Workfront Fusion], voir [Connexion de l&#39;application du module ou du service Web à  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) dans l&#39;article [Créer un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Que dois-je faire si je suis un utilisateur [!DNL Google Workspace] ? {#what-should-i-do-if-im-a-g-suite-user}

Aucune action n’est requise.
