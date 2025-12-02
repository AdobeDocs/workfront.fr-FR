---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Environnement  [!DNL Adobe Workfront]  sandbox d’actualisation personnalisé
description: Le sandbox à actualisation personnalisée est un environnement dans lequel vous pouvez effectuer des tests et travailler en utilisant les données de votre environnement de production. Il est également idéal pour réaliser des formations et déterminer le fonctionnement d’une configuration.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 5b5f9083ed4b60fa6642100cfb9b0da46799dffa
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 91%

---

# Environnement de sandbox à actualisation personnalisée [!DNL Adobe Workfront]

Le sandbox à actualisation personnalisée est un environnement dans lequel vous pouvez effectuer des tests et travailler en utilisant les données de votre environnement de production. Il est également idéal pour réaliser des formations et déterminer le fonctionnement d’une configuration.

>[!NOTE]
>
>Il est différent du sandbox de prévisualisation, qui est également un environnement de test qui reproduit votre environnement de production de [!DNL Workfront].
>
>* Les nouvelles fonctionnalités sont introduites dans le sandbox de prévisualisation avant d’être disponibles dans l’environnement de production.
>* Les nouvelles fonctionnalités ne sont pas introduites dans le sandbox à actualisation personnalisée avant d’être disponibles en production.
>
>  De plus, l’obtention du sandbox à actualisation personnalisée nécessite un coût supplémentaire, qui n’est pas nécessaire pour le sandbox de prévisualisation.
>
>  Pour plus d’informations sur le sandbox de prévisualisation, voir [Environnement du sandbox de prévisualisation  [!DNL Adobe Workfront] &#x200B;](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Workfront</td> 
   <td> <p>Prime ou Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Licence Workfront</td> 
   <td> <p>Standard</p><p>Plan</p>  </td> 
  </tr> 
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td><p>Vous devez être un administrateur ou une administratrice Workfront.</p>
   </td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Actualiser le sandbox à actualisation personnalisée

Le sandbox à actualisation personnalisée contient vos données de production réelles et ne s’actualise pas tant que vous ne le planifiez pas. Vous pouvez planifier une actualisation au moment qui vous convient, jusqu’à une fois par semaine.

>[!NOTE]
>
>* Vous ne pouvez pas planifier une actualisation pour le jour en cours. Si, par exemple, la date d’aujourd’hui est le 1er juin, la date la plus proche à laquelle vous pouvez planifier une actualisation est le 2 juin.
>* L’actualisation planifiée se produit parfois pendant la nuit, en fonction du cluster de l’utilisateur ou de l’utilisatrice (les clusters des États-Unis s’actualisent la nuit aux États-Unis). L’heure spécifique est imprévisible en raison des autres clientes et clients de la file d’attente et de la quantité de données actualisée. Si la file d’attente compte de nombreux éléments volumineux, votre actualisation peut ne pas s’exécuter avant plus tard ce jour-là ou le jour suivant.
>* Votre sandbox à actualisation personnalisée comporte toujours les mêmes fonctionnalités de produit que votre environnement de production. Cependant, lorsque vous actualisez votre sandbox à actualisation personnalisée, le branding n’est conservé que pour la couleur d’arrière-plan de l’écran de connexion. L’écran de connexion et les logos de la barre de navigation sont réinitialisés à leurs valeurs par défaut de [!DNL Workfront] et les images de branding que vous avez modifiées avant l’actualisation ne s’affichent pas.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Accéder à la sandbox à actualisation personnalisée à partir de votre environnement de production {#access-the-custom-refresh-sandbox-from-your-production-environment}

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez accéder à votre sandbox à actualisation personnalisée à partir de votre environnement de production.

>[!NOTE]
>
>Si votre compte se trouve sur le cluster 4 (cluster EMEA), vous ne pouvez pas accéder à votre sandbox à actualisation personnalisée à partir de l’environnement de production. Pour plus d’informations sur la manière dont vous pouvez accéder à votre sandbox à actualisation personnalisée lorsque vous avez un compte sur le cluster 4, voir [Accéder au sandbox à actualisation personnalisée pour les comptes sur le cluster 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Accéder au sandbox à actualisation personnalisée pour les comptes sur le cluster 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Pour accéder à votre sandbox à actualisation personnalisée :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![Icône des paramètres d’engrenage](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Système]** > **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Environnement de test]**, cliquez sur **[!UICONTROL Sandbox 1]** ou **[!UICONTROL Sandbox 2]**.

   Votre package de soutien indique si vous avez accès à un seul ou à deux sandbox à actualisation personnalisée.

1. Connectez-vous à l’aide de vos identifiants de sandbox à actualisation personnalisée.

   Vos identifiants de sandbox à actualisation personnalisée sont les mêmes que ceux de production, à moins que vous n’ayez modifié vos identifiants de production depuis la dernière actualisation de votre sandbox à actualisation personnalisée. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu. Elles ne se synchronisent pas automatiquement.

   Le sandbox à actualisation personnalisée affiche la version ainsi que la date de la dernière actualisation dans la bannière en haut de l’écran. Toutes les informations issues de la production sont disponibles et prêtes à l’emploi après une actualisation.

## Accéder au sandbox à actualisation personnalisée à l’aide d’une URL {#access-the-custom-refresh-sandbox-using-a-url}

Toute personne peut accéder au sandbox à actualisation personnalisée à l’aide d’une URL.

* [Accéder au sandbox à actualisation personnalisée pour les comptes des clusters 1, 2, 3 et 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Accéder au sandbox à actualisation personnalisée pour les comptes sur le cluster 4 (comptes EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Accéder au sandbox à actualisation personnalisée pour les comptes des clusters 1, 2, 3 et 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

En fonction de votre package de prise en charge, vous avez accès à un ou deux sandbox à actualisation personnalisée.

Pour accéder à votre sandbox à actualisation personnalisée à l’aide d’une URL :

1. Accédez à cette URL si vous n’avez qu’un seul sandbox à actualisation personnalisée :

   `https://companyname.sb01.workfront.com` (ancienne URL :`https://cr1.attasksandbox.com/`.)

   Ou, si vous disposez de deux sandbox à actualisation personnalisée, en plus des URL ci-dessus, vous pouvez également accéder à l’URL suivante pour accéder à votre deuxième sandbox à actualisation personnalisée :

   `https://companyname.sb02.workfront.com` (ancienne URL :`https://cr2.attasksandbox.com/`)

1. Sur l’écran de connexion, connectez-vous à l’aide de vos identifiants de sandbox à actualisation personnalisée.
1. Les informations d’identification de votre sandbox à actualisation personnalisée sont les mêmes que celles de votre environnement de production, sauf si vous les avez modifiées depuis la dernière actualisation de votre sandbox. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu. Elles ne se synchronisent pas automatiquement.

### Accéder au sandbox à actualisation personnalisée pour les comptes sur le cluster 4 (comptes EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Si votre compte [!DNL Workfront] se trouve sur le cluster 4 (cluster EMEA), vous ne pouvez accéder à votre sandbox à actualisation personnalisée qu’à l’aide d’une URL. Pour savoir à quel cluster appartient votre compte, contactez notre équipe d’assistance clientèle.

En fonction de votre package de prise en charge, vous avez accès à un ou deux sandbox à actualisation personnalisée.

Pour accéder à votre sandbox à actualisation personnalisée à l’aide d’une URL :

1. Accédez à cette URL si vous n’avez qu’un seul sandbox à actualisation personnalisée :

   `https://companyname.sb01.workfront.com` (ancienne URL :`https://cr3.attasksandbox.com`)

   Ou

   Accédez à l’une ou l’autre de ces URL si vous avez deux sandbox à actualisation personnalisée :

   `https://companyname.sb01.workfront.com` (ancienne URL :`https://cr3.attasksandbox.com`)

   `https://companyname.sb02.workfront.com` (ancienne URL :`https://cr4.attasksandbox.com`)

1. Sur l’écran de connexion, connectez-vous à l’aide de vos identifiants de sandbox à actualisation personnalisée.

   Les informations d’identification de votre sandbox à actualisation personnalisée sont les mêmes que celles de votre environnement de production, sauf si vous les avez modifiées depuis la dernière actualisation de votre sandbox. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu. Elles ne se synchronisent pas automatiquement.

## Planifier l’actualisation de votre sandbox à actualisation personnalisée

>[!IMPORTANT]
>
>La durée d’actualisation dépend de la taille des données à actualiser. Pendant le processus d’actualisation, il est essentiel que votre environnement de sandbox à actualisation personnalisée ne soit pas utilisé de quelque manière que ce soit (y compris par les appels API et les intégrations), afin de ne pas faire obstacle au processus d’actualisation. [!DNL Workfront] désactive l’environnement de sandbox à actualisation personnalisée avant qu’il ne se lance, mais vous devez mettre fin à toutes les sessions actives pour vous assurer que l’actualisation soit effectuée.

Si vous avez planifié une actualisation de votre sandbox à actualisation personnalisée, vous pouvez l’annuler en cliquant sur [!UICONTROL Annuler] en haut de la page. Vous pouvez également la reporter à une date ultérieure.

>[!NOTE]
>
>Il n’est pas possible de planifier des actualisations automatiques de sandbox.

Pour planifier une actualisation de votre sandbox à actualisation personnalisée :

1. Connectez-vous à votre sandbox à actualisation personnalisée.
1. Cliquez sur **[!UICONTROL Planifier]** dans la bannière en haut de l’écran et sélectionnez une date dans le calendrier.
1. Sélectionnez une date d’actualisation, puis cliquez sur **[!UICONTROL Planifier l’actualisation]**.

## Passer à l’environnement de production depuis le sandbox à actualisation personnalisée

1. Connectez-vous à votre sandbox à actualisation personnalisée.

   Pour plus d’informations sur l’accès à votre sandbox à actualisation personnalisée, voir [Accéder au sandbox à actualisation personnalisée depuis votre environnement de production](#access-the-custom-refresh-sandbox-from-your-production-environment) ou [Accéder au sandbox à actualisation personnalisée à l’aide d’une URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Cliquez sur **[!UICONTROL Accéder à la production]** dans la bannière en haut de l’écran.

   N’oubliez pas que le travail effectué dans le sandbox ne sera pas visible dans l’environnement de [!UICONTROL production], car le transfert de données est unidirectionnel, de la production vers votre sandbox à actualisation personnalisée, et non l’inverse.

## Recevoir des e-mails du sandbox à actualisation personnalisée

[!DNL Workfront] désactive toute communication par e-mail à partir de l’environnement de sandbox à actualisation personnalisée. Si vous souhaitez recevoir des notifications par e-mail de l’environnement de sandbox à actualisation personnalisée, vous devez activer cette fonctionnalité dans vos paramètres utilisateur. Pour plus d’informations sur l’activation des notifications par e-mail dans l’environnement de sandbox à actualisation personnalisée, voir [Activer l’envoi d’e-mails à partir de l’environnement de prévisualisation des sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La remise de rapports et les notifications push sur l’application mobile sont toujours désactivées pour l’environnement de sandbox à actualisation personnalisée. Ni vous ni l’équipe d’administration de [!DNL Workfront] ne pouvez activer la remise de rapports ou les notifications push pour l’application mobile lorsque vous accédez à l’environnement de sandbox à actualisation personnalisée.\
>Pour plus d’informations sur les remises de rapports pour l’environnement de production, voir [Vue d’ensemble de la remise de rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md). Pour plus d’informations sur les notifications push sur l’application mobile pour l’environnement de production, voir la section dans .

## Configurer l’authentification unique dans le sandbox à actualisation personnalisée

Si vous souhaitez configurer votre sandbox à actualisation personnalisée pour qu’il fonctionne avec une solution d’authentification unique, vous pouvez le faire en le configurant séparément de votre environnement de production. La configuration SSO dans le sandbox à actualisation personnalisée est indépendante de votre configuration SSO dans l’environnement de production.\
Lorsque vous actualisez votre sandbox à actualisation personnalisée, les informations SSO ne sont pas copiées à partir de votre environnement de production pour remplacer la configuration du sandbox à actualisation personnalisée.

Les étapes de configuration de l’authentification unique dans le sandbox à actualisation personnalisée sont similaires à celles de l’environnement de production.\
Pour plus d’informations sur la configuration SSO pour [!DNL Workfront], consultez la section [Vue d’ensemble de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>L’authentification unique n’est pas disponible si l’instance [!DNL Workfront] de votre entreprise utilise l’authentification Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

## Recalcul automatique des chronologies des projets

Recalculer les chronologies permet aux personnes gestionnaires de voir comment des forces extérieures au projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévisionnelles pour le projet.

En tant qu’administrateur ou administratrice Workfront, vous pouvez configurer le moment où Workfront recalcule automatiquement les chronologies de projet. Workfront peut recalculer les chronologies de projet toutes les nuits ou lorsque la portée du projet change, ou les deux.

Pour plus d’informations, voir [Configuration des recalculs de chronologie pour les projets](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Pour l’environnement de sandbox d’actualisation personnalisée, le recalcul nocturne est désactivé et les chronologies du projet ne sont pas recalculées automatiquement. Vous devez recalculer manuellement la chronologie du projet pour l’environnement de sandbox d’actualisation personnalisée. Pour plus d’informations, voir [Recalculer la chronologie du projet](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Utilisation prévue et disponibilité

* Les environnements de sandbox à actualisation personnalisée [!DNL Workfront] ne sont pas destinés aux tests de performance ou de charge. Utilisez-les plutôt pour valider l’efficacité des fonctionnalités avec les workflows existants de votre entreprise.

* Les workflows impliquant des documents doivent se concentrer sur les processus et non sur les tests de chargement. Les fichiers volumineux ne sont pas pris en charge dans les environnements Sandbox.

* Les environnements de sandbox à actualisation personnalisée [!DNL Workfront] sont conçus pour être toujours disponibles. Toute interruption d’un environnement de sandbox à actualisation personnalisée Workfront pendant les heures de bureau sera traitée en priorité, immédiatement après la résolution des problèmes de production, le cas échéant. Toute panne d’un sandbox à actualisation personnalisée Workfront le week-end (le samedi et le dimanche) sera résolue afin d’assurer son fonctionnement pendant les heures de travail le lundi.

* La relecture n’est pas disponible dans les sandbox à actualisation personnalisée.

* Les notifications suivantes ne sont pas disponibles pour une utilisation dans les environnements de sandbox d’actualisation personnalisée :

   * Notifications de rappel
   * Notifications automatiques de rappel de retard ou d’avance
