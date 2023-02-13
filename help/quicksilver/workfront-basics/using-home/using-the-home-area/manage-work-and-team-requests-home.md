---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Gérer les requêtes de travail et d’équipe dans la zone d’accueil
description: Lorsque des tâches et des problèmes vous sont assignés, ils sont répertoriés dans la liste [!UICONTROL Liste de tâches] dans le [!UICONTROL Accueil] zone. Vous pouvez afficher, réaffecter, répondre, travailler ou supprimer une requête. Requêtes de travail dans le [!UICONTROL Accueil] ne se limite pas aux problèmes associés aux files d’attente de demandes.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Gérer les requêtes de travail et d’équipe dans [!UICONTROL Accueil] area

Lorsque des tâches et des problèmes vous sont assignés, ils sont répertoriés dans la liste [!UICONTROL Liste de tâches] dans le [!UICONTROL Accueil] zone. Vous pouvez afficher, réaffecter, répondre, travailler ou supprimer une requête. Requêtes de travail dans le [!UICONTROL Accueil] ne se limite pas aux problèmes associés aux files d’attente de demandes.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Accès à [!UICONTROL Modifier] Tâches et problèmes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Attribuez des autorisations ou des autorisations supérieures aux tâches et problèmes sur lesquels vous devez travailler.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Affichage d’une requête de travail

Les requêtes de travail qui vous sont affectées s’affichent dans le panneau de gauche dans [!UICONTROL Accueil]. Vous pouvez configurer les requêtes qui s’affichent dans [!UICONTROL Accueil] en utilisant le filtre en haut de la page [!UICONTROL Liste de tâches].

Vous pouvez sélectionner des filtres qui affichent des éléments prêts à être utilisés ou des éléments sur lesquels vous travaillez déjà.

Cet article décrit comment utiliser les filtres dans la variable [!UICONTROL Accueil] pour afficher les éléments sur lesquels vous travaillez actuellement ou sur lesquels vous envisagez de commencer à travailler. Pour plus d’informations sur tous les filtres de la variable [!UICONTROL Accueil] zone, voir [Afficher des éléments dans la liste des tâches du [!UICONTROL Accueil] area](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur le bouton **[!UICONTROL Filtrer]** menu déroulant.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Cliquez sur l’une ou l’autre des options suivantes pour les tâches :

   **[!UICONTROL Prêt à démarrer]:** Affiche uniquement les tâches et les problèmes prêts à démarrer. Les deux instructions suivantes doivent être vraies :

   * Les tâches et leurs parents n&#39;ont pas de prédécesseurs ou de contraintes de tâche qui les empêchent de travailler.
   * Le [!UICONTROL Date de début planifiée] La liste des tâches ou des problèmes se situe dans les deux dernières semaines ou plus à l’avenir.

   **[!UICONTROL Pas prêt]**: Affiche uniquement les tâches et les problèmes qui ne sont pas encore prêts à démarrer. L’une des instructions suivantes doit être vraie :

   * Les tâches et leurs parents peuvent avoir des prédécesseurs ou des contraintes de tâche qui les empêchent de travailler.
   * Les tâches ou les problèmes ont une [!UICONTROL Date de début planifiée] c&#39;est plus de deux semaines à l&#39;avenir.



1. Cliquez sur **[!UICONTROL Utilisation de]** under [!UICONTROL Tâches] ou [!UICONTROL Problèmes] pour afficher les tâches et les problèmes sur lesquels vous travaillez actuellement.
1. Cliquez sur **[!UICONTROL Demandé]** under [!UICONTROL Problèmes] pour afficher les problèmes qui vous ont été demandés (vous y êtes affecté), mais sur lesquels vous n’avez pas encore accepté de travailler.

## Accès à une demande d’équipe

Vous pouvez accéder à une requête affectée à votre équipe directement à partir de la [!UICONTROL Accueil] zone. Pour plus d’informations sur les requêtes de l’équipe, voir [Présentation des requêtes d’équipe](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans le **[!UICONTROL Liste de tâches]** , cliquez sur pour développer la zone **[!UICONTROL Requêtes d’équipe]** regroupement.

   Si aucune requête n’est affectée à votre équipe, le regroupement ne s’affiche pas.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Cliquez sur le nom de l’équipe.\
   Le **[!UICONTROL Requêtes d’équipe]** affiche et affiche toutes les requêtes affectées à votre équipe. Pour plus d’informations sur l’utilisation des requêtes de l’équipe, voir [Gérer les requêtes de travail et d’équipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Réaffecter une requête

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans le **[!UICONTROL Liste de tâches]** , sélectionnez la requête à réaffecter.

1. Cliquez sur le bouton **[!UICONTROL Affectations]** et supprimez-vous de la requête, puis saisissez le nom de l’utilisateur auquel vous souhaitez réaffecter la requête.

   >[!TIP]
   >
   >Si la demande de travail se trouve toujours à l’état Prêt à démarrer ou Pas prêt, vous pouvez utiliser la variable **[!UICONTROL Réaffecter]** dans le **[!UICONTROL Plus]** dans le menu [!UICONTROL Liste de tâches].\
   >![Bouton Réaffecter](assets/reassign-in-left-panel-350x204.png)

1. Si l’état d’une tâche est modifié en [!UICONTROL Nouveau] ou [!UICONTROL En cours] une fois l’affectation terminée, vous devez annuler l’affectation de l’utilisateur, enregistrer la tâche, puis réaffecter l’utilisateur afin que la tâche réapparaisse dans sa liste de tâches domestiques.

## Réponse à une requête

Vous pouvez répondre à une demande afin de clarifier la demande ou proposer une nouvelle date.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans le **[!UICONTROL Liste de tâches]** , sélectionnez la requête à laquelle vous souhaitez répondre.
1. Localisez la personne qui vous a affecté la requête.

   Vous trouverez ces informations dans la [!UICONTROL Mises à jour] de la tâche. Assurez-vous que l’option **[!UICONTROL Afficher les mises à jour du système]** est activée.

1. Cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et commencez à taper votre réponse.
1. Saisissez le nom du destinataire dans le champ **[!UICONTROL Notifier]** , puis cliquez sur **[!UICONTROL Mettre à jour]**.

   >[!TIP]
   >
   >Si la requête de travail se trouve toujours dans la zone Prêt à démarrer ou [!UICONTROL Pas prêt] vous pouvez utiliser la variable **[!UICONTROL Répondre]** dans le **[!UICONTROL Plus]** dans le menu [!UICONTROL Liste de tâches].\
   >![[!UICONTROL Bouton Répondre]](assets/reassign-in-left-panel-350x204.png)   >

## Utilisation d’une requête

Lorsque vous cliquez sur le bouton [!UICONTROL Travailler dessus] , vous indiquez à l’utilisateur qui a soumis la requête et à tout autre utilisateur qui pourrait être affecté à la requête que vous allez commencer à travailler sur la requête. Pour plus d’informations sur l’utilisation des requêtes, voir  [Gérer les requêtes de travail et d’équipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans le **[!UICONTROL Liste de tâches]** , sélectionnez la requête à utiliser, puis cliquez sur **[!UICONTROL Travailler dessus]**.\
   Les informations sur le problème s’affichent dans le panneau de droite.

## Suppression d’une requête

Si vous décidez de ne pas travailler sur la requête, vous pouvez convertir la tâche ou la renvoyer vers une requête ou la supprimer de votre liste.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans le **[!UICONTROL Liste de tâches]**, pointez sur l’élément en attente de traitement.
1. Cliquez sur le bouton **[!UICONTROL Affectations]** et supprimez-vous. Cette opération supprime l’élément de travail de votre liste de tâches. Si la requête n’est affectée à personne d’autre ou à une autre équipe ou rôle de tâche, elle n’est pas affectée.

   Ou

   Cliquez sur le bouton **[!UICONTROL Plus]** icône de menu ![](assets/more-icon.png) à droite du nom de la tâche ou du problème dans la [!UICONTROL Travail domestique] Liste.

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Sélectionnez l’une des options suivantes :

   * **[!UICONTROL Convertir en requête de travail]:** Sélectionnez cette option pour convertir à nouveau l’élément de travail en requête de travail.\

      L’élément de travail est redirigé vers une requête et vous restez affecté à la requête.\
      Vous pouvez accepter la demande ultérieurement en cliquant sur **[!UICONTROL Travail dessus]** encore une fois.

   * **[!UICONTROL Supprimer]:** Sélectionnez cette option pour supprimer une requête de votre [!UICONTROL Liste de tâches].\

      Vous n’êtes pas affecté à la requête et celle-ci n’est plus associée à votre nom dans [!DNL Adobe Workfront].\
      Si la requête n’est affectée à personne d’autre ou à une autre équipe ou rôle de tâche, elle n’est pas affectée.
