---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Gestion du journal agile
description: Les tâches et les problèmes peuvent être attribués à une équipe agile et ajoutés à la liste d’attente de l’équipe sous forme d’histoires, selon la méthodologie agile utilisée par l’équipe.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 94%

---

# Gérer la liste d’attente agile

Les tâches suivantes peuvent être affectées à une équipe agile et ajoutées à la liste d’attente de l’équipe en tant qu’histoires, en fonction de la méthodologie agile utilisée par l’équipe :

* **[!UICONTROL Équipes agile Scrum] :** les tâches et les problèmes peuvent être affectés à l’équipe agile et ajoutés à la liste d’attente.
* **[!UICONTROL Équipes agile Kanban : les tâches peuvent être affectées à l’équipe agile et ajoutées à la liste d’attente. ]** Les utilisateurs et utilisatrices peuvent afficher la liste d’attente directement à partir du StoryBoard agile, comme décrit dans la section Ajouter la liste d’attente au tableau Kanban. [](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md) L’équipe utilise cette liste d’attente pour prioriser et gérer sa file d’attente de travail.

Les tâches ou les problèmes peuvent être affectés à l’équipe (et par la suite ajoutés à la liste d’attente de l’équipe) à partir de n’importe quel emplacement d’. [!DNL Adobe Workfront] Par exemple, une seule équipe peut se voir affecter du travail provenant de plusieurs projets.

>[!NOTE]
>
>Si vous ajoutez plusieurs équipes à un élément de liste d’attente, la tâche ou le problème s’affiche uniquement sur la liste d’attente de l’équipe principale. L’équipe principale est la première équipe affectée.

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
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p> 
   ou
   <p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès en [!UICONTROL Manage] au projet contenant l’histoire </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer et gérer des histoires sur la liste d’attente

* [Réorganiser les histoires](#reorder-stories)
* [[!UICONTROL Ventiler] les histoires](#break-down-stories)
* [Modifier les histoires](#edit-stories)

### Réorganiser les histoires {#reorder-stories}

Vous pouvez réorganiser les histoires dans la liste d’attente à l’aide de la méthode du glisser-déposer.

1. Accédez à la liste d’attente agile dans lequel vous souhaitez réorganiser les histoires.
1. Dans le menu déroulant **[!UICONTROL Affichage]**, sélectionnez la vue **[!UICONTROL Liste d’attente]** ou une vue personnalisée qui contient la colonne **[!UICONTROL Ordre]**.

   >[!NOTE]
   >
   >Si une équipe agile est affectée à une tâche ou un problème et que le projet n’est pas dans un statut correspondant à Actuel, ils ne s’affichent pas dans la liste d’attente. Toutefois, ils affectent toujours le nombre d’éléments présents dans la liste d’attente dans la colonne Ordre.

1. Sélectionnez une ou plusieurs histoires, puis faites-les glisser dans l’ordre dans lequel vous souhaitez qu’elles apparaissent dans la liste d’attente.
   ![Glisser-déposer des éléments de liste d’attente](assets/agile-backlog-drag-and-drop.png)

### Ventiler les histoires {#break-down-stories}

Comme les histoires dans une  liste d’attente varient en taille, vous pouvez les ventiler en tailles exploitables pour une itération. La ventilation d’une histoire crée des sous-tâches sur la tâche que l’histoire représente, et remplace la tâche d’origine dans la liste d’attente. Une tâche parent ou ses sous-tâches peuvent être affectées à une équipe agile, mais les deux tâches ne peuvent pas être affectées simultanément à une équipe.

>[!NOTE]
>
>Tenez compte des limites suivantes lors de la ventilation d’histoires :
>
>* Seules les histoires qui représentent des tâches peuvent être ventilées. Vous ne pouvez pas ventiler des histoires qui représentent des problèmes.
>* Les histoires ne peuvent être ventilées que si elles sont associées à un projet.


Pour ventiler une histoire, procédez comme suit :

1. Accédez au journal contenant l’histoire que vous souhaitez ventiler.
1. Sélectionnez l’article que vous souhaitez ventiler, puis cliquez sur **[!UICONTROL Article de ventilation]**.
La boîte de dialogue [!UICONTROL Répartition de l’histoire] s’affiche.
   ![Boîte de dialogue pour la ventilation d’histoires](assets/backlog-breakdown-dialog.png)

1. Spécifiez un nom et une estimation pour l’histoire, et indiquez si l’histoire est prête.
1. Cliquez sur **[!UICONTROL Ajouter une histoire]** pour créer une autre histoire à partir de l’histoire originale.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

### Modifier les histoires {#edit-stories}

Vous pouvez modifier les histoires directement à partir des onglets [!UICONTROL Histoires] ou [!UICONTROL Problèmes] dans la liste d’attente comme vous le feriez lorsque vous modifiez en masse les tâches ou les problèmes d’un projet, tel que décrit dans [Modifier les tâches en masse](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) dans les sections [Modifier les tâches](../../manage-work/tasks/manage-tasks/edit-tasks.md), et [Modifier les problèmes](../../manage-work/issues/manage-issues/edit-issues.md).

## Créer des histoires dans la liste d’attente {#create-new-stories-on-the-backlog}

Dans la liste d’attente, vous pouvez créer des histoires en créant l’histoire directement à partir de celle-ci, ou en assignant une tâche ou un problème existant à une équipe Agile.

* [Créer une histoire dans la liste d’attente](#create-a-story-from-the-backlog)
* [Affecter une tâche ou un problème à une équipe agile](#assign-a-task-or-issue-to-an-agile-team)

### Créer une histoire dans la liste d’attente {#create-a-story-from-the-backlog}

Lorsque vous créez une histoire dans la liste d’attente, elle est créée en tant que tâche ou problème dans un projet. Vous ne pouvez pas créer une histoire dans la liste d’attente en tant que problème.

Pour créer une histoire dans la liste d’attente :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche et sélectionnez-la lorsqu’elle s’affiche.

1. Sélectionnez **[!UICONTROL Liste d’attente]** dans le panneau de gauche.
1. Effectuez l’une des opérations suivantes, selon que vous souhaitez créer une tâche ou un problème :

   * **Pour créer une tâche :** cliquez sur **[!UICONTROL Histoires]**.

   * **Pour créer un problème :** cliquez sur **[!UICONTROL Problèmes]**.

1. Cliquez sur **[!UICONTROL Nouvelle histoire]** ou **[!UICONTROL Nouveau problème]**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td> Saisissez un nom pour l’histoire.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>(Facultatif) Saisissez une description pour l’histoire.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Indiquez si l’histoire est prête à être ajoutée à une itération. Ce paramètre est fourni uniquement à titre d’information. Les histoires peuvent être ajoutées à une itération, quel que soit le statut de ce paramètre.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Spécifiez une estimation point ou horaire pour l’histoire. Les estimations affectent le graphique d’avancement. Le graphique d’avancement d’une itération n’est exact que si chaque histoire contient une estimation exacte. (Si vous fournissez une estimation par point, vous devez avoir déjà indiqué dans les paramètres de l’équipe combien d’heures chaque point représente.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Commencez à saisir le nom du projet dans lequel cette histoire sera créée, puis cliquez sur le nom qui apparaît dans la liste déroulante.<br>Le statut du projet doit être défini sur [!UICONTROL Current]. Si le statut du projet est autre que [!UICONTROL Current], il ne s’affiche pas dans le menu déroulant.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>(Facultatif) Commencez à saisir le nom de la tâche parent à laquelle cettte histoire est subordonnée, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Facultatif) Sélectionnez les formulaires personnalisés à ajouter à cette histoire.</td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Enregistrer l’histoire]**.

### Affecter une tâche ou un problème à une équipe agile {#assign-a-task-or-issue-to-an-agile-team}

Vous pouvez affecter une tâche ou un problème à une équipe agile. Après son affectation, la tâche ou le problème apparaît comme une nouvelle histoire dans la liste d’attente de l’équipe.

Pour affecter une tâche ou un problème à une équipe agile :

1. Accédez au projet contenant la tâche que vous souhaitez affecter.
1. Sélectionnez la tâche ou le problème dans la liste.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. Cliquez sur **[!UICONTROL Affectations]**.
1. (Facultatif) Supprimez les personnes cessionnaires existantes.
1. Cliquez sur **[!UICONTROL Ajouter une personne cessionnaire]**.
1. Commencez à saisir le nom de l’équipe agile que vous souhaitez affecter à la tâche ou au problème, puis cliquez sur le nom de l’équipe lorsqu’il apparaît dans la liste déroulante.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**
. La tâche ou le problème est désormais disponible dans la liste d’attente de l’équipe.

## Déplacer des articles dans ou hors du journal

* [Déplacer des histoires de la liste d’attente vers un panorama d’itération ou autre](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Déplacer des histoires existantes vers la liste d’attente](#move-existing-stories-to-the-backlog)
* [Exporter les histoires de la liste d’attente](#export-stories-from-the-backlog)

### Déplacer des histoires de la liste d’attente vers un panorama d’itération ou autre

1. Rendez-vous dans la liste d’attente de l’équipe agile.
1. Sélectionnez les articles que vous souhaitez déplacer vers un panorama d’itération ou Kanban, puis cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Déplacer vers]**.
Si vous déplacez l’histoire vers un panorama [!UICONTROL Kanban], le panorama [!UICONTROL Déplacer l’article vers le panorama Kanban] s’affiche.
Si vous déplacez l’histoire vers une itération, la boîte de dialogue [!UICONTROL Déplacer l’histoire vers une itération] est affichée.
   ![Boîte de dialogue Déplacer l’histoire](assets/agile-backlog-addtoiteration.png)

1. Utilisez l’une des méthodes suivantes :

   * **Pour les équipes Scrum :** dans le champ **[!UICONTROL Sélectionner l’itération]**, choisissez l’itération dans laquelle vous souhaitez déplacer les histoires.

   * **Pour les équipes Kanban : dans le champ Sélectionner le tableau Kanban, choisissez le tableau Kanban de votre équipe.****** (Les équipes Kanban ne peuvent avoir qu’un seul tableau [!UICONTROL Kanban].)

1. Cliquez sur **[!UICONTROL Déplacer l’histoire]**.

### Déplacer les histoires existantes vers la liste d’attente {#move-existing-stories-to-the-backlog}

Si vous décidez que votre équipe n’est pas encore prête à travailler sur une histoire, vous pouvez déplacer l’histoire dans la liste d’attente.

Pour plus d’informations, voir [Déplacer une histoire agile](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exporter les histoires de la liste d’attente {#export-stories-from-the-backlog}

Vous pouvez exporter une ou plusieurs histoires (y compris des tâches et des problèmes) directement à partir de la liste d’attente.

Les histoires de la liste d’attente s’exportent de la même manière que d’autres données dans [!DNL Workfront], comme décrit dans [Exporter des données](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
