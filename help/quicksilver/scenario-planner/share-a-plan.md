---
product-area: enterprise-scenario-planner-product-area
keywords: plan,autorisations,partager,initiatives,scénarios,scénario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Partage d’un plan dans le planificateur de scénarios
description: Vous pouvez partager un plan que vous avez créé dans le planificateur de scénarios Adobe Workfront avec d’autres personnes.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 85%

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
   <td> <p>[!DNL Adobe Workfront] paquet</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTE</b></p>
<p>Contactez votre représentant Workfront si vous disposez d’un autre package Workfront.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence</p> </td> 
   <td> <p>[!UICONTROL Light] ou version ultérieure</p> 
   <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
    <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès [!UICONTROL Edit] à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour un plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur l’accès au planificateur de scénarios, voir [&#x200B; Accès nécessaire pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Documentation sur les exigences d’accès à Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

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
* Vous pouvez partager une URL vers un plan avec une autre personne. Si la personne ne dispose pas des autorisations nécessaires pour au moins afficher le plan, elle peut demander l’accès au plan à une autre personne lorsqu’elle reçoit l’URL. Pour plus d’informations sur la demande d’accès à un plan, consultez [Demande d’autorisations pour un plan dans le [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
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

1. (Conditionnel) Si vous avez ouvert un plan, cliquez sur l’icône **[!UICONTROL Plus]** ![Icône Plus](assets/more-icon.png) située à droite du nom [!UICONTROL Plan], puis cliquez sur **[!UICONTROL Partager]**

   Ou

   Si vous avez sélectionné plusieurs plans pour les partager en bloc, cliquez sur l’icône **[!UICONTROL Partager]** ![Icône Partager](assets/share-icon-26x26.png) en haut de la liste des plans pour ouvrir la zone d’accès [!UICONTROL Plan].

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


