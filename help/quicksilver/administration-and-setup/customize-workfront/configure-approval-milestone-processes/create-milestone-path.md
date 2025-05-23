---
title: Créer un chemin jalonné
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des chemins jalonnés qui peuvent ensuite être appliqués à n’importe quel projet du système. Les modifications apportées aux chemins jalonnés dans cette zone affectent l’ensemble du système Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 64%

---

# Créer un chemin jalonné

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des chemins jalonnés qui peuvent ensuite être appliqués à n’importe quel projet du système. Les modifications apportées aux chemins jalonnés dans cette zone affectent l’ensemble du système Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Jalons et chemins jalonnés

Vous pouvez associer les tâches clés d’un projet à des jalons prédéfinis. Cette fonction permet de fournir aux responsables et aux autres parties prenantes une vue d’ensemble détaillée de la progression d’un projet.

La somme de tous les jalons prédéfinis est appelée un chemin jalonné.

La première étape de la création d’un chemin jalonné consiste à identifier les étapes de jalon et à définir les jalons. Puisque vous pouvez associer un chemin jalonné à plusieurs projets, les étapes de jalon doivent être des phases générales ou des stades d’un projet.

Pour plus d’informations sur l’association d’un chemin jalonné à un projet et d’un jalon à une tâche, voir [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Créer un chemin jalonné

{{step-1-to-setup}}

1. Cliquez sur **Processus** > **Chemins jalonnés**.
1. Cliquez sur **Nouveau chemin jalonné**.
1. Indiquez les informations suivantes dans la zone **Informations de base** :

   <table style="table-layout:auto">
    <tr>
      <td>Nom du chemin jalonné</td>
       <td>Saisissez un nom pour le chemin jalonné.</td>
    </tr>
    <tr>
      <td>Description</td>
      <td>Saisissez une description pour définir le chemin jalonné.</td>
    </tr>
    <tr>
       <td>Est active</td>
      <td>Cochez cette case si vous souhaitez que le chemin jalonné soit actif. D’autres utilisateurs et utilisatrices peuvent trouver ce chemin et le joindre à des projets lors de la création ou de la modification de projets. Les chemins jalonnés inactifs ne peuvent pas être associés aux projets. Cette option est activée par défaut.</td>
    </tr>
    <tr>
      <td>Groupes</td>
      <td>Sélectionnez les groupes répertoriés pour permettre aux utilisateurs et utilisatrices de ces groupes d’afficher et d’appliquer ce chemin jalonné à leurs projets. Le groupe principal de l’utilisateur ou utilisatrice qui saisit le chemin jalonné est sélectionné par défaut.</td>
    </tr>
   </table>

1. Indiquez les informations suivantes dans la zone **Jalons** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Saisissez des noms descriptifs pour chaque jalon.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description du jalon.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Choisissez une couleur à associer à votre jalon. </p> <p>Si vous ne choisissez pas de couleur, le système choisit la dernière couleur utilisée dans un chemin jalonné. Nous vous recommandons de choisir une couleur unique pour chaque jalon. La couleur est utilisée à des fins visuelles et de création de rapports.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Ajouter le jalon** et continuez à ajouter des jalons, si nécessaire, jusqu’à ce que le chemin soit terminé.

1. Cliquez sur **Créer un chemin jalonné** pour enregistrer vos modifications.

   Votre chemin jalonné est prêt à être associé à un projet.

   Pour plus d’informations sur l’association des chemins jalonnés à des projets et des jalons à des tâches, voir [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).


1. (Facultatif) Cliquez sur l’icône **Exporter** ![Icône Exporter](assets/export-icon.png), puis sélectionnez l’un des formats suivants pour exporter la liste de chemins jalonnés vers un fichier :

   * PDF
   * Excel
   * Excel (xlsx)
   * Délimité par des tabulations

1. (Facultatif) Sélectionnez un jalon dans la liste des jalons, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) pour modifier les informations du jalon.
1. (Facultatif) Sélectionnez un jalon dans la liste des jalons, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete-icon.png) pour le supprimer.
1. Cliquez sur **Oui, supprimer**.
Le jalon est supprimé et ne peut pas être récupéré. Toutes les informations de projet associées au jalon et toutes les informations de tâche associées aux chemins jalonnés sont également supprimées.


## Affichage des détails du chemin jalonné dans un rapport de projet

Vous pouvez afficher les détails d’un chemin jalonné dans un rapport de projet.

Vous devez associer un chemin jalonné à un projet avant de pouvoir afficher ses détails dans un rapport de projet.

Pour plus d’informations sur l’association de chemins jalonnés à des projets, voir [Modifier des projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis sur **Projet**.
1. Cliquez sur **Ajouter une colonne**.
1. Dans la zone **Afficher dans cette colonne**, commencez à saisir **Chemin jalonné**, puis cliquez sur **Nom du chemin jalonné** lorsqu’il s’affiche.
1. (Facultatif) Cliquez sur **Filtres** et ajoutez le filtre suivant au rapport : **L’ID de chemin jalonné du projet n’est pas vide**.

   Le filtre vous garantit d’afficher uniquement les projets associés à un chemin jalonné dans le rapport.

1. Cliquez sur **Enregistrer + Fermer**.
1. Ajoutez un nom à votre rapport, puis cliquez sur **Appliquer**.

   Le rapport de projet s’affiche. Les chemins jalonnés associés à chaque projet s&#39;affichent dans la dernière colonne du rapport.
1. Cliquez sur le nom d&#39;un chemin jalonné dans la dernière colonne du rapport.

   Les détails du chemin jalonné s’affichent.

   ![Détails du chemin jalonné du rapport de projet](assets/milestone-details-from-project-report.png)

   La page de détails du chemin jalonné affiche les informations suivantes :

   * Nom, ID et description du chemin jalonné
   * Groupes de chemins jalonnés
   * Noms de jalons, descriptions, couleurs et icônes de couleur

1. (Facultatif) Cliquez sur **Précédent** pour revenir au rapport du projet.



