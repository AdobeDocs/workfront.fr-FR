---
product-area: projects
navigation-topic: use-the-home-area
title: Utiliser la zone Mes mises à jour
description: La zone [!UICONTROL Mes mises à jour] vous permet d’examiner rapidement les approbations en attente de votre décision ou les conversations auxquelles vous participez.
author: Lisa
feature: Get Started with Workfront
exl-id: 809605a0-8c24-4873-b98f-504a158be022
source-git-commit: 4c17466705873b06e7ea7bb08bb78a7e68078f8b
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 92%

---

# Utiliser la zone [!UICONTROL Mes mises à jour]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: there is a similar article like this in the "My Work" folder that is conditioned for Classic only)</p>
-->

La zone [!UICONTROL Mes mises à jour] vous permet d’examiner rapidement les approbations en attente de votre décision ou les conversations auxquelles vous participez.

En tant que titulaire d’une licence de [!UICONTROL Révision], vous trouverez la zone [!UICONTROL Mes mises à jour] dans le [!UICONTROL Menu Principal] par défaut et la zone [!UICONTROL Mes mises à jour] est la page de destination par défaut.

Pour plus d’informations sur les licences [!DNL Adobe Workfront], consultez la section [[!DNL Adobe Workfront] Vue d’ensemble des licences](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Si vous avez un type de licence autre que Révision, l’administrateur ou l’administratrice [!DNL Workfront] ou de groupe doit ajouter la zone [!UICONTROL Mes mises à jour] à votre modèle de mise en page pour l’afficher dans le menu principal. Pour plus d’informations, consultez la section [Personnaliser le [!UICONTROL Menu Principal] à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure</p>
   Ou   
   <p>Actuel : [!UICONTROL Request] ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>Accès en affichage ou supérieur à tout objet pour lequel vous êtes tagué dans une conversation ou pour lequel vous devez résoudre une approbation (projets, tâches, problèmes, documents)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations d’[!UICONTROL View] ou supérieures pour les projets, les tâches, les problèmes et les documents où vous êtes tagué dans une conversation ou devez résoudre une approbation</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront]. Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Vous devez disposer des éléments suivants avant de commencer :

* Si vous avez une licence [!DNL Workfront] autre que [!UICONTROL Révision], votre administrateur ou administratrice [!DNL Workfront] ou de groupe doit ajouter la zone [!UICONTROL Mes mises à jour] au [!UICONTROL Menu Principal] à l’aide d’un modèle de mise en page et vous attribuer ce modèle.

* Pour les titulaires d’une licence de révision, la zone [!UICONTROL Mes mises à jour] s’affiche par défaut dans le [!UICONTROL Menu Principal].

## Accéder à la zone [!UICONTROL Mes mises à jour]

1. Cliquez sur **[!UICONTROL Mes mises à jour]** dans le **[!UICONTROL Menu principal]**.

   ![](assets/access-my-updates-from-main-menu-reviewer-user-nwe-350x294.png)

   La zone [!UICONTROL Mes mises à jour] s’affiche.

   Les approbations et demandes d’accès qui vous sont affectées sont répertoriées dans la première moitié de la page, sous **Mes mises à jour**.

   ![](assets/my-updates-mentions-for-reviwers-nwe-350x418.png)

1. (Facultatif) Faites défiler l’écran jusqu’au bas de la zone [!UICONTROL Mes mises à jour] et cliquez sur la flèche droite pour afficher davantage d’approbations sur d’autres pages.

   >[!TIP]
   >
   >Les cinq premières approbations ou demandes d’accès s’affichent par défaut. Les approbations restantes s’affichent sur les pages suivantes. Vous pouvez afficher un maximum de 2 000 approbations dans la zone [!UICONTROL Mes mises à jour].

   ![](assets/pagination-for-my-updates-page-highlighted-nwe-350x78.png)

1. (Facultatif) Développez le menu déroulant **[!UICONTROL Filtrer]** ![](assets/filter-nwepng.png) dans le coin supérieur droit de la section **[!UICONTROL Mes mises à jour]** et sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>Approbations qui vous sont soumises ou qui vous ont été déléguées par une autre personne. Pour plus d’informations sur la délégation des approbations, consultez la section <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Déléguer une demande d’approbation</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated Approvals]</strong></td> 
      <td>Approbations qui vous ont été déléguées par une autre personne </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Approvals]</strong></td> 
      <td> <p>Approbations qui vous ont été envoyées. </p> <p>Pour plus d’informations sur l’approbation d’éléments, consultez la section <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Approuver le travail</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pour approuver ou rejeter un élément ou suggérer des modifications à un document avant d’approuver, procédez comme suit :

   1. (Facultatif) Cliquez sur l’icône **menu déroulant** ![](assets/down-arrow-blue.png) en regard de votre décision d’approbation (**[!UICONTROL Approuver]**, **[!UICONTROL Modifications]**,**[!UICONTROL Rejeter]**), puis ajoutez un commentaire et cliquez sur **[!UICONTROL Ajouter]**.

      Ou

      Cliquez sur **[!UICONTROL Ignorer]** si vous ne souhaitez pas saisir de commentaire.

      ![](assets/approval-decision-buttons-in-my-updates-with-comment-box-nwe-350x183.png)

      >[!NOTE]
      >
      >L’option [!UICONTROL Modifications] s’affiche uniquement pour les approbations de documents.

      Selon l’icône déroulante que vous avez sélectionnée, l’élément est approuvé, rejeté ou, dans le cas d’une approbation de document, approuvé avec une demande de modification supplémentaire.

      >[!TIP]
      >
      >Si vous ne souhaitez pas ajouter de commentaire à votre décision, cliquez sur le bouton **[!UICONTROL Approuver]**, **[!UICONTROL Rejeter]** ou **[!UICONTROL Modifications]** pour entériner directement votre décision d’approbation.
      >
      >
      >![](assets/approval-decision-buttons-in-my-updates-nwe-350x169.png)
      >
      >Pour plus d’informations sur l’approbation du travail, consultez la section [Approuver le travail](../../../review-and-approve-work/manage-approvals/approving-work.md).

1. Cliquez sur **[!UICONTROL Accorder l’accès]** pour accorder la demande d’accès qui vous a été envoyée.

   Ou

   Développez le menu déroulant **[!UICONTROL Modifier l’accès]** pour modifier l’accès demandé avant de l’accorder.

   ![](assets/grant-access-button-in-my-updates-nwe-350x224.png)

1. (Facultatif) Cliquez sur **[!UICONTROL Ignorer]** pour effacer la demande d’accès de votre liste d’approbation sans l’accorder.
1. Cliquez sur **[!UICONTROL Déléguer mes approbations]** pour déléguer les approbations qui vous ont été envoyées si vous n’êtes pas en mesure de prendre des décisions d’approbation pendant une certaine période. Pour plus d’informations sur la délégation des approbations, consultez la section [Déléguer une demande d’approbation](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).
1. Faites défiler l’écran jusqu’à la zone **[!UICONTROL Mentions]** sous vos approbations. Vous y trouverez tous les éléments qui mentionnent votre nom dans une conversation.

   ![](assets/mentions-area-for-reviewers-nwe-350x191.png)

   >[!TIP]
   >
   >Les 50 premières mentions s’affichent par défaut.

1. (Facultatif) Cliquez sur **[!UICONTROL Afficher d’autres mises à jour]** pour afficher d’autres mentions.
1. (Facultatif) Cliquez sur **[!UICONTROL Répondre]** pour répondre à un commentaire, puis effectuez l’une des opérations suivantes :
   * Commencer à saisir une réponse
   * Utilisez la barre d’outils Texte enrichi pour mettre en forme le texte, ajouter des liens, des listes, des émoticônes, des guillemets ou des images à votre message.
   * Ajoutez des utilisateurs ou des équipes pour les avertir de votre réponse.

     Une fois la réponse ajoutée, cliquez sur **[!UICONTROL Répondre]** encore une fois.

     ![](assets/reply-in-the-my-updates-area.png)
1. (Facultatif) Cliquez sur **[!UICONTROL Épingler la page active]** pour épingler la zone [!UICONTROL Mes mises à jour] dans votre navigation supérieure.
