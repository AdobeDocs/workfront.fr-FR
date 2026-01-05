---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Afficher le journal d’activité Jira
description: En tant qu’administrateur ou administratrice  [!DNL Jira] , vous pouvez visualiser les exceptions et erreurs qui se produisent lors de la synchronisation ou de la création des tickets entre  [!DNL Adobe Workfront]  et  [!DNL Jira]  dans un journal d’activité.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 66%

---

# Afficher le Journal d’activité [!UICONTROL [!DNL Jira]]

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

En tant qu’administrateur ou administratrice [!DNL Jira], vous pouvez visualiser les exceptions et erreurs qui se produisent lors de la synchronisation ou de la création des tickets entre [!DNL Adobe Workfront] et [!DNL Jira] dans un [!UICONTROL Journal d’activité].

Vous pouvez voir jusqu’à 500 éléments dans le journal d’activité. Ils sont répertoriés en partant des plus récents.

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

+++

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez :

* Installer [!DNL Workfront for Jira]

  Pour obtenir des instructions sur l’installation de [!DNL Workfront for Jira], voir [Installer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Accédez au Journal d’activité [!UICONTROL [!DNL Jira]] :

1. Connectez-vous à Jira en tant qu’administrateur ou administratrice système.
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu [!DNL Jira] principal.
1. Cliquez sur **[!UICONTROL Modules complémentaires]**, puis sur **[!UICONTROL Gérer les modules complémentaires]**.

1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur ou administratrice système.
1. Sélectionnez l’onglet **[!UICONTROL Journal d’activité]**.

   Affichez des informations sur les exceptions et les erreurs survenues lors de la création d’éléments ou de la synchronisation de champs entre les deux applications.

   Le journal comprend les champs suivants :

   * Date de l’occurrence
   * Nom de l’utilisateur ou de l’utilisatrice dans Jira
   * Numéro du problème Jira
   * Brève description de l’erreur qui s’est produite.
