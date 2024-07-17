---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Gérer les requêtes de travail et d’équipe dans la zone d’accueil
description: Lorsque des tâches et des problèmes vous sont assignés, ils sont répertoriés sur la [!UICONTROL liste de tâches] dans la zone [!UICONTROL Accueil]. Vous pouvez afficher, réaffecter, répondre, travailler ou supprimer une requête. Les demandes de travail dans la zone [!UICONTROL Accueil] ne se limitent pas aux problèmes associés aux files d’attente de demandes.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 8%

---

# Gérer les requêtes de travail et d&#39;équipe dans la zone [!UICONTROL Accueil]

Lorsque des tâches et des problèmes vous sont assignés, ils sont répertoriés sur la [!UICONTROL liste de tâches] dans la zone [!UICONTROL Accueil]. Vous pouvez afficher, réaffecter, répondre, travailler ou supprimer une requête. Les demandes de travail dans la zone [!UICONTROL Accueil] ne se limitent pas aux problèmes associés aux files d’attente de demandes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Accès [!UICONTROL Edit] aux tâches et aux problèmes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de contribution ou niveau supérieur pour les tâches et les problèmes sur lesquels vous devez travailler</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Affichage d’une requête de travail

Les requêtes de travail qui vous sont affectées sont affichées dans le panneau de gauche de [!UICONTROL Home]. Vous pouvez configurer les requêtes qui s’affichent dans [!UICONTROL Home] à l’aide du filtre situé en haut de la [!UICONTROL liste de travail].

Vous pouvez sélectionner des filtres qui affichent des éléments prêts à être utilisés ou des éléments sur lesquels vous travaillez déjà.

Cet article décrit comment utiliser les filtres dans la zone [!UICONTROL Accueil] pour afficher les éléments sur lesquels vous travaillez actuellement ou sur lesquels vous pouvez envisager de commencer à travailler. Pour plus d’informations sur tous les filtres de la zone [!UICONTROL Accueil], voir [Afficher les éléments dans la liste de travail dans la [!UICONTROL zone d’accueil]](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **[!UICONTROL Accueil]**.
1. Cliquez sur le menu déroulant **[!UICONTROL Filtre]** .

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Cliquez sur l’une ou l’autre des options suivantes pour les tâches :

   **[!UICONTROL Prêt à démarrer] :** affiche uniquement les tâches et les problèmes prêts à démarrer. Les deux instructions suivantes doivent être vraies :

   * Les tâches et leurs parents n&#39;ont pas de prédécesseurs ou de contraintes de tâche qui les empêchent de travailler.
   * La [!UICONTROL date de début planifiée] des tâches ou des problèmes se situe dans le passé ou jusqu’à deux semaines à l’avenir.

   **[!UICONTROL Non prêt]** : affiche uniquement les tâches et les problèmes qui ne sont pas encore prêts à démarrer. L’une des instructions suivantes doit être vraie :

   * Les tâches et leurs parents peuvent avoir des prédécesseurs ou des contraintes de tâche qui les empêchent de travailler.
   * Les tâches ou problèmes ont une [!UICONTROL Date de début planifiée] qui est de plus de deux semaines à l’avenir.


1. Cliquez sur **[!UICONTROL Travailler sur]** sous [!UICONTROL Tâches] ou [!UICONTROL Problèmes] pour afficher les tâches et les problèmes sur lesquels vous travaillez actuellement.
1. Cliquez sur **[!UICONTROL Requested]** sous [!UICONTROL Problèmes] pour afficher les problèmes qui vous ont été demandés (vous y êtes affecté), mais vous n’avez pas encore accepté de travailler.

## Accès à une demande d’équipe

Vous pouvez accéder à une requête affectée à votre équipe directement depuis la zone [!UICONTROL Accueil]. Pour plus d’informations sur les demandes de l’équipe, voir [Présentation des demandes de l’équipe](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Liste de travail]**, cliquez pour développer le regroupement **[!UICONTROL Requêtes d’équipe]**.

   Si aucune requête n’est affectée à votre équipe, le regroupement ne s’affiche pas.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Cliquez sur le nom de l’équipe.\
   La section **[!UICONTROL Requêtes d’équipe]** s’affiche et affiche toutes les requêtes affectées à votre équipe. Pour plus d’informations sur l’utilisation des requêtes de l’équipe, voir [Gérer les requêtes de travail et d’équipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Réaffecter une requête

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Liste de travail]**, sélectionnez la requête à réaffecter.

1. Cliquez sur le widget **[!UICONTROL Affectations]** et supprimez-vous de la requête, puis saisissez le nom de l’utilisateur auquel vous souhaitez réaffecter la requête.

   >[!TIP]
   >
   >Si la requête de travail est toujours à l’état Prêt à démarrer ou Non prêt, vous pouvez utiliser le bouton **[!UICONTROL Réaffecter]** dans le menu **[!UICONTROL Plus]** de la [!UICONTROL liste de travail].\
   >![Bouton Réaffecter](assets/reassign-in-left-panel-350x204.png)

1. Si l’état d’une tâche est modifié en [!UICONTROL Nouveau] ou [!UICONTROL En cours] une fois qu’elle a été terminée, vous devez annuler l’affectation de l’utilisateur, enregistrer la tâche, puis réaffecter l’utilisateur afin que la tâche réapparaisse dans sa liste de tâches à domicile.

## Réponse à une requête

Vous pouvez répondre à une demande afin de clarifier la demande ou proposer une nouvelle date.

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Work List]**, sélectionnez la requête à laquelle vous souhaitez répondre.
1. Localisez la personne qui vous a affecté la requête.

   Vous trouverez ces informations dans l’onglet [!UICONTROL Mises à jour] de la tâche. Assurez-vous que l’option **[!UICONTROL Afficher les mises à jour du système]** est activée.

1. Cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et commencez à saisir votre réponse.
1. Saisissez le nom du destinataire dans la zone **[!UICONTROL Notifier]**, puis cliquez sur **[!UICONTROL Mettre à jour]**.

   >[!TIP]
   >
   >Si la requête de travail se trouve toujours à l’état Ready to Start ou [!UICONTROL Not Ready] , vous pouvez utiliser le bouton **[!UICONTROL Reply]** dans le menu **[!UICONTROL More]** de la [!UICONTROL Work List].\
   >![[!UICONTROL Bouton Répondre]](assets/reassign-in-left-panel-350x204.png)   >

## Utilisation d’une requête

Lorsque vous cliquez sur le bouton [!UICONTROL Travailler dessus], vous indiquez à l’utilisateur qui a soumis la demande et à tout autre utilisateur qui pourrait être affecté à la demande que vous allez commencer à travailler sur la demande. Pour plus d’informations sur l’utilisation des requêtes, voir [Gérer les requêtes de travail et d’équipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **[!UICONTROL Accueil]**.
1. Dans la zone **[!UICONTROL Work List]**, sélectionnez la requête sur laquelle vous souhaitez travailler, puis cliquez sur **[!UICONTROL Work On It]**.\
   Les informations sur le problème s’affichent dans le panneau de droite.

## Suppression d’une requête

Si vous décidez de ne pas travailler sur la requête, vous pouvez convertir la tâche ou la renvoyer vers une requête ou la supprimer de votre liste.

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **[!UICONTROL Accueil]**.
1. Dans la **[!UICONTROL liste de travail]**, pointez sur l’élément en attente de traitement.
1. Cliquez sur le widget **[!UICONTROL Affectations]** et supprimez-vous. Cette opération supprime l’élément de travail de votre liste de tâches. Si la requête n’est affectée à personne d’autre ou à une autre équipe ou rôle de tâche, elle n’est pas affectée.

   Ou

   Cliquez sur l’icône de menu **[!UICONTROL Plus]** ![](assets/more-icon.png) à droite du nom de la tâche ou du problème dans la liste [!UICONTROL Travail à domicile].

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Sélectionnez l’une des options suivantes :

   * **[!UICONTROL Convertir en requête de travail] :** Sélectionnez cette option pour convertir à nouveau l’élément de travail en requête de travail.\

     L’élément de travail est redirigé vers une requête et vous restez affecté à la requête.\
      Vous pouvez accepter la demande ultérieurement en cliquant de nouveau sur **[!UICONTROL Travailler dessus]**.

   * **[!UICONTROL Supprimer] :** Sélectionnez cette option pour supprimer une requête de votre [!UICONTROL liste de travail].\

     Vous n’êtes pas affecté à la requête et celle-ci n’est plus associée à votre nom dans [!DNL Adobe Workfront].\
      Si la requête n’est affectée à personne d’autre ou à une autre équipe ou rôle de tâche, elle n’est pas affectée.
