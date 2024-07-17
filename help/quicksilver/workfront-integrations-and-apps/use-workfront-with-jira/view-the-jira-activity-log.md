---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Afficher le journal d’activité Jira
description: En tant qu'administrateur  [!DNL Jira] , vous pouvez afficher les exceptions et erreurs qui se produisent lors de la synchronisation ou de la création des tickets entre  [!DNL Adobe Workfront]  et  [!DNL Jira]  dans un journal d'activité.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 23%

---

# Afficher le [!UICONTROL [!DNL Jira] Journal d’activité ]

En tant qu&#39;administrateur [!DNL Jira], vous pouvez afficher les exceptions et erreurs qui se produisent lors de la synchronisation ou de la création des tickets entre [!DNL Adobe Workfront] et [!DNL Jira] dans un [!UICONTROL Journal d&#39;activité].

Vous pouvez voir jusqu’à 500 éléments dans le journal d’activité. Ils sont répertoriés à partir des plus récents.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] licences </a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] afin de vous consacrer à cette intégration, plutôt que d’utiliser des comptes existants pouvant être joints aux utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et les administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez :

* Installer [!DNL Workfront for Jira]

  Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Jira], voir [Installation [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Accédez au [!UICONTROL [!DNL Jira] Journal d’activité ] :

1. Connectez-vous à Jira en tant qu’administrateur système.
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu principal [!DNL Jira].
1. Cliquez sur **[!UICONTROL Add-ons]**, puis **[!UICONTROL Gérer les modules complémentaires]**.

1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur système.
1. Sélectionnez l’onglet **[!UICONTROL Journal d’activité]** .

   Affichez des informations sur les exceptions et les erreurs survenues lors de la création d’éléments ou de la synchronisation de champs entre les deux applications.

   Le journal comprend les champs suivants :

   * Date de l’occurrence
   * Nom de l’utilisateur dans Jira
   * Numéro de problème Jira
   * Brève description de l’erreur qui s’est produite.
