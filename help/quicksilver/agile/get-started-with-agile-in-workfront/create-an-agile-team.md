---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Créer une équipe agile
description: Adobe Workfront permet aux équipes Agile d’effectuer leur travail de manière progressive et organisée.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 91%

---

# Créer une équipe Agile

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] permet aux équipes Agile d’effectuer leur travail de manière progressive et organisée.

Tout utilisateur ou utilisatrice de l’entreprise peut voir l’équipe Agile et afficher tous les composants agiles de l’équipe, y compris la liste d’attente, les itérations, le storyboard et les histoires individuelles. Toutefois, seuls les membres de l’équipe disposant d’un accès [!UICONTROL Modifier] au travail peuvent apporter des modifications au travail affecté à l’équipe.

[!DNL Workfront] prend en charge les méthodologies Agile suivantes :

* **[!UICONTROL Scrum]** : les équipes ont une liste d’attente de travail à faire. Lorsque l’équipe est prête à travailler sur un bloc de travail spécifique, le travail est déplacé de la liste d’attente vers une itération. Pour plus d’informations sur la gestion d’une équipe Scrum, voir [Scrum dans une équipe Agile](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban] :** les équipes déplacent le travail dans la vue Kanban à travers des statuts prédéterminés. Les statuts par défaut sont les suivants : liste d’attente, en cours et terminé. Pour plus d’informations sur la gestion d’une équipe Kanban, voir [Kanban dans une équipe Agile](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouveau : Standard</p>
   Actuel : 
   <ul><li><p>[!UICONTROL Plan] pour créer une nouvelle équipe Agile</p></li> 
   <li><p>[!UICONTROL Work] ou supérieure pour convertir une équipe en équipe Agile</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Choisir une méthodologie Agile

Vous pouvez utiliser une méthodologie agile Scrum ou Kanban pour votre équipe Agile. Chaque méthodologie présente divers avantages. Le fonctionnement de votre équipe Agile détermine la méthodologie Agile que vous choisissez d’utiliser.

Les méthodologies Agile Scrum et Kanban dans [!DNL Workfront] vous permettent de déplacer des histoires dans un storyboard pour indiquer un changement de statut et la progression de l’histoire.

Les méthodologes Agile Scrum et Kanban dans [!DNL Workfront] diffèrent de la manière suivante :

### Avantages de l’utilisation de Kanban dans [!DNL Workfront]

La méthodologie Agile [!DNL Kanban] dans [!DNL Workfront] vous permet de déplacer plus facilement les histoires sur un storyboard agile tout en limitant la quantité de travail en cours. Il n’y a pas de date de début et de fin lors de l’utilisation de la méthodologie Agile [!DNL Kanban].

Les fonctionnalités suivantes prennent en charge cette méthodologie :

* Affichez le journal en souffrance sur le tableau de bord agile [!DNL Kanban].
Pour plus d’informations, voir [Ajouter la liste d’attente au storyboard [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configurez les éléments sur le journal en attente pour qu’ils soient automatiquement ajoutés au panorama d’articles agile [!UICONTROL Kanban] lorsque d’autres éléments sont déplacés vers un état qui correspond à Terminé.
Pour plus d’informations, voir la section [Configurer des histoires à ajouter automatiquement à partir de la liste d’attente](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) dans l’article [Configurer Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configurez une limite de travail en cours (WIP) à afficher sur le panorama dynamique [!UICONTROL Kanban].
Pour plus d’informations, voir [Gérer la limite de travail en cours (WIP) sur le storyboard Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Avantages de l’utilisation de Scrum dans [!DNL Workfront]

La méthodologie Agile Scrum dans [!DNL Workfront] vous permet d’ajouter un ensemble d’histoires à une itération agile et de créer un storyboard pour cette itération. L’itération est basée sur les dates de début et de fin que vous définissez.

Les fonctionnalités suivantes prennent en charge cette méthodologie :

* Inclure les problèmes sur le storyboard [!UICONTROL Scrum]
* Inclure les problèmes sur la liste d’attente d’une équipe Agile
* Les sous-tâches peuvent être affichées sur le storyboard [!UICONTROL Scrum]
* Affichage d’un graphique de condensation pour voir la progression par rapport aux histoires lors de l’itération
Pour plus d’informations, consultez la [présentation d’un graphique de condensation agile](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Créer une équipe Agile

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]**![Icône Changer d’équipe](assets/switch-team-icon.png), puis cliquez sur **[!UICONTROL Créer une nouvelle équipe]**.

   ![Sélectionnez Créer une équipe.](assets/create-new-team-350x198.png)

   La zone Nouvelle équipe s’affiche.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Saisissez le nom de la nouvelle équipe agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL This is an Agile Team]</strong> </td> 
      <td>Sélectionnez cette option pour que cette nouvelle équipe soit configurée comme une équipe agile.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
      <td>Sélectionnez cette option pour activer cette équipe. Les équipes inactives ne sont pas visibles par les autres utilisateurs et utilisatrices pour les affecter au travail. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Commencez à saisir le nom d’un groupe à ajouter à l’équipe, puis sélectionnez-le lorsqu’il apparaît dans la liste déroulante.</p> <p><b>NOTE</b></p> <p> Lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs et administratrices de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membres. Les administrateurs et administratrices de groupe peuvent accéder à la zone [!UICONTROL Teams] à partir du [!UICONTROL Main Menu] et cliquer sur la flèche [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’ils gèrent.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Commencez à saisir le nom d’un utilisateur ou d’une utilisatrice à ajouter à l’équipe, puis sélectionnez le nom lorsqu’il apparaît dans la liste déroulante.<br>Répétez cette procédure pour ajouter plusieurs utilisateurs et utilisatrices à l’équipe.<br>Comme les utilisateurs et utilisatrices peuvent appartenir à plusieurs équipes, ils peuvent appartenir à des équipes agiles et non agiles.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>Saisissez une description pour l’équipe.</p> <p>La description s’affiche en haut à droite de la zone [!UICONTROL Teams] lorsque l’équipe est sélectionnée.</p>
      <p>Si la description est longue, vous pouvez cliquer dessus pour en afficher la description complète dans une fenêtre contextuelle. Si vous avez un accès en modification aux [!UICONTROL team settings], vous pouvez également modifier la description directement dans le pop-up.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer]**.

   Pour plus d’informations sur la configuration d’une équipe agile, voir les articles suivants :

   * [Configurer [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurer [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Convertir une équipe existante en équipe agile

Vous pouvez convertir une équipe existante en équipe agile :

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe que vous souhaitez convertir en équipe agile.
1. Cliquez sur le bouton **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.

   Seuls les membres de l’équipe disposant d’une licence [!UICONTROL Standard], [!UICONTROL Plan] ou [!UICONTROL Work] peuvent voir cette option.
   ![](assets/edit-team-settings-350x205.png)

1. Dans la section **[!UICONTROL Agile]**, sélectionnez **[!UICONTROL Ceci est une équipe agile]**.

1. Dans la section **[!UICONTROL Méthodologie]**, choisissez si l’équipe utilisera une méthodologie agile **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]**.

1. Cliquez sur **Enregistrer les modifications**.

   L’équipe est enregistrée en tant qu’équipe agile. Vous pouvez configurer la nouvelle équipe en tant qu’équipe Scrum ou Kanban lorsque vous la modifiez.

   Pour plus d’informations, consultez les articles suivants :

   * [Configurer [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurer [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
