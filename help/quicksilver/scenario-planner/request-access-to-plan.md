---
product-area: enterprise-scenario-planner-product-area
keywords: plan,autorisations,partager,initiatives,scénarios,scénario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Demander l’accès à un plan dans le planificateur de scénarios
description: Vous pouvez demander l’accès à un plan dans le planificateur de scénarios Adobe Workfront lorsque le lien vers le plan est partagé avec vous.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 8%

---

# Demander l’accès à un plan dans le [!DNL Scenario Planner]

Vous pouvez demander l’accès à un plan dans le [!DNL Adobe Workfront Scenario Planner] lorsque le lien vers le plan est partagé avec vous.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p> Formule [!UICONTROL Adobe Workfront]*</p> </td> 
   <td> <p>Actuel : [!UICONTROL Entreprise] ou version ultérieure</p>
   <p>Nouveau : Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td> <p>Nouveau : Léger ou supérieur</p> 
   <p>Actuel : [!UICONTROL Révision] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td>Produit* </td> 
   <td> 
   <p>Pour les plans Workfront actuels : </p>
   <p>Vous devez acheter une licence supplémentaire pour le [!DNL Adobe Workfront Scenario Planner] afin d’accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’accès et les autorisations pour [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser le [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Niveau d’accès </td> 
   <td> <p>Accès à l’[!UICONTROL View] au [!DNL Scenario Planner]</p> </td> 
  </tr> 
   </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir demander l’accès à un plan dans le [!DNL Scenario Planner], vous devez disposer des éléments suivants :

* Lien vers le plan.

>[!NOTE]
>
>Si vous ne disposez pas des droits de niveau d&#39;accès à [!DNL Scenario Planner] et que vous essayez d&#39;accéder à un plan à partir d&#39;un lien, vous ne pouvez pas demander l&#39;accès au plan. À la place, un écran s’affiche pour vous informer de contacter l’administrateur [!DNL Workfront].

## Demande d’accès aux plans dans le [!DNL Workfront Scenario Planner]

Si vous ne disposez pas déjà d’autorisations sur un plan et que vous y accédez à partir d’un lien partagé avec vous, un écran s’affiche pour vous informer que vous ne disposez pas des autorisations nécessaires pour afficher le plan. Vous êtes invité à demander des autorisations au créateur du plan.

>[!TIP]
>
>Vous pouvez uniquement demander des autorisations au propriétaire ou au créateur d’un plan. Vous ne pouvez pas demander d’autorisations à d’autres utilisateurs qui ont également accès au plan.

Pour demander des autorisations :

1. Cliquez sur un lien vers un plan.

   ![](assets/request-access-to-plan-350x277.png)

1. Dans le menu déroulant **[!UICONTROL Demander l’accès à]** , indiquez le niveau d’autorisation que vous souhaitez obtenir. Sélectionnez l’une des options suivantes :

   * [!UICONTROL Afficher]
   * [!UICONTROL Gérer]

   Vous ne pouvez pas demander une autorisation supérieure à votre niveau d’accès à [!DNL Scenario Planner]. Par exemple, vous ne pouvez pas demander les autorisations [!UICONTROL Gérer] si vous disposez d’un accès Affichage à [!DNL Scenario Planner].

   Pour plus d’informations sur les différents niveaux d’autorisations, voir [Partage d’un plan dans le  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

   Pour plus d’informations sur un administrateur Workfront qui peut gérer l’accès à [!DNL Scenario Planner], voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facultatif) Saisissez un commentaire ou une requête dans la **[!UICONTROL zone Laisser le commentaire]**, puis cliquez sur **[!UICONTROL Demander l’accès]**.

   Les événements suivants se produisent :

   * [!DNL Workfront] envoie une notification électronique au propriétaire du plan où il peut lui accorder les autorisations demandées.\
     ![](assets/request-access-to-plan-email-350x156.png)

   * Une fois que le propriétaire du plan a accordé les autorisations demandées, vous recevez un courrier électronique vous indiquant que les autorisations ont été accordées si l’administrateur [!DNL Workfront] a activé le partage d’objet avec la notification utilisateur dans votre système et que vous activez la notification électronique [!UICONTROL Quelqu’un partage un objet avec moi] dans votre profil.

     ![](assets/access-granted-to-plan-email-350x172.png)

   * Vous pouvez également accorder des autorisations aux plans de la zone [!UICONTROL Accueil] et de l’application mobile [!DNL Workfront].

   Pour plus d&#39;informations sur l&#39;activation des notifications système, voir [Configuration des notifications d&#39;événement pour tous les membres du système](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Pour plus d’informations sur l’activation des notifications dans votre profil, voir [Notifications : Informations diverses](../workfront-basics/using-notifications/notifications-misc-information.md).
