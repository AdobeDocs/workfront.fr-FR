---
product-area: projects
navigation-topic: use-predecessors
title: Appliquer les tâches antérieures
description: Les tâches antérieures sont des tâches dont dépend l’achèvement d’autres tâches. Les relations d’antériorité affectent les dates de début et d’achèvement des tâches et donc la chronologie du projet.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 97%

---

# Appliquer les tâches antérieures

<!-- Audited: 2/2024 -->

Les tâches antérieures sont des tâches dont dépend l’achèvement d’autres tâches. Les relations d’antériorité affectent les dates de début et d’achèvement des tâches et donc la chronologie du projet.

Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

En définissant des relations d’antériorité entre les tâches, vous définissez comment le début ou la fin d’une tâche dépendante dépend du début ou de la fin de ses tâches antérieures. Pour ce faire, utilisez différents types de dépendances.

Pour plus d’informations sur les types de dépendances, voir [Vue d’ensemble des types de dépendances de tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Vue d’ensemble des tâches antérieures appliquées

>[!IMPORTANT]
>
>Vous devez appliquer des tâches antérieures afin d’exiger que des relations d’antériorité soient respectées. Si vous n’appliquez pas de tâches antérieures, les tâches dépendantes peuvent commencer et se terminer indépendamment du début et de la fin de leurs tâches antérieures, quels que soient leurs types de dépendances.

Vous pouvez appliquer une relation d’antériorité lors de la définition des tâches antérieures sur un projet.

Si une tâche antérieure est appliquée, la tâche ultérieure ne peut pas commencer tant que la tâche antérieure n’est pas terminée. Par exemple, l’application d’une relation Terminer-Démarrer entre la tâche A et la tâche B signifie que la tâche B ne peut pas commencer (le statut doit rester Nouveau et le pourcentage terminé doit rester à 0 %) tant que la tâche A n’est pas marquée comme terminée. L’application des relations s’applique à tous les types de tâches antérieures.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
      <p>Nouvelle : standard</p> 
      <p>OU</p>
      <p>Actuelle : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès en modification aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Autorisations de gestion sur les tâches et le projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Appliquer une tâche antérieure au niveau de la tâche

1. Accédez à la tâche ultérieure à laquelle vous souhaitez appliquer une tâche antérieure.
1. Cliquez sur **Tâches antérieures** dans le panneau de gauche, puis sur **Ajouter antérieur**. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Tâches antérieures**.
1. (Conditionnel) Si vous souhaitez ajouter une tâche antérieure interprojets, supprimez le nom du projet dans le champ **Projet parent** et remplacez-le par un autre projet.
1. Spécifiez le nom de la ou des tâches antérieures dans le champ **Tâche**.
1. Spécifiez le **Type de dépendance** entre ces deux tâches.

   Par défaut, le **Type de dépendance** est **Terminer-Démarrer**.

1. Sélectionnez le champ **Forcé** pour appliquer la tâche antérieure.
1. Cliquer sur **Enregistrer**.

## Appliquer une tâche antérieure d’une liste de tâches

1. Accédez à une liste des tâches sur un projet.
1. Dans le menu déroulant **Afficher**, sélectionnez la **Vue standard**.

1. Gardez en mémoire le nombre de tâches que vous allez désigner comme tâche antérieure.
1. Recherchez la tâche ultérieure à laquelle vous souhaitez appliquer la tâche antérieure.
1. Dans la colonne **Tâches antérieures**, commencez à saisir le numéro de la tâche antérieure suivi de « e ». Par exemple, saisissez « 1e » pour ajouter la tâche numéro 1 en tant que tâche antérieure à la tâche sélectionnée.
1. Cliquez sur Entrée pour enregistrer les informations de votre tâche antérieure pour la tâche.

   ![predecessor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
