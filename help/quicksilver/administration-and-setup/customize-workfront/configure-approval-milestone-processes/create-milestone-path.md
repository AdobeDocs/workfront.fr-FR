---
title: Création d’un chemin Milestone
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des chemins jalonnés qui peuvent ensuite être appliqués à n’importe quel projet du système. Les modifications apportées aux chemins jalonnés dans cette zone affectent l’ensemble du système Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 99%

---

# Créer un chemin jalonné

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des chemins jalonnés qui peuvent ensuite être appliqués à n’importe quel projet du système. Les modifications apportées aux chemins jalonnés dans cette zone affectent l’ensemble du système Workfront.

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
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
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
