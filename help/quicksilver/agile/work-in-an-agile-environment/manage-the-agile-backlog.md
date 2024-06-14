---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Gérer la liste d’attente agile
description: Les tâches et les problèmes peuvent être attribués à une équipe agile et ajoutés au journal de l’équipe sous forme d’articles, selon la méthodologie agile utilisée par l’équipe.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 4%

---

# Gérer la liste d’attente agile

Les tâches suivantes peuvent être affectées à une équipe agile et ajoutées au journal de l’équipe en tant qu’articles, en fonction de la méthodologie agile utilisée par l’équipe :

* **[!UICONTROL Scrum agile équipes]:** Les tâches et les problèmes peuvent être attribués à l’équipe agile et ajoutés au journal.
* **[!UICONTROL équipes agiles de Kanban]:** Les tâches peuvent être affectées à l’équipe agile et ajoutées au journal en souffrance. Les utilisateurs peuvent afficher le journal en souffrance directement à partir du tableau de bord agile, comme décrit dans la section [[!UICONTROL Ajouter le journal des travaux] sur le panorama de Kanban](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). L’équipe utilise ce journal pour prioriser et gérer sa file d’attente de travail.

Les tâches ou les problèmes peuvent être affectés à l’équipe (et par la suite ajoutés au journal de l’équipe) depuis n’importe quel emplacement dans [!DNL Adobe Workfront]. Par exemple, une seule équipe peut se voir affecter des affectations de travail à partir de plusieurs projets.

>[!NOTE]
>
>Si vous ajoutez plusieurs équipes à un élément de journal, la tâche ou le problème s’affiche uniquement sur le journal de l’équipe principale. L’équipe principale est la première équipe affectée.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license</strong></td> 
   <td> <p>Nouveau : [!UICONTROL Standard]</p><p>Ou</p><p>Actuel : [!UICONTROL Travail] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>Nouveau : [!UICONTROL Standard]</p><p>Ou</p><p>Actuel : [!UICONTROL Worker] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] Accès au projet sur lequel se trouve l’article</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer et gérer des articles en souffrance

* [Réorganiser les articles](#reorder-stories)
* [[!UICONTROL Ventiler] contes](#break-down-stories)
* [Modifier des articles](#edit-stories)

### Réorganiser les articles {#reorder-stories}

Vous pouvez réorganiser les articles dans la liste de journal en souffrance à l’aide de la méthode glisser-déposer.

1. Accédez au journal agile dans lequel vous souhaitez réorganiser les articles.
1. Dans le **[!UICONTROL Affichage]** , sélectionnez la variable **[!UICONTROL Backlog]** affichage ou affichage personnalisé qui contient la variable **[!UICONTROL Commande]** colonne .

   >[!NOTE]
   >
   >Si une équipe agile est affectée à une tâche ou un problème et que le projet n’est pas dans un état correspondant à Actuel, il ne s’affiche pas dans le journal des travaux en souffrance. Toutefois, elles n’affectent pas le nombre de dossiers dans la colonne Ordre.

1. Sélectionnez un ou plusieurs articles, puis faites-les glisser dans l’ordre dans lequel vous souhaitez qu’ils apparaissent dans le journal.\
   ![Glisser-déposer des éléments en souffrance](assets/agile-backlog-drag-and-drop.png)

### Ventiler les histoires {#break-down-stories}

Comme les articles dans un journal en souffrance varient en taille, les utilisateurs peuvent les ventiler en tailles exploitables pour une itération. La ventilation d’un article crée des sous-tâches sur la tâche que l’article représente, et remplace la tâche d’origine dans le journal. Une tâche parent ou ses sous-tâches peuvent être affectées à une équipe agile, mais les deux tâches ne peuvent pas être affectées simultanément à une équipe.

>[!NOTE]
>
>Tenez compte des limites suivantes lors de la ventilation d’articles :
>
>* Seules les histoires qui représentent des tâches peuvent être ventilées. Vous ne pouvez pas ventiler des histoires qui représentent des problèmes.
>* Les articles ne peuvent être ventilés que s’ils sont associés à un projet.


Pour raconter une histoire :

1. Accédez au journal contenant l’article que vous souhaitez ventiler.
1. Sélectionnez l’article à ventiler, puis cliquez sur **[!UICONTROL Histoire de ventilation]**.\
   La variable [!UICONTROL Histoire de ventilation] s’affiche.\
   ![Boîte de dialogue Répartition de l’article](assets/backlog-breakdown-dialog.png)

1. Indiquez un nom et une estimation pour l’article, puis indiquez si l’article est prêt.
1. Cliquez sur **[!UICONTROL Ajout d’un article]** pour créer une autre histoire à partir de l&#39;histoire originale.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

### Modifier des articles {#edit-stories}

Vous pouvez modifier des articles directement à partir du [!UICONTROL Histoires] ou [!UICONTROL Problèmes] onglets sur le journal en souffrance, comme vous le feriez pour modifier en bloc les tâches ou problèmes d’un projet, comme décrit dans la section [Modifier les tâches en bloc](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) in [Modifier les tâches](../../manage-work/tasks/manage-tasks/edit-tasks.md), et [Modification des problèmes](../../manage-work/issues/manage-issues/edit-issues.md).

## Créer de nouveaux articles sur le journal en souffrance {#create-new-stories-on-the-backlog}

Vous pouvez créer de nouveaux articles sur le journal en souffrance en créant l’article directement à partir du journal, ou en affectant une tâche ou un problème existant à une équipe agile.

* [Création d’un article à partir du journal](#create-a-story-from-the-backlog)
* [Affecter une tâche ou un problème à une équipe agile](#assign-a-task-or-issue-to-an-agile-team)

### Création d’un article à partir du journal {#create-a-story-from-the-backlog}

Lorsque vous créez un article dans le journal, il est créé en tant que tâche ou problème dans un projet. Vous ne pouvez pas créer un article à partir du journal en souffrance comme problème.

Pour créer un article à partir du journal :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche et sélectionnez-la lorsqu’elle s’affiche.

1. Sélectionner **[!UICONTROL Backlog]** dans le panneau de gauche.
1. Effectuez l’une des opérations suivantes, selon que vous souhaitez créer une tâche ou un problème :

   * **Pour créer une tâche :** Cliquez sur **[!UICONTROL Histoires]**.

   * **Pour créer un problème :** Cliquez sur **[!UICONTROL Problèmes]**.

1. Cliquez sur **[!UICONTROL New Story]** ou **[!UICONTROL Nouveau problème]**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td> Saisissez le nom de l’article.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>(Facultatif) Saisissez une description pour l’article.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Indiquez si l’article est prêt à être ajouté à une itération. Ce paramètre est fourni uniquement à titre d’information. Les articles peuvent être ajoutés à une itération, quel que soit l’état de ce paramètre.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td>Spécifiez une estimation point ou horaire pour l’article. Les estimations affectent le graphique de ventilation. Le graphique de condensation d’une itération n’est exact que si chaque article contient une estimation exacte. (Si vous fournissez une estimation du point, vous devez avoir déjà indiqué dans les paramètres de l’équipe combien d’heures chaque point représente.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Commencez à saisir le nom du projet dans lequel cet article sera créé, puis cliquez sur le nom qui apparaît dans la liste déroulante.<br>L’état du projet doit être défini sur [!UICONTROL Actuel]. Si l’état du projet est autre que [!UICONTROL Actuel], il ne s’affiche pas dans le menu déroulant.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tâche Parente]</strong></td>
      <td>(Facultatif) Commencez à saisir le nom de la tâche parent à laquelle cet article est subordonné, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Forms personnalisé]</strong></td>
      <td> (Facultatif) Sélectionnez les formulaires personnalisés à ajouter à cet article.</td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Enregistrer l’article]**.

### Affecter une tâche ou un problème à une équipe agile {#assign-a-task-or-issue-to-an-agile-team}

Vous pouvez affecter une tâche ou un problème à une équipe agile. Une fois qu’elle a été affectée, la tâche ou le problème apparaît comme un nouvel article dans le journal de l’équipe.

Pour affecter une tâche ou un problème à une équipe agile :

1. Accédez au projet contenant la tâche que vous souhaitez affecter.
1. Sélectionnez la tâche ou le problème dans la liste.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. Cliquez sur **[!UICONTROL Affectations]**.
1. (Facultatif) Supprimez les personnes désignées existantes.
1. Cliquez sur **[!UICONTROL Ajouter un cessionnaire]**.
1. Commencez à saisir le nom de l’équipe agile que vous souhaitez affecter à la tâche ou au problème, puis cliquez sur le nom de l’équipe lorsqu’il apparaît dans la liste déroulante.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   La tâche ou le problème est désormais disponible dans le journal des travaux de l’équipe.

## Déplacer des articles dans ou hors du journal

{#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Déplacer des articles du journal vers un panorama ou une itération](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Déplacer les articles existants dans le journal](#move-existing-stories-to-the-backlog)
* [Exporter des articles depuis le journal en souffrance](#export-stories-from-the-backlog)

### Déplacer des articles du journal vers un panorama ou une itération

1. Accédez au journal de l’équipe agile.
1. Sélectionnez les articles à déplacer sur un panorama d’itération ou Kanban, puis cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Déplacer vers]**.\
   Si vous déplacez l’histoire vers une [!UICONTROL Kanban] panorama, [!UICONTROL Déplacer l&#39;histoire vers le Kanban] Panorama s’affiche.\
   Si vous déplacez l’histoire vers une itération, la variable [!UICONTROL Déplacer l’article vers une itération] s’affiche.\
   ![Boîte de dialogue Déplacer l’article](assets/agile-backlog-addtoiteration.png)

1. Effectuez l’une des opérations suivantes :

   * **Pour les équipes Scrum :** Dans le **[!UICONTROL Sélectionner une itération]** sélectionnez l’itération dans laquelle vous souhaitez déplacer les articles.

   * **Pour les équipes de Kanban :** Dans le **[!UICONTROL Sélectionner le panorama Kanban]** champ, sélectionnez votre équipe [!UICONTROL Kanban] panorama. (Les équipes de Kanban ne peuvent avoir qu’une seule [!UICONTROL Kanban] panorama.)

1. Cliquez sur **[!UICONTROL Déplacer l’article]**.

### Déplacer les articles existants dans le journal {#move-existing-stories-to-the-backlog}

Si vous décidez que votre équipe n&#39;est pas encore prête à travailler sur une histoire, vous pouvez la réorganiser en retard.

Pour plus d’informations, voir [Déplacer une histoire agile](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exporter des articles depuis le journal en souffrance {#export-stories-from-the-backlog}

Vous pouvez exporter un ou plusieurs articles (y compris des tâches et des problèmes) directement à partir du journal.

Vous exportez des articles du journal de la même manière que vous exportez d’autres données dans [!DNL Workfront], comme décrit dans [Exporter des données](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
