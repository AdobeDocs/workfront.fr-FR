---
product-area: projects
navigation-topic: create-tasks
title: Créer des tâches récurrentes
description: Vous pouvez créer des tâches récurrentes pour les tâches que vous devez répéter dans le cadre d’un seul projet.
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Créer des tâches récurrentes

Vous pouvez créer des tâches récurrentes pour les tâches que vous devez répéter dans le cadre d’un seul projet.

Pour obtenir des informations générales sur les tâches récurrentes, y compris l’impact de la modification d’une tâche récurrente existante, voir [Présentation des tâches récurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux tâches, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Accorder l’accès aux tâches</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuez des autorisations au projet avec la possibilité d’ajouter des tâches ou plus.</p> <p>Lorsque vous créez une tâche, vous recevez automatiquement les autorisations Gérer pour la tâche.</p> <p> Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Partage d’une tâche </a>. </p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créer une tâche récurrente

>[!NOTE]
>
>Vous ne pouvez pas créer une tâche récurrente en modifiant une tâche existante. Vous devez créer une tâche à partir de zéro.

1. Accédez au projet dans lequel vous souhaitez créer une tâche récurrente, puis cliquez sur le bouton **Tâches** dans le panneau de gauche.
1. Cliquez sur **Nouvelle tâche**.

   La boîte de dialogue Nouvelle tâche s’affiche.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Cliquez sur **Plus d’options** puis saisissez un nom pour la tâche dans la **Nom de la tâche** champ .
1. Continuez à mettre la tâche à jour comme vous le feriez si vous ajoutiez une nouvelle tâche. Pour plus d’informations sur l’ajout d’une nouvelle tâche, voir [Création de tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)
1. Cliquez sur **Présentation** dans le panneau de gauche.
1. Faites défiler l’écran vers le bas jusqu’à **Planning de périodicité** , puis sélectionnez l’option **En faire une tâche récurrente** .

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. Dans le **Fréquence** dans la liste déroulante, sélectionnez le nombre d’unités de temps au moment où vous souhaitez que la tâche se produise et le type d’unités de temps. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type de récurrence</th> 
      <th>Description</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Jour</strong> </td> 
      <td> <p>La tâche se répète tous les jours, tous les 2 jours, tous les 3 jours, etc., selon le rythme que vous choisissez. Vous pouvez configurer des tâches à répéter tous les 6 jours au maximum. Le paramètre par défaut est 1 jour. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Jour de travail</strong> </td> 
      <td> <p> La tâche se répète tous les jours ouvrés, tous les 2 jours ouvrés, tous les 3 jours ouvrés, etc., selon la cadence que vous sélectionnez. Vous pouvez configurer des tâches à répéter tous les 6 jours ouvrés au maximum.</p> <p>Cette option utilise le planning par défaut défini par l’administrateur système, comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Création d’un planning</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Semaine</strong> </td> 
      <td> <p> La tâche se répète chaque semaine, toutes les 2 semaines, toutes les 3 semaines, etc., selon le rythme que vous sélectionnez.</p> <p>Dans le <strong>Répéter</strong> , sélectionnez le jour de la semaine où vous souhaitez que chaque tâche se produise. Vous pouvez sélectionner plusieurs jours. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mois</strong> </td> 
      <td> <p>La tâche se répète tous les mois, tous les 2 mois, tous les 3 mois, etc, selon la cadence que vous sélectionnez. Vous pouvez sélectionner entre 1 et 12 mois. </p> <p>Dans le <strong>Répéter</strong> , sélectionnez l’une des options suivantes lorsque vous souhaitez que la tâche se produise :</p> 
       <ul> 
        <li> <p><strong>tous les mois, jour &lt;month date=""&gt;</strong> </p> <p>Vous pouvez choisir entre 1 et 30 jours ou sélectionner <strong>last</strong>. Par exemple, vous pouvez sélectionner "tous les mois le 30". </p> </li> 
        <li> <p><strong>chaque mois sur la &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>Dans le premier menu déroulant, vous pouvez sélectionner un nombre compris entre 1 et 4 pour le numéro de la semaine du mois ou sélectionner "dernier". </p> <p>Dans le deuxième menu déroulant, vous pouvez sélectionner n’importe quel jour de la semaine. </p> <p>Par exemple, vous pouvez sélectionner "tous les mois le 2e mardi". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Si une exception de planification est associée au planning du projet, les tâches récurrentes ne peuvent pas démarrer pendant l’exception. Les tâches récurrentes qui se produisent pendant l’exception de planification sont planifiées pour commencer le premier jour ouvré suivant l’exception. Pour plus d’informations sur les exceptions de planification, consultez l’article . [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. Dans le **Démarrages** , sélectionnez la date et l’heure de début des tâches récurrentes.
1. Dans le **Fin** , sélectionnez la date et l’heure auxquelles les tâches récurrentes doivent être terminées.

   Ou

   Sélectionner **after `<number>` occurrences** pour indiquer le nombre de fois où la tâche récurrente doit se produire. Workfront crée le même nombre de répétitions pour les tâches que le nombre indiqué dans ce champ.

1. Cliquez sur **Créer une tâche.**

   La liste des tâches s’affiche. La tâche récurrente est créée en tant que parent et toutes les récurrences sont ses enfants. Workfront a généré automatiquement les noms des tâches enfants, à l’aide du nom que vous avez saisi pour le parent, suivi d’un numéro. Pour plus d’informations sur les champs remplis automatiquement à partir de la tâche récurrente parent, voir [Présentation des tâches récurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Facultatif) Modifiez chaque tâche récurrente comme vous le feriez pour toute autre tâche du projet.

   Par exemple, vous pouvez ajouter des affectations, des prédécesseurs, des durées et modifier toute autre information concernant la tâche, y compris les champs personnalisés.

   >[!IMPORTANT]
   >
   >La modification de la périodicité parente après modification individuelle des enfants peut entraîner des informations différentes entre les enfants ou entre les enfants et le parent. Pour plus d’informations, voir [Présentation des tâches récurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
