---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: L’environnement de sandbox à actualisation personnalisée  [!DNL Adobe Workfront]
description: Le sandbox à actualisation personnalisée est un environnement dans lequel vous pouvez effectuer des tests et travailler à l’aide des données de votre environnement de production. Il est également idéal pour exécuter des formations et déterminer les fonctionnalités de configuration.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 99%

---

# L’environnement de sandbox à actualisation personnalisée [!DNL Adobe Workfront]

Le sandbox à actualisation personnalisée est un environnement dans lequel vous pouvez effectuer des tests et travailler à l’aide des données de votre environnement de production. Il est également idéal pour exécuter des formations et déterminer les fonctionnalités de configuration.

>[!NOTE]
>
>Ceci diffère de la prévisualisation de sandbox, qui est également un environnement de test reproduisant votre environnement de production [!DNL Workfront].
>
>* Les nouvelles fonctionnalités sont introduites dans la prévisualisation de sandbox avant qu’elles ne soient disponibles en production.
>* Les nouvelles fonctionnalités ne sont pas introduites dans le sandbox à actualisation personnalisée avant qu’elles ne soient disponibles en production.
>
>  En outre, l’obtention du sandbox à actualisation personnalisée qui n’est pas requis pour la prévisualisation de sandbox entraîne des frais supplémentaires.
>
>  Pour plus d’informations sur la prévisualisation de sandbox, voir [ l’ [!DNL Adobe Workfront] environnement de prévisualisation de sandbox](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>[!UICONTROL Business] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licence</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et administratrices [!DNL Workfront], voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès d’administration complet à un utilisateur ou une utilisatrice</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Package de prise en charge</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] ou [!UICONTROL Enterprise]</p> <p>Le package de prise en charge standard n’inclut pas l’accès au sandbox à actualisation personnalisée, mais il inclut l’accès au sandbox de prévisualisation.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Actualisation du sandbox à actualisation personnalisée

Le sandbox à actualisation personnalisée contient vos données de production réelles et ne s’actualise pas tant que vous ne le planifiez pas. Vous pouvez planifier une actualisation à tout moment, à raison d’une fois par semaine, par exemple.

>[!NOTE]
>
>* Vous ne pouvez pas planifier une actualisation pour le jour en cours. Si, par exemple, la date d’aujourd’hui est le 1er juin, la date la plus proche à laquelle vous pouvez planifier une actualisation est le 2 juin.
>* L’actualisation planifiée se produit parfois pendant la nuit, en fonction du cluster de l’utilisateur ou de l’utilisatrice (les clusters des États-Unis s’actualisent la nuit aux États-Unis). L’heure spécifique est imprévisible en raison des autres clientes et clients de la file d’attente et de la quantité de données actualisée. Si la file d’attente compte de nombreux éléments volumineux, votre actualisation peut ne pas s’exécuter avant plus tard ce jour-là ou le jour suivant.
>* Votre sandbox à actualisation personnalisée comporte toujours les mêmes fonctionnalités de produit que votre environnement de production. Cependant, lorsque vous actualisez votre sandbox à actualisation personnalisée, le branding n’est conservé que pour la couleur d’arrière-plan de l’écran de connexion. L’écran de connexion et les logos de la barre de navigation sont réinitialisés sur les valeurs par défaut de [!DNL Workfront]. Les images de branding que vous avez modifiées avant l’actualisation ne s’affichent pas.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Accéder au sandbox à actualisation personnalisée à partir de votre environnement de production {#access-the-custom-refresh-sandbox-from-your-production-environment}

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez accéder à votre sandbox à actualisation personnalisée à partir de votre environnement de production.

>[!NOTE]
>
>Si votre compte se trouve sur le cluster 4 (cluster EMEA), vous ne pouvez pas accéder à votre sandbox à actualisation personnalisée à partir de l’environnement de production. Pour plus d’informations sur la manière dont vous pouvez accéder à votre sandbox à actualisation personnalisée lorsque vous disposez d’un compte sur le cluster 4, voir [Accéder au sandbox à actualisation personnalisée pour les comptes sur un cluster 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Accéder au sandbox à actualisation personnalisée pour les comptes sur un cluster 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Pour accéder à votre sandbox à actualisation personnalisée :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Système]** > **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Environnement de test]**, cliquez sur **[!UICONTROL Sandbox 1]** ou **[!UICONTROL Sandbox 2]**.

   Votre package de prise en charge indique si vous avez accès à un ou deux sandbox à actualisation personnalisée.

1. Connectez-vous à l’aide de vos informations d’identification de sandbox à actualisation personnalisée.

   Vos informations d’identification de sandbox à actualisation personnalisée sont identiques à celles de votre production, sauf si vous les avez modifiées depuis la dernière actualisation de votre sandbox à actualisation personnalisée. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

   Le sandbox à actualisation personnalisée affiche la version ainsi que la date de la dernière actualisation dans la bannière en haut de l’écran. Toutes les informations de production sont disponibles et prêtes à l’emploi une fois l’actualisation terminée.

## Accéder au sandbox à actualisation personnalisée à l’aide d’une URL {#access-the-custom-refresh-sandbox-using-a-url}

Toute personne peut accéder au sandbox à actualisation personnalisée à l’aide d’une URL.

* [Accéder au sandbox à actualisation personnalisée pour les comptes des clusters 1, 2, 3 et 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Accéder au sandbox à actualisation personnalisée pour les comptes du cluster 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Accéder au sandbox à actualisation personnalisée pour les comptes des clusters 1, 2, 3 et 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Selon votre package d’assistance, vous devez avoir accès à un ou deux sandbox à actualisation personnalisée.

Pour accéder à votre sandbox à actualisation personnalisée à l’aide d’une URL :

1. Accédez à cette URL si vous n’avez qu’un sandbox à actualisation personnalisée :

   https://companyname.sb01.workfront.com (old URL:https://cr1.attasksandbox.com/.)

   Ou si vous disposez de deux sandbox à actualisation personnalisée, en plus des URL ci-dessus, vous pouvez également accéder à l’URL suivante pour accéder à votre second sandbox à actualisation personnalisée :

   https://companyname.sb02.workfront.com (old URL:https://cr2.attasksandbox.com/)

1. Dans l’écran de connexion, connectez-vous à l’aide de vos informations d’identification de sandbox à actualisation personnalisée.
1. Vos informations d’identification de sandbox à actualisation personnalisée sont identiques à celles de votre environnement de production, sauf si vous avez modifié vos informations d’identification d’environnement de production depuis la dernière actualisation de votre sandbox à actualisation personnalisé. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

### Accéder au sandbox à actualisation personnalisée pour les comptes du cluster 4 (comptes EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Si votre compte [!DNL Workfront] se trouve sur le cluster 4 (cluster EMEA), vous ne pouvez accéder à votre sandbox à actualisation personnalisée qu’à l’aide d’une URL. Pour savoir sur quel cluster se trouve votre compte, contactez notre équipe d’assistance clientèle.

Selon votre package d’assistance, vous devez avoir accès à un ou deux sandbox à actualisation personnalisée.

Pour accéder à votre sandbox à actualisation personnalisée à l’aide d’une URL :

1. Accédez à cette URL si vous n’avez qu’un sandbox à actualisation personnalisée :

   https://companyname.sb01.workfront.com (ancienne URL):https:/cr3.attasksandbox)

   Ou

   Accédez à l’une de ces URL si vous disposez de deux sandbox à actualisation personnalisée :

   https://companyname.sb01.workfront.com (ancienne URL):https:/cr3.attasksandbox)

   https://companyname.sb02.workfront.com (ancienne URL):https:/cr4.attasksandbox)

1. Dans l’écran de connexion, connectez-vous à l’aide de vos informations d’identification de sandbox à actualisation personnalisée.

   Vos informations d’identification de sandbox à actualisation personnalisée sont identiques à celles de votre environnement de production, sauf si vous avez modifié vos informations d’identification d’environnement de production depuis la dernière actualisation de votre sandbox à actualisation personnalisé. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

## Planifier une actualisation de votre sandbox à actualisation personnalisée

>[!IMPORTANT]
>
>La durée de l’actualisation dépend de la taille des données en cours d’actualisation. Pendant le processus d’actualisation, il est essentiel que votre sandbox à actualisation personnalisée ne soit pas utilisé de quelque manière que ce soit (y compris les appels API et les intégrations), car cela empêchera l’actualisation du sandbox de se terminer. [!DNL Workfront] désactivera le sandbox à actualisation personnalisée avant qu’il ne commence, mais vous devez mettre fin à toutes les sessions actives pour vous assurer de la réussite de l’actualisation de votre sandbox.

Après avoir planifié une actualisation de votre sandbox à actualisation personnalisée, vous pouvez l’annuler en cliquant sur [!UICONTROL Annuler] en haut de la page. Vous pouvez également la replanifier ultérieurement.

>[!NOTE]
>
>Vous ne pouvez pas planifier d’actualisation automatique du sandbox.

Pour planifier une actualisation de votre sandbox à actualisation personnalisée :

1. Connectez-vous à votre sandbox à actualisation personnalisée.
1. Cliquez sur **[!UICONTROL Planifier]** dans la bannière en haut de l’écran, puis sélectionnez une date dans le calendrier.
1. Sélectionnez une date d’actualisation, puis cliquez sur **[!UICONTROL Planifier l’actualisation]**.

## Basculer vers l’environnement de production à partir du sandbox à actualisation personnalisée

1. Connectez-vous à votre sandbox à actualisation personnalisée.

   Pour plus d’informations sur l’accès à votre sandbox à actualisation personnalisée, voir [Accéder au sandbox à actualisation personnalisée à partir de votre environnement de production](#access-the-custom-refresh-sandbox-from-your-production-environment) ou [Accéder au sandbox à actualisation personnalisée à l’aide d’une URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Cliquez sur **[!UICONTROL Accéder à l’environnement de production]** dans la bannière en haut de l’écran.

   N’oubliez pas que le travail effectué dans le sandbox ne sera pas visible dans l’environnnement de [!UICONTROL production], car le transfert des données est unidirectionnel, de l’environnement de production vers votre sandbox à actualisation personnalisée, et non l’inverse.

## Recevoir des e-mails à partir du sandbox à actualisation personnalisée

[!DNL Workfront] désactive toutes les communications par e-mail à partir du sandbox à actualisation personnalisée. Si vous souhaitez recevoir des notifications par e-mail du sandbox à actualisation personnalisée, vous devez activer cette fonctionnalité dans vos paramètres d’utilisation. Pour plus d’informations sur l’activation des notifications par e-mail dans le sandbox à actualisation personnalisée, voir [Activer la diffusion des e-mails à partir du sandbox de prévisualisation](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La diffusion de rapports et les notifications push sur l’application mobile sont toujours désactivées pour le sandbox à actualisation personnalisée. Ni vous ni l’administrateur ou administratrice [!DNL Workfront] ne pouvez activer la diffusion de rapports ou des notifications push pour l’application mobile lorsque vous accédez au sandbox à actualisation personnalisée.\
>Pour plus d’informations sur les diffusions de rapports pour l’environnement de production, voir [Vue d’ensemble de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md). Pour plus d’informations sur les notifications push sur l’application mobile pour l’environnement de production, consultez la section dans .

## Configurer l’authentification unique dans le sandbox à actualisation personnalisée

Si vous souhaitez configurer votre sandbox à actualisation personnalisée pour qu’il fonctionne avec une solution à authentification unique, vous pouvez le faire en le configurant séparément de votre environnement de production. La configuration de l’authentification unique dans le sandbox à actualisation personnalisée est indépendante de la configuration de l’authentification unique dans l’environnement de production.\
Lorsque vous actualisez votre sandbox à actualisation personnalisée, les informations d’authentification unique ne sont pas copiées à partir de votre environnement de production pour remplacer la configuration du sandbox à actualisation personnalisée.

Les étapes de configuration de l’authentification unique dans le sandbox à actualisation personnalisée sont similaires à celles de la configuration dans l’environnement de production.\
Pour plus d’informations sur la configuration de [!DNL Workfront] avec l’authentification unique, voir [Vue d’ensemble de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance [!DNL Workfront] de votre organisation est activée avec Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

## Utilisation prévue et disponibilité

* [!DNL Workfront] Les sandbox à actualisation personnalisée ne sont pas destinés aux tests de performance ou de chargement. Utilisez plutôt ces environnements pour valider la fonctionnalité avec les workflows existants de votre organisation.

* [!DNL Workfront] Les sandbox à actualisation personnalisée sont conçus pour être toujours disponibles. Toute panne d’un sandbox à actualisation personnalisée de Workfront pendant les heures de travail habituelles sera une priorité immédiatement après la résolution des problèmes de production, le cas échéant. Toute panne d’un sandbox à actualisation personnalisée Workfront le week-end (le samedi et le dimanche) sera résolue afin d’assurer son fonctionnement pendant les heures de travail le lundi.

* La relecture n’est pas disponible dans les sandbox à actualisation personnalisée.
