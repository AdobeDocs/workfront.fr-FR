---
product-area: enterprise-scenario-planner-product-area
keywords: plan,autorisations,partager,initiatives,scénarios,scénario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Partage d’un plan dans le planificateur de scénarios
description: Vous pouvez partager un plan que vous avez créé dans le planificateur de scénarios Adobe Workfront avec d’autres utilisateurs.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# Partager un plan dans la [!DNL Scenario Planner]

Vous pouvez partager un plan dans la variable [!DNL Adobe Workfront Scenario Planner] avec d’autres utilisateurs, afin qu’ils puissent collaborer sur le même travail que vous.

>[!TIP]
>
>Si vous envoyez un lien vers un plan à d’autres personnes, vous devez également partager le plan avec elles pour qu’elles puissent le consulter.

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
   <td> <p>[!UICONTROL Review] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produit</b> </td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour la variable [!DNL Adobe Workfront Scenario Planner] pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention de [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Accès à l’accès à la fonction [!UICONTROL Modifier] [!DNL Scenario Planner]</p> <p>Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p> Autorisations [!UICONTROL Gérer] pour le plan
     <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL Demander] l’accès à un plan dans la variable [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

* Les utilisateurs auxquels sont attribués des autorisations pour le plan doivent avoir accès à la variable [!DNL Scenario Planner] dans leur niveau d’accès, comme le prévoit votre [!DNL Workfront] pour recevoir des autorisations sur un plan.

   Par exemple : [!UICONTROL Demandeurs] ne peuvent pas afficher, créer ou modifier des plans. Gardez cela à l’esprit lorsque vous partagez une formule avec un utilisateur disposant d’une licence Requestor.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Pour plus d’informations sur l’accès au [!DNL Scenario Planner] pour différents types de licence, voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considérations sur le partage des plans

* Vous pouvez partager un seul plan, ou partager plusieurs plans, en bloc.
* Vous ne pouvez pas afficher les plans que vous n’avez pas créés ou qui ne sont pas partagés avec vous.
* Vous pouvez uniquement partager un forfait avec d’autres utilisateurs. Vous ne pouvez pas partager des plans avec des groupes, des équipes ou des entreprises.
* Vous devez d’abord enregistrer un plan avant de pouvoir le partager.
* Vous pouvez partager une URL avec un plan avec un autre utilisateur. Si l’utilisateur ne dispose pas des autorisations nécessaires pour au moins afficher le plan, il peut demander l’accès au plan à un autre utilisateur lorsqu’il reçoit l’URL. Pour plus d’informations sur la demande d’accès à un plan, voir [Demandez l’accès à un plan dans la [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Lors du partage de plusieurs plans qui ont déjà été partagés avec d’autres, les utilisateurs avec lesquels vous partagez ne remplacent pas mais sont ajoutés aux utilisateurs existants de chaque plan que vous avez sélectionné.

## Partage de plans

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **[!UICONTROL Scénarios]**.
1. Cliquez sur le nom d&#39;un plan pour l&#39;ouvrir.

   Ou

   Sélectionnez plusieurs plans pour les partager en bloc.

   >[!TIP]
   >
   >Vous pouvez partager un plan en cliquant sur les avatars des utilisateurs avec lesquels le plan est partagé dans le coin supérieur droit de l’en-tête du plan.

1. (Conditionnel) Si vous avez ouvert un plan, cliquez sur le bouton **[!UICONTROL Plus]** icon ![](assets/more-icon.png) à droite du [!UICONTROL Plan] name, puis cliquez sur **[!UICONTROL Partager]**

   Ou

   Si vous avez sélectionné plusieurs plans à partager en bloc, cliquez sur l’icône **[!UICONTROL Partager]** icon ![](assets/share-icon-26x26.png) en haut de la liste des projets d’ouverture de la [!UICONTROL Plan] de la boîte d’accès.

   >[!TIP]
   >
   >* Les utilisateurs qui disposent d’autorisations pour tous les plans que vous sélectionnez s’affichent dans la variable [!UICONTROL Plan] de la boîte d’accès.
   >* Tous les utilisateurs supplémentaires sont ajoutés et ne remplacent pas les utilisateurs existants sur tous les plans sélectionnés.


1. Dans le **[!UICONTROL Accéder à un plan]** , commencez à saisir le nom des utilisateurs avec lesquels vous souhaitez partager le plan, puis sélectionnez-les lorsqu’ils apparaissent dans la liste.
1. Dans le menu déroulant Autorisations situé à droite du nom d’utilisateur, sélectionnez le niveau d’autorisation que vous souhaitez leur accorder au plan.
1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>Les utilisateurs avec lesquels vous partagez le plan auront l’autorisation d’afficher le plan. Ils ne peuvent pas modifier les informations sur le plan, ajouter des initiatives, des scénarios ou publier des scénarios. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Gérer]</td> 
      <td> <p>Les utilisateurs avec lesquels vous partagez le plan disposent des autorisations nécessaires pour le gérer, ce qui inclut la modification des informations, l’ajout d’initiatives, de scénarios et la publication du plan. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Vous ne pouvez supprimer un plan que lorsque vous l’avez créé. Vous ne pouvez pas supprimer les plans qui sont partagés avec vous.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Le plan est maintenant partagé avec les utilisateurs que vous avez spécifiés.

   Vous pouvez afficher les utilisateurs qui possèdent des autorisations sur le plan dans la colonne Partagé avec moi dans une liste de plans ou dans le coin supérieur droit de l’en-tête du plan.

   >[!TIP]
   >
   >Vous pouvez afficher les plans qui sont partagés avec vous en appliquant le [!UICONTROL Partagé avec moi] filtrer dans une liste de plans.

## Options d’autorisation Planifier

Le tableau suivant répertorie les autorisations que vous pouvez accorder lors du partage d’un plan. Pour plus d’informations sur l’accès des utilisateurs en fonction de leur licence, voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Actions</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Gérer]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Afficher le plan </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Afficher les initiatives </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Affichage des scénarios</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>Affichage des rôles de tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Afficher les informations sur le coût et le budget*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Gérer les informations de coût et de budget*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Créer des initiatives</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Création de scénarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Suppression d’initiatives ou de scénarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Copie de scénarios</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Scénarios de publication**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Vous devez avoir accès aux données financières pour pouvoir afficher ou gérer les informations financières sur les plans, même si vous disposez des autorisations de gestion des plans. Pour plus d’informations sur l’accès aux données financières, voir [Accorder l&#39;accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Pour pouvoir publier des scénarios, vous devez avoir accès aux autorisations de création et de gestion des projets.

Pour plus d’informations sur le niveau d’accès au projet, voir [Accorder l’accès aux projets](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Pour plus d’informations sur les autorisations de projet, voir [Partage d’un projet dans [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
