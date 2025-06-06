---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation d’antériorité à l’aide de la zone Tâches antérieures
description: Vous pouvez utiliser des tâches antérieures (ou simplement des prédécesseurs) pour lier des tâches qui dépendent d'autres tâches à démarrer ou à terminer.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 59%

---

# Créer une relation d’antériorité à l’aide de la zone Tâches antérieures

<!-- Audited: 5/2025 -->

Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne voudriez pas héberger une partie (tâche dépendante) avant d&#39;envoyer les invitations (tâche antérieure).

Cet article montre comment vous pouvez définir des tâches antérieures à l’aide de l’onglet Tâches antérieures dans une tâche.

Pour plus d’informations sur la définition de tâches antérieures dans une liste de tâches, voir [Créer une relation d’antériorité dans la liste des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Vous pouvez afficher les tâches antérieures de tâches dans les zones suivantes d’Adobe Workfront :

* Dans la section Tâches antérieures des tâches dépendantes
* Dans le graphique de Gantt.
* Dans la liste des tâches, dans la colonne Tâches antérieures

Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Nouveau : Standard </p>
   <p>Ou </p>
   <p>Actuel : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une tâche antérieure pour une tâche

1. Accédez à la tâche que vous souhaitez désigner comme tâche dépendante.

1. Dans le panneau de gauche, cliquez sur **Prédécesseurs**.

1. Dans la section **Prédécesseurs**, cliquez sur **+Ajouter le prédécesseur**. La boîte de dialogue **Ajouter un prédécesseur** s’ouvre.

1. (Facultatif) Pour ajouter un projet transversal antérieur, remplacez le nom du projet dans le champ **Projet parent** par un autre projet.

   Pour plus d’informations, voir [Création de projets transversaux antérieurs](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Dans le champ **Tâches**, saisissez le nom de la ou des tâches que vous souhaitez désigner comme prédécesseurs, puis sélectionnez-les lorsqu’elles s’affichent dans la liste déroulante.

1. Sélectionnez un **Type de dépendance**.

   Pour plus d&#39;informations, voir [Présentation des types de dépendance de tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Saisissez un montant **Décalage**.

   &#x200B; Pour plus d’informations, voir Présentation [ types décalage](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Boîte de dialogue Ajouter le prédécesseur](assets/add-predecessor-dialog-box.png)

1. Cochez la case **Appliquée** si vous souhaitez appliquer la relation de prédécesseur entre les deux tâches.

   Pour plus d’informations, voir [Appliquer les prédécesseurs](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Cliquer sur **Enregistrer**.
