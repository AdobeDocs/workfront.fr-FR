---
product-area: projects
navigation-topic: use-predecessors
title: Création de prédécesseurs sur plusieurs projets
description: Un prédécesseur multi-projets est une tâche dont dépend une autre tâche (appelée tâche de remplacement) dans un autre projet. Le prédécesseur est la tâche qui a la priorité sur la tâche dépendante (qui lui succède). Par exemple, vous pouvez créer une dépendance qui nécessite que la tâche du prédécesseur soit marquée comme Terminée avant que la tâche dépendante puisse commencer.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Création de prédécesseurs sur plusieurs projets

<!--Audited: 12/2023-->

Un prédécesseur multi-projet est une tâche dont dépend une autre tâche (appelée tâche de remplacement) dans un autre projet. Le prédécesseur est la tâche qui a la priorité sur la tâche dépendante (qui lui succède). Par exemple, vous pouvez créer une dépendance qui nécessite que la tâche du prédécesseur soit marquée comme Terminée avant que la tâche dépendante puisse commencer.

Adobe Workfront permet aux tâches de dépendre des tâches d’autres projets, tout comme il permet aux prédécesseurs d’un seul projet.

>[!INFO]
>
>Par exemple, une entreprise d’excavation n’a qu’une seule arrière-plan et deux projets ont des tâches qui nécessitent l’utilisation de la arrière-plan. Le chef de projet peut faire de la tâche du premier projet un prédécesseur de la tâche du deuxième projet. Cela montre que le deuxième projet peut commencer à utiliser la rétrospective lorsque le premier projet est terminé.

Lors de la liaison de projets par le biais de prédécesseurs interprojets, les dates du projet principal (celui qui a la tâche précédente) auront un impact sur le projet secondaire (celui qui a la tâche qui lui succède).

>[!TIP]
>
>Vous devez recalculer les chronologies pour les projets afin d’afficher les dates mises à jour pour le projet secondaire. Pour plus d’informations sur le nouveau calcul des chronologies, voir [Configuration de nouveaux calculs de chronologie pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Pour plus d’informations sur les relations de prédécesseur, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Exigences d’accès

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
 <tr> 
  <td role="rowheader">Licence Adobe Workfront*</td> 
  <td> <p>Nouveau : Standard </p>
 <p>ou</p> 
<p>Actuel : formule </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour les tâches et les projets</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’un prédécesseur multi-projet

1. Accédez à la tâche qui sera votre successeur (tâche dépendante).
1. Cliquez sur **Prédécesseurs** dans le panneau de gauche.
1. Cliquez sur **Ajoutez le prédécesseur.**
1. Dans le **Projet parent** , commencez à saisir le nom du projet qui contient la tâche que vous souhaitez remplacer par la tâche en cours.
1. Cliquez sur le nom qui apparaît dans la liste déroulante.
1. Dans le **Tâche** , commencez à saisir le nom de la tâche que vous souhaitez remplacer par la tâche en cours.
1. Indiquez les informations suivantes pour définir la relation entre le prédécesseur et la tâche dépendante :

   * **Type de dépendance :** Sélectionnez la relation que vous souhaitez que la tâche de prédécesseur ait avec la tâche dépendante. La relation par défaut est &quot;Finish-Start&quot;, ce qui signifie que la tâche du prédécesseur doit se terminer avant que la tâche dépendante puisse commencer. Pour plus d’informations sur les différents types de dépendances, voir [Présentation des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Indicateur :** Spécifiez le temps qui doit s’écouler après la fin d’un prédécesseur appliqué jusqu’à ce que la tâche dépendante puisse commencer. Pour plus d’informations sur les différents types de retard, voir [Types de balises - Aperçu](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Application :** Lorsque cette option est sélectionnée, la relation de dépendance entre les deux tâches ne peut pas être contournée par les utilisateurs qui commencent les tâches tôt. Par exemple, si vous appliquez une relation entre la tâche A et la tâche B, la tâche B ne peut pas être lancée tant que la tâche A n’est pas terminée. Pour plus d’informations sur l’application des prédécesseurs, voir [Application des prédécesseurs](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Lorsque cette option n’est pas sélectionnée, la dépendance est traitée comme une suggestion aux utilisateurs. Par exemple, les utilisateurs peuvent démarrer la tâche B avant que la tâche A ne soit terminée.

1. Cliquer sur **Enregistrer**.

   Les tâches qui ont un prédécesseur multi-projet affichent le numéro de référence du projet auquel appartient le prédécesseur et le numéro de la tâche, séparé par un deux-points, dans la colonne Prédécesseurs d’une liste de tâches.

   ![prédécesseur multi-projet](assets/cross-project-predecessor-in-list-view.png)

   L’icône du prédécesseur devient verte lorsque la tâche du prédécesseur est marquée comme terminée. Cela indique que la tâche dépendante est prête pour le travail.

   Passez la souris sur cette valeur pour obtenir plus d’informations sur le prédécesseur, le projet et les dates. Cliquez sur le prédécesseur de plusieurs projets dans la zone Détails pour ouvrir la tâche.

   Cliquez sur près de la partie supérieure de la fenêtre de survol pour afficher plus d’informations sur le projet du prédécesseur.

   Cliquez sur **Voir Projet** pour ouvrir le projet du prédécesseur.

   ![Détails des prédécesseurs sur plusieurs projets](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   La variable **Voir Projet** s’affiche uniquement lors de l’affichage d’un prédécesseur multi-projet.

