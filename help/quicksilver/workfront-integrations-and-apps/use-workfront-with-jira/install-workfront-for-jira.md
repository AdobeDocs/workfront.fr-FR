---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installer  [!DNL Adobe Workfront]  pour  [!DNL Jira]
description: Vous pouvez utiliser  [!DNL Adobe Workfront]  pour  [!DNL Jira]  afin d’intégrer vos systèmes  [!DNL Jira]  et  [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 79%

---

# Installer [!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, l’intégration Workfront for Jira ne sera plus disponible après le **28 février 2026**.
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre organisation à Jira.
>
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Jira, voir [Modules logiciels Jira](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Vous pouvez utiliser [!DNL Adobe Workfront for Jira] pour intégrer vos systèmes [!DNL Jira] et [!DNL Workfront].

Après l’installation du module complémentaire, vous pouvez définir des workflows qui créent automatiquement des problèmes [!DNL Jira] lorsque des éléments de travail [!DNL Workfront] sont créés. Les éléments des deux applications sont liés et certaines de leurs informations peuvent être automatiquement mises à jour dans les deux systèmes.

Tous les utilisateurs et utilisatrices de [!DNL Workfront] et [!DNL Jira] peuvent bénéficier de cette intégration. Ils n’ont besoin d’une licence que pour le système dans lequel ils travaillent le plus, et non pour les deux systèmes.

Ce module complémentaire est disponible pour les versions [!UICONTROL Serveur] et [!UICONTROL OnDemand] (ou [!UICONTROL Cloud]) du logiciel [!DNL Jira]. Ce module complémentaire n’est pas disponible pour la version [!DNL Data Center] du logiciel [!DNL Jira].

Pour une liste des versions [!DNL Jira] actuellement prises en charge par [!DNL Workfront for Jira], voir [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) sur l’Atlassian Marketplace.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Accès Jira</td> 
   <td> <p>Accès pour l’administration système</p> <p>Important : nous vous recommandons de créer des comptes d’administrateur système distincts dans Jira et Workfront à dédier à cette intégration, plutôt que d’utiliser des comptes existants qui peuvent être associés aux utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++## Installer [!DNL Workfront] pour [!DNL Jira]

L’installation de [!DNL Workfront] pour [!DNL Jira] OnDemand est identique à son installation sur une instance du serveur [!DNL Jira].

Vous devez être un administrateur ou une administratrice de [!DNL Jira] pour installer le module complémentaire [!DNL Workfront].

Si vous n’êtes pas administrateur ou administratrice de [!DNL Jira], vous pouvez rechercher le module complémentaire [!DNL Workfront] et demander son installation. Votre demande est envoyée à l’administration de [!DNL Jira] pour approbation et installation.

Pour plus d’informations sur les demandes d’installation de modules complémentaires sur votre application [!DNL Jira], voir [Gérer les demandes d’utilisateurs et d’utilisatrices relatives aux modules complémentaires.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Pour installer [!DNL Workfront for Jira] :

1. Connectez-vous à [!DNL Jira] en tant qu’administrateur ou administratrice de [!DNL Jira].
1. Recherchez le module complémentaire **[!DNL Workfront for Jira]** dans l’[[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Cliquez sur **[!UICONTROL Obtenir maintenant]** pour l’installer.

   Une fois l’installation terminée, vous pouvez vous connecter à [!DNL Workfront] depuis [!DNL Jira] et configurer votre intégration.

   Pour plus d’informations, voir [Configurer Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considérations pour une installation [!DNL Jira Server]

>[!NOTE]
>
>Ces conditions ne s’appliquent pas à la version [!UICONTROL OnDemand] ([!UICONTROL Cloud]) du logiciel [!DNL Jira].

Bien que l’installation du module complémentaire [!DNL Workfront] soit similaire dans les deux environnements [!DNL Jira], vous devez tenir compte des points suivants lorsque vous utilisez une installation [!DNL Jira Server] :

* Lors de la configuration du module complémentaire dans [!DNL Jira], il se peut que l’adresse spécifiée dans le champ **[!DNL JIRA Base URL]** ne soit pas la même URL utilisée pour accéder à [!DNL Jira] sur votre serveur privé. L’**[!DNL JIRA Base URL]** doit être une adresse accessible au public connectée à votre serveur privé à l’aide de protocoles NAT ou de proxy inverse, de façon à ce que [!DNL Workfront] puisse y accéder pour envoyer des demandes à votre serveur.

* Vous devez utiliser le chiffrement SSL pour sécuriser la communication entre [!DNL Jira] et [!DNL Workfront]. Lorsque vous activez SSL, vous devez disposer d’une pile complète de certificats SSL provenant d’une autorité de certification. Nous ne prenons pas en charge les certificats auto-signés.
* Vous devez vous assurer que le domaine [!DNL jira.workfront.com] est accessible à partir des serveurs de votre entreprise. Il sert d’environnement intermédiaire entre [!DNL Workfront] et [!DNL Jira] et est nécessaire au fonctionnement du module complémentaire.

  Vous devez également ajouter les adresses IP statiques suivantes à la liste autorisée de votre pare-feu pour les connexions sortantes et entrantes.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Pour plus d’informations sur la configuration de votre pare-feu pour des fonctionnalités optimales avec [!DNL Workfront], voir [Configurer votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
