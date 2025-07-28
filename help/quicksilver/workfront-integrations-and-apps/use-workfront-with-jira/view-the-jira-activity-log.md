---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Afficher le journal d’activité Jira
description: En tant qu’administrateur ou administratrice  [!DNL Jira] , vous pouvez visualiser les exceptions et erreurs qui se produisent lors de la synchronisation ou de la création des tickets entre  [!DNL Adobe Workfront]  et  [!DNL Jira]  dans un journal d’activité.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 71%

---

# Afficher le Journal d’activité [!UICONTROL [!DNL Jira]]

>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, l’intégration Workfront for Jira ne sera plus disponible après le **28 février 2026**.
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre organisation à Jira.
>
>Huit modèles prêts à l’emploi d’automatisation et d’intégration de Workfront pour Jira seront disponibles d’ici août pour aider à répliquer les workflows courants et à accélérer la mise en œuvre. Les modèles sont entièrement personnalisables pour répondre aux besoins spécifiques de l’entreprise et peuvent être étendus en fonction de l’évolution des besoins.
> 
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Jira, voir [Modules logiciels Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

En tant qu’administrateur ou administratrice [!DNL Jira], vous pouvez visualiser les exceptions et erreurs qui se produisent lors de la synchronisation ou de la création des tickets entre [!DNL Adobe Workfront] et [!DNL Jira] dans un [!UICONTROL Journal d’activité].

Vous pouvez voir jusqu’à 500 éléments dans le journal d’activité. Ils sont répertoriés en partant des plus récents.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan <a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accès</td> 
   <td> <p>Accès pour l’administration système</p> <p>Important : nous vous recommandons de créer des comptes d’administration système distincts dans [!DNL Jira] et [!DNL Workfront] qui seront dédiés à cette intégration, plutôt que d’utiliser des comptes existants, pouvant être associés à des utilisateurs ou utilisatrices existants.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif complet à une personne</a>.</p> <p>Remarque : si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour savoir comment une équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

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
