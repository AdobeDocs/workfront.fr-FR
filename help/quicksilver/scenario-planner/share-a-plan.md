---
product-area: enterprise-scenario-planner-product-area
keywords: plan,autorisations,partager,initiatives,scénarios,scénario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Partager un plan dans le planificateur de scénarios
description: Vous pouvez partager un plan que vous avez créé dans le planificateur de scénarios Adobe Workfront avec d’autres utilisateurs.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 8%

---

# Partager un plan dans le [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Vous pouvez partager un plan dans le [!DNL Adobe Workfront Scenario Planner] avec d’autres utilisateurs afin qu’ils puissent collaborer sur le même travail que vous.

>[!TIP]
>
>Si vous envoyez un lien vers un plan à d’autres personnes, vous devez également partager le plan avec elles pour qu’elles puissent le consulter.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] forfait*</p> </td> 
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
   <td> <p>Accès à l’accès à la fonction [!UICONTROL Modifier] [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demander l’accès à un plan dans le [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

* Les utilisateurs auxquels des autorisations sont accordées au plan doivent avoir accès à la zone [!DNL Scenario Planner] de leur niveau d’accès, comme accordé par votre administrateur [!DNL Workfront], afin de recevoir des autorisations pour un plan.

  Par exemple, [!UICONTROL Requestors] ne peut pas afficher, créer ou modifier des plans. Gardez cela à l’esprit lorsque vous partagez une formule avec un utilisateur disposant d’une licence Requestor.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Pour plus d’informations sur l’accès à [!DNL Scenario Planner] pour différents types de licence, voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considérations sur le partage des plans

* Tous les utilisateurs, y compris les administrateurs système, n’ont accès qu’aux plans qu’ils ont créés.
* Vous pouvez partager un seul plan, ou partager plusieurs plans, en bloc.
* Vous ne pouvez pas afficher les plans que vous n’avez pas créés ou qui ne sont pas partagés avec vous.
* Vous pouvez uniquement partager un forfait avec d’autres utilisateurs. Vous ne pouvez pas partager des plans avec des groupes, des équipes ou des entreprises.
* Vous devez d’abord enregistrer un plan avant de pouvoir le partager.
* Vous pouvez partager une URL avec un plan avec un autre utilisateur. Si l’utilisateur ne dispose pas des autorisations nécessaires pour au moins afficher le plan, il peut demander l’accès au plan à un autre utilisateur lorsqu’il reçoit l’URL. Pour plus d’informations sur la demande d’accès à un plan, voir [Demande d’accès à un plan dans le  [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Lors du partage de plusieurs plans qui ont déjà été partagés avec d’autres, les utilisateurs avec lesquels vous partagez ne remplacent pas mais sont ajoutés aux utilisateurs existants de chaque plan que vous avez sélectionné.

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
   <td>Scénarios Publish**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Vous devez avoir accès aux données financières pour pouvoir afficher ou gérer les informations financières sur les plans, même si vous disposez des autorisations de gestion des plans. Pour plus d&#39;informations sur l&#39;accès aux données financières, voir [Accorder l&#39;accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Pour pouvoir publier des scénarios, vous devez avoir accès aux autorisations de création et de gestion des projets.

Pour plus d’informations sur le niveau d’accès aux projets, voir [Accorder l’accès aux projets](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Pour plus d’informations sur les autorisations de projet, voir [Partage d’un projet dans [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

## Partage de plans

{{step1-to-scenario-planner}}

1. Cliquez sur le nom d&#39;un plan pour l&#39;ouvrir.

   Ou

   Sélectionnez plusieurs plans pour les partager en bloc.

   >[!TIP]
   >
   >Vous pouvez partager un plan en cliquant sur les avatars des utilisateurs avec lesquels le plan est partagé dans le coin supérieur droit de l’en-tête du plan.

1. (Conditionnel) Si vous avez ouvert un plan, cliquez sur l’icône **[!UICONTROL Plus]** ![](assets/more-icon.png) à droite du nom [!UICONTROL Plan], puis cliquez sur **[!UICONTROL Partager]**

   Ou

   Si vous avez sélectionné plusieurs plans pour les partager en bloc, cliquez sur l&#39;icône **[!UICONTROL Partager]** ![](assets/share-icon-26x26.png) en haut de la liste des plans pour ouvrir la boîte d&#39;accès [!UICONTROL Plan].

   >[!TIP]
   >
   >* Les utilisateurs qui disposent d’autorisations pour tous les plans que vous sélectionnez s’affichent dans la zone d’accès [!UICONTROL Plan] .
   >* Tous les utilisateurs supplémentaires sont ajoutés et ne remplacent pas les utilisateurs existants sur tous les plans sélectionnés.

1. Dans le champ **[!UICONTROL Accorder l’accès au plan à]** , commencez à saisir le nom des utilisateurs avec lesquels vous souhaitez partager le plan, puis sélectionnez-les lorsqu’ils apparaissent dans la liste.
1. Dans le menu déroulant Autorisations situé à droite du nom d’utilisateur, sélectionnez le niveau d’autorisation que vous souhaitez leur accorder au plan.
1. Sélectionnez l’une des options suivantes :

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
   >Vous pouvez afficher les plans qui sont partagés avec vous en appliquant le filtre [!UICONTROL Partagé avec moi] dans une liste de plans.


