---
product-area: agile-and-teams
navigation-topic: iterations
title: Créer une itération
description: Les itérations sont un élément clé pour les équipes agiles de Scrum dans la planification de la capacité de travail. [!DNL Adobe Workfront]  permet aux équipes agiles de Scrum de gérer leur travail en créant plusieurs itérations pour répondre aux besoins de l’équipe.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 3%

---

# Créer une itération

Les itérations sont un élément clé pour les équipes agiles de Scrum dans la planification de la capacité de travail. [!DNL Adobe Workfront] permet aux équipes agiles de Scrum de gérer leur travail en créant plusieurs itérations pour répondre aux besoins de l’équipe.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur [!DNL Workfront].

## Ajouter une itération

Utilisez la fonction [!UICONTROL Ajouter une itération] pour créer rapidement une itération et ajouter ultérieurement des tâches et des problèmes.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Equipes]**.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sur l’onglet **[!UICONTROL Itérations]**, cliquez sur **[!UICONTROL Ajouter une itération]**.\
   ![](assets/add-iteration-adobe-350x275.png)

1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Saisissez le nom de l’itération.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Goal]</strong></td> 
      <td>Ajoutez les objectifs dont vous disposez pour l’itération.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Date de début]</strong></td> 
      <td>Saisissez la date de début de l’itération.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Date de fin]</strong></td> 
      <td><p>Saisissez la date de fin de l’itération. [!DNL Workfront] recommande de définir une date de fin ne dépassant pas 4 semaines à compter de la date de début.</p><p>Conseil : Veillez à choisir un jour de travail comme date de fin. Le graphique de charge utilise uniquement les jours de travail dans ses calculs.<br>Par défaut, le graphique de ventilation utilise la planification par défaut pour définir les jours de travail (comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Créer un planning</a>). Ou, pour incorporer des jours non ouvrés spécifiques à l’équipe, les équipes agiles peuvent choisir d’utiliser un autre planning (comme décrit dans "Définition d’un autre planning d’équipe pour les graphiques de Burndown" dans <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Créer une équipe agile</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Spécifiez la capacité d’itération. Il s’agit du nombre de points ou d’heures que votre équipe est en mesure d’accomplir dans l’itération. Le nombre saisi doit être égal ou supérieur au nombre de points ou d’heures à partir de la somme de tous les articles de l’itération.<br>[!DNL Workfront] préremplit ce champ de 50 capacité par défaut. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Définissez le pourcentage de focus de l’équipe. Si tous les membres de l’équipe se concentrent entièrement sur cette itération, l’accent sera mis à 100 %.<br>[!DNL Workfront] préremplit ce champ de 100 % par défaut. </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Submit]**. Maintenant que vous avez créé une itération, vous devez ajouter des histoires. Pour plus d’informations, voir [Ajout d’articles à une itération existante](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planifiez une itération sur l’onglet [!UICONTROL Backlog]

Utilisez la fonction [!UICONTROL  Plan Iteration] pour créer une itération à l’aide des tâches de votre journal de bord.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Equipes]**.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez **[!UICONTROL Backlog]** dans le panneau de gauche. Cliquez ensuite sur **[!UICONTROL Plan Iteration]**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Spécifiez un nom pour l’itération.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Date de début]</strong></td> 
      <td> Indiquez la date de début de l’itération.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Date de fin]</strong> </td> 
      <td><p>Indiquez la date de fin de l’itération. [!DNL Workfront] recommande de définir une date de fin ne dépassant pas 4 semaines à compter de la date de début.</p><p>Conseil : Veillez à choisir un jour de travail comme date de fin. Le graphique de charge utilise uniquement les jours de travail dans ses calculs.<br>Par défaut, le graphique de ventilation utilise la planification par défaut pour définir les jours de travail (comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Créer un planning</a>). Ou, pour incorporer des jours non ouvrés spécifiques à l’équipe, les équipes agiles peuvent choisir d’utiliser un autre planning (comme décrit dans la section <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Utiliser un autre planning d’équipe pour les graphiques de condensation</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Définissez le pourcentage de focus de l’équipe. Si tous les membres de l’équipe se concentrent entièrement sur cette itération, l’accent sera mis à 100 %.<br>[!DNL Workfront] préremplit ce champ avec la valeur moyenne des itérations passées de votre équipe. S’il s’agit de la première itération de votre équipe, la valeur de ce champ est 0 par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Spécifiez la capacité d’itération. Il s’agit du nombre de points ou d’heures que votre équipe est en mesure d’accomplir dans l’itération. Le nombre saisi doit être égal ou supérieur au nombre de points ou d’heures à partir de la somme de tous les articles de l’itération.<br>[!DNL Workfront] préremplit ce champ avec la valeur moyenne des itérations passées de votre équipe. S’il s’agit de la première itération de votre équipe, la valeur de ce champ est 0 par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> Spécifiez un objectif pour l’itération. Ce champ n’est pas obligatoire.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Sélectionnez des articles à ajouter à l’itération maintenant ou ignorez cette étape et ajoutez des articles à une itération ultérieurement. Les histoires qui se trouvent en haut du journal sont prioritaires. Les histoires sont surlignées en vert lorsqu’elles correspondent à la capacité ; elles sont surlignées en rouge si elles ne le sont pas.\
   Vous pouvez ajouter des tâches et des problèmes à une seule itération :

   * **Pour ajouter des tâches à l’itération :** Sur l’onglet **[!UICONTROL Backlog]**, assurez-vous que l’onglet **[!UICONTROL Stories]** est sélectionné (cet onglet est sélectionné par défaut lors de l’affichage du backlog). Sélectionnez les articles à ajouter à l’itération.\

     Lorsque vous ajoutez des tâches à une itération, la date de début de la tâche est calculée comme décrit dans la section [[!UICONTROL Comprendre] comment les dates de début de la tâche sont calculées lorsqu&#39;elles sont ajoutées à une itération](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Pour ajouter des problèmes à l’itération :** Dans l’onglet **[!UICONTROL Backlog]**, cliquez sur l’onglet **[!UICONTROL Problèmes]**. Sélectionnez les problèmes que vous souhaitez ajouter à l’itération.

1. Cliquer sur **[!UICONTROL Enregistrer].**
L’itération est créée.

1. (Facultatif) Pour ajouter des articles à une itération existante, voir [Ajout d’articles à une itération existante](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Comprendre comment les dates de début de tâche sont calculées lorsqu’elles sont ajoutées à une itération {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Lorsque vous ajoutez une tâche en tant qu’article à une itération, la contrainte [!UICONTROL Must Finish On task] est utilisée pour chaque article. Dans la plupart des cas, la date de début prévue de la tâche est calculée selon la formule suivante :

[!UICONTROL Date de fin de l’itération] moins (-) [!UICONTROL Durée de la tâche] égale (=) [!UICONTROL Date de début planifiée de la tâche]

La [!UICONTROL date de fin du projet] est utilisée à la place de   si la date de début du projet est postérieure à la date de début de l’itération et que la date de fin du projet est postérieure à la date de fin de l’itération.

Vous pouvez configurer des équipes Scrum individuelles pour utiliser les dates du projet par défaut plutôt que les dates d’itération. Pour plus d’informations, reportez-vous à la section [Configuration de la manière dont les dates sont appliquées lors de l’ajout d’éléments de travail à une itération](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans l’article [Configurer le graphique](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
