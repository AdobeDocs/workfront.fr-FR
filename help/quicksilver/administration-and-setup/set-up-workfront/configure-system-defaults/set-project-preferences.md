---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configuration des préférences du projet à l’échelle du système
description: En tant qu'administrateur  [!DNL Adobe Workfront] , vous pouvez configurer les préférences par défaut pour tous les projets créés dans tout le système. Ces préférences ont un impact sur le projet, la tâche et le comportement du problème.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '2561'
ht-degree: 4%

---

# Configuration des préférences de projet à l’échelle du système

<!--Audited: 12/2023-->

En tant qu&#39;administrateur [!DNL Adobe Workfront], vous pouvez configurer les préférences par défaut pour tous les projets créés dans l&#39;ensemble du système. Ces préférences ont un impact sur le projet, la tâche et le comportement du problème.

>[!NOTE]
>
>Par défaut, ces préférences sont verrouillées et les administrateurs de groupe ne peuvent pas les modifier au niveau du groupe, sauf si vous les déverrouillez pour tous les groupes du système. Pour plus d’informations, voir [Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan</p></td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>[!UICONTROL Administrateur système]</p> <p><b>NOTE</b> :</p><p>Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configuration des préférences de projet pour l’ensemble de l’entreprise

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets]**.

1. Sur la page **Préférences du projet**, passez à l’une des 4 sections répertoriées ci-dessous pour configurer les préférences pour [!UICONTROL État du projet], [!UICONTROL Chronologies], [!UICONTROL Analyses de cas] et [!UICONTROL Durée de vie après la mort].
1. Si vous souhaitez que tous les groupes de l’organisation utilisent les mêmes préférences de projet, assurez-vous que chaque préférence est verrouillée ![](assets/lock-toggle-button.png) (il s’agit de la valeur par défaut).

   >[!IMPORTANT]
   >
   >Lorsqu’une préférence de projet est verrouillée, toutes les modifications que vous apportez à cette préférence sont héritées par tous les groupes du système. Il est important de communiquer avec les utilisateurs et les groupes de votre organisation pour vous assurer que tous les besoins sont pris en compte dans la configuration des préférences du projet.

   Pour plus d’informations sur le déverrouillage d’une préférence afin que tous les groupes puissent la configurer et la gérer eux-mêmes, voir [Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

* [[!UICONTROL État du projet]](#project-status)
* [[!UICONTROL Chronologies]](#timelines)
* [[!UICONTROL Analyses de cas]](#business-cases)
* [[!UICONTROL Durée de vie après la mort]](#life-after-death)

### Statut de projet {#project-status}

Configurez l’une des préférences suivantes pour les projets nouvellement créés dans tout le système :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autoriser les utilisateurs à créer des projets sans utiliser de modèle]</td> 
   <td>  <p>Cette préférence permet aux utilisateurs de créer des projets sans utiliser de modèle lors de la création d’un projet à partir des zones suivantes : </p>
      <ul>
        <li>
        <p>Utiliser l’option [!UICONTROL Nouveau projet] dans une liste de projets</p>
        </li>
          <li>
          <p>Convertir un problème en projet à partir de la page du problème</p>
          </li>
         </ul>
        <p>Cette préférence est activée par défaut. </p> 
        <p><b>NOTE</b></p>
        <p> Un administrateur de groupe peut modifier cette préférence pour un groupe. Lorsqu’un utilisateur appartient à plusieurs groupes avec des préférences différentes, il peut créer un projet sans modèle si cette préférence est activée pour son groupe d’accueil.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Définir l’état du nouveau projet sur]</td> 
   <td> <p>Déterminez l’état des nouveaux projets.</p>  <p><b>NOTE</b>  
     <ul> 
      <li>Si vous ou un autre administrateur [!DNL Workfront] masque l’état sélectionné ici, l’état par défaut passe au premier état de la liste des états.</li> 
     </ul> 
     <ul> 
      <li> <p>Si un état de groupe ou système verrouillé est défini comme état par défaut et qu’une personne le déverrouille par la suite, le système tente de le remplacer par un état verrouillé du même type.</p> <p>S’il n’en trouve pas, il recherche un statut requis :</p> 
       <ul> 
        <li>Si un état obligatoire correspond à l’état par défaut déverrouillé, l’état requis devient l’état par défaut, même s’il est déverrouillé.</li> 
        <li>Si aucun des états requis n’équivaut à l’état par défaut déverrouillé, le premier état requis dans la liste des états devient l’état par défaut.</li> 
       </ul> <p>Pour plus d’informations sur les états requis, voir les articles <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des états du projet système</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des états des tâches système</a> et <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des états des problèmes système</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculer le pourcentage terminé en fonction de]</td> 
   <td> <p>Workfront calcule le pourcentage d’achèvement d’un projet ou d’une tâche mère à l’aide du pourcentage d’achèvement de chaque tâche du projet et soit de la durée, soit des heures planifiées de chaque tâche.</p><p>Le pourcentage d’achèvement de chaque tâche est défini manuellement par les personnes désignées.</p><p>Vous pouvez choisir ici si Workfront utilisera la Durée ou les Heures planifiées des tâches pour calculer le pourcentage de réalisation des projets.</p> <p>Si vous sélectionnez [!UICONTROL Durée], la Durée de chaque tâche d’un projet détermine le pourcentage global terminé pour le projet, et la Durée de chaque sous-tâche détermine le pourcentage global terminé pour sa tâche parent.</p> <p>Si vous sélectionnez [!UICONTROL Durée], veillez à spécifier les heures [!UICONTROL Typical hours per work day] et les jours de travail standard par semaine dans la section [!UICONTROL Timelines]. [!DNL Workfront] utilise ces informations lors du calcul du pourcentage de réalisation d’une tâche en fonction de la durée. </p> <p>Si vous sélectionnez [!UICONTROL Heures planifiées], assurez-vous que toutes les tâches de chaque projet ont la quantité d’[!UICONTROL Heures planifiées] définie et que le montant n’est pas nul.</p><p>Pour plus d’informations, voir <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Présentation du pourcentage de projet terminé</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Définir automatiquement la condition du projet en fonction de l’état de progression]</td> 
   <td> <p>Cette préférence permet aux utilisateurs de définir manuellement la [!UICONTROL Condition] d’un projet sur ([!UICONTROL Sur Target], [!UICONTROL À risque], [!UICONTROL À problème]) ou de définir [!DNL Workfront] la [!UICONTROL Condition] (État de progression) automatiquement en fonction de la progression du projet dans la chronologie. Pour plus d’informations sur la condition des projets, voir <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Présentation de la condition et du type de condition du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Créer des lignes de base automatiquement]</p> </td> 
   <td> <p>Cette préférence crée automatiquement une ligne de base (instantané) des détails de la tâche et du projet lorsque l’état du projet passe à [!UICONTROL Actuel]. Pour plus d’informations sur la création de lignes de base, voir <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Création de lignes de base de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Méthode d’index de performance] </p> </td> 
   <td> <p>La méthode d’index de performance (PIM) du projet contrôle la méthode [!DNL Workfront] utilisée pour calculer les mesures de valeur acquise telles que [!UICONTROL Cost Performance Index] (IPC) et [!UICONTROL Estimate At Completion] (EAC). Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcul de l’index de performance des coûts UICONTROL] (IPC)</a> et <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculer l’estimation à l’achèvement] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong> : [!DNL Workfront] utilise [!UICONTROL Hours planifiés] pour calculer des mesures de performances telles que le taux de rafraîchissement de la dette (EAC) et l’IPC. Lorsque le PIM est calculé en fonction des heures, le CAE s’affiche sous la forme d’un nombre d’heures. Assurez-vous que vous disposez d’une valeur pour [!UICONTROL Heures planifiées] autre que zéro.</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong> : [!DNL Workfront] utilise [!UICONTROL Scheduler Labor Cost] pour calculer des mesures de performances telles que EAC et IPC. Assurez-vous que vos rôles de tâche ou utilisateurs sont associés aux taux de coût par heure. Lorsque le PIM est calculé en fonction des coûts, le contrôle qualité s’affiche sous la forme d’une valeur monétaire.</p> <p>Le chef de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone [!UICONTROL Finance] dans [!UICONTROL Détails du projet]. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gérer les informations dans la zone du projet [!UICONTROL Finance]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimation à l’achèvement ]</p> </td> 
   <td> <p>Déterminez quelles données [!DNL Workfront] utilisent pour calculer l’[!UICONTROL Estimation à la fin] (EAC) qui représente le coût total prévu d’un projet.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcul au niveau du projet]</strong> : les champs de contrôle d’accès de la tâche et du projet parents sont déterminés en saisissant [!UICONTROL Heures réelles] ou [!UICONTROL Coût réel de la main-d’oeuvre] dans les formules du contrôle d’accès. Ce calcul comprend les éléments [!UICONTROL Heures réelles] ou [!UICONTROL Coûts et dépenses] ajoutés directement à la tâche ou au projet parent.</li> 
     <li> <p><strong>[!UICONTROL Cumul à partir de tâches/sous-tâches]</strong> : les champs d’évaluation cumulés de la tâche parent et du projet sont déterminés en additionnant les champs d’évaluation cumulés de chaque tâche enfant. Ce calcul exclut les [!UICONTROL Heures réelles] ou les [!UICONTROL Coûts et dépenses réels] ajoutés directement à la tâche ou au projet parent.</p> <p>Le chef de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone [!UICONTROL Finance] dans [!UICONTROL Détails du projet]. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestion des informations dans la zone [!UICONTROL Finance] du projet </a>.</p> </li> 
    </ul> <p>Pour plus d’informations sur la façon dont le CAE calcule, voir <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcul de l’[!UICONTROL Estimation à l’achèvement] (CAE)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Chronologies {#timelines}

Configurez l’une des préférences suivantes pour les projets nouvellement créés dans tout le système :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planification À Partir De]</td> 
   <td> <p>Déterminez si les nouveaux projets sont planifiés à partir de la date de début ou de la date de fin au moment de leur création.</p> 
    <ul> 
     <li><strong>[!UICONTROL Date de début]</strong> : les nouvelles tâches sont définies par défaut sur [!UICONTROL Dès que possible]. La contrainte de tâche et les gestionnaires de projet sont invités à fournir une [!UICONTROL Date de début planifiée] pour le projet.</li> 
     <li><strong>[!UICONTROL Date d’achèvement]</strong> : les nouvelles tâches prennent par défaut la valeur [!UICONTROL Dès que possible]. La contrainte de tâche et les gestionnaires de projet sont invités à fournir une [!UICONTROL Date d’achèvement planifiée] pour le projet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Déterminez si le délai de désactivation du cessionnaire Principal d’une tâche ajuste les dates prévues pour cette tâche sur un projet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Envisager le temps de pause de l’utilisateur pendant les durées de la tâche]</strong> : tout temps de pause planifié pour le responsable de Principal d’une tâche ajuste les dates prévues de la tâche si le temps de pause survient pendant la durée de la tâche. Il s’agit du paramètre par défaut. </p> <p>Par exemple, si une tâche avec une contrainte de [!UICONTROL Dès que possible] est planifiée pour commencer le 1er juin et se terminer le 3 juin, et que la personne désignée par le Principal a marqué le 2 juin pour le délai de fin, les dates prévues de la tâche s’ajustent du 1er au 4 juin.</p> <p><b>IMPORTANT</b> :</p> <p>La durée de la tâche n’est pas modifiée lorsque vous sélectionnez ce paramètre. Seules les dates planifiées changent, en fonction de la contrainte de tâche.</p> </li> 
     <li><strong>[!UICONTROL Ignorer le temps de pause de l’utilisateur pendant les durées de la tâche]</strong> : les dates planifiées de chaque tâche sur un projet restent telles que prévues initialement, même si le cessionnaire Principal d’une tâche a un temps de pause pendant sa durée.</li> 
    </ul> <p>Tenez compte des éléments suivants lorsque vous sélectionnez l’une des options disponibles pour ce paramètre :</p> 
    <ul> 
     <li>Lorsque vous modifiez ce paramètre, seuls les projets et les modèles créés après la modification héritent du paramètre mis à jour. </li> 
     <li> <p>La valeur Task Constraint de la tâche détermine les dates de tâche planifiées à ajuster : </p> 
      <ul> 
       <li>Date de début planifiée</li> 
       <li>Date d'achèvement prévue</li> 
       <li>Les deux dates</li> 
       <li>Ni l'une ni l'autre. </li> 
      </ul> <p>Par exemple, si une tâche présente une contrainte de [!UICONTROL Dates fixes], les dates ne s’ajustent pas lorsque le cessionnaire Principal a un délai d’expiration, même si l’option [!UICONTROL Envisager le temps d’arrêt de l’utilisateur dans la durée de la tâche] est sélectionnée. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Présentation de la contrainte de tâche</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Les chronologies de projet sont automatiquement recalculées]</p> </td> 
   <td> <p>Déterminez quand la chronologie d’un projet est recalculée. Pour plus d’informations sur le recalculage de la chronologie du projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer la chronologie du projet</a>.</p> <p>Les options suivantes sont activées par défaut. Vous pouvez sélectionner un ou plusieurs des paramètres suivants :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Chaque nuit]</strong> : sélectionnez cette option pour recalculer les calendriers du projet toutes les nuits. Les modifications que vous apportez au projet susceptibles d’affecter la chronologie ne sont pas immédiatement visibles. [!DNL Workfront​​​] recalcule les chronologies la nuit uniquement pour les projets pour lesquels les deux conditions suivantes sont remplies :</p> <p> 
       <ul> 
        <li>ont l’état [!UICONTROL Actuel] ;</li> 
        <li>ont eu une mise à jour au cours des 3 derniers mois ;</li> 
        <li>possèdent un type de mise à jour de l’une des valeurs suivantes :</li>
        <ul>
        <li>Automatique et en cas de modification</li>
        <li>Modification uniquement</li>
        <li>Automatique uniquement</li> 
      </ul>       
    <b>TIP:</b>
    <p>Les projets dont le type de mise à jour est Manuel uniquement ne sont pas affectés par ce paramètre.</p>
    <li> <p><strong>Lorsque la portée d’un projet change</strong> : sélectionnez cette option pour recalculer immédiatement les chronologies du projet au fur et à mesure que la portée du projet change. Pour plus d’informations sur ce qui constitue un changement de portée de projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les chronologies de projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Lorsque plusieurs utilisateurs sont affectés à une tâche, utilisez le planning de]</p> </td> 
   <td> <p>Si un planning n'est pas affecté à un projet ou si aucun planning n'est affecté aux utilisateurs affectés à ses tâches, [!DNL Workfront] utilise le planning par défaut du système pour calculer la chronologie des tâches.</p> <p>Si vous affectez plusieurs utilisateurs à la même tâche dans un projet et que le projet comporte un planning affecté et que les utilisateurs affectés aux tâches disposent également d’un planning, [!UICONTROL Workfront] utilise les plannings suivants :</p> 
    <ul> 
     <li><strong>[!UICONTROL Attribution de Principal]</strong> : [!DNL Workfront] utilise le planning de l’attribution de Principal sur la tâche pour calculer les chronologies.</li> 
     <li><strong>[!UICONTROL Project]</strong> : [!DNL Workfront] utilise la planification du projet pour calculer la chronologie de chaque tâche.</li> 
    </ul> <p>Pour plus d’informations sur les plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Création d’un planning</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Calculs chronologiques] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Horaires types par jour de travail]</strong> : définissez le nombre d’heures par jour de travail standard pour les utilisateurs qui travailleront sur des projets. La valeur par défaut est de 8 heures.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Jours de travail standard par semaine]</strong> : définissez la semaine de travail standard pour les utilisateurs qui travaillent sur des projets. La valeur par défaut est de 5 jours.</li> 
    </ul> <p>Ces 2 options convertissent les jours en heures ou les semaines en jours.</p> <p>Par exemple, si vous avez une tâche avec 8 heures planifiées et que la durée est calculée en fonction des heures planifiées, [!DNL Workfront] convertit ces heures en jours afin d’afficher la durée en jours.</p> <p>À partir du champ [!UICONTROL jours de travail par semaine] standard, [!DNL Workfront] calcule la valeur de l’équivalent à temps complet (FTE) pour votre système. C’est ce que [!DNL Workfront] utilise lors du calcul des allocations pour les utilisateurs.</p> <p>Ces valeurs sont utilisées lorsque vous planifiez les calendriers des projets, la planification des ressources ou la journalisation du temps par rapport aux projets. </p> <p>Elles ne sont pas utilisées lorsque vous définissez des feuilles de temps pour les utilisateurs du système, comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configurer] timesheet and hour preferences</a>.</p> <p><b>NOTE</b> :</p> <p>[!DNL Workfront] Les administrateurs ne peuvent pas déverrouiller les préférences [!UICONTROL Calculs chronologiques] .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestres personnalisés]</p> </td> 
   <td> <p>Configurez des trimestres annuels personnalisés pour les utilisateurs qui vont travailler sur des projets. Les trimestres personnalisés sont généralement des trimestres qui ne correspondent pas à la répartition traditionnelle des trimestres au cours d'une année civile. Vous pouvez ajouter plusieurs quartiers personnalisés. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Activation des trimestres personnalisés pour les projets</a>.</p>  <p><b>NOTE</b> : </p><p>[!DNL Workfront] Les administrateurs ne peuvent pas déverrouiller les préférences [!UICONTROL Trimestres personnalisés].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Analyses de cas] {#business-cases}

Vous pouvez créer un Business Case pour les projets nouvellement créés dans tout le système afin d’envoyer des demandes de projet. Vous pouvez définir des préférences pour déterminer les zones visibles sur le formulaire **[!UICONTROL Business Case]**. Nous vous recommandons d’activer ces options afin que d’autres outils, tels que [!UICONTROL Portfolio Optimizer], soient correctement mis à jour. Pour plus d&#39;informations sur l&#39;affichage de chaque champ, voir [Définition d&#39;un cas d&#39;affaire : index d&#39;article](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Une fois que l’administrateur [!DNL Workfront] a activé les sections sur l’ [!UICONTROL analyse de cas ], un propriétaire de projet peut créer une analyse de cas au niveau du projet. Pour plus d’informations sur la création d’un cas d’entreprise, voir [Création d’un cas d’entreprise pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Durée de vie après la mort] {#life-after-death}

Configurez l’une des préférences suivantes pour les projets nouvellement créés dans tout le système :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Une fois qu’un projet a été marqué comme terminé, les personnes peuvent toujours le faire] </p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) pour déterminer si une tâche ou un problème peut être supprimé une fois que l’état du projet a été marqué [!UICONTROL Terminé].</p> 
    <ul> 
     <li><strong>[!UICONTROL Supprimer les tâches]</strong> : permet aux utilisateurs de supprimer des tâches d’un projet une fois le projet marqué [!UICONTROL Terminé].<br></li> 
     <li><strong>[!UICONTROL Problèmes de suppression]</strong> : permet aux utilisateurs de supprimer des problèmes d’un projet une fois le projet marqué [!UICONTROL Terminé].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Une fois qu’un projet est marqué comme terminé, mort ou en attente d’approbation, les personnes peuvent toujours le faire]</p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) concernant les tâches, problèmes, documents et autres objets dans un projet une fois que l’état du projet a été marqué <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Mort]</strong> ou est <strong>[!UICONTROL En attente d’approbation]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Ajouter et modifier des tâches]</strong> Permet aux utilisateurs de :
      <ul>
       <li>Modifiez les tâches d’un projet une fois que le projet a été marqué [!UICONTROL Terminé], [!UICONTROL Mort] ou est [!UICONTROL En attente d’approbation]. Cela inclut l’ajout d’heures et la modification des entrées de dépenses sur une tâche.</li>
       <li>Ajoutez des tâches à un projet.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Ajouter et modifier des problèmes]</strong> : permet aux utilisateurs de :
      <ul>
       <li>Modifiez les problèmes d’un projet une fois que le projet a été marqué comme [!UICONTROL terminé], [!UICONTROL mort] ou [!UICONTROL En attente d’approbation].</li>
       <li>Ajoutez des problèmes à un projet une fois que le projet a été marqué [!UICONTROL Terminé] ou [!UICONTROL Mort]. (Vous ne pouvez pas ajouter de problèmes à un projet qui est [!UICONTROL Autorisation en attente].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Ajouter des documents au projet et à ses tâches et problèmes]</strong> : permet aux utilisateurs d’ajouter des documents à un projet (ou d’ajouter des documents à des tâches et à des problèmes dans le projet) une fois le projet marqué [!UICONTROL Terminé] ou [!UICONTROL Mort].</p> <p>Cette option ne s’applique pas aux projets en attente de validation.</p> </li> 
     <li> <p><strong>[!UICONTROL Joindre des modèles]</strong> : permet aux utilisateurs de joindre des modèles à un projet une fois le projet marqué [!UICONTROL Terminé] ou [!UICONTROL Mort].</p> <p>Cette option ne s’applique pas aux projets en attente de validation.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
