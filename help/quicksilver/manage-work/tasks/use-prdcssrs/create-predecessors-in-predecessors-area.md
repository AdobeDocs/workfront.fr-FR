---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation d’antériorité à l’aide de la zone Tâches antérieures
description: Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne souhaiteriez pas organiser une fête (tâche dépendante) avant d’avoir envoyé les invitations (tâche antérieure).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 100%

---

# Créer une relation d’antériorité à l’aide de la zone Tâches antérieures

Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne souhaiteriez pas organiser une fête (tâche dépendante) avant d’avoir envoyé les invitations (tâche antérieure).

Cet article montre comment vous pouvez définir des tâches antérieures à l’aide de l’onglet Tâches antérieures dans une tâche.

Pour plus d’informations sur la définition de tâches antérieures dans une liste de tâches, voir [Créer une relation d’antériorité dans la liste des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Vous pouvez afficher les tâches antérieures de tâches dans les zones suivantes d’Adobe Workfront :

* Dans la section Tâches antérieures des tâches dépendantes
* Dans le graphique de Gantt.
* Dans la liste des tâches, dans la colonne Tâches antérieures

Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Créer une tâche antérieure pour une tâche

1. Accédez à la tâche que vous souhaitez désigner comme tâche dépendante, puis cliquez sur **Tâches antérieures** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Tâches antérieures**.

1. Cliquez sur **+Ajouter antérieur**.
1. (Facultatif) Pour ajouter projet transversal antérieur, remplacez le nom du projet dans le champ **Projet parent** par un autre projet, puis saisissez le nom de la ou des tâches que vous souhaitez définir comme tâches antérieures.

   Pour plus d’informations sur l’ajout de projets transversaux antérieurs, voir [Créer des projets transversaux antérieurs](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Saisissez le nom de la ou des tâches que vous souhaitez désigner comme tâches antérieures.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Sélectionnez un **Type de dépendance**.

   Pour plus d’informations sur les types de dépendances de tâches, voir [Vue d’ensemble des types de dépendances de tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Spécifiez une durée de **Décalage** en jours.

   Pour plus d’informations sur les types de décalage, voir [Vue d’ensemble des types de décalage](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Sélectionnez **Forcé** si vous souhaitez appliquer la relation d’antériorité entre les deux tâches.

   Pour plus d’informations la manière de forcer des tâches antérieures, voir [Forcer les tâches antérieures](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Cliquer sur **Enregistrer**.
