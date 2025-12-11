---
navigation-topic: use-lists
title: Commencer avec les listes dans  [!DNL Adobe Workfront]
description: Vous pouvez consulter des listes d’objets sur  [!DNL Adobe Workfront]  afin d’obtenir des informations à leur sujet, telles que leurs dates de début et d’échéance, les utilisateurs et utilisatrices qui leur sont affectés et les autres objets qui leur sont associés.
feature: Get Started with Workfront
author: Nolan
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '2301'
ht-degree: 72%

---

# Commencer avec les listes dans [!DNL Adobe Workfront]

<!--Audited: 12/2025-->

Vous pouvez consulter des listes d’objets sur [!DNL Adobe Workfront] pour obtenir des informations sur ces derniers, telles que leurs dates de début et d’échéance, les utilisateurs et utilisatrices qui leur sont affectés et les autres objets qui leur sont associés.

Voici quelques caractéristiques des listes dans [!DNL Workfront] :

* Les listes sont actualisées automatiquement toutes les cinq minutes pour mettre à jour les informations que d’autres utilisateurs et utilisatrices du système sont en train de mettre à jour ailleurs.
* Certaines zones dans [!DNL Workfront] sont préconfigurées avec des listes d’objets par défaut.

  Vous pouvez personnaliser la plupart de ces listes préconfigurées.

* Un administrateur ou une administratrice de [!DNL Workfront] peut créer des listes personnalisées à appliquer à diverses zones de [!DNL Workfront].

  Pour plus d’informations sur la création de listes au niveau du système, voir l’article [Créer, modifier et partager des filtres, des vues et des regroupements par défaut](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

* Voici les types de listes disponibles dans Workfront :

   * Listes standard
   * Listes améliorées

  Pour plus d’informations, consultez la section [La différence entre les listes standard et améliorées](#the-difference-between-the-standard-and-the-enhanced-lists) dans cet article.

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures à un filtre, une vue ou un regroupement avec accès à partager </p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>[!UICONTROL View] or higher access to filters, views, groupings</p> <P>For items in the [!UICONTROL Setup] area, you need administrative access for the item or the [!UICONTROL System Administrator] access level.</P> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level.<br>For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>[!UICONTROL View] or higher permissions with access to share</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.
-->

## Listes d’objets

Vous trouverez ci-dessous quelques types de listes d’objets que vous pouvez trouver sur [!DNL Workfront] et certaines des zones où elles s’affichent par défaut lorsque vous avez le droit d’afficher un objet.

>[!NOTE]
>
>Cette liste n’est pas exhaustive. Chacune de ces listes d’objets peut également apparaître dans un rapport ou un tableau de bord. Par exemple, un rapport de projet ou un tableau de bord contenant un rapport de projet affiche également une liste de projets.



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] Liste</strong></th> 
   <th><strong>Emplacement de la liste d’objets</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Liste de portfolios</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste de programmes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL cliquer sur un portfolio] &gt;[!UICONTROL Programmes]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste de projets</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL cliquer sur un portfolio] &gt;[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL cliquer sur un portfolio] &gt;[!UICONTROL Programmes] &gt;[!UICONTROL cliquer sur un programme] &gt;[!UICONTROL Projets]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste de tâches</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt; [!UICONTROL Tasks]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL click a task] &gt;[!UICONTROL Subtasks]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL click a task] &gt; [!UICONTROL Predecessors*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste de problèmes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL click] a project &gt;[!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL click a task] &gt; [!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL click a task] &gt;[!UICONTROL Subtasks] &gt;[!UICONTROL click a task] &gt; [!UICONTROL Issues]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des rapports</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Reports]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des tableaux de bords</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dashboards]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des itérations</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] &gt; [!UICONTROL Iterations]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des utilisateurs et des utilisatrices</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Users]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des documents</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL cliquer sur un portfolio] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt; [!UICONTROL cliquer sur un portfolio] &gt;[!UICONTROL Programmes] &gt;[!UICONTROL cliquer sur un programme] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL click a task] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL click] a project &gt; [!UICONTROL Issues] &gt;[!UICONTROL click an issue] &gt; [!UICONTROL Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des feuilles de temps</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Feuilles de temps] &gt; [!UICONTROL Toutes les feuilles de temps]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des taux de facturation</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Billing Rates*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des enregistrements de facturation</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL click a project] &gt; [!UICONTROL Billing Records]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des risques</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Risks]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des dépenses</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click] a project &gt;[!UICONTROL Expenses]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL click a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL click a task] &gt;[!UICONTROL Expenses]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des entrées d’heure</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click] un projet</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL click a task] &gt;[!UICONTROL Hours]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click] un projet &gt;[!UICONTROL Issues] &gt;[!UICONTROL click] un événement &gt;[!UICONTROL Hours]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des formulaires personnalisés</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Setup] &gt;[!UICONTROL Custom Forms] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Liste des groupes ou sous-groupes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL click the parent group] &gt;[!UICONTROL Subgroups] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des équipes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des entreprises</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Companies]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des planifications</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Schedules]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des modèles de mise en page</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Layout Templates]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

*Vous ne pouvez pas personnaliser la liste dans la zone spécifiée. Un administrateur ou une administratrice [!DNL Workfront] peut créer une liste personnalisée au niveau du système, ou vous pouvez créer un rapport pour cet objet si votre niveau d’accès vous permet de modifier des rapports.

## Éléments de liste

Une liste contient certains éléments qui définissent son format et les informations qui s’affichent. Plusieurs éléments de liste de système sont disponibles par défaut. Vous pouvez également créer des éléments personnalisés pour répondre à vos besoins.

>[!NOTE]
>
>Lorsque vous sélectionnez un nouveau filtre, une nouvelle vue ou un nouveau regroupement dans une liste, cette sélection est conservée même si vous vous déconnectez de [!DNL Workfront] ou si vous fermez votre navigateur.

Les éléments d’une liste sont les suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Élément</strong></th> 
   <th><strong>Explication</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Filter]</strong></td> 
   <td> <p>Les filtres éliminent les informations inutiles d’une liste, en fonction des critères que vous spécifiez. </p> <p>Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Vue d’ensemble des filtres</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>Les vues définissent les champs (colonnes) à afficher à l’écran.</p> <p>Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Vue d’ensemble des vues dans [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Grouping]</strong></td> 
   <td> <p>Les regroupements séparent les objets de la liste en zones en fonction des critères que vous spécifiez.</p> <p>Par exemple, les problèmes d’une liste peuvent être affichés dans des sections par statut ou par priorité.</p> <p>Vous pouvez avoir jusqu’à trois couches de regroupements dans un groupement standard, et vous pouvez ajouter une quatrième couche si vous configurez un regroupement en mode Texte.</p> <p>Pour plus d’informations sur les regroupements, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Vue d’ensemble des regroupements dans [!DNL Adobe Workfront]</a>.</p> <p>Pour plus d’informations sur le mode Texte, voir <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Vue d’ensemble du mode Texte</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Ces éléments s’affichent par défaut en haut de chaque liste. Ils sont épinglés et ne se déplacent pas lorsque vous faites défiler la liste. Passez la souris sur l’icône de chaque élément pour l’identifier.

![Liste des éléments](assets/nwe-list-elements.png)

Vous pouvez personnaliser les éléments de la liste dans les domaines suivants et les partager avec d’autres personnes :

* Toute liste par défaut du système trouvée dans la section [Commencer avec les listes dans  [!DNL Adobe Workfront]](#default-workfront-lists) dans cet article.
* Tout rapport partagé avec vous.

Les éléments constitutifs des listes sont les mêmes que ceux des rapports.

Pour plus d’informations sur la création et la personnalisation des éléments constitutifs des listes et des rapports, voir [Éléments de rapport : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Répertorier des actions

Vous pouvez effectuer les actions suivantes dans une liste :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong></th> 
   <th><strong>Informations</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Modifier en ligne</strong> </td> 
   <td> <p>Modifiez les objets et leurs informations directement dans la liste.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Modifier en ligne les éléments d’une liste dans [!DNL Adobe Workfront]</a>.</p> 
   <p><b>NOTE :</b></p>
   <p>La modification en ligne n’est pas possible dans un regroupement.</p>

</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Mettre à jour avec le [!UICONTROL Summary]</strong> </td> 
   <td> <p>Mettez à jour les tâches et les problèmes au niveau du projet en utilisant le panneau [!UICONTROL Summary].</p> <p><b>CONSEIL :</b></p> <p>Le résumé n'est pas disponible pour tous les objets et n'est pas disponible dans les rapports Tâches ou Événements.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Vue d’ensemble du résumé</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personnaliser l’affichage de la liste</strong> </td> 
   <td> <p>Personnalisez l’aspect et la convivialité d’une liste, la disposition des colonnes, l’ordre de tri des éléments ou le nombre d’éléments affichés.</p> <p><b>NOTE :</b></p> <p>Les modifications apportées au nombre d’éléments à afficher sur une page sont annulées lorsque vous vous déconnectez d’[!DNL Workfront] ou fermez votre navigateur. Les modifications peuvent également être annulées après une période de 8 heures.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modifier l’affichage d’une liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtre rapide</strong> </td> 
   <td> <p>Appliquez un filtre rapide pour ne trouver que les éléments qui sont importants pour vous afin de pouvoir les consulter, les mettre à jour ou les partager rapidement avec d’autres personnes.</p> <p><b>IMPORTANT :</b></p> <p> À l’aide du filtre rapide, vous pouvez trouver les éléments qui contiennent un mot de recherche, que cet élément soit visible à l’écran ou qu’il s’affiche après un défilement vers le bas de la page. Lorsque vous utilisez les fonctions de recherche de votre navigateur, vous ne pouvez trouver que des éléments déjà visibles à l’écran. Si votre liste comporte plusieurs pages, les filtres rapides ne recherchent que les éléments de la page en cours.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Appliquer le filtre rapide à une liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exporter</strong> </td> 
   <td> <p>Exportez une liste d’objets à partir de [!DNL Workfront]. Lorsqu’une liste contient plus de 2 000 éléments, l’exportation de la liste est le seul moyen de consulter tous les éléments sur une seule page.</p> <p>Pour plus d’informations sur l’exportation d’une liste, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Exporter une liste</a>. Pour plus d’informations sur les formats et les limites d’export, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exporter des données</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barre d’outils de la liste

Le tableau suivant répertorie un grand nombre d’icônes disponibles dans la barre d’outils et indique ce qui se passe lorsque vous cliquez dessus :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icône</strong></td> 
   <td><strong>Description</strong></td> 
   <td><strong>En cas de clic</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Add item or user]</td> 
   <td>Ouvrez plus d’options, y compris l’ajout d’un nouvel élément ou d’un nouvel utilisateur ou d’une nouvelle utilisatrice.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task above]</td> 
   <td> <p>Insérez une tâche au-dessus de la tâche sélectionnée.</p> <p>Cette option n’est disponible que pour les tâches. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task below]</td> 
   <td> <p>Insérez une tâche sous la tâche sélectionnée.</p> <p>Cette option n’est disponible que pour les tâches. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Edit]</td> 
   <td>Modifiez l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>Copiez l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Delete]</td> 
   <td>Supprimez l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Add to]</td> 
   <td> <p>Ouvrez la boîte de dialogue pour ajouter le problème sélectionné à une itération.</p> <p>Cette option n’est disponible que pour les problèmes.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>Partagez l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Indent and outdent tasks] </td> 
   <td> <p>Créez un alinéa ou un retrait pour la tâche sélectionnée. </p> <p>Cette option n’est disponible que pour les tâches. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL More]</td> 
   <td>Ouvrez des options supplémentaires pour l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Quick filter] </p> </td> 
   <td> <p>Ouvrez la zone de recherche de filtre rapide pour trouver des éléments dans la liste affichée.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Exportez la liste vers des fichiers PDF, Excel ou délimités par des tabulations.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Affichez la liste dans la vue Agile.<br>Cette option n’est disponible que pour les tâches.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Affichez la liste dans la vue [!UICONTROL Gantt Chart].</p> <p>Cette option n’est disponible que pour les projets et les tâches.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menu déroulant des [!UICONTROL Filter].</td> 
   <td> <p>Affichez une liste de filtres et des options supplémentaires pour gérer les filtres, y compris pour créer un filtre. </p> <p>Sur un petit écran, le nom du filtre est remplacé par l’icône du filtre. Un point bleu s’affiche sur l’icône Filtre lorsque vous appliquez un filtre autre que « [!UICONTROL All] ».</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu déroulant des [!UICONTROL View].</td> 
   <td> <p>Affichez une liste de vues et des options supplémentaires pour gérer les vues, y compris pour créer une vue. </p> <p>Sur un petit écran, le nom de la vue est remplacé par l’icône [!UICONTROL view]. Un point bleu s’affiche sur l’icône [!UICONTROL View] lorsque vous appliquez une vue autre que « [!UICONTROL Standard] ».</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu déroulant de [!UICONTROL Grouping]</td> 
   <td> <p>Affichez une liste de regroupements et des options supplémentaires pour gérer les regroupements, y compris pour créer un regroupement. </p> <p>Sur un petit écran, le nom du regroupement est remplacé par l’icône [!UICONTROL grouping]. Un point bleu s’affiche sur l’icône [!UICONTROL Grouping] lorsque vous appliquez un regroupement autre que « [!UICONTROL Nothing] ».</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Plan mode]</p> </td> 
   <td> <p>Choisissez si vous souhaitez enregistrer automatiquement ou manuellement les modifications apportées à une liste de tâches. </p> <p>Pour plus d’informations sur la modification des tâches dans une liste, voir <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Modifier les tâches dans une liste</a>. </p> <p>Cette option n’est disponible que pour les tâches.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Summary]</td> 
   <td> <p>Affiche ou masque la case [!UICONTROL Summary] pour l’élément sélectionné.</p> <p>Cette option n’est disponible que pour les tâches et les problèmes.</p> <p>Pour plus d’informations sur le panneau [!UICONTROL Summary], consultez <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Summary overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Remove]</td> 
   <td>Supprimez un élément de la liste. Par exemple, en tant qu’administrateur ou administratrice de groupes gérant les personnes membres d’un groupe ou d’un sous-groupe, vous pouvez supprimer une personne membre d’un groupe comme expliqué dans <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Afficher et gérer les appartenances à un groupe</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>Saisissez un commentaire ou une mise à jour.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Différence entre les listes et les rapports

Les listes et les rapports sont des grilles qui contiennent des informations sur un type d’objet.

Le tableau suivant présente les similitudes et les différences entre les listes et les rapports :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Fonctionnalité</strong> </th> 
   <th><strong>Liste</strong> </th> 
   <th><strong>Rapport</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>N’importe quelle personne peut les créer.</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Seuls un administrateur ou une administratrice [!DNL Workfront] et les utilisateurs et utilisatrices disposant d’une licence [!UICONTROL Plan] peuvent les créer.</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Un jeu par défaut est disponible auprès de [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personnalisable en mode standard</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personnalisable en mode texte</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les partager avec d’autres utilisateurs et utilisatrices.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les partager à l’échelle du système.</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les partager en dehors du système.</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez exporter vers les formats .pdf, [!DNL Excel] et texte séparé par des tabulations.</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez planifier leur diffusion dans un e-mail.</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les ajouter à un modèle de mise en page.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les ajouter à des sections personnalisées. </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les ajouter à un tableau de bord.</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez utiliser les invites pour personnaliser ce qu’elles affichent.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les afficher dans un graphique.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez y modifier des objets en ligne.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

*Vous devez avoir accès aux filtres, vues et regroupements pour pouvoir les créer. Pour plus d’informations, voir [Accorder l’accès aux filtres, vues et regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

**Pour pouvoir créer des filtres, des vues et des regroupements, ainsi que des rapports, des tableaux de bord et des calendriers, vous devez y avoir accès. Pour plus d’informations, voir [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

***Vous pouvez personnaliser des listes pour les rapports placés sur un tableau de bord uniquement si le créateur du rapport a configuré les éléments de liste pour qu’ils soient visibles sur le tableau de bord.

>[!NOTE]
>
>Vous ne pouvez pas ajouter une liste à un tableau de bord sans créer un rapport et l’ajouter au tableau de bord au préalable.

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Pour plus d’informations sur la création de sections personnalisées, voir [Créer des onglets ou des sections personnalisés](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## La différence entre les listes standard et améliorées

Il existe deux types de listes dans [!DNL Workfront] :

* Listes standard

  ![Liste de projets standard](assets/standard-list-screen-shot-gray-groupings.png)

* Listes améliorées

  ![Listes améliorées](assets/enhanced-status-list.png)

Les fonctionnalités de chaque liste améliorée varient en fonction de la page à partir de laquelle vous y accédez.

Pour plus d’informations sur les listes améliorées, voir [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).



Le tableau suivant présente quelques-unes des différences entre les listes standard et améliorées dans [!DNL Workfront] :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Listes standard</b></td> 
   <td><b>Listes améliorées</b></td> 
  </tr> 
  <tr>
  <td> <p>Afficher <strong>Tous</strong> ou jusqu’à <strong>2 000</strong> éléments par défaut</p> </td> 
   <td> Afficher tous les éléments de la liste après un défilement manuel </td> 
  </tr>

<tr> 
   <td>L’interaction avec les éléments de la liste est cohérente pour tous les types d’objet. Pour ce faire, utilisez les icônes situées en haut de la liste.  </td> 
   <td>L’interaction avec les éléments de la liste peut varier en fonction du type d’objet. Pour ce faire, utilisez les icônes situées en haut de la liste ou la barre d’outils bleue activée après avoir sélectionné les éléments de la liste. </td> 
  </tr>

</td> 
  </tr> 
  <tr> 
   <td><p>Vous pouvez appliquer des modifications de couleur de cellule aux éléments d’une liste</p></td>
   <td><p>Vous ne pouvez pas appliquer de modifications de la couleur des cellules aux éléments d’une liste. </p></td>
   </td> 
   <td></td> 
  </tr> 
 </tbody> 
</table>

<!--
consider adding things like adding fields on the fly in an enhanced list when we will be able to do this-->

<!--old table: 
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Legacy lists</b></td> 
   <td><b>Updated lists</b></td> 
  </tr> 
  <td> <p>Display <strong>100</strong> items by default</p> </td> 
   <td> <p>Display <strong>All</strong> or up to <strong>2000</strong> items by default</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Use CTRL+F to find items in a list</p> </td> 
   <td> <p>Use quick filters to quickly find information in a large list</p> <p>For information about using quick filters in lists, see <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Apply the quick filter to a list</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>You can't inline edit custom fields with rich text formatting.</td> 
   <td> <p>Text in custom fields with formatting can be configured to allow bold, italics, underline, bullets, numbering, hyperlinks, and block quotes.</p> <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Conditional formatting can change the text color of links in a list</td> 
   <td>Cannot apply text color changes to links in a list</td> 
  </tr> 
 </tbody> 
</table>
-->
