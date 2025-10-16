---
title: Création ou modification d’une condition personnalisée
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer ou modifier une condition personnalisée pour des projets, des tâches et des problèmes en fonction des besoins de votre entreprise.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: e50afb39f151ae8663ca2903454b475b21aa6f83
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 83%

---

# Créer ou modifier une condition personnalisée

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer ou modifier une condition personnalisée pour des projets, des tâches et des problèmes en fonction des besoins de votre entreprise.

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
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer ou modifier une condition personnalisée

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Conditions**.

1. Cliquez sur l’onglet du type d’objet (**Projet**, **Tâche**, ou **Problème**) que vous souhaitez associer à la condition.

1. Pour créer une condition, cliquez sur **Ajouter une nouvelle condition**.

   Ou

   Pour modifier une condition existante, cliquez sur **Modifier** en regard du nom de la condition.

   ![Modifier la condition personnalisée](assets/custom-conditions-0825.png)

1. Configurez votre condition personnalisée à l’aide des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nom de la condition</td> 
      <td>(Obligatoire) Attribuez un nom explicite au groupe.</td> 
     </tr> 
     <tr> 
      <td>Description</td> 
      <td>(Facultatif) Saisissez une description de l’objectif de la condition à destination des personnes qui vont l’utiliser.</td> 
     </tr> 
     <tr> 
      <td>Couleur</td> 
      <td>(Facultatif) Cliquez sur l’icône des couleurs, puis sélectionnez la couleur d’affichage de la condition dans les projets, les tâches ou les problèmes. Vous pouvez également saisir un nombre hexadécimal.</td> 
     </tr> 
     <tr> 
      <td>Équivaut à </td> 
      <td><p>(Obligatoire, pour les projets uniquement) Cliquez sur l’option de la liste déroulante qui décrit le mieux la fonction de votre nouvelle condition. Par exemple, pour une condition nommée Progresse bien, cliquez sur Dans les temps. Cela détermine le fonctionnement de vos conditions par défaut. Chaque condition que vous créez doit correspondre à l’une des options du menu déroulant.</p>
      <p>Pour plus d’informations sur les conditions par défaut, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Définir une condition personnalisée comme condition par défaut pour les projets</a> et <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Définir une condition personnalisée comme condition par défaut pour les tâches et les problèmes</a>.</p>
      <p>Cette option ne peut pas être modifiée une fois la création de la condition terminée.</p></td> 
     </tr> 
     <tr> 
      <td>Clé</td> 
      <td><p>(Obligatoire) Pour une condition de projet, saisissez une abréviation alphanumérique que les utilisateurs et les utilisatrices pourront reconnaître. Pour une condition de tâche ou de problème, saisissez un code numérique à deux chiffres compris entre 01 et 99. </p>
      <p>Cette clé, qui est utilisée dans l’API et qui peut être utilisée à des fins de création de rapports, doit être unique pour chaque objet.</p>
      <p>Vous ne pouvez pas modifier la clé d’une condition après avoir enregistré la condition. </p></td> 
     </tr> 
     <tr> 
      <td>Masquer la condition</td> 
      <td><p>(Facultatif) Cette option est disponible pour les conditions personnalisées que vous ne souhaitez plus que les personnes utilisent, mais que vous souhaitez conserver pour des raisons d’archivage. </p>
      <p>Si vous masquez une condition personnalisée qui est utilisée pour des éléments de travail, elle continue de s’afficher dans ces éléments de travail après que vous l’avez masquée. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Vous pouvez normaliser la terminologie et les couleurs des conditions des trois types d’objets. Pour ce faire, copiez le nom de la condition et le code hexadécimal de la couleur d’un onglet (Projet, Tâche, Problème) de la condition correspondante vers les deux autres onglets.

1. (Facultatif) Faites glisser ![icône Déplacer](assets/move-icon---dots.png) toute condition vers un nouvel emplacement pour réorganiser la liste.

   Cela modifie l’ordre dans lequel les conditions s’affichent dans les projets, tâches et problèmes :

   * Lorsqu’un utilisateur ou une utilisatrice modifie un projet.

     ![Modifier la condition lors de la modification du projet](assets/change-condition-edit-project-0825.png)

   * Lorsqu’une personne modifie la condition d’une tâche ou d’un problème en mode Liste :

     ![Modifier la condition dans la liste](assets/change-conditions-list-dropdown-0925.png)

     >[!NOTE]
     >
     >Dans l’affichage Condition par défaut, le champ **Condition** est un type de champ qui ne peut pas être modifié en ligne. Lorsque vous ajoutez le champ **Condition** séparément à une vue, il est modifiable. Pour plus d’informations sur la modification en ligne, voir [Modification en ligne d’éléments d’une liste dans Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

1. Cliquer sur **Enregistrer**.

Vous pouvez définir votre condition personnalisée comme condition par défaut pour les projets ou pour les tâches et les problèmes. Pour plus d’informations, voir la section [Définir une condition personnalisée comme condition par défaut pour les projets](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) et [Définir une condition personnalisée comme condition par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Pour plus d’informations sur les conditions personnalisées, voir la section [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).


<!-- THIS WAS ORIGINALLY BETWEEN THE OTHER TWO BULLETS.
   * When a user is changing the condition for a task or issue on the Updates tab:

     ![Change condition when updating comment](assets/change-condition-update-comment.png)
   -->
