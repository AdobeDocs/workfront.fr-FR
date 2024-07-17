---
title: Création ou modification d’une condition personnalisée
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer ou modifier une condition personnalisée pour les projets, les tâches et les problèmes en fonction des besoins de votre entreprise.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 15%

---

# Création ou modification d’une condition personnalisée

En tant qu’administrateur Adobe Workfront, vous pouvez créer ou modifier une condition personnalisée pour les projets, les tâches et les problèmes en fonction des besoins de votre entreprise.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td>Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Création ou modification d’une condition personnalisée

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet** > **Conditions**.

1. Cliquez sur l’onglet du type d’objet (**Projet**, **Tâche** ou **Problème**) que vous souhaitez associer à la condition.

1. Pour créer une condition, cliquez sur **Ajouter une nouvelle condition**.

   Ou

   Pour modifier une condition existante, survolez la condition à modifier, puis cliquez sur l’icône **Modifier** qui s’affiche à l’extrême droite.

   ![](assets/custom-condition-edit-nwe.jpg)

1. Configurez votre condition personnalisée à l’aide des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nom de la condition</td> 
      <td>(Obligatoire) Saisissez un nom explicite pour la condition.</td> 
     </tr> 
     <tr> 
      <td>Description</td> 
      <td>(Facultatif) Saisissez une description de l’objectif de la condition pour les utilisateurs.</td> 
     </tr> 
     <tr> 
      <td>Couleur</td> 
      <td>(Facultatif) Cliquez sur l’icône de couleur, puis sélectionnez la couleur de votre choix pour la condition lorsqu’elle s’affiche dans des projets, des tâches ou des problèmes. Vous pouvez également saisir un nombre hexadécimal.</td> 
     </tr> 
     <tr> 
      <td>Équivaut à </td> 
      <td><p>(Obligatoire, pour les projets uniquement) Cliquez sur l’option de la liste déroulante qui décrit le mieux la fonction de votre nouvelle condition. Par exemple, pour une condition nommée Tracking Well, cliquez sur On Target. Cela détermine le fonctionnement de vos conditions par défaut. Chaque condition que vous créez doit correspondre à l’une des options du menu déroulant.</p>
      <p>Pour plus d’informations sur les conditions par défaut, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Définition d’une condition personnalisée comme condition par défaut pour les projets</a> et <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Définition d’une condition personnalisée comme condition par défaut pour les tâches et les problèmes</a>.</p>
      <p>Cette option ne peut pas être modifiée une fois la création de la condition terminée.</p></td> 
     </tr> 
     <tr> 
      <td>Clé</td> 
      <td><p>(Obligatoire) Pour une condition de projet, saisissez une abréviation alphanumérique que les utilisateurs pourront identifier. Pour une tâche ou une condition de problème, saisissez un code numérique à deux chiffres compris entre 01 et 99. </p>
      <p>Cette clé, qui est utilisée dans l’API et qui peut être utilisée à des fins de création de rapports, doit être unique pour chaque objet.</p>
      <p>Vous ne pouvez pas modifier la clé d’une condition après avoir enregistré la condition. </p></td> 
     </tr> 
     <tr> 
      <td>Masquer le statut</td> 
      <td><p>(Facultatif) Cette option est disponible pour les conditions personnalisées que vous ne souhaitez plus que les personnes utilisent, mais que vous souhaitez conserver pour des raisons historiques. </p>
      <p>Si vous masquez une condition personnalisée qui a été utilisée sur des éléments de travail, elle continue de s’afficher sur ces éléments de travail une fois que vous l’avez masquée. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Vous pouvez normaliser la terminologie et les couleurs des conditions dans les trois types d’objets. Pour ce faire, copiez le nom de la condition et le code hexadécimal de couleur d’un onglet (Projet, Tâche, Problème) dans la condition correspondante sur les deux autres onglets.

1. (Facultatif) Faites glisser ![](assets/move-icon---dots.png) toute condition vers une nouvelle position pour réorganiser la liste.

   Cela modifie l’ordre dans lequel les conditions s’affichent dans les projets, tâches et problèmes :

   * Lorsqu’un utilisateur modifie un projet

     ![](assets/change-condition-edit-project.png)

   * Lorsqu’un utilisateur modifie la condition d’une tâche ou d’un problème dans l’onglet Mises à jour :

     ![](assets/change-condition-update-comment.png)

   * Lorsqu’un utilisateur modifie la condition d’une tâche ou d’un problème en mode Liste :

     ![](assets/change-conditions-list-dropdown-only.png)

1. Cliquer sur **Enregistrer**.

Vous pouvez définir votre condition personnalisée comme condition par défaut pour les projets ou pour les tâches et les problèmes. Pour plus d’informations, voir [Définition d’une condition personnalisée comme condition par défaut pour les projets](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) et [Définition d’une condition personnalisée comme condition par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Pour plus d’informations sur les conditions personnalisées, voir [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
