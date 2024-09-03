---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Gérer les demandes de travail et d’équipe dans la zone d’accueil
description: Lorsque des tâches et des problèmes vous sont affectés, ils sont répertoriés dans la [!UICONTROL liste de travail] dans la zone d’[!UICONTROL accueil]. Vous pouvez consulter une demande, la réaffecter, y répondre, y travailler ou la supprimer. Les demandes de travail dans la zone d’[!UICONTROL accueil] ne se limitent pas aux problèmes liés aux files d’attente des demandes.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 100%

---

# Gérer les demandes de travail et d’équipe dans la zone d’[!UICONTROL accueil] 

Lorsque des tâches et des problèmes vous sont attribués, ils sont répertoriés dans la [!UICONTROL liste de travail] dans la zone d’[!UICONTROL accueil]. Vous pouvez consulter une demande, la réaffecter, y répondre, y travailler ou la supprimer. Les demandes de travail dans la zone d’[!UICONTROL accueil] ne se limitent pas aux problèmes liés aux files d’attente des demandes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Edit] l’accès aux tâches et aux problèmes</p> <p>Note : si vous n’avez toujours pas d’accès, demandez à votre administrateur ou administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies dans votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de contribution ou niveau supérieur pour les tâches et les problèmes sur lesquels vous devez travailler</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Afficher une demande de travail

Les demandes de travail qui vous sont affectées sont affichées dans le panneau de gauche dans l’[!UICONTROL accueil]. Vous pouvez configurer les demandes qui sont affichées dans l’[!UICONTROL accueil] à l’aide du filtre situé en haut de la [!UICONTROL liste de travail].

Vous pouvez sélectionner des filtres qui affichent les éléments prêts à être traités ou les éléments sur lesquels vous travaillez déjà.

Cet article explique comment utiliser les filtres de la zone d’[!UICONTROL accueil] pour afficher les éléments sur lesquels vous travaillez actuellement ou sur lesquels vous pourriez envisager de commencer à travailler. Pour plus d’informations sur tous les filtres de la zone d’[!UICONTROL accueil], voir [Afficher les éléments de la liste de travail dans la zone d’[!UICONTROL accueil]](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur le menu déroulant **[!UICONTROL Filtre]**.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Cliquez sur l’une ou l’autre des options suivantes pour les tâches :

   **[!UICONTROL Prêt à démarrer] :** affiche uniquement les tâches et les problèmes qui sont prêts à démarrer. Les deux affirmations suivantes doivent être vraies :

   * Les tâches et leurs parents n’ont pas de tâches/parents antérieurs ou de contraintes de tâches qui les empêchent d’être traités.
   * La [!UICONTROL date de début prévue] des tâches ou des problèmes se situe dans le passé ou jusqu’à deux semaines dans le futur.

   **[!UICONTROL Pas prêt]** : affiche uniquement les tâches et les problèmes qui ne sont pas encore prêts à démarrer. L’une ou l’autre des affirmations suivantes doit être vraie :

   * Les tâches et leurs parents peuvent avoir des tâches/parents antérieurs ou des contraintes de tâches qui les empêchent d’être traités.
   * Les tâches ou les problèmes ont une [!UICONTROL date de début planifiée] qui se situe plus de deux semaines dans le futur.


1. Cliquez sur **[!UICONTROL En train de travailler sur]** sous [!UICONTROL Tâches] ou [!UICONTROL Problèmes] pour afficher les tâches et les problèmes sur lesquels vous travaillez actuellement.
1. Cliquez sur **[!UICONTROL Demandés]** sous [!UICONTROL Problèmes] pour afficher les problèmes qui vous ont été demandés (qui vous sont affectés), mais sur lesquels vous n’avez pas encore accepté de travailler.

## Accéder à une demande d’équipe

Vous pouvez accéder à une demande assignée à votre équipe directement à partir de la zone  d’[!UICONTROL accueil]. Pour plus d’informations sur les demandes d’équipe, voir [Vue d’ensemble des demandes d’équipe](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Liste de travail]**, cliquez pour développer le regroupement **[!UICONTROL Demandes d’équipe]**.

   Si aucune demande n’est affectée à votre équipe, le regroupement ne s’affiche pas.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Cliquez sur le nom de l’équipe.\
   La section **[!UICONTROL Demandes d’équipe]** affiche toutes les demandes affectées à votre équipe. Pour plus d’informations sur l’utilisation des demandes d’équipe, voir [Gérer les demandes d’équipe et de travail](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Réaffecter une demande

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Liste de travail]**, sélectionnez la demande que vous souhaitez réaffecter.

1. Cliquez sur le widget **[!UICONTROL Affectations]** et retirez-vous de la demande, puis tapez le nom de l’utilisateur ou l’utilisatrice à qui vous voulez réattribuer la demande.

   >[!TIP]
   >
   >Si la demande de travail est toujours au statut Prête à démarrer ou Pas prête, vous pouvez utiliser le bouton **[!UICONTROL Réaffecter]** dans le menu **[!UICONTROL Plus]** dans la [!UICONTROL Liste de travail].\
   >![Bouton de réaffectation](assets/reassign-in-left-panel-350x204.png)

1. Si le statut d’une tâche passe à [!UICONTROL Nouvelle] ou [!UICONTROL En cours] après qu’elle ait été achevée, vous devez annuler l’affectation de l’utilisateur ou de l’utilisatrice, enregistrer la tâche, puis réaffecter l’utilisateur ou l’utilisatrice pour que la tâche réapparaisse dans sa Liste de travail de l’accueil.

## Répondre à une demande

Vous pouvez répondre à une demande pour la clarifier davantage ou pour proposer une nouvelle date.

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Liste de travail]**, sélectionnez la requête à laquelle vous souhaitez répondre.
1. Localisez la personne qui vous a affecté la requête.

   Vous trouverez ces informations dans l’onglet [!UICONTROL Mises à jour] de la tâche. Assurez-vous que l’option **[!UICONTROL Afficher les mises à jour système]** est activée.

1. Cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et commencez à saisir votre réponse.
1. Saisissez le nom de la personne destinataire dans la case **[!UICONTROL Notifier]**, puis cliquez sur **[!UICONTROL Mettre à jour]**.

   >[!TIP]
   >
   >Si la requête de travail a toujours le statut Prêt à démarrer ou [!UICONTROL Pas prêt], vous pouvez utiliser le bouton **[!UICONTROL Répondre]** dans le menu **[!UICONTROL Plus]** de la [!UICONTROL liste de travail].\
   >![[!UICONTROL Bouton Répondre]](assets/reassign-in-left-panel-350x204.png) >

## Travailler sur une requête

Lorsque vous cliquez sur le bouton [!UICONTROL Travailler sur ce projet], vous indiquez à l’utilisateur ou l’utilisatrice qui a soumis la requête et à toute autre personne qui pourrait être affectée à la requête que vous allez commencer à travailler sur celle-ci. Pour plus d’informations sur le traitement des requêtes, consultez [Gérer les requêtes de travail et d’équipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Liste de travail]**, sélectionnez la requête sur laquelle vous voulez travailler, puis cliquez sur **[!UICONTROL Travailler sur ce projet]**.\
   Des informations sur le problème s’affichent dans le panneau de droite.

## Supprimer une requête

Si vous décidez de ne pas travailler sur la requête, vous pouvez soit reconvertir la tâche ou le problème en requête, soit la supprimer de votre liste.

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans la **[!UICONTROL liste de travail]**, pointez l’élément en attente de traitement.
1. Cliquez sur le widget **[!UICONTROL Affectations]** et retirez-vous de la liste. Cette opération supprime l’élément de votre liste de travail. Si la requête n’est affectée à personne d’autre, ni à une autre équipe ou à une autre fonction, elle reste non affectée.

   Ou

   Cliquez sur l’icône de menu **[!UICONTROL Plus]** ![](assets/more-icon.png) à droite du nom de la tâche ou du problème dans la [!UICONTROL Liste de travail de l’accueil].

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Sélectionnez l’une des options suivantes :

   * **[!UICONTROL Convertir en demande de travail] :** sélectionnez cette option pour reconvertir l’élément de travail en requête.

     L’élément de travail redevient une requête et vous restez la personne affectée à la requête.\
      Vous pouvez accepter la requête ultérieurement en cliquant à nouveau sur **[!UICONTROL Travailler sur ce projet]**.

   * **[!UICONTROL Supprimer] :** sélectionnez cette option pour supprimer une requête de votre [!UICONTROL liste de travail].

     Votre affectation à la requête est annulée et celle-ci n’est plus associée à votre nom dans [!DNL Adobe Workfront].\
      Si la requête n’est affectée à personne d’autre, ni à une autre équipe ou à une autre fonction, elle reste non affectée.
