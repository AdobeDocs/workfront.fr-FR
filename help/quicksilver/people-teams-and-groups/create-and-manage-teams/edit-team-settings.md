---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Modifier les paramètres de l’équipe
description: Les administrateurs et administratrices et les utilisateurs et utilisatrices de Workfront disposant d’une licence Plan ou Travail peuvent modifier les paramètres des équipes.
author: Lisa
feature: People Teams and Groups
exl-id: b6761188-8630-446e-bc70-70fe272881ce
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 92%

---

# Modifier les paramètres des équipes

En tant qu&#39;administrateur [!DNL Adobe Workfront] ou utilisateur disposant d&#39;une licence [!UICONTROL Standard], [!UICONTROL Plan] ou [!UICONTROL Travail], vous pouvez modifier les [!UICONTROL Paramètres de l&#39;équipe].

Vous pouvez ajouter des utilisateurs et utilisatrices à une équipe, définir le modèle de mise en page de l’équipe et définir la manière dont le statut est enregistré lorsque des éléments de travail sont terminés par une équipe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuellement : Travail ou licence supérieure</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier les paramètres des équipes

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Cliquez sur le menu **[!UICONTROL Plus]** ![](assets/more-icon.png), puis sélectionnez **[!UICONTROL Modifier]**.

   Seuls les membres de l’équipe possédant une licence [!UICONTROL Standard], [!UICONTROL Plan] ou [!UICONTROL Work] peuvent voir cette option.

   Au cas où vous devriez voir l’option [!UICONTROL Modifier] mais qu’elle n’est pas visible, demandez à votre administrateur ou administratrice Workfront de vérifier que [!UICONTROL Paramètres d’équipe] est visible dans le modèle de mise en page pour [!UICONTROL Équipe Scrum], [!UICONTROL Équipe Kanban] ou [!UICONTROL Équipe Waterfall].

   ![](assets/edit-team-settings.png)

1. Dans les paramètres d’équipe, vous pouvez apporter les modifications suivantes :

   * Modifier le nom de l’équipe
   * Désactiver l’équipe
   * Associer l’équipe à un groupe

     >[!NOTE]
     >
     >Lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, l’équipe d’administration peut se charger de la gestion sans en être membre. Les administrateurs et administratrices de groupes peuvent accéder à la zone Équipes à partir du menu principal et cliquer sur la flèche [!UICONTROL Changer d’équipe] ![Icône Changer d’équipe](assets/switch-team-icon.png) pour dresser la liste de toutes les équipes affectées aux groupes qu’ils gèrent.

     Vous pouvez vous assurer que vous associez le bon groupe à l’équipe en le survolant et en cliquant sur l’icône d’information ![](assets/info-icon.png) qui s’affiche à côté. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.

   * Désigner la personne propriétaire de l’équipe
   * Ajouter et supprimer des personnes membres de l’équipe
   * Ajouter une description de l’équipe
   * Appliquer un modèle de mise en page à l’équipe

     Pour plus d’informations sur l’application d’un modèle de mise en page personnalisé à une équipe, consultez la section « Appliquer un modèle personnalisé à une équipe » dans Modifier les zones [!UICONTROL Mon travail] et [!UICONTROL Demandes de travail] avec des modèles de mise en page.

   * Décider si cette équipe est une équipe agile, en sélectionnant l’option **[!UICONTROL Ceci est une équipe Agile]**.

     Pour plus d’informations sur les équipes Agile et sur la manière de gérer le travail au sein d’une équipe Agile, consultez [Créer une équipe Agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * Transformez le bouton [!UICONTROL Travailler sur ce projet] en bouton [!UICONTROL Démarrer]. Pour plus d’informations sur la configuration du bouton [!UICONTROL Démarrer], consultez [Remplacer le bouton Travailler sur ce projet par un bouton [!UICONTROL Démarrer]](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Personnalisez le bouton **[!UICONTROL Terminé]**. Pour plus d’informations sur la personnalisation du bouton [!UICONTROL Terminé], consultez ce qui suit :

      * [Configurer le bouton [!UICONTROL Terminé] pour les tâches](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
      * [Configurer le bouton [!UICONTROL Terminé] pour les problèmes](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
