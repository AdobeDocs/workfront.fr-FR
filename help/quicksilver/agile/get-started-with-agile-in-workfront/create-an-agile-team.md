---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Créer une équipe Agile
description: Adobe Workfront permet aux équipes Agile d’effectuer le travail de manière incrémentielle et organisée.
author: Jenny
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 56%

---

# Créer une équipe Agile

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] permet aux équipes Agile d’effectuer le travail de manière incrémentielle et organisée.

Tout utilisateur de l’organisation peut voir l’équipe Agile et afficher tous les composants Agile de l’équipe, y compris la liste d’attente, les itérations, le storyboard et les histoires individuelles. Toutefois, seuls les membres de l’équipe disposant d’un accès [!UICONTROL Modifier] au travail peuvent apporter des modifications au travail affecté à l’équipe.

[!DNL Workfront] prend en charge les méthodologies Agile suivantes :

* **[!UICONTROL Scrum]** : les équipes ont une liste d’attente de travail à faire. Lorsque l’équipe est prête à travailler sur un bloc de travail spécifique, le travail est déplacé de la liste d’attente vers une itération. Pour plus d&#39;informations sur la gestion d&#39;une équipe Scrum, voir [Scrum dans une équipe Agile](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban] :** les équipes déplacent le travail dans la vue Kanban à travers des statuts prédéterminés. Les statuts par défaut sont les suivants : liste d’attente, en cours et terminé. Pour plus d’informations sur la gestion d’une équipe Kanban, voir [Kanban dans une équipe Agile](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Prévoyez de créer une nouvelle équipe Agile</p>
  <p>Travail ou version ultérieure pour convertir une équipe en équipe Agile</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Choix d’une méthodologie Agile

Vous pouvez utiliser une méthodologie Agile Scrum ou Kanban pour votre équipe Agile. Chaque méthodologie présente divers avantages. La façon dont votre équipe Agile travaille détermine la méthodologie Agile que vous choisissez d&#39;utiliser.

Les méthodologies Scrum et Kanban Agile dans [!DNL Workfront] vous permettent de déplacer des histoires à travers un storyboard pour indiquer un changement de statut et la progression de l’histoire.

Les méthodologies Scrum et Kanban Agile dans [!DNL Workfront] diffèrent des manières suivantes :

### Avantages de l’utilisation de Kanban dans [!DNL Workfront]

La méthodologie [!DNL Kanban] Agile d’[!DNL Workfront] vous permet de déplacer plus facilement des articles dans un storyboard agile tout en limitant la quantité de travail en cours. Il n’existe pas de dates de début et de fin lors de l’utilisation de la méthodologie Agile [!DNL Kanban].

Les fonctionnalités suivantes prennent en charge cette méthodologie :

* Affichez la liste d’attente sur le storyboard [!DNL Kanban] Agile.
Pour plus d’informations, voir [Ajouter la liste d’attente au storyboard [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configurez les éléments de la liste d’attente pour qu’ils soient automatiquement ajoutés au storyboard agile [!UICONTROL Kanban] lorsque d’autres éléments sont déplacés vers un statut équivalent à Terminé.
Pour plus d’informations, voir la section [Configurer des histoires à ajouter automatiquement à partir de la liste d’attente](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) dans l’article [Configurer Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configurez une limite de travail en cours (WIP) à afficher sur le storyboard agile [!UICONTROL Kanban].
Pour plus d’informations, voir [Gérer la limite de travail en cours (WIP) sur le storyboard Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Avantages de l’utilisation de Scrum dans [!DNL Workfront]

La méthodologie Scrum Agile dans [!DNL Workfront] vous permet d’ajouter un ensemble d’histoires à une itération Agile et de créer un storyboard pour cette itération. L’itération est basée sur les dates de début et de fin que vous définissez.

Les fonctionnalités suivantes prennent en charge cette méthodologie :

* Inclure les problèmes sur le storyboard [!UICONTROL Scrum]
* Inclure les événements dans la liste d&#39;attente d&#39;une équipe Agile
* Les sous-tâches peuvent être affichées sur le storyboard [!UICONTROL Scrum]
* Afficher un graphique d’avancement pour voir la progression par rapport aux histoires pendant l’itération
Pour plus d&#39;informations, voir [Présentation des graphiques d&#39;avancement Agile](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Créer une équipe Agile

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]**![Icône Changer d’équipe](assets/switch-team-icon.png), puis cliquez sur **[!UICONTROL Créer une nouvelle équipe]**.

   ![Sélectionnez Créer une équipe](assets/create-new-team.png)

   La zone Nouvelle équipe s’affiche.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Saisissez un nom pour la nouvelle équipe Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL This is an Agile Team]</strong> </td> 
      <td>Sélectionnez cette option pour configurer cette nouvelle équipe en tant qu’équipe Agile.</td> 
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
      <td>Commencez à saisir le nom d’un utilisateur ou d’une utilisatrice à ajouter à l’équipe, puis sélectionnez le nom lorsqu’il apparaît dans la liste déroulante.<br>Répétez cette procédure pour ajouter plusieurs utilisateurs et utilisatrices à l’équipe.<br>Comme les utilisateurs peuvent faire partie de plusieurs équipes, ils peuvent faire partie à la fois d’équipes Agile et non Agile.</td> 
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

Vous pouvez convertir une équipe existante en équipe Agile :

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l&#39;équipe que vous souhaitez convertir en équipe Agile.
1. Cliquez sur le bouton **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.

   Seuls les membres de l&#39;équipe disposant d&#39;une licence [!UICONTROL Standard], [!UICONTROL Plan] ou [!UICONTROL Work] voient cette option.
   ![Sélectionnez Modifier](assets/edit-team-settings.png)

1. Dans la section **[!UICONTROL Agile]**, sélectionnez **[!UICONTROL Ceci est une équipe agile]**.

1. Dans la section **[!UICONTROL Méthodologie]**, indiquez si l’équipe utilisera une méthodologie Agile **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]**.

1. Cliquez sur **Enregistrer les modifications**.

   L’équipe est enregistrée en tant qu’équipe agile. Vous pouvez configurer la nouvelle équipe en tant qu’équipe Scrum ou Kanban lorsque vous la modifiez.

   Pour plus d’informations, consultez les articles suivants :

   * [Configurer [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurer [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
