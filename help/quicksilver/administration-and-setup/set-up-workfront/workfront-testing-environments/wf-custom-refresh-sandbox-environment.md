---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: La variable [!DNL Adobe Workfront] Environnement Sandbox d’actualisation personnalisée
description: L’environnement de test d’actualisation personnalisée est un environnement dans lequel vous pouvez tester et travailler à l’aide des données de votre environnement de production. Il est également idéal pour exécuter des formations et déterminer les fonctionnalités de configuration.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# La variable [!DNL Adobe Workfront] Environnement Sandbox d’actualisation personnalisée

L’environnement de test d’actualisation personnalisée est un environnement dans lequel vous pouvez tester et travailler à l’aide des données de votre environnement de production. Il est également idéal pour exécuter des formations et déterminer les fonctionnalités de configuration.

>[!NOTE]
>
>Ceci diffère de l’environnement de test de prévisualisation, qui est également un environnement de test qui reproduit votre [!DNL Workfront] environnement de production.
>
>* De nouvelles fonctionnalités sont introduites dans l’environnement de test de prévisualisation avant qu’elles ne soient disponibles dans la production.
>* Les nouvelles fonctionnalités ne sont pas introduites dans l’environnement de test d’actualisation personnalisée avant qu’elles ne soient disponibles dans l’environnement de production.
>
>  En outre, l’obtention de l’environnement de test d’actualisation personnalisée qui n’est pas requis pour l’environnement de test d’aperçu entraîne des frais supplémentaires.
>
>  Pour plus d’informations sur l’aperçu de l’environnement de test, voir [La variable [!DNL Adobe Workfront] Aperçu de l’environnement de test](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>[!UICONTROL Business] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] license</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Package de support</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Privilégié] ou [!UICONTROL Enterprise]</p> <p>Le package de prise en charge standard n’a pas accès à l’environnement de test d’actualisation personnalisée, mais il a accès à l’environnement de test d’aperçu.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Actualisation de l’environnement de test d’actualisation personnalisé

L’environnement de test d’actualisation personnalisée contient vos données de production réelles et il ne s’actualise pas tant que vous ne le planifiez pas. Vous pouvez planifier une actualisation à tout moment, aussi fréquemment qu’une fois par semaine.

>[!NOTE]
>
>* Vous ne pouvez pas planifier une actualisation pour le jour en cours. Si, par exemple, la date d’aujourd’hui est le 1er juin, la date la plus proche à laquelle vous pouvez planifier une actualisation est le 2 juin.
>* L’actualisation planifiée se produit parfois pendant la nuit, en fonction de la grappe de l’utilisateur (les grappes des États-Unis s’actualisent la nuit aux États-Unis). L’heure spécifique est imprévisible en raison des autres clients de la file d’attente et de la quantité de données actualisée. Si la file d’attente compte de nombreux clients volumineux, votre actualisation peut ne pas s’exécuter avant plus tard ce jour-là ou le jour suivant.
>* Votre environnement de test d’actualisation personnalisée comporte toujours les mêmes fonctionnalités de produit que votre environnement de production. Cependant, lorsque vous actualisez votre environnement de test d’actualisation personnalisée, la valorisation de marque n’est conservée que pour la couleur d’arrière-plan de l’écran de connexion. L’écran de connexion et les logos de la barre de navigation sont réinitialisés sur [!DNL Workfront] les valeurs par défaut et les images de marque que vous avez modifiées avant l’actualisation ne s’affichent pas.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Accès à l’environnement de test d’actualisation personnalisé à partir de votre environnement de production {#access-the-custom-refresh-sandbox-from-your-production-environment}

Comme [!DNL Workfront] administrateur, vous pouvez accéder à votre environnement de test d’actualisation personnalisée à partir de votre environnement de production.

>[!NOTE]
>
>Si votre compte se trouve sur la grappe 4 (grappe EMEA), vous ne pouvez pas accéder à votre environnement de test d’actualisation personnalisé à partir de l’environnement de production. Pour plus d’informations sur la manière dont vous pouvez accéder à votre sandbox d’actualisation personnalisée lorsque vous disposez d’un compte sur la grappe 4, voir [Accès à l’environnement de test d’actualisation personnalisée pour les comptes sur une grappe 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Accès à l’environnement de test d’actualisation personnalisée pour les comptes sur une grappe 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Pour accéder à votre sandbox d’actualisation personnalisée :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Système]** >**[!UICONTROL Préférences]**.

1. Dans le **[!UICONTROL Environnement de test]** , cliquez sur **[!UICONTROL Sandbox 1]** ou **[!UICONTROL Sandbox 2]**.

   Votre module de prise en charge indique si vous avez accès à un ou deux environnements de test d’actualisation personnalisée.

1. Connectez-vous à l’aide de vos informations d’identification Sandbox d’actualisation personnalisée.

   Vos informations d’identification Sandbox d’actualisation personnalisée sont identiques à celles de votre production, sauf si vous avez modifié vos informations d’identification de production depuis la dernière actualisation de votre environnement de test d’actualisation personnalisé. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

   L’environnement de test d’actualisation personnalisée affiche la version ainsi que la date de la dernière actualisation dans la bannière en haut de l’écran. Toutes les informations de production sont disponibles et prêtes à l’emploi une fois l’actualisation terminée.

## Accès à l’environnement de test d’actualisation personnalisé à l’aide d’une URL {#access-the-custom-refresh-sandbox-using-a-url}

Tout utilisateur peut accéder à l’environnement de test d’actualisation personnalisée à l’aide d’une URL.

* [Accès à l’environnement de test d’actualisation personnalisée pour les comptes des grappes 1, 2, 3 et 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Accès à l’environnement de test d’actualisation personnalisée pour les comptes sur une grappe 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Accès à l’environnement de test d’actualisation personnalisée pour les comptes des grappes 1, 2, 3 et 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Selon votre module d’assistance, vous devez avoir accès à un ou deux environnements de test d’actualisation personnalisée.

Pour accéder à votre sandbox d’actualisation personnalisée à l’aide d’une URL :

1. Accédez à cette URL si vous n’avez qu’un sandbox d’actualisation personnalisée :

   https://companyname.sb01.workfront.com (ancienne URL):https://cr1.attasksandbox.com/.)

   Ou si vous disposez de deux sandbox d’actualisation personnalisée, en plus des URL ci-dessus, vous pouvez également accéder à l’URL suivante pour accéder à votre second sandbox d’actualisation personnalisée :

   https://companyname.sb02.workfront.com (ancienne URL):https://cr2.attasksandbox.com/)

1. Dans l’écran de connexion, connectez-vous à l’aide de vos informations d’identification Sandbox d’actualisation personnalisée.
1. Vos informations d’identification Sandbox d’actualisation personnalisée sont identiques à celles de votre production, sauf si vous avez modifié vos informations d’identification de production depuis la dernière actualisation de votre environnement de test d’actualisation personnalisé. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

### Accès à l’environnement de test d’actualisation personnalisée pour les comptes sur une grappe 4 (comptes EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Si votre [!DNL Workfront] Le compte se trouve sur la grappe 4 (grappe EMEA), vous ne pouvez accéder à votre environnement de test d’actualisation personnalisée qu’à l’aide d’une URL. Pour savoir quelle grappe se trouve votre compte, contactez notre équipe d’assistance clientèle.

Selon votre module d’assistance, vous devez avoir accès à un ou deux environnements de test d’actualisation personnalisée.

Pour accéder à votre sandbox d’actualisation personnalisée à l’aide d’une URL :

1. Accédez à cette URL si vous n’avez qu’un sandbox d’actualisation personnalisée :

   https://companyname.sb01.workfront.com (ancienne URL):https:/cr3.attasksandbox)

   Ou

   Accédez à l’une de ces URL si vous disposez de deux sandbox d’actualisation personnalisée :

   https://companyname.sb01.workfront.com (ancienne URL):https:/cr3.attasksandbox)

   https://companyname.sb02.workfront.com (ancienne URL):https:/cr4.attasksandbox)

1. Dans l’écran de connexion, connectez-vous à l’aide de vos informations d’identification Sandbox d’actualisation personnalisée.

   Vos informations d’identification Sandbox d’actualisation personnalisée sont identiques à celles de votre production, sauf si vous avez modifié vos informations d’identification de production depuis la dernière actualisation de votre environnement de test d’actualisation personnalisé. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

## Planification d’une actualisation de votre environnement de test d’actualisation personnalisé

>[!IMPORTANT]
>
>La durée de l’actualisation dépend de la taille des données en cours d’actualisation. Pendant le processus d’actualisation, il est essentiel que votre environnement de test d’actualisation personnalisé ne soit pas utilisé de quelque manière que ce soit (y compris les appels d’API et les intégrations), car cela empêchera l’actualisation de l’environnement de test de se terminer avec succès. [!DNL Workfront] désactive l’environnement de test d’actualisation personnalisé avant qu’il ne commence, mais vous devez mettre fin à toutes les sessions actives pour vous assurer que l’actualisation de votre environnement de test est réussie.

Après avoir planifié une actualisation de votre sandbox d’actualisation personnalisée, vous pouvez l’annuler en cliquant sur [!UICONTROL Annuler] en haut de la page. Vous pouvez également le replanifier ultérieurement.

>[!NOTE]
>
>Vous ne pouvez pas planifier d’actualisation automatique des environnements de test.

Pour planifier une actualisation de votre environnement de test d’actualisation client :

1. Connectez-vous à votre environnement de test d’actualisation personnalisé.
1. Cliquez sur **[!UICONTROL Planification]** dans la bannière en haut de l’écran, puis sélectionnez une date dans le calendrier.
1. Sélectionnez une date pour laquelle l’actualisation doit avoir lieu, puis cliquez sur **[!UICONTROL Actualisation de la planification]**.

## Basculez vers Production à partir de l’environnement de test d’actualisation personnalisée

1. Connectez-vous à votre environnement de test d’actualisation personnalisé.

   Pour plus d’informations sur l’accès à votre sandbox d’actualisation personnalisée, voir [Accès à l’environnement de test d’actualisation personnalisé à partir de votre environnement de production](#access-the-custom-refresh-sandbox-from-your-production-environment) ou [Accès à l’environnement de test d’actualisation personnalisé à l’aide d’une URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Cliquez sur **[!UICONTROL Aller à la production]** dans la bannière en haut de l’écran.

   N’oubliez pas que le travail effectué dans l’environnement de test ne sera pas visible dans la variable [!UICONTROL production] , car le transfert des données est unidirectionnel, de la production vers votre environnement de test d’actualisation personnalisée, et non inverse.

## Réception d’emails à partir de l’environnement de test d’actualisation personnalisée

[!DNL Workfront] désactive toutes les communications par courrier électronique à partir de l’environnement Sandbox d’actualisation personnalisée. Si vous souhaitez recevoir des notifications par courrier électronique de l’environnement Sandbox d’actualisation personnalisée, vous devez activer cette fonctionnalité dans vos paramètres utilisateur. Pour plus d’informations sur l’activation des notifications par courrier électronique dans l’environnement Sandbox d’actualisation personnalisée, voir [Activation de la diffusion des emails à partir de l’environnement Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La diffusion de rapports et les notifications push sur l’application mobile sont toujours désactivées pour l’environnement Sandbox d’actualisation personnalisée. Ni vous ni le [!DNL Workfront] Lorsque vous accédez à l’environnement Sandbox d’actualisation personnalisée, l’administrateur peut activer la remise de rapports ou les notifications push pour l’application mobile.\
>Pour plus d’informations sur les diffusions de rapports pour l’environnement de production, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Pour plus d’informations sur les notifications push sur l’application mobile pour l’environnement de production, consultez la section dans .

## Configuration de l’authentification unique dans l’environnement de test d’actualisation personnalisée

Si vous souhaitez configurer votre environnement de test d’actualisation personnalisé pour qu’il fonctionne avec une solution de connexion unique, vous pouvez le faire en le configurant séparément de votre environnement de production. La configuration SSO dans l’environnement de test d’actualisation personnalisée est indépendante de la configuration SSO dans l’environnement de production.\
Lorsque vous actualisez votre environnement de test d’actualisation personnalisée, les informations d’authentification unique ne sont pas copiées à partir de votre environnement de production pour remplacer la configuration de l’environnement de test d’actualisation personnalisée.

Les étapes de configuration de l’authentification unique dans l’environnement de test d’actualisation personnalisée sont similaires à celles de la configuration dans l’environnement de production.\
Pour plus d’informations sur la configuration [!DNL Workfront] avec SSO, voir [Présentation de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Cette option n’est pas disponible si la variable [!DNL Workfront] est activée avec Adobe IMS. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

## Utilisation prévue et disponibilité

* [!DNL Workfront] Les environnements Sandbox d’actualisation personnalisée ne sont pas destinés aux tests de performance ou de chargement. Utilisez plutôt ces environnements pour valider la fonctionnalité avec les workflows existants de votre entreprise.

* [!DNL Workfront] Les environnements Sandbox d’actualisation personnalisée sont conçus pour être toujours disponibles. Toute panne d’un environnement Sandbox d’actualisation personnalisée de Workfront pendant les heures de bureau normales sera une priorité immédiatement après que les problèmes de production seront résolus, le cas échéant. Toute panne d’un environnement Sandbox d’actualisation personnalisée Workfront le week-end (le samedi et le dimanche) sera corrigée afin que l’environnement soit en cours d’exécution pendant les heures ouvrables le lundi.

* La vérification n’est pas disponible dans les environnements Sandbox d’actualisation personnalisée.
