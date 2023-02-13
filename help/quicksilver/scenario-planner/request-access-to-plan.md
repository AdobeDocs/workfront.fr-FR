---
product-area: enterprise-scenario-planner-product-area
keywords: plan,autorisations,partager,initiatives,scénarios,scénario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Demande d’accès à un plan dans le planificateur de scénarios
description: Vous pouvez demander l’accès à un plan dans le planificateur de scénarios Adobe Workfront lorsque le lien vers le plan est partagé avec vous.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Demandez l’accès à un plan dans la [!DNL Scenario Planner]

Vous pouvez demander l’accès à un plan dans le [!DNL Adobe Workfront Scenario Planner] lorsque le lien vers le plan est partagé avec vous.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review], [!UICONTROL Work] ou [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Product*</strong> </td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour la variable [!DNL Adobe Workfront Scenario Planner] pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention de [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire à l’utilisation du [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Accédez au [!DNL Scenario Planner]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan, type de licence ou accès vous avez, ou si votre société a acheté la variable [!DNL Workfront Scenario Planner], contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Avant de pouvoir demander l’accès à un plan dans le [!DNL Scenario Planner], vous devez disposer des éléments suivants :

* Lien vers le plan.

>[!NOTE]
>
>Si vous ne disposez pas des droits de niveau d’accès à la variable [!DNL Scenario Planner] et si vous essayez d&#39;accéder à un plan à partir d&#39;un lien, vous ne pouvez pas demander l&#39;accès au plan. À la place, un écran s’affiche pour vous informer de contacter le [!DNL Workfront] administrateur.

## Demandez l’accès aux plans dans la section [!DNL Workfront Scenario Planner]

Si vous ne disposez pas déjà d’autorisations sur un plan et que vous y accédez à partir d’un lien partagé avec vous, un écran s’affiche pour vous informer que vous ne disposez pas des autorisations nécessaires pour afficher le plan. Vous êtes invité à demander des autorisations au créateur du plan.

>[!TIP]
>
>Vous pouvez uniquement demander des autorisations au propriétaire ou au créateur d’un plan. Vous ne pouvez pas demander d’autorisations à d’autres utilisateurs qui ont également accès au plan.

Pour demander des autorisations :

1. Cliquez sur un lien vers un plan.

   ![](assets/request-access-to-plan-350x277.png)

1. Dans le **[!UICONTROL Demander l’accès à]** menu déroulant, indiquez le niveau d’autorisation que vous souhaitez accorder. Sélectionnez l’une des options suivantes :

   * [!UICONTROL Afficher]
   * [!UICONTROL Gérer]

   Vous ne pouvez pas demander une autorisation supérieure à votre niveau d’accès au [!DNL Scenario Planner]. Par exemple, vous ne pouvez pas demander [!UICONTROL Gérer] Si vous disposez de l’accès Affichage à la variable [!DNL Scenario Planner].

   Pour plus d’informations sur les différents niveaux d’autorisations, voir [Partager un plan dans la [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

   Pour plus d’informations sur un administrateur Workfront qui peut gérer l’accès à la variable [!DNL Scenario Planner], voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facultatif) Saisissez un commentaire ou une requête dans la variable **[!UICONTROL Laissez la zone de commentaire]**, puis cliquez sur **[!UICONTROL Demande d’accès]**.

   Les événements suivants se produisent :

   * [!DNL Workfront] envoie une notification par e-mail au propriétaire du plan où il peut lui accorder les autorisations demandées.\
      ![](assets/request-access-to-plan-email-350x156.png)

   * Une fois que le propriétaire du plan a accordé les autorisations demandées, vous recevez un courrier électronique vous indiquant que les autorisations ont été accordées si votre [!DNL Workfront] l’administrateur a activé le partage d’objet vers la notification utilisateur dans votre système et vous activez l’option [!UICONTROL Quelqu&#39;un partage un objet avec moi] notification électronique dans votre profil.

      ![](assets/access-granted-to-plan-email-350x172.png)

   * Vous pouvez également accorder des autorisations aux plans à partir de la [!UICONTROL Accueil] et de la zone [!DNL Workfront] application mobile.
   Pour plus d’informations sur l’activation des notifications système, voir [Configuration des notifications d’événement pour tous les membres du système](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Pour plus d’informations sur l’activation des notifications dans votre profil, voir [Notifications : Informations diverses](../workfront-basics/using-notifications/notifications-misc-information.md).
