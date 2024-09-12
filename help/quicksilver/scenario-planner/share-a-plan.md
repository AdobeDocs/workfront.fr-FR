---
product-area: enterprise-scenario-planner-product-area
keywords: plan,autorisations,partager,initiatives,scénarios,scénario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Partager un plan dans le planificateur de scénarios
description: Vous pouvez partager un plan que vous avez créé dans le planificateur de scénarios Adobe Workfront avec d’autres personnes.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 93%

---

# Partager un plan dans le [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Vous pouvez partager un plan dans le [!DNL Adobe Workfront Scenario Planner] avec d’autres personnes, afin qu’elles puissent collaborer sur le même travail que vous.

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
   <td> <p>[!DNL Adobe Workfront] formule*</p> </td> 
   <td> <ul></li>
   <li><p>Nouveau : Ultimate </p></li>
   <p>Le planificateur de scénario n’est pas disponible pour le nouveau plan Workfront Select ou Workfront. </p>
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
   <td> <p>Accès [!UICONTROL Edit] à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, consultez <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demander l’accès à un plan dans le [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

* Les personnes auxquelles sont attribuées des autorisations pour le plan doivent avoir accès à la zone [!DNL Scenario Planner] dans leurs niveaux d’accès, comme le prévoit votre équipe d’administration [!DNL Workfront] pour recevoir des autorisations sur un plan.

  Par exemple : [!UICONTROL les personnes demandeuses] ne peuvent pas afficher, créer ou modifier des plans. Gardez cela à l’esprit lorsque vous partagez un plan avec une personne disposant d’une licence Demandeur.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Pour plus d’informations sur l’accès au [!DNL Scenario Planner] pour différents types de licence, voir [Accorder l’accès au  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considérations sur le partage des plans

* Tous les utilisateurs, y compris les administrateurs système, n’ont accès qu’aux plans qu’ils ont créés.
* Vous pouvez partager un seul plan, ou partager plusieurs plans, en bloc.
* Vous ne pouvez pas afficher les plans que vous n’avez pas créés ou qui ne sont pas partagés avec vous.
* Vous pouvez uniquement partager un plan avec d’autres personnes. Vous ne pouvez pas partager des plans avec des groupes, des équipes ou des entreprises.
* Vous devez enregistrer le plan avant de pouvoir le partager.
* Vous pouvez partager une URL vers un plan avec une autre personne. Si la personne ne dispose pas des autorisations nécessaires pour au moins afficher le plan, elle peut demander l’accès au plan à une autre personne lorsqu’elle reçoit l’URL. Pour plus d’informations sur la demande d’accès à un plan, voir [Demander l’accès à un plan dans le  [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Lors du partage de plusieurs plans qui ont déjà été partagés avec d’autres personnes, les personnes avec lesquelles vous partagez ne remplacent personne mais sont ajoutées aux personnes existantes de chaque plan que vous avez sélectionné.

## Options d’autorisation pour les plans

Le tableau suivant répertorie les autorisations que vous pouvez accorder lors du partage d’un plan. Pour plus d’informations sur l’accès des personnes en fonction de leur licence, consultez la section [Accorder l’accès au  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Actions</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
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
   <td>Afficher les scénarios</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>Afficher les fonctions</td> 
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
   <td> <p>Créer des scénarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supprimer des initiatives ou des scénarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Copier des scénarios</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Publier des scénarios**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

* Vous devez avoir accès aux données financières pour pouvoir afficher ou gérer les informations financières des plans, même si vous disposez d’autorisations de gestion pour ces derniers. Pour plus d’informations sur l’accès aux données financières, consultez la section [Accorder l’accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

** Pour pouvoir publier des scénarios, vous devez disposer des autorisations de création et de gestion des projets.

Pour plus d’informations sur le niveau d’accès au projet, consultez la section [Accorder l’accès aux projets](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Pour plus d’informations sur les autorisations de projet, voir [Partager un projet dans  [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

## Partager des plans

{{step1-to-scenario-planner}}

1. Cliquez sur le nom de l’objet pour l’ouvrir,

   Ou

   sélectionnez plusieurs plans pour les partager en bloc.

   >[!TIP]
   >
   >Vous pouvez partager un plan en cliquant sur les avatars des personnes avec lesquelles le plan est partagé dans le coin supérieur droit de l’en-tête du plan.

1. (Le cas échéant) Si vous avez ouvert un plan, cliquez sur l’icône **[!UICONTROL Plus]** ![](assets/more-icon.png) à droite du nom du [!UICONTROL Plan], puis cliquez sur **[!UICONTROL Partager]**,

   Ou

   si vous avez sélectionné plusieurs plans à partager en bloc, cliquez sur l’icône **[!UICONTROL Partager]** ![](assets/share-icon-26x26.png) en haut de la liste des plans pour ouvrir la zone d’accès [!UICONTROL Plan].

   >[!TIP]
   >
   >* Les personnes qui disposent d’autorisations pour tous les plans que vous sélectionnez s’affichent dans la zone d’accès [!UICONTROL Plan].
   >* Toutes les personnes supplémentaires sont ajoutées et ne remplacent pas les personnes existantes sur tous les plans sélectionnés.

1. Dans le champ **[!UICONTROL Donner accès au plan à]**, commencez à saisir le nom des personnes avec lesquelles vous souhaitez partager le plan, puis sélectionnez-les lorsqu’elles apparaissent dans la liste.
1. Dans le menu déroulant Autorisations situé à droite du nom d’utilisateur ou d’utilisatrice, sélectionnez le niveau d’autorisation que vous souhaitez leur accorder au plan.
1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>Les personnes avec lesquelles vous partagez le plan auront l’autorisation de l’afficher. Elles ne peuvent pas modifier les informations du plan, ajouter des initiatives ou des scénarios ou publier des scénarios. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Manage]</td> 
      <td> <p>Les personnes avec lesquelles vous partagez le plan disposent des autorisations nécessaires pour le gérer, notamment la modification d’informations, l’ajout d’initiatives ou de scénarios et la publication du plan. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Un plan ne peut être supprimé que par son créateur ou créatrice. Vous ne pouvez pas supprimer les plans qui sont partagés avec vous.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Le plan est maintenant partagé avec les personnes que vous avez spécifiées.

   Vous pouvez afficher les personnes qui disposent d’autorisations pour le plan dans la colonne Partagé avec moi d’une liste de plans ou dans le coin supérieur droit de l’en-tête du plan.

   >[!TIP]
   >
   >Vous pouvez afficher les plans qui sont partagés avec vous en appliquant le filtre [!UICONTROL Partagé avec moi] dans une liste de plans.


