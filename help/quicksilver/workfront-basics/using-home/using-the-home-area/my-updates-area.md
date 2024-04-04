---
product-area: projects
navigation-topic: use-the-home-area
title: Utilisation de la zone Mes mises à jour
description: Vous pouvez utiliser la variable [!UICONTROL Mes mises à jour] pour vérifier rapidement les approbations en attente de votre décision ou les conversations dans lesquelles vous avez été inclus.
author: Lisa
feature: Get Started with Workfront
exl-id: 809605a0-8c24-4873-b98f-504a158be022
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Utilisez la variable [!UICONTROL Mes mises à jour] area

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: there is a similar article like this in the "My Work" folder that is conditioned for Classic only)</p>
-->

Vous pouvez utiliser la variable [!UICONTROL Mes mises à jour] pour vérifier rapidement les approbations en attente de votre décision ou les conversations dans lesquelles vous avez été inclus.

En tant qu’utilisateur avec un [!UICONTROL Réviser] , vous pouvez trouver le [!UICONTROL Mes mises à jour] dans la zone [!UICONTROL Menu Principal] par défaut et la variable [!UICONTROL Mes mises à jour] est la page d’entrée par défaut.

Pour plus d’informations sur [!DNL Adobe Workfront] licences, voir [[!DNL Adobe Workfront] Présentation des licences](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Si vous avez un type de licence différent de Review, la variable [!DNL Workfront] ou l’administrateur de groupe doit ajouter la variable [!UICONTROL Mes mises à jour] à votre modèle de mise en page pour l’afficher dans le menu principal. Pour plus d’informations, voir [Personnalisez le [!UICONTROL Menu Principal] utilisation d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Nouveau : contributeur ou version ultérieure</p>
   Ou   
   <p>Actuel : [!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>Afficher l’accès ou une version supérieure à tout objet pour lequel vous êtes balisé dans une conversation ou dont vous devez résoudre une approbation (Projets, tâches, problèmes, documents)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations [!UICONTROL Afficher] ou supérieures pour les projets, les tâches, les problèmes, les documents dans lesquels vous êtes balisé dans une conversation ou qui doivent résoudre une approbation</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Avant de commencer, vous devez disposer des éléments suivants :

* Si vous avez une [!DNL Workfront] licence autre que [!UICONTROL Réviser], votre [!DNL Workfront] ou l’administrateur de groupe doit ajouter la variable [!UICONTROL Mes mises à jour] à la zone [!UICONTROL Menu Principal] en utilisant un modèle de mise en page et en vous attribuant ce modèle.

* Les utilisateurs de licence de révision peuvent afficher la variable [!UICONTROL Mes mises à jour] leur zone [!UICONTROL Menu Principal] par défaut.

## Accédez au [!UICONTROL Mes mises à jour] area

1. Cliquez sur **[!UICONTROL Mes mises à jour]** dans le **[!UICONTROL Menu Principal]**.

   ![](assets/access-my-updates-from-main-menu-reviewer-user-nwe-350x294.png)

   La variable [!UICONTROL Mes mises à jour] s’ouvre.

   Les approbations et demandes d’accès qui vous sont affectées sont répertoriées dans la première moitié de la page, sous **Mes mises à jour**.

   ![](assets/my-updates-mentions-for-reviwers-nwe-350x418.png)

1. (Facultatif) Faites défiler l’écran jusqu’au bas de la page [!UICONTROL Mes mises à jour] et cliquez sur la flèche pointant vers la droite pour afficher davantage de validations affichées sur des pages supplémentaires.

   >[!TIP]
   >
   >Les cinq premières validations ou demandes d&#39;accès s&#39;affichent par défaut. Les validations restantes s’affichent sur des pages supplémentaires. Vous pouvez afficher un maximum de 2 000 approbations dans la variable [!UICONTROL Mes mises à jour] zone.

   ![](assets/pagination-for-my-updates-page-highlighted-nwe-350x78.png)

1. (Facultatif) Développez la variable **[!UICONTROL Filtrer]** menu déroulant ![](assets/filter-nwepng.png) dans le coin supérieur droit du **[!UICONTROL Mes mises à jour]** et sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Toutes]</strong></td> 
      <td>Approbations qui vous sont soumises ou qui vous ont été déléguées par un autre utilisateur. Pour plus d’informations sur la délégation des approbations, voir <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Déléguer la demande d’approbation</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approbations déléguées]</strong></td> 
      <td>Approbations déléguées par un autre utilisateur. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Mes approbations]</strong></td> 
      <td> <p>Validations qui vous ont été soumises. </p> <p>Pour plus d’informations sur l’approbation des éléments, voir <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Valider le travail </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pour approuver ou rejeter un élément ou suggérer des modifications à un document avant d’approuver, procédez comme suit :

   1. (Facultatif) Cliquez sur le **menu déroulant** icon ![](assets/down-arrow-blue.png) en regard de votre décision d’approbation (**[!UICONTROL Approuver]**, **[!UICONTROL Modifications]**,**[!UICONTROL Rejeter]**), puis ajoutez un commentaire, puis cliquez sur **[!UICONTROL Ajouter]**.

      Ou

      Cliquez sur **[!UICONTROL Ignorer]** si vous ne souhaitez pas saisir de commentaire.

      ![](assets/approval-decision-buttons-in-my-updates-with-comment-box-nwe-350x183.png)

      >[!NOTE]
      >
      >La variable [!UICONTROL Modifications] s’affiche uniquement pour les approbations de documents.

      Selon l’icône déroulante que vous avez sélectionnée, l’élément est approuvé, rejeté ou, dans le cas d’une validation de document, approuvé avec une demande de modification supplémentaire.

      >[!TIP]
      >
      >Si vous ne souhaitez pas ajouter de commentaire à votre décision, vous pouvez cliquer sur le bouton **[!UICONTROL Approuver]**, **[!UICONTROL Rejeter]**, ou **[!UICONTROL Modifications]** et la décision de validation est immédiatement accordée.
      >
      >
      >![](assets/approval-decision-buttons-in-my-updates-nwe-350x169.png)
      >
      >Pour plus d’informations sur la validation d’un travail, voir [Valider le travail](../../../review-and-approve-work/manage-approvals/approving-work.md).

1. Cliquez sur **[!UICONTROL Accorder l’accès]** pour accorder la demande d’accès qui vous a été envoyée

   Ou

   Développez l’objet **[!UICONTROL Modifier l’accès]** menu déroulant pour modifier l’accès demandé avant de l’octroyer.

   ![](assets/grant-access-button-in-my-updates-nwe-350x224.png)

1. (Facultatif) Cliquez sur **[!UICONTROL Ignorer]** pour effacer la demande d’accès de votre liste de validation sans l’octroyer.
1. Cliquez sur **[!UICONTROL Déléguer mes approbations]** pour déléguer les validations qui vous ont été soumises si vous n’êtes pas en mesure de prendre des décisions d’approbation pendant un certain temps. Pour plus d’informations sur la délégation des approbations, voir [Déléguer la demande d’approbation](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).
1. Faites défiler l’écran jusqu’à **[!UICONTROL Mentions]** sous vos approbations. Ici, vous pouvez afficher tous les éléments pour lesquels vous avez été inclus dans une conversation.

   ![](assets/mentions-area-for-reviewers-nwe-350x191.png)

   >[!TIP]
   >
   >Les 50 premières mentions s’affichent par défaut.

1. (Facultatif) Cliquez sur **[!UICONTROL Afficher d’autres mises à jour]** pour afficher d’autres mentions.
1. (Facultatif) Cliquez sur **[!UICONTROL Répondre]** pour répondre à un commentaire, saisissez votre réponse, puis cliquez sur **[!UICONTROL Répondre]** encore une fois.

   Pour plus d’informations sur la mise à jour des éléments, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Facultatif) Cliquez sur **[!UICONTROL Pincer la page active]** pour épingler la variable [!UICONTROL Mes mises à jour] à votre navigation supérieure.
