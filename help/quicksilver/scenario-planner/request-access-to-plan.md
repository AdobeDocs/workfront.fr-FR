---
product-area: enterprise-scenario-planner-product-area
keywords: plan, permissions, partage, initiatives, scénarios, scénario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Demander l’accès à un plan dans le planificateur de scénarios
description: Vous pouvez demander l’accès à un plan dans le planificateur de scénarios Adobe Workfront lorsque le lien vers le plan vous est communiqué.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 88%

---

# Demander l’accès à un plan dans le [!DNL Scenario Planner]

Vous pouvez demander l’accès à un plan sur le [!DNL Adobe Workfront Scenario Planner] lorsque le lien vers le plan vous est communiqué.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] formule*</p> </td> 
   <td> <ul></li>
   <li><p>Nouveau : Ultimate </p></li>
   <p>Le planificateur de scénario n’est pas disponible pour les nouveaux plans Workfront Select ou Workfront Prime. </p>
   <li><p>Actuel : [!UICONTROL Business] ou de niveau supérieur</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td> <p>Nouveau : Light ou supérieur</p> 
   <p>Actuel : [!UICONTROL Révision] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td>Produit* </td> 
   <td> <ul><li><p>Pour les nouveaux plans Workfront :</p><p> Adobe Workfront</li></p>
   <li><p>Pour les plans Workfront actuels : </p>
   <p>Adobe Workfront</p> <p>Planificateur de scénarios Adobe Workfront</p></li></ul>

<p>Pour plus d’informations, voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Niveau d’accès </td> 
   <td>  <p>[!UICONTROL View] ou un accès supérieur à [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir demander l’accès à un plan sur le [!DNL Scenario Planner], vous devez disposer des éléments suivants :

* Un lien vers le plan.

>[!NOTE]
>
>Si vous n’avez pas de droits de niveau d’accès au [!DNL Scenario Planner] et que vous essayez d’accéder à un plan à partir d’un lien, vous ne pouvez pas demander l’accès au plan. Au lieu de cela, un écran s’affiche et vous invite à contacter l’administrateur ou l’administratrice de [!DNL Workfront].

## Demander l’accès aux plans dans le [!DNL Workfront Scenario Planner]

Si vous n’avez pas encore d’autorisations pour un plan et que vous y accédez à partir d’un lien partagé avec vous, un écran s’affiche pour vous informer que vous n’avez pas les autorisations nécessaires pour consulter le plan. Vous recevez une invitation à demander des autorisations au créateur ou à la créatrice du plan.

>[!TIP]
>
>Vous ne pouvez demander des autorisations qu’auprès de la personne propriétaire ou créatrice d’un plan. Vous ne pouvez pas demander des autorisations à d’autres utilisateurs ou utilisatrices qui ont également accès au plan.

Pour demander des autorisations :

1. Cliquez sur un lien vers un plan.

   ![](assets/request-access-to-plan-350x277.png)

1. Dans le menu déroulant **[!UICONTROL Demander l’accès à]**, indiquez le niveau d’autorisation que vous souhaitez obtenir. Sélectionnez l’une des options suivantes :

   * [!UICONTROL Afficher]
   * [!UICONTROL Gérer]

   Vous ne pouvez pas demander une autorisation supérieure à votre niveau d’accès au [!DNL Scenario Planner]. Par exemple, vous ne pouvez pas demander d’autorisations [!UICONTROL Gérer] si vous disposez de l’accès Afficher au [!DNL Scenario Planner].

   Pour plus d’informations sur les différents niveaux d’autorisations, voir [Partager un plan dans le  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

   Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut gérer l’accès au [!DNL Scenario Planner], voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facultatif) Saisissez un commentaire ou une demande dans la zone **[!UICONTROL Laisser un commentaire]**, puis cliquez sur **[!UICONTROL Demander l’accès]**.

   Ce qui suit se produit :

   * [!DNL Workfront] envoie une notification par e-mail au ou à la propriétaire du plan afin qu’il ou elle accorde les autorisations demandées.\
     ![](assets/request-access-to-plan-email-350x156.png)

   * Une fois que le ou la propriétaire du plan a accordé les autorisations demandées, vous recevez un e-mail indiquant que les autorisations ont été accordées si votre administrateur ou administratrice de [!DNL Workfront] a activé la notification Partage d’objet avec l’utilisateur ou l’utilisatrice dans votre système et si vous avez activé la notification par e-mail [!UICONTROL Quelqu’un partage un objet avec moi] dans votre profil.

     ![](assets/access-granted-to-plan-email-350x172.png)

   * Vous pouvez également accorder des autorisations à des plans à partir de la zone [!UICONTROL Accueil] et de l’application mobile [!DNL Workfront].

   Pour plus d’informations sur l’activation des notifications système, voir [Configurer les notifications d’événements pour tous les utilisateurs et toutes les utilisatrices du système](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Pour plus d’informations sur l’activation des notifications dans votre profil, voir [Notifications : informations diverses](../workfront-basics/using-notifications/notifications-misc-information.md).
