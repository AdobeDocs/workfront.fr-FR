---
product-area: projects
navigation-topic: use-predecessors
title: Appliquer les tâches antérieures
description: Les prédécesseurs sont des tâches sur lesquelles d’autres tâches dépendent pour être terminées. Les relations du prédécesseur affectent les dates de début et de fin des tâches et, en fin de compte, affectent la chronologie du projet.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 9%

---

# Appliquer les tâches antérieures

<!-- Audited: 2/2024 -->

Les prédécesseurs sont des tâches sur lesquelles d’autres tâches dépendent pour être terminées. Les relations du prédécesseur affectent les dates de début et de fin des tâches et, en fin de compte, affectent la chronologie du projet.

Pour plus d’informations sur les prédécesseurs, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

En définissant les relations de prédécesseur entre les tâches, vous définissez comment le début ou la fin d’une tâche dépendante dépend du début ou de la fin de ses tâches de prédécesseur. Pour ce faire, utilisez différents types de dépendance.

Pour plus d’informations sur les types de dépendance, voir [Présentation des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Présentation des prédécesseurs appliqués

>[!IMPORTANT]
>
>Vous devez imposer aux prédécesseurs d&#39;exiger que les relations de prédécesseur soient respectées. Sans appliquer les prédécesseurs, les tâches dépendantes peuvent commencer et se terminer indépendamment du début et de la fin de leurs prédécesseurs, quels que soient leurs types de dépendances.

Vous pouvez appliquer la relation de prédécesseur lors de la définition des prédécesseurs sur un projet.

Si un prédécesseur est appliqué, la tâche qui lui succède ne peut pas commencer avant l’achèvement du prédécesseur. Par exemple, l’application d’une relation Finish-Start entre la tâche A et la tâche B signifie que la tâche B ne peut pas démarrer (l’état doit rester Nouveau et le pourcentage terminé doit rester 0 %) jusqu’à ce que la tâche A soit marquée comme terminée. L’application des relations s’applique à tous les types de prédécesseur.

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
      <p>Nouveau : Standard</p> 
      <p>OU</p>
      <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Gérer les autorisations pour les tâches et le projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Application d’un prédécesseur au niveau de la tâche

1. Accédez à la tâche qui lui succède et dont vous souhaitez appliquer le prédécesseur.
1. Cliquez sur **Prédécesseurs** dans le panneau de gauche, puis cliquez sur **Ajouter un prédécesseur**. Vous devrez peut-être cliquer sur **Afficher plus**, puis **Prédécesseurs**.
1. (Conditionnel) Si vous souhaitez ajouter un prédécesseur de plusieurs projets, supprimez le nom du projet dans la variable **Projet parent** et remplacez-le par un autre projet.
1. Indiquez le nom de la ou des tâches du prédécesseur dans la fonction **Tâche** champ .
1. Spécifiez la variable **Type de dépendance** entre ces deux tâches.

   Par défaut **Type de dépendance** is **Finish-Start**.

1. Sélectionnez la variable **Enchaîné** pour appliquer le prédécesseur.
1. Cliquer sur **Enregistrer**.

## Application d’un prédécesseur à une liste de tâches

1. Accédez à une liste de tâches sur un projet.
1. Dans la **Affichage** , sélectionnez la variable **Vue standard**.

1. Notez mentalement le nombre de tâches que vous allez désigner comme prédécesseur.
1. Recherchez la tâche de remplacement dont vous souhaitez appliquer le prédécesseur.
1. Dans le **Prédécesseurs** , commencez à saisir le numéro de la tâche précédente suivie de &quot;e&quot;. Par exemple, saisissez &quot;1e&quot; pour ajouter la tâche numéro 1 en tant que prédécesseur à la tâche sélectionnée.
1. Cliquez sur Entrée pour enregistrer les informations de votre prédécesseur pour la tâche.

   ![prédécesseur_forced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
