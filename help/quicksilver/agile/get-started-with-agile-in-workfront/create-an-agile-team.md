---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Créer une équipe Agile
description: Adobe Workfront permet aux équipes agiles d’effectuer leur travail de manière progressive et organisée.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 3%

---

# Créer une équipe Agile

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] permet aux équipes agiles de terminer le travail de manière progressive et organisée.

Tout utilisateur de l’entreprise peut voir l’équipe agile et afficher tous les composants agiles de l’équipe, y compris le journal en souffrance, les itérations, le panorama d’articles et les articles individuels. Toutefois, seuls les membres de l’équipe avec [!UICONTROL Modifier] l’accès au travail peut apporter des modifications au travail assigné à l’équipe.

[!DNL Workfront] prend en charge les méthodologies agile suivantes :

* **[!UICONTROL Scrum]**: les équipes ont un retard de travail à faire. Lorsque l’équipe est prête à travailler sur un bloc de travail spécifique, le travail est déplacé du journal en souffrance vers une itération. Pour plus d’informations sur la gestion d’une équipe Scrum, voir [Scrum dans une équipe agile](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Les équipes déplacent le travail dans la vue Kanban à travers des états prédéterminés. Les états par défaut sont les suivants : en retard, en cours de traitement et terminé. Pour plus d’informations sur la gestion d’une équipe Kanban, voir [Kanban dans une équipe agile](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>Nouveau : Standard</p>
   Actuel : 
   <ul><li><p>[!UICONTROL Formule] pour créer une équipe agile</p></li> 
   <li><p>[!UICONTROL Travail] ou version ultérieure pour convertir une équipe en équipe agile</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

+++

## Choix d’une méthodologie agile

Vous pouvez utiliser une méthodologie Scrum ou Kanban agile pour votre équipe agile. Chaque méthodologie présente divers avantages. Le fonctionnement de votre équipe agile détermine la méthodologie agile que vous choisissez d’utiliser.

Scrum et Kanban : [!DNL Workfront] vous permet de déplacer des articles dans un panorama pour indiquer un changement d’état et la progression de l’histoire.

Méthodes agiles Scrum et Kanban [!DNL Workfront] Les différences sont les suivantes :

### Avantages de Kanban dans [!DNL Workfront]

La variable [!DNL Kanban] la méthodologie agile [!DNL Workfront] vous permet de déplacer plus facilement les articles sur un panorama agile tout en limitant la quantité de travail en cours. Il n’existe aucune date de début et de fin lors de l’utilisation de la variable [!DNL Kanban] méthodologie agile.

Les fonctionnalités suivantes prennent en charge cette méthodologie :

* Afficher le journal en souffrance sur le [!DNL Kanban] tableau de bord agile.\
   Pour plus d’informations, voir [Ajoutez le journal en souffrance au [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configurez les éléments du journal en attente à ajouter automatiquement au journal [!UICONTROL Kanban] tableau de bord agile lorsque d’autres éléments sont déplacés vers un état qui correspond à Terminé.\
   Pour plus d’informations, voir la section [Configurer des articles à ajouter automatiquement à partir du journal](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) dans l’article [Configurer Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configurez une limite de travail en cours à afficher sur la [!UICONTROL Kanban] tableau de bord agile.\
   Pour plus d’informations, voir [Gérer la limite de travail en cours sur le panorama Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Avantages de Scrum dans [!DNL Workfront]

La méthodologie Scrum agile [!DNL Workfront] vous permet d’ajouter un ensemble d’articles à une itération agile et de créer un panorama pour cette itération. L’itération est basée sur les dates de début et de fin que vous définissez.

Les fonctionnalités suivantes prennent en charge cette méthodologie :

* Inclure les problèmes sur la variable [!UICONTROL Scrum] page d’article
* Inclure les problèmes sur le journal d’une équipe agile
* Les sous-tâches peuvent s’afficher sur la [!UICONTROL Scrum] page d’article
* Affichage d’un graphique de condensation pour voir la progression par rapport aux histoires lors de l’itération\
   Pour plus d’informations, voir [Présentation du graphique en décharge agile](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Créer une équipe Agile

{{step1-to-team}}

1. Cliquez sur le bouton **[!UICONTROL Changer d’équipe]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis cliquez sur **[!UICONTROL Créer une nouvelle équipe]**.

   ![Sélectionnez Créer une nouvelle équipe.](assets/create-new-team-350x198.png)

   La boîte Nouvelle équipe s’affiche.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nom de l’équipe]</strong> </td> 
      <td>Saisissez le nom de la nouvelle équipe agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Ceci est une équipe agile]</strong> </td> 
      <td>Sélectionnez cette option pour configurer cette nouvelle équipe afin qu’elle soit agile.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Est Actif]</strong> </td> 
      <td>Sélectionnez cette option pour activer cette équipe. Les équipes inactives ne sont pas visibles par d’autres utilisateurs pour les affecter au travail. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Commencez à saisir le nom d’un groupe à ajouter à l’équipe, puis sélectionnez-le lorsqu’il apparaît dans la liste déroulante.</p> <p><b>NOTE</b></p> <p> Lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans être membres de l’équipe. Les administrateurs de groupe peuvent accéder à la zone [!UICONTROL Équipes] à partir du [!UICONTROL Menu principal] et cliquer sur la flèche [!UICONTROL Switch Teams] . <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’elles gèrent.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Membres de l’équipe]</strong> </td> 
      <td>Commencez à saisir le nom d’un utilisateur qui doit faire partie de l’équipe, puis sélectionnez le nom lorsqu’il apparaît dans la liste déroulante.<br>Répétez cette procédure pour ajouter plusieurs utilisateurs à l’équipe.<br>Comme les utilisateurs peuvent appartenir à plusieurs équipes, ils peuvent appartenir à des équipes agiles et non agiles.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>Saisissez une description pour l’équipe.</p> <p>La description s’affiche en haut à droite de la zone [!UICONTROL Équipes] lorsque l’équipe est sélectionnée.</p>
      <p>Si la description est longue, vous pouvez cliquer dessus pour afficher la description complète dans une fenêtre contextuelle. Si vous avez accès à la modification des [!UICONTROL paramètres de l’équipe], vous pouvez également modifier la description directement dans la fenêtre contextuelle.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer]**.

   Pour plus d’informations sur la configuration d’une équipe Agile, consultez les articles suivants :

   * [Configurer [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurer [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Convertir une équipe existante en équipe agile

Vous pouvez convertir une équipe existante en équipe agile :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.
1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe que vous souhaitez convertir en équipe agile.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.\
   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Planifier] ou [!UICONTROL Travail] voir cette option.\
   ![](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , sélectionnez **[!UICONTROL Voici une équipe agile]**.

1. Dans le **[!UICONTROL Méthodologie]** , choisissez si l’équipe utilisera une **[!UICONTROL Scrum]** ou **[!UICONTROL Kanban]** méthodologie agile.

1. Cliquez sur **Enregistrez les modifications.**

   L&#39;équipe est enregistrée comme équipe agile. Vous pouvez configurer la nouvelle équipe en tant que Scrum ou équipe Kanban lorsque vous modifiez l’équipe.

   Pour plus d’informations, voir les articles suivants :

   * [Configurer [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurer [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
