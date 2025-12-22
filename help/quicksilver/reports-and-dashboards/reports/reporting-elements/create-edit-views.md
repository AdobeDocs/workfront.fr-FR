---
product-area: reporting
navigation-topic: reporting-elements
title: Créer ou modifier des vues dans Adobe Workfront
description: Vous pouvez personnaliser le type d’informations affichées à l’écran à l’aide des vues. Vous pouvez utiliser plusieurs types de vues dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 61%

---

# Créer ou modifier des vues dans Adobe Workfront

<!-- Audited: 11/2024 -->

Vous pouvez personnaliser le type d’informations affichées à l’écran à l’aide des vues. Vous pouvez utiliser plusieurs types de vues dans Adobe Workfront.

Cet article décrit comment créer et modifier des vues standard pour les listes et les rapports.

Pour plus d’informations, consultez l’article [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</strong></td> 
   <td> 
    <p>Contributeur ou version ultérieure</p>
    <p>Requête ou supérieure</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux rapports, aux tableaux de bord et aux calendriers pour créer une vue dans un rapport</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour créer ou modifier une vue dans un rapport</p> <p>Gérer les autorisations d’une vue pour la modifier</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Créer ou personnaliser une vue

Le processus de création ou de personnalisation d’une vue diffère selon que vous créez ou personnalisez une vue standard ou une vue de panorama.

### Créer ou personnaliser une vue standard {#create-or-customize-a-standard-view}

Vous pouvez créer une nouvelle vue standard ou personnaliser une vue standard existante que vous avez créée précédemment.

1. Cliquez sur le menu déroulant **Vue** dans toute liste où vous souhaitez créer ou personnaliser une vue.

1. Cliquez sur le bouton **+ Nouvel affichage** pour créer un affichage.
Ou
Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) qui s’affiche lorsque vous pointez à droite d’une vue existante à modifier.
La boîte de dialogue **Personnaliser la vue** s’affiche.

1. Dans la section **Aperçu de la colonne**, effectuez l’une des opérations suivantes :

   * Modifiez la valeur de n’importe quelle colonne en cliquant sur le titre de la colonne et en sélectionnant un nouveau champ.
   * Ajoutez une colonne en cliquant sur **Ajouter une colonne**, commencez à saisir le nom de la colonne que vous souhaitez ajouter, puis cliquez dessus lorsqu’elle apparaît dans la liste déroulante.
   * Ajustez l’ordre d’apparition des colonnes en faisant glisser le titre de la colonne vers un nouvel emplacement.

   * Dans la zone **Paramètres de colonne**, cliquez sur **Résumer cette colonne par** et choisissez comment vous souhaitez que les données s’affichent dans la colonne. Cette option est disponible pour les types de colonnes suivants :
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Champs de date</strong></td> 
           <td><ul>
           <li>Maximum</li>
         <li>Minimum</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Champs de devise</strong></td> 
           <td><ul>
           <li>Nombre</li>
         <li>Sum</li>
           <li>Moyenne</li>
         <li>Maximum</li>
           <li>Minimum</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Chaîne et champs booléens</strong></td> 
           <td><ul><li>Nombre</li></ul>
           <p>Remarque : Workfront ne recommande généralement pas de synthétiser un champ booléen par nombre, car la valeur sera toujours true/false.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >Les exceptions suivantes s&#39;appliquent aux objets parents (par exemple, les tâches parents) lorsque vous récapitulez les valeurs des champs suivants dans des regroupements :
     >   
     > * Tous les champs de nombre et de devise, à l&#39;exception des heures réelles (par exemple, coût prévu/réel de la main-d&#39;œuvre, coût prévu/réel des dépenses, coût prévu/réel, heures prévues) résument les valeurs pour les tâches enfants uniquement et les tâches autonomes. Elles ne résument pas les valeurs des tâches parents ou des parents de parents.
     > * Le tableau Heures réelles récapitule les valeurs des tâches parents principales et autonomes ; il ne récapitule pas les valeurs des parents des tâches parents ou des tâches enfants.
     > * Les champs de données personnalisés pour les valeurs numériques et monétaires résument toutes les tâches : parents, enfants, parents de parents et tâches autonomes.
     >
     >Pour plus d’informations sur l’utilisation des regroupements dans un rapport, voir l’article [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Facultatif) Cliquez sur **Options avancées** pour spécifier les informations suivantes de la colonne :

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Personnaliser le libellé de colonne</strong></td> 
           <td><p>Spécifiez un libellé personnalisé pour la colonne. Ce libellé remplace le libellé par défaut. Nous vous recommandons d’utiliser uniquement des caractères UTF-8 pour éviter des problèmes de compatibilité.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Format du champ</strong></td> 
           <td>Sélectionnez le format dans lequel vous souhaitez que les valeurs soient affichées pour les champs de la colonne.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Afficher cette colonne lorsque le graphique est visible sur un tableau de bord.</strong></td> 
           <td><p>Sélectionnez cette option pour afficher cette colonne dans un tableau de bord, lorsque le rapport est affiché côte à côte avec un autre rapport. Lorsque cette option n’est pas sélectionnée, cette colonne n’apparaît pas lorsque le rapport est affiché sur un tableau de bord où les rapports sont affichés côte à côte.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Règles de la colonne</strong></td> 
           <td><p>Cliquez sur <strong>+ Ajouter une règle pour cette colonne</strong> afin de définir une règle pour la colonne. Après avoir ajouté une règle, vous pouvez définir des styles de champ et de texte définissant le mode d’affichage des champs correspondant à cette règle. Cliquez sur <strong>Ajouter une règle</strong> lorsque vous avez terminé de définir la règle.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Pour plus d’informations sur la mise en forme conditionnelle des vues dans les rapports, voir l’article [Utiliser la mise en forme conditionnelle en mode texte](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Le cas échéant) Si vous avez cliqué sur **Options avancées**, cliquez sur **Terminé**.

1. Cliquez sur **Enregistrer la vue** pour créer une vue ou remplacer la vue actuelle par vos modifications.\
   Ou\
   Cliquez sur **Enregistrer en tant que nouvelle vue** pour enregistrer vos modifications dans une nouvelle vue.

   >[!TIP]
   >
   >L’option **Enregistrer en tant que nouvelle vue** est la seule option disponible lorsque vous personnalisez une vue Workfront intégrée.

   Votre accès détermine la manière selon laquelle la vue est enregistrée. Si vous avez créé la vue à l’origine, vous pouvez enregistrer les modifications ; sinon, vous recevez une invitation à enregistrer une version. Gardez à l’esprit que que les modifications que vous apportez à l’affichage ont un impact sur les utilisateurs et utilisatrices avec lesquels l’affichage a été partagé.

### Création ou personnalisation d’une vue de tableau {#create-or-customize-an-agile-view}

Vous pouvez gérer les projets selon une méthodologie Agile à l’aide d’une vue Tableau.

Les affichages du tableau ne sont disponibles que pour les listes de tâches et d’événements d’un projet.

Ils sont préconfigurés, mais vous pouvez modifier certains paramètres pour eux.

Pour plus d’informations sur Agile ou les vues de tableau, consultez l’article [Gérer un projet Agile dans la vue Tableau](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the Agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the Agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the Agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
