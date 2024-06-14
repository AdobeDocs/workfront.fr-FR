---
title: Créer un chemin jalonné
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer des chemins de jalon qui peuvent ensuite être appliqués à n’importe quel projet du système. Les modifications apportées aux chemins d’accès aux jalons dans cette zone affectent l’ensemble du système Workfront.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 12%

---

# Créer un chemin jalonné

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

En tant qu’administrateur Adobe Workfront, vous pouvez créer des chemins de jalon qui peuvent ensuite être appliqués à n’importe quel projet du système. Les modifications apportées aux chemins d’accès aux jalons dans cette zone affectent l’ensemble du système Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Jalons et chemins de jalon

Vous pouvez associer les tâches clés d’un projet à des jalons prédéfinis. Cette fonction permet aux gestionnaires et aux autres parties prenantes de disposer d’un aperçu général de la progression d’un projet.

La somme de tous les jalons prédéfinis est appelée chemin de jalon.

La première étape de la création d’un chemin de jalon consiste à identifier les étapes de jalon et à définir les jalons. Puisque vous pouvez associer un chemin de jalon à plusieurs projets, les étapes de jalon doivent être des phases générales ou des étapes d’un projet.

Pour plus d’informations sur la manière d’associer un chemin de jalon à un projet et un jalon à une tâche, voir [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Créer un chemin jalonné

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Processus** > **Chemins Milestone**.
1. Cliquez sur **Nouveau Chemin Milestone.**
1. Indiquez les informations suivantes dans la variable **Informations de base** area :

   <table style="table-layout:auto">
    <tr>
      <td>Nom du chemin jalonné</td>
       <td>Saisissez un nom pour le chemin du jalon.</td>
    </tr>
    <tr>
      <td>Description</td>
      <td>Saisissez une description pour définir le chemin du jalon.</td>
    </tr>
    <tr>
       <td>Est active</td>
      <td>Cochez cette case si vous souhaitez que le chemin du jalon soit actif. D’autres utilisateurs peuvent trouver ce chemin et le joindre à des projets lors de la création ou de la modification de projets. Les chemins de jalon inactifs ne peuvent pas être associés aux projets. Cette option est activée par défaut.</td>
    </tr>
    <tr>
      <td>Groupes</td>
      <td>Sélectionnez les groupes répertoriés pour permettre aux utilisateurs de ces groupes d’afficher et d’appliquer ce chemin d’accès de jalon à leurs projets. Le groupe d’accueil de l’utilisateur qui saisit le chemin du jalon est sélectionné par défaut.</td>
    </tr>
   </table>

1. Indiquez les informations suivantes dans la variable **Jalons** area :

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
      <td>Saisissez une description pour le jalon.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Choisissez une couleur à associer à votre jalon. </p> <p>Si vous ne choisissez pas de couleur, le système choisit la dernière couleur utilisée dans un chemin de jalon. Nous vous recommandons de choisir une couleur unique pour chaque jalon. La couleur est utilisée à des fins visuelles et de création de rapports.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Ajouter Milestone** et continuez à ajouter des jalons, si nécessaire, jusqu’à ce que le chemin soit terminé.
1. Cliquez sur **Créer un chemin Milestone** pour enregistrer vos modifications.

   Votre chemin de jalon est prêt à être associé à un projet.

   Pour plus d’informations sur la manière d’associer des chemins de jalon à des projets et des jalons à des tâches, voir [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
