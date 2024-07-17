---
product-area: reporting
navigation-topic: using-built-in-reports
title: Icônes de statut intégrées dans les vues
description: Vous pouvez ajouter le champ Icônes d’état intégré en tant que colonne dans vos vues afin d’améliorer la visibilité sur les points clés de vos objets.
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 12%

---

# Icônes de statut intégrées dans les vues

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

Vous pouvez ajouter le champ Icônes d’état intégré en tant que colonne dans vos vues afin d’améliorer la visibilité sur les points clés de vos objets. À l’aide des icônes d’état, vous pouvez voir en un coup d’oeil les conditions suivantes :

* Un objet est associé à des documents
* Un objet est associé à un processus de validation
* Un objet est associé à des remarques supplémentaires.
* Une dépense est facturable ou remboursable
* Une tâche est sur un chemin critique
* Un utilisateur appartient à une entreprise, à une équipe ou se trouve dans un fuseau horaire différent.

Tenez compte des points suivants :

* La plupart des indicateurs du champ Icônes d’état sont des liens rapides vers l’objet ou la zone de l’objet qu’ils représentent.

* Si l’un des éléments représentés par les icônes est absent de l’objet, l’icône représentant l’élément manquant apparaît grisée dans la colonne Icônes d’état au lieu d’une image colorée.

  ![task_status_icons.png](assets/task-status-icons.png)

  Pour plus d’informations, reportez-vous à la section [Aperçu des icônes d’état et des indicateurs](#overview-of-status-icons-and-flags) de cet article.

* Dans certaines vues, le champ **Icônes d’état** est nommé **Indicateurs** ou **Icônes d’affichage**.\
  Vous ne pouvez pas personnaliser l’aspect des icônes incluses dans le champ Icônes d’état .

* Vous ne pouvez pas modifier le nombre d’icônes dans le champ Icônes d’état .

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour l’ajout de colonnes à un rapport</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour une vue existante</p> <p>Gérer les autorisations d’un rapport pour y ajouter des colonnes</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Ajout du champ Icônes d’état à une vue

Certains rapports et vues intégrés disposent déjà du champ Icônes d’état inclus.

Vous ne pouvez pas ajouter le champ Icônes d’état à toutes les vues.

Pour ajouter le champ Icônes d’état à une vue personnalisée entièrement créée :

1. Accédez à une liste de l’un des objets suivants :

   * Tâches
   * Problèmes
   * Projets
   * Tâches de modèles
   * Modèles
   * Frais
   * Documents
   * Utilisateurs\
     Seuls ces objets ont le champ **Icônes d’état** disponible.\
     Pour plus d’informations sur les listes d’objets, voir [Prise en main des listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Dans la zone **Afficher dans cette colonne**, commencez à saisir les noms de champ suivants, puis sélectionnez-le lorsqu’il apparaît dans la liste :

   * *Icônes de statut*
   * *Indicateurs*
   * *Icônes d’affichage * (uniquement en mode Document).

   Les icônes intégrées sont répertoriées sous l’un de ces noms.\
   Une vue Modèle contient les champs **Icônes d’état** et **Indicateurs**. Dans ce cas, les deux colonnes contiennent des icônes identiques.\
   Les vues de document contiennent un champ **Icônes d’affichage**.

1. Cliquez sur **Enregistrer la vue**.
1. (Facultatif) Spécifiez un nouveau nom pour votre vue, puis cliquez sur **Enregistrer la vue**.\
   Cela ajoute la colonne **Icônes d’état** à votre vue.
1. (Facultatif) Placez le pointeur de la souris sur une icône pour comprendre ce qu’elle représente.
1. (Facultatif) Cliquez sur une icône pour accéder à la zone de l’objet qu’il représente.\
   Toutes les icônes ne sont pas des liens vers des objets.\
   Pour obtenir la liste complète des attributs de chaque icône, reportez-vous à la section [Aperçu des icônes et indicateurs d’état](#overview-of-status-icons-and-flags) .

## Icônes et indicateurs d’état - Aperçu {#overview-of-status-icons-and-flags}

Le tableau suivant répertorie toutes les icônes d’état disponibles dans Workfront, le type d’objet qui peut être associé à ces icônes, ainsi que ce qui se passe lorsque vous cliquez dessus.

Vous devez disposer des autorisations nécessaires pour au moins Afficher les objets afin de pouvoir cliquer sur certaines des icônes suivantes et accéder à ces objets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Icône d’état ou indicateur</strong> </th> 
   <th><strong>Description</strong> </th> 
   <th><strong>Objet</strong> </th> 
   <th>En cliquant</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">ou <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_troubl.png" style="width: 29;height: 26;"> ou <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_Risk.png" style="width: 27;height: 28;"> ou <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Indique que la condition du projet est Sur la cible (vert), En danger (rouge) ou À risque (jaune).<br>Pour plus d’informations sur la condition du projet, voir <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Présentation de la condition et du type de condition du projet</a>.</td> 
   <td>Projets</td> 
   <td>Cliquez pour ouvrir la liste des tâches du projet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Indique que l’objet comporte des notes (mises à jour) dans l’onglet Mises à jour .</td> 
   <td> <p>Projets<br>Tâches<br>Problèmes<br>Modèles<br>Tâches de modèle</p> </td> 
   <td> <p>Cliquez pour ouvrir l’onglet Mises à jour de l’objet. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">ou <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Indique que des documents sont attachés à l’objet. </td> 
   <td> Projets<br>Tâches<br>Problèmes<br>Modèles<br>Tâches de modèle </td> 
   <td>Cliquez pour ouvrir l’onglet Documents de l’objet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">ou <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Indique que des problèmes sont en cours sur le projet ou la tâche.</td> 
   <td> Projets<br>Tâches </td> 
   <td>Cliquez sur pour ouvrir l’objet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> ou <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>Indique qu’il y a une validation sur l’objet.</td> 
   <td> Projets<br>Tâches<br>Problèmes<br>Modèles<br>Tâches de modèle </td> 
   <td>Cliquez sur pour ouvrir l’objet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="dépense_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>Vous pouvez ajouter une colonne Icône Dépenses dans votre vue pour afficher cette icône. Cela indique que des dépenses sont associées au projet ou à la tâche.</p> </td> 
   <td> <p>Projets</p> <p>Tâches</p> </td> 
   <td>Cliquez pour ouvrir l'onglet Dépenses du projet ou de la tâche. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_Risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Indique que l’état de progression d’une tâche est l’un des suivants :</p> 
    <ul> 
     <li>Heure d’activation (carré vert)</li> 
     <li>Tard (cercle rouge)</li> 
     <li>En danger (diamant bleu)</li> 
     <li>Derrière (triangle jaune)</li> 
    </ul> <p>Pour plus d’informations sur l’état de progression des tâches, consultez la <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">présentation de l’état de progression de la tâche</a>.</p> </td> 
   <td>Tâches</td> 
   <td>Cliquez sur pour ouvrir la tâche. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> ou <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>Indique que la tâche se trouve actuellement sur le chemin critique. <br>Pour plus d’informations sur les tâches sur un chemin critique du projet, voir <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">Présentation du projet Chemin critique</a>.</td> 
   <td>Tâches</td> 
   <td>Cliquez sur pour ouvrir la tâche.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Indique que la tâche est associée à un jalon. Votre administrateur système peut personnaliser la couleur du diamant dans votre environnement.<br>Pour plus d’informations sur les jalons, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Création d’un chemin de jalon</a>.</td> 
   <td>Tâches</td> 
   <td>Cliquez sur pour ouvrir la tâche. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Lien vers l’objet source d’un problème. L’objet source d’un problème est l’objet sur lequel le problème a été consigné. Une tâche ou un projet peut être un objet source pour les problèmes. </td> 
   <td>Problèmes</td> 
   <td>Cliquez pour ouvrir l’objet source (tâche ou projet) d’un problème. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolve_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Indique qu’un objet de résolution résout finalement le problème. Dans ce cas, vous ne pouvez pas terminer le problème. Elle est terminée lorsque l’objet de résolution est terminé. <br>Pour plus d’informations sur la résolution d’objets, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution d’objets résolvables </a>.</td> 
   <td>Problèmes</td> 
   <td>Cliquez pour ouvrir l’objet de résolution du problème. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>Affichez un document.</td> 
   <td>Documents</td> 
   <td>Cliquez sur pour télécharger le document.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>Téléchargez un document.</td> 
   <td>Documents</td> 
   <td>Cliquez sur pour télécharger le document.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>Indique le type de document.</td> 
   <td>Documents</td> 
   <td>Cliquez sur pour télécharger le document.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_belongs_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Indique que l’utilisateur est associé à une société. </td> 
   <td>Utilisateurs</td> 
   <td>Indisponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_Team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Indique que l’utilisateur est associé à une équipe.</td> 
   <td>Utilisateurs</td> 
   <td>Cliquez sur pour ouvrir le profil utilisateur.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Raccourci vers l’onglet Affectation de l’utilisateur. </td> 
   <td>Utilisateurs</td> 
   <td>Cliquez pour ouvrir l’onglet Affectation de l’utilisateur et découvrez les tâches qui lui sont affectées.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>Indique que l’utilisateur se trouve dans un fuseau horaire différent de celui du système.</td> 
   <td>Utilisateurs</td> 
   <td>Indisponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_dépense_icon.png" style="width: 44;height: 45;"> </td> 
   <td>Indique qu’une dépense est facturable.<br>Pour plus d'informations sur les dépenses, consultez la section <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gérer les dépenses de projet </a>.</td> 
   <td>Frais</td> 
   <td>Indisponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="dépense_remboursable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> Indique qu’une dépense est remboursable.<br>Pour plus d'informations sur les dépenses, consultez la section <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gérer les dépenses de projet </a>.</td> 
   <td>Frais</td> 
   <td>Indisponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="discount_dépense_icon.png" style="width: 44;height: 43;"></td> 
   <td> Indique qu’une dépense a été remboursée.<br>Pour plus d'informations sur les dépenses, consultez la section <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gérer les dépenses de projet </a>.</td> 
   <td>Frais</td> 
   <td>Indisponible</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
