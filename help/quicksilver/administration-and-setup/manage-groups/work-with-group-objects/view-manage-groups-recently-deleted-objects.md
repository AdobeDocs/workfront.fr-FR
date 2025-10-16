---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Afficher et gérer les éléments récemment supprimés d'un groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher, filtrer, restaurer et exporter les tâches, documents et modèles récemment supprimés.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: 7eaff1c74cd880bde062e6fdf169c73d6eeb7f75
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 91%

---

# Afficher et gérer les éléments récemment supprimés d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et utiliser ses projets, tâches, problèmes, documents et modèles récemment supprimés comme suit :

* Afficher, filtrer et regrouper une liste d’éléments récemment supprimés
* Restaurer les éléments récemment supprimés que vous avez sélectionnés.
* Exporter une liste d’éléments récemment supprimés

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur les éléments supprimés, consultez [Gérer les éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr>
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr>
  <tr> 
   <td>Autorisations d’objet</td>
   <td>Les éléments supprimés doivent être associés au groupe ou à l’un de ses sous-groupes.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher et gérer les éléments récemment supprimés d’un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe.
1. Dans le panneau de gauche, cliquez sur **Récemment supprimé**.
1. Ouvrez l’un des onglets suivants où vous souhaitez afficher et gérer les éléments récemment supprimés du groupe :

   * Projets
   * Tâches
   * Problèmes
   * Documents
   * Modèles

   Chaque onglet répertorie les éléments du type d’objet correspondant qui appartiennent au groupe actif ou à ses sous-groupes et qui ont été supprimés au cours des 30 derniers jours.

   >[!NOTE]
   >
   >Si une personne a supprimé un projet, toutes les tâches, tous les problèmes et tous les documents qui le composent ont été supprimés en même temps. Ils ne s’affichent pas individuellement dans les onglets Tâches, Problèmes, Documents ou Modèles. Cependant, la restauration du projet restaure également tous les objets enfant dans le projet.
   >
   >
   >Si une personne a supprimé une tâche, un problème, un document ou un modèle individuellement, vous pouvez l’afficher et le gérer dans l’onglet approprié.

1. Effectuez l’une des actions suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Restaurer des objets</p> </td> 
      <td> <p>Sélectionnez jusqu’à dix objets, puis cliquez sur <strong>Restaurer</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Exporter la liste complète des objets de l’onglet</p> </td> 
      <td> <p>Cliquez sur <strong>Exporter</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Modifier l’affichage des informations dans la liste</p> </td> 
      <td> <p>Dans le coin supérieur droit de la liste, utilisez <strong>Filtrer</strong> pour définir ce qui s’affiche en fonction des critères que vous fournissez. Utilisez <strong>Affichage</strong> pour définir quels champs sont affichés sous forme de colonnes. Utilisez <strong>Regroupement</strong> pour regrouper les éléments en catégories.</p> </td> 
     </tr> 
    </tbody> 
   </table>
