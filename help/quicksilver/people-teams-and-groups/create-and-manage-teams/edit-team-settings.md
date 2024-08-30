---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Modifier les paramètres de l’équipe
description: Les administrateurs Workfront et les utilisateurs disposant d’une licence Plan ou Travail peuvent modifier les paramètres de l’équipe.
author: Lisa
feature: People Teams and Groups
exl-id: b6761188-8630-446e-bc70-70fe272881ce
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 40%

---

# Modifier les paramètres des équipes

En tant qu&#39;administrateur [!DNL Adobe Workfront] ou utilisateur disposant d&#39;une licence [!UICONTROL Standard], [!UICONTROL Plan] ou [!UICONTROL Travail], vous pouvez modifier les [!UICONTROL Paramètres de l&#39;équipe].

Vous pouvez ajouter des utilisateurs à une équipe, définir le modèle de mise en page de l’équipe et définir comment l’état est enregistré lorsqu’une équipe termine les tâches.

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

   Seuls les membres de l’équipe qui disposent d’une licence de [!UICONTROL plan] ou de [!UICONTROL travail] peuvent voir cette option.

   Si vous devez disposer de l’option [!UICONTROL Modifier] mais que vous ne la voyez pas, demandez à votre administrateur Workfront de vérifier que [!UICONTROL Paramètres de l’équipe] est visible dans le modèle de mise en page pour [!UICONTROL Équipe de déploiement], [!UICONTROL Équipe de Kanban] ou [!UICONTROL Équipe de chute d’eau].

   ![](assets/edit-team-settings-1.png)

1. Dans les paramètres de l’équipe, vous pouvez effectuer les types de modifications suivants :

   * Modification du nom de l’équipe
   * Désactivation de l’équipe
   * Associer l’équipe à un groupe

     >[!NOTE]
     >
     >Lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, l’équipe d’administration peut se charger de la gestion sans en être membre. Les administrateurs de groupe peuvent accéder à la zone Équipes à partir du menu principal et cliquer sur la flèche [!UICONTROL Changer d’équipe] ![Icône Changer d’équipe](assets/switch-team-icon.png) pour répertorier toutes les équipes affectées aux groupes qu’ils gèrent.

     Vous pouvez vous assurer que vous associez le groupe approprié à l’équipe en pointant dessus et en cliquant sur l’icône d’information ![](assets/info-icon.png) qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.

   * Désignation du propriétaire de l’équipe
   * Ajout et suppression de membres de l’équipe
   * Ajouter une description de l’équipe
   * Application d’un modèle de mise en page à l’équipe

     Pour plus d’informations sur l’application d’un modèle de mise en page personnalisé à une équipe, reportez-vous à la section &quot;Application d’un modèle personnalisé à une équipe&quot; dans Modification des zones [!UICONTROL Mon travail] et [!UICONTROL Requêtes de travail] avec des modèles de mise en page.

   * Déterminez si cette équipe est agile en sélectionnant l’option **[!UICONTROL This is an Agile Team]** .

     Pour plus d’informations sur les équipes agiles et sur la gestion du travail au sein d’une équipe agile, voir [Création d’une équipe agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * Remplacez le bouton [!UICONTROL Work On It] par un bouton [!UICONTROL Start]. Pour plus d’informations sur la configuration du bouton [!UICONTROL Démarrer], voir [Remplacer le bouton Travailler dessus par un bouton [!UICONTROL Démarrer]](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Personnalisez le bouton **[!UICONTROL Terminé]** . Pour plus d’informations sur la personnalisation du bouton [!UICONTROL Terminé], voir :

      * [Configurer le bouton [!UICONTROL Terminé] pour les tâches](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
      * [Configurer le bouton [!UICONTROL Terminé] pour les problèmes](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
