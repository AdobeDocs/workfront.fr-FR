---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation d’antériorité à l’aide de la zone Prédécesseurs
description: Vous pouvez utiliser les tâches précédentes (ou simplement les prédécesseurs) pour lier des tâches qui dépendent d’autres tâches à démarrer ou à terminer. Par exemple, vous ne souhaitez pas héberger une partie (tâche dépendante) avant d’envoyer les invitations (tâche prédécesseur).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 32%

---

# Créer une relation d’antériorité à l’aide de la zone Prédécesseurs

Vous pouvez utiliser les tâches précédentes (ou simplement les prédécesseurs) pour lier des tâches qui dépendent d’autres tâches à démarrer ou à terminer. Par exemple, vous ne souhaitez pas héberger une partie (tâche dépendante) avant d’envoyer les invitations (tâche prédécesseur).

Cet article explique comment définir les prédécesseurs à l’aide de l’onglet Prédécesseurs dans une tâche.

Pour plus d’informations sur la définition des prédécesseurs dans une liste de tâches, voir [Création d’une relation de prédécesseur sur la liste de tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Vous pouvez afficher les prédécesseurs des tâches dans les zones suivantes d’Adobe Workfront :

* Dans la section Prédécesseurs des tâches dépendantes
* Dans le diagramme de Gantt
* Dans la liste des tâches de la colonne Prédécesseurs

Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion sur les tâches et le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Création d’un prédécesseur pour une tâche

1. Accédez à une tâche que vous souhaitez désigner comme tâche dépendante, puis cliquez sur **Prédécesseurs** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Tâches antérieures**.

1. Cliquez sur **+Ajouter le prédécesseur**.
1. (Facultatif) Pour ajouter un prédécesseur de plusieurs projets, remplacez le nom du projet dans le champ **Projet parent** par un autre projet, puis saisissez le nom de la ou des tâches que vous souhaitez réaliser en tant que prédécesseurs.

   Pour plus d’informations sur l’ajout de prédécesseurs sur plusieurs projets, voir [Création de prédécesseurs sur plusieurs projets](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Saisissez le nom de la ou des tâches que vous souhaitez désigner comme prédécesseurs.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Sélectionnez un **Type de dépendance**.

   Pour plus d’informations sur les types de dépendance de tâche, voir [Présentation des types de dépendance de tâche](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Indiquez un nombre **Lag** en jours.

   Pour plus d’informations sur les types de balise, consultez la [présentation des types de balise](../../../manage-work/tasks/use-prdcssrs/lag-types.md) &#x200B;.

1. Sélectionnez **Enchaîné** si vous souhaitez appliquer la relation de prédécesseur entre les deux tâches.

   Pour plus d’informations sur l’application des prédécesseurs, voir [Application des prédécesseurs](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Cliquer sur **Enregistrer**.
