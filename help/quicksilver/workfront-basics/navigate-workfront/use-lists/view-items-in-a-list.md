---
navigation-topic: use-lists
title: Prise en main des listes dans [!DNL Adobe Workfront]
description: Vous pouvez afficher des listes d’objets dans  [!DNL Adobe Workfront] pour obtenir des informations à leur sujet, telles que leurs dates de début et d’échéance, les utilisateurs qui leur sont affectés et d’autres objets qui leur sont associés.
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 7d43486ca566ae044fac1bbe20874bb45f833ef7
workflow-type: tm+mt
source-wordcount: '2388'
ht-degree: 4%

---

# Prise en main des listes dans [!DNL Adobe Workfront]

Vous pouvez afficher des listes d’objets dans [!DNL Adobe Workfront] pour obtenir des informations à leur sujet, telles que leurs dates de début et d’échéance, les utilisateurs qui leur sont affectés et d’autres objets qui leur sont associés.

Voici quelques caractéristiques de listes dans [!DNL Workfront] :

* Les listes sont actualisées automatiquement toutes les cinq minutes afin de mettre à jour les informations que d’autres utilisateurs du système mettent à jour ailleurs.
* Certaines zones de [!DNL Workfront] sont préconfigurées avec des listes d’objets par défaut.

  Vous pouvez personnaliser la plupart de ces listes préconfigurées.

* Un administrateur [!DNL Workfront] peut créer des listes personnalisées à appliquer à différentes zones de [!DNL Workfront].

  Pour plus d’informations sur la création de listes au niveau du système, consultez l’article [Créer, modifier et partager des filtres, des vues et des regroupements par défaut](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur à des filtres, vues, regroupements</p> <P>Pour les éléments de la zone [!UICONTROL Configuration], vous avez besoin d’un accès administratif pour l’élément ou le niveau d’accès [!UICONTROL Administrateur système].</P> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès.<br>Pour plus d'informations sur la façon dont un administrateur [!DNL Workfront] peut modifier votre niveau d'accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d'accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Vue] ou autorisations supérieures avec accès au partage</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

## Listes d’objets

Vous trouverez ci-dessous quelques types de listes d’objets que vous pouvez trouver dans [!DNL Workfront] et certaines des zones où elles s’affichent par défaut lorsque vous disposez des droits d’affichage d’un objet.

>[!NOTE]
>
>* Cette liste n&#39;est pas exhaustive. Chacune de ces listes d’objets peut également apparaître sur un rapport ou un tableau de bord. Par exemple, un rapport Projet ou un tableau de bord contenant un rapport Projet affiche également une liste de projets.
>* Dans cette liste, &quot;select&quot; signifie que vous devez cliquer sur le nom de l’élément, et non sur la case à cocher située à gauche du nom.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] list</strong></th> 
   <th><strong>Emplacement de la liste d’objets</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Liste des portefeuilles</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolio]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des programmes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL sélectionner un portefeuille] &gt;[!UICONTROL Programmes]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programmes]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des projets</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL sélectionner un portefeuille] &gt;[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL sélectionner un portefeuille] &gt;[!UICONTROL Programmes] &gt;[!UICONTROL sélectionner un programme] &gt;[!UICONTROL Projets]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des tâches</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner un projet] &gt; [!UICONTROL Tâches]</p> </li> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Tâches] &gt;[!UICONTROL sélectionner une tâche] &gt;[!UICONTROL Sous-tâches]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL sélectionner une tâche] &gt; [!UICONTROL Predecessors*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des problèmes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets] &gt; [!UICONTROL sélectionner] un projet &gt;[!UICONTROL Problèmes]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL sélectionner une tâche] &gt; [!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Tâches] &gt;[!UICONTROL sélectionner une tâche] &gt;[!UICONTROL Sous-tâches] &gt;[!UICONTROL sélectionner une tâche] &gt; [!UICONTROL Problèmes]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des rapports</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Rapports]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des tableaux de bord</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Tableaux de bord]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des itérations</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Équipes] &gt; [!UICONTROL Itérations]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des utilisateurs</td> 
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
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL sélectionner un portefeuille] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt; [!UICONTROL sélectionner un portefeuille] &gt;[!UICONTROL Programmes] &gt;[!UICONTROL sélectionner un programme] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Tâches] &gt;[!UICONTROL sélectionner une tâche] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projets] &gt; [!UICONTROL sélectionner] un projet &gt; [!UICONTROL Problèmes] &gt; [!UICONTROL sélectionner un problème] &gt; [!UICONTROL Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des feuilles de temps</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Feuille de calcul] s &gt; [!UICONTROL Toutes les feuilles de calcul]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des taux de facturation</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Taux de facturation*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des enregistrements de facturation</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets] &gt; [!UICONTROL sélectionner un projet] &gt; [!UICONTROL Enregistrements de facturation]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des risques</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Risques]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des dépenses</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner] un projet &gt;[!UICONTROL Dépenses]</p> </li> 
     <li> <p>[!UICONTROL Projets] &gt; [!UICONTROL sélectionner un projet] &gt;[!UICONTROL Tâches] &gt;[!UICONTROL sélectionner une tâche] &gt;[!UICONTROL Dépenses]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des entrées d’heure</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets] &gt;[!UICONTROL sélectionner] un projet</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL sélectionner un projet] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL sélectionner une tâche] &gt;[!UICONTROL HEURES]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL sélectionner] un projet &gt;[!UICONTROL Issues] &gt;[!UICONTROL Select] un problème &gt;[!UICONTROL Hours]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des formulaires personnalisés</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Configuration] &gt;[!UICONTROL Forms personnalisée] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Liste des groupes ou sous-groupes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuration] &gt; [!UICONTROL Groupes]</p> </li>
     <li> <p>[!UICONTROL Configuration] &gt;[!UICONTROL Groupes] &gt;[!UICONTROL Sélectionner le groupe parent] &gt;[!UICONTROL Sous-groupes] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste des équipes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuration] &gt;[!UICONTROL Équipes]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des entreprises</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuration] &gt;[!UICONTROL Sociétés]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des plannings</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuration] &gt;[!UICONTROL Planifications]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste des modèles de mise en page</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuration] &gt;[!UICONTROL Modèles de mise en page]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

Vous ne pouvez pas personnaliser la liste dans la zone spécifiée. Un administrateur [!DNL Workfront] peut créer une liste personnalisée au niveau du système ou vous pouvez créer un rapport pour cet objet si votre niveau d’accès vous permet d’accéder aux rapports de modification.

## Eléments de liste

Une liste contient certains éléments qui définissent son format et les informations qui s’affichent. Vous trouverez plusieurs éléments de liste système disponibles par défaut. Vous pouvez également créer des éléments personnalisés en fonction de vos besoins.

>[!NOTE]
>
>Lorsque vous sélectionnez un nouveau filtre, une nouvelle vue ou un nouveau regroupement dans une liste, cette sélection est conservée même si vous vous déconnectez de [!DNL Workfront] ou fermez votre navigateur.

Voici les éléments d&#39;une liste :

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
   <td> <p>Les filtres conservent dans une liste des informations inutiles, en fonction des critères que vous spécifiez. </p> <p>Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Présentation des filtres</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>Les vues définissent les champs (colonnes) que vous affichez à l’écran.</p> <p>Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Présentation des vues dans [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Groupement]</strong></td> 
   <td> <p>Les groupes séparent les objets de la liste en zones en fonction des critères que vous spécifiez.</p> <p>Par exemple, les problèmes d’une liste peuvent s’afficher dans des sections par statut ou par priorité.</p> <p>Vous pouvez avoir jusqu’à trois couches de groupement dans un groupement standard et vous pouvez ajouter une quatrième couche si vous configurez un groupement en mode texte.</p> <p>Pour plus d'informations sur les groupements, consultez la <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">présentation des groupements dans [!DNL Adobe Workfront]</a>.</p> <p>Pour plus d’informations sur le mode texte, voir <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Présentation du mode texte</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Par défaut, ces éléments s’affichent en haut de chaque liste. Ils sont collants et ne bougent pas lorsque vous faites défiler la liste. Pointez sur l’icône de chaque élément pour l’identifier.

![](assets/nwe-list-elements.png)

Vous pouvez personnaliser des éléments de liste dans les zones suivantes et les partager avec d’autres utilisateurs :

* Toute liste système par défaut trouvée dans la section [Prise en main des listes dans  [!DNL Adobe Workfront]](#default-workfront-lists) de cet article
* Tout rapport partagé avec vous

Les éléments de création des listes sont identiques à ceux des rapports.

Pour plus d’informations sur la création et la personnalisation des éléments de création des listes et des rapports, voir [Éléments de création de rapports : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Actions de liste

Vous pouvez effectuer les actions suivantes dans une liste :

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
   <td><strong>Modification en ligne</strong> </td> 
   <td> <p>Modifiez les objets et leurs informations directement dans la liste.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Modification en ligne d’éléments dans une liste dans [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Mise à jour avec le [!UICONTROL Summary]</strong> </td> 
   <td> <p>Mettez à jour les tâches et les problèmes au niveau du projet à l’aide du panneau [!UICONTROL Résumé].</p> <p>Conseil : Le résumé n’est pas disponible pour tous les objets et il n’est pas disponible dans les rapports Tâche ou Problème .</p> <p>Pour plus d’informations, consultez <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Vue d’ensemble du résumé</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personnaliser l’affichage de liste</strong> </td> 
   <td> <p>Personnalisez l’aspect d’une liste, la disposition des colonnes, l’ordre de tri des éléments ou le nombre d’éléments qui s’affichent.</p> <p>Remarque : Les modifications que vous apportez au nombre d’éléments à afficher sur une page sont annulées lorsque vous vous déconnectez de [!DNL Workfront] ou fermez votre navigateur. Les modifications peuvent également être annulées après une période de 8 heures.</p> <p>Pour plus d'informations, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modification de l'affichage d'une liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtre rapide</strong> </td> 
   <td> <p>Appliquez un filtre rapide pour rechercher uniquement les éléments qui vous intéressent afin de pouvoir rapidement les vérifier, les mettre à jour ou les partager avec d’autres personnes.</p> <p>Important : Vous pouvez trouver les éléments qui contiennent un mot de recherche à l’aide du filtre rapide, que cet élément soit visible à l’écran ou s’affiche après avoir fait défiler la page vers le bas. Lorsque vous utilisez les fonctionnalités de recherche de votre navigateur, vous ne pouvez trouver que les éléments déjà visibles à l’écran. Si votre liste comporte plusieurs pages, les filtres rapides ne recherchent que les éléments de la page active.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Appliquer le filtre rapide à une liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Export</strong> </td> 
   <td> <p>Exportez une liste d’objets de [!DNL Workfront]. Lorsqu’une liste contient plus de 2 000 éléments, l’exportation de la liste est le seul moyen de passer en revue tous les éléments d’une page.</p> <p>Pour plus d'informations sur l'export d'une liste, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Export d'une liste</a>. Pour plus d’informations sur les formats et les limites d’exportation, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Export data</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barre d’outils Liste

Le tableau suivant répertorie de nombreuses icônes disponibles dans la barre d’outils et indique ce qui se passe lorsque vous cliquez dessus :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icône</strong></td> 
   <td><strong>Description</strong></td> 
   <td><strong>En cliquant</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Ajouter un élément ou un utilisateur]</td> 
   <td>Ouvrez d’autres options, y compris l’ajout d’un nouvel élément ou d’un nouvel utilisateur.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insérer la tâche ci-dessus]</td> 
   <td> <p>Insérez une tâche au-dessus de la tâche sélectionnée.</p> <p>Cette option est disponible uniquement pour les tâches. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insérer la tâche ci-dessous]</td> 
   <td> <p>Insérez une tâche sous la tâche sélectionnée.</p> <p>Cette option est disponible uniquement pour les tâches. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Edit]</td> 
   <td>Modifiez l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copie]</td> 
   <td>Copiez l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Delete]</td> 
   <td>Supprimer l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Ajouter à]</td> 
   <td> <p>Ouvrez la boîte de dialogue pour ajouter le problème sélectionné à une itération.</p> <p>Cette option est disponible uniquement pour les problèmes.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>Partagez l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Tâches de retrait et de retrait] </td> 
   <td> <p>Retrait ou retrait de la tâche sélectionnée. </p> <p>Cette option est disponible uniquement pour les tâches. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Plus]</td> 
   <td>Ouvrir les options supplémentaires de l’élément sélectionné.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Filtre rapide] </p> </td> 
   <td> <p>Ouvrez la zone de recherche de filtre rapide pour rechercher des éléments dans la liste affichée.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Exportez la liste dans des fichiers PDF, Excel ou séparés par des tabulations.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Affichez la liste en mode Agile.<br>Cette option est disponible uniquement pour les tâches.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Graphique de Gantt]</td> 
   <td> <p>Affichez la liste dans la vue [!UICONTROL Gantt Chart].</p> <p>Cette option est disponible uniquement pour les projets et les tâches.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menu déroulant [!UICONTROL Filtrer]</td> 
   <td> <p>Affichez une liste de filtres et d’autres options pour gérer les filtres, y compris en créer un. </p> <p>Sur un petit écran, le nom du filtre est remplacé par l’icône de filtre. Un point bleu s’affiche sur l’icône Filtrer lorsque vous appliquez un filtre autre que "[!UICONTROL Tout]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu déroulant [!UICONTROL Vue]</td> 
   <td> <p>Affichez une liste de vues et d’autres options pour gérer les vues, y compris en créer une. </p> <p>Sur un petit écran, le nom de la vue est remplacé par l’icône [!UICONTROL Vue]. Un point bleu s’affiche sur l’icône [!UICONTROL Vue] lorsque vous appliquez une vue autre que "[!UICONTROL Standard]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu déroulant [!UICONTROL Groupement]</td> 
   <td> <p>Affichez une liste de regroupements et d’autres options pour gérer les regroupements, y compris en créer un. </p> <p>Sur un petit écran, le nom du groupement est remplacé par l’icône [!UICONTROL regroupement] . Un point bleu s’affiche sur l’icône [!UICONTROL Groupement] lorsque vous appliquez un autre regroupement que "[!UICONTROL Rien]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Mode Plan]</p> </td> 
   <td> <p>Choisissez si vous souhaitez enregistrer automatiquement ou manuellement les modifications que vous effectuez dans une liste de tâches. </p> <p>Pour plus d’informations sur l’édition des tâches dans une liste, voir <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Modifier les tâches dans une liste</a>. </p> <p>Cette option est disponible uniquement pour les tâches.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Summary]</td> 
   <td> <p>Affichez ou masquez la zone [!UICONTROL Summary] pour l’élément sélectionné.</p> <p>Cette option est disponible uniquement pour les tâches et les problèmes.</p> <p>Pour plus d’informations sur le panneau [!UICONTROL Summary] dans la nouvelle expérience [!DNL Adobe Workfront], voir <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Summary overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Supprimer]</td> 
   <td>Supprimez quelque chose de la liste. Par exemple, en tant qu’administrateur de groupe gérant les appartenances à un groupe ou à un sous-groupe, supprimez un membre du groupe comme expliqué dans la section <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Afficher et gérer les appartenances à un groupe</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>Saisissez un commentaire ou une mise à jour.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Différence entre listes et rapports

Les listes et les rapports sont des grilles qui contiennent des informations sur un type d’objet.

Le tableau suivant présente les similitudes et les différences entre les listes et les rapports :

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
   <td> <p>N’importe qui peut les créer</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Seul un administrateur [!DNL Workfront] et des utilisateurs possédant une licence [!UICONTROL Plan] peuvent les créer.</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Un ensemble par défaut est disponible dans [!DNL Workfront]</p> </td> 
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
   <td> <p>Vous pouvez les partager avec d’autres utilisateurs.</p> </td> 
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
   <td> <p>Vous pouvez exporter vers les formats .pdf, [!DNL Excel] et Délimité par des onglets.</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les planifier pour diffusion dans un email.</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez ajouter à un modèle de disposition</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les ajouter aux sections personnalisées </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les ajouter à un tableau de bord</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez utiliser des invites pour personnaliser ce qu’elles affichent.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez les afficher sous forme de graphique.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vous pouvez y insérer des objets de modification.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Vous devez avoir accès aux filtres, aux vues et aux regroupements pour pouvoir les créer. Pour plus d’informations, voir [Accorder l’accès aux filtres, aux vues et aux regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Pour pouvoir les créer, vous devez avoir accès aux filtres, vues et regroupements, ainsi qu’aux rapports, tableaux de bord et calendriers. Pour plus d’informations, voir [Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Vous ne pouvez personnaliser les listes des rapports placés sur un tableau de bord que si l’auteur du rapport a configuré les éléments de liste pour qu’ils soient visibles dans le tableau de bord.

>[!NOTE]
>
>Vous ne pouvez pas ajouter une liste à un tableau de bord sans créer de rapport et l’ajouter au tableau de bord en premier.

Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Pour plus d’informations sur la création de sections personnalisées, voir [Création d’onglets ou de sections personnalisés](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## Différence entre les listes mises à jour et héritées

Il existe deux types de listes dans [!DNL Workfront] :

* Listes héritées

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Listes mises à jour

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Les deux types de listes apparaissent dans le [!DNL Adobe Workfront].

Toutes les listes et tous les rapports de [!DNL Adobe Workfront] sont des listes mises à jour, à l’exception des éléments suivants :

* Listes dans la zone [!UICONTROL Setup]
* Listes dans la zone [!UICONTROL Rapports]

Le tableau suivant présente certaines des différences entre les listes héritées et mises à jour dans [!DNL Workfront] :

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Listes héritées</b></td> 
   <td><b>Listes mises à jour</b></td> 
  </tr> 
  <tr> 
   <td> <p>Polices héritées, en-têtes de colonne, modèle de couleur de regroupement bleu</p> </td> 
   <td> <p>Polices mises à jour, en-têtes de colonne, jeu de couleurs de regroupement gris</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modification en ligne plus lente</p> </td> 
   <td> <p>Modification en ligne plus rapide</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Afficher les <strong>100</strong> éléments par défaut</p> </td> 
   <td> <p>Afficher <strong>Tous</strong> ou jusqu’à <strong>2 000</strong> éléments par défaut</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilisez Ctrl+F pour rechercher des éléments dans une liste.</p> </td> 
   <td> <p>Utilisez des filtres rapides pour trouver rapidement des informations dans une liste volumineuse.</p> <p>Pour plus d'informations sur l'utilisation de filtres rapides dans les listes, voir <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Appliquer le filtre rapide à une liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Vous ne pouvez pas insérer des champs personnalisés avec la mise en forme de texte enrichi.</td> 
   <td> <p>Le texte des champs personnalisés avec mise en forme peut être configuré pour autoriser le gras, l’italique, le soulignement, les puces, la numérotation, les liens hypertexte et les guillemets de bloc.</p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Concevoir un formulaire à l’aide du créateur de formulaire</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>La mise en forme conditionnelle peut modifier la couleur du texte des liens dans une liste.</td> 
   <td>Impossible d’appliquer des modifications de couleur de texte aux liens d’une liste</td> 
  </tr> 
 </tbody> 
</table>
