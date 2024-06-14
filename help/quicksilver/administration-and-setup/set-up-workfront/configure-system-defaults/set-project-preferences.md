---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configuration des préférences de projet à l’échelle du système
description: Comme [!DNL Adobe Workfront] admin, vous pouvez configurer les préférences par défaut pour tous les projets créés dans l’ensemble du système. Ces préférences ont un impact sur le projet, la tâche et le comportement du problème.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '2524'
ht-degree: 1%

---

# Configuration des préférences de projet à l’échelle du système

<!--Audited: 12/2023-->

Comme [!DNL Adobe Workfront] admin, vous pouvez configurer les préférences par défaut pour tous les projets créés dans l’ensemble du système. Ces préférences ont un impact sur le projet, la tâche et le comportement du problème.

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
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>Nouveau : [!UICONTROL Standard]</p>
   Ou
   <p>Actuel : formule [!UICONTROL]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>[!UICONTROL Administrateur système]</p> <p><b>REMARQUE</b>:</p><p>Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configuration des préférences de projet pour l’ensemble de l’entreprise

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets]**.

1. Sur le **Préférences du projet** , continuez avec l’une des 4 sections répertoriées ci-dessous pour configurer les préférences de [!UICONTROL État du projet], [!UICONTROL Chronologies], [!UICONTROL Analyses de cas], et [!UICONTROL La vie après la mort].
1. Si vous souhaitez que tous les groupes de l’organisation utilisent les mêmes préférences de projet, assurez-vous que chaque préférence est verrouillée. ![](assets/lock-toggle-button.png) (il s’agit de la valeur par défaut).

   >[!IMPORTANT]
   >
   >Lorsqu’une préférence de projet est verrouillée, toutes les modifications que vous apportez à cette préférence sont héritées par tous les groupes du système. Il est important de communiquer avec les utilisateurs et les groupes de votre organisation pour vous assurer que tous les besoins sont pris en compte dans la configuration des préférences du projet.

   Pour plus d’informations sur le déverrouillage d’une préférence afin que tous les groupes puissent la configurer et la gérer eux-mêmes, voir [Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

* [[!UICONTROL État du projet]](#project-status)
* [[!UICONTROL Chronologies]](#timelines)
* [[!UICONTROL Analyses de cas]](#business-cases)
* [[!UICONTROL La vie après la mort]](#life-after-death)

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
   <td> <p>Déterminez l’état des nouveaux projets.</p>  <p><b>REMARQUE</b>  
     <ul> 
      <li>Si vous ou un autre [!DNL Workfront] L’administrateur masque l’état sélectionné ici. l’état par défaut passe au premier état dans la liste des états.</li> 
     </ul> 
     <ul> 
      <li> <p>Si un état de groupe ou système verrouillé est défini comme état par défaut et qu’une personne le déverrouille par la suite, le système tente de le remplacer par un état verrouillé du même type.</p> <p>S’il n’en trouve pas, il recherche un statut requis :</p> 
       <ul> 
        <li>Si un état obligatoire correspond à l’état par défaut déverrouillé, l’état requis devient l’état par défaut, même s’il est déverrouillé.</li> 
        <li>Si aucun des états requis n’équivaut à l’état par défaut déverrouillé, le premier état requis dans la liste des états devient l’état par défaut.</li> 
       </ul> <p>Pour plus d’informations sur les états requis, voir les articles <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des états des projets système</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des états des tâches système</a>, et <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des problèmes système</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculer le pourcentage terminé en fonction de]</td> 
   <td> <p>Le pourcentage d’achèvement d’un projet ou d’une tâche parente repose sur l’état d’avancement global des tâches. Ces informations peuvent être calculées en fonction de la Durée ou des Heures planifiées des tâches d’un projet.</p> <p>Si vous sélectionnez [!UICONTROL Durée], la Durée de chaque tâche d’un projet détermine le pourcentage global terminé pour le projet, et la Durée de chaque sous-tâche détermine le pourcentage global terminé pour sa tâche parent.</p> <p>Si vous sélectionnez [!UICONTROL Durée], veillez à spécifier les heures [!UICONTROL Typical hours per work day] et les jours de travail standard par semaine dans la section [!UICONTROL Timelines]. [!DNL Workfront] utilise ces informations lors du calcul du pourcentage de réalisation d’une tâche en fonction de la durée. </p> <p>Si vous sélectionnez [!UICONTROL Heures planifiées], assurez-vous que toutes les tâches de chaque projet ont la quantité d’[!UICONTROL Heures planifiées] définie et que le montant n’est pas nul.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Définir automatiquement la condition du projet en fonction de l’état de progression]</td> 
   <td> <p>Cette préférence permet aux utilisateurs de définir manuellement la [!UICONTROL Condition] d’un projet sur ([!UICONTROL Sur Target], [!UICONTROL À risque], [!UICONTROL À risque] ou d’avoir la variable [!DNL Workfront] définissez la [!UICONTROL Condition] (État de progression) automatiquement en fonction de la progression du projet dans la chronologie. Pour plus d’informations sur la condition des projets, voir <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Présentation de la condition et du type de condition du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Créer des lignes de base automatiquement]</p> </td> 
   <td> <p>Cette préférence crée automatiquement une ligne de base (instantané) des détails de la tâche et du projet lorsque l’état du projet passe à [!UICONTROL Actuel]. Pour plus d’informations sur la création de lignes de base, voir <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Création de lignes de base de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Méthode d’index de performance] </p> </td> 
   <td> <p>La méthode d’index de performance (PIM) du projet contrôle la méthode . [!DNL Workfront] utilise pour calculer les mesures de valeur obtenue, telles que [!UICONTROL Cost Performance Index] (IPC) et [!UICONTROL Estimate At Completion] (EAC). Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcul de l’[!UICONTROL indice de performance des coûts] (IPC)</a> et <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculer L’Estimation À L’Achèvement] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Basé sur l’heure]</strong>: [!DNL Workfront] utilise [!UICONTROL Heures planifiées] pour calculer des mesures de performances telles que le contrôle de l’accès et l’indice des prix à la consommation. Lorsque le PIM est calculé en fonction des heures, le CAE s’affiche sous la forme d’un nombre d’heures. Assurez-vous que vous disposez d’une valeur pour [!UICONTROL Heures planifiées] autre que zéro.</li> 
     <li> <p><strong>[!UICONTROL Basé sur les coûts]</strong>: [!DNL Workfront] utilise [!UICONTROL Coût planifié de la main-d’oeuvre] pour calculer des mesures de performances telles que le taux de sinistralité et l’indice des prix à la consommation. Assurez-vous que vos rôles de tâche ou utilisateurs sont associés aux taux de coût par heure. Lorsque le PIM est calculé en fonction des coûts, le contrôle qualité s’affiche sous la forme d’une valeur monétaire.</p> <p>Le chef de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone [!UICONTROL Finance] dans [!UICONTROL Détails du projet]. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestion des informations dans la zone du projet [!UICONTROL Finance]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimation à l’achèvement ]</p> </td> 
   <td> <p>Déterminer quelles données [!DNL Workfront] utilise pour calculer l’[!UICONTROL estimation à la fin] (EAC) qui représente le coût total prévu d’un projet.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcul au niveau du projet]</strong>: le champ EAC de la tâche et du projet parents est déterminé en saisissant [!UICONTROL Heures réelles] ou [!UICONTROL Coût réel de la main-d’oeuvre] dans les formules EAC. Ce calcul comprend les éléments [!UICONTROL Heures réelles] ou [!UICONTROL Coûts et dépenses] ajoutés directement à la tâche ou au projet parent.</li> 
     <li> <p><strong>[!UICONTROL Cumul à partir de tâches/sous-tâches]</strong>: les champs de contrôle d’accès de la tâche parent et du projet sont déterminés en additionnant les champs de contrôle d’accès de chaque tâche enfant. Ce calcul exclut les [!UICONTROL Heures réelles] ou les [!UICONTROL Coûts et dépenses réels] ajoutés directement à la tâche ou au projet parent.</p> <p>Le chef de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone [!UICONTROL Finance] dans [!UICONTROL Détails du projet]. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestion des informations dans la zone du projet [!UICONTROL Finance]</a>.</p> </li> 
    </ul> <p>Pour plus d’informations sur le mode de calcul du CAE, voir <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculer [!UICONTROL Estimer À L’Achèvement] (EAC)</a>.</p> </td> 
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
     <li><strong>[!UICONTROL Date de début]</strong>: les nouvelles tâches sont définies par défaut sur [!UICONTROL Dès que possible]. La contrainte de tâche et les chefs de projet sont invités à fournir une [!UICONTROL Date de début planifiée] pour le projet.</li> 
     <li><strong>[!UICONTROL Date d’achèvement]</strong>: les nouvelles tâches sont définies par défaut sur [!UICONTROL Autant que possible]. La contrainte de tâche et les gestionnaires de projet sont invités à fournir une [!UICONTROL Date d’achèvement planifiée] pour le projet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Déterminez si le délai de désactivation du cessionnaire Principal d’une tâche ajuste les dates prévues pour cette tâche sur un projet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Envisager le temps de pause de l’utilisateur dans les durées de tâche]</strong>: tout temps de congé planifié pour le cessionnaire Principal d’une tâche ajuste les dates planifiées de la tâche si le temps de congé survient pendant la durée de la tâche. Il s’agit du paramètre par défaut. </p> <p>Par exemple, si une tâche avec une contrainte de [!UICONTROL Dès que possible] est planifiée pour commencer le 1er juin et se terminer le 3 juin, et que la personne désignée par le Principal a marqué le 2 juin pour le délai de fin, les dates prévues de la tâche s’ajustent du 1er au 4 juin.</p> <p><b>IMPORTANT</b>:</p> <p>La Durée de la tâche ne change pas lorsque vous sélectionnez ce paramètre. Seules les dates planifiées changent, en fonction de la contrainte de tâche.</p> </li> 
     <li><strong>[!UICONTROL Ignorer le temps de pause de l’utilisateur pendant les tâches]</strong>: les dates prévues de chaque tâche sur un projet restent comme initialement prévues, même si le cessionnaire Principal d’une tâche a un délai d’expiration pendant sa durée.</li> 
    </ul> <p>Tenez compte des points suivants lors de la sélection des options de ce paramètre :</p> 
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
   <td> <p>Déterminez quand la chronologie d’un projet est recalculée. Pour plus d’informations sur le nouveau calcul de la chronologie du projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les calendriers du projet</a>.</p> <p>Les options suivantes sont activées par défaut. Vous pouvez sélectionner un ou plusieurs des paramètres suivants :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Chaque nuit]</strong>: sélectionnez cette option pour recalculer les chronologies de projet toutes les nuits. Les modifications que vous apportez au projet susceptibles d’affecter la chronologie ne sont pas immédiatement visibles. [!DNL Workfront​​​] recalcule les chronologies la nuit uniquement pour les projets pour lesquels les deux conditions suivantes sont remplies :</p> <p> 
       <ul> 
        <li>ont l’état [!UICONTROL Actuel] ;</li> 
        <li>ont eu une mise à jour au cours des 3 derniers mois ;</li> 
        <li>possèdent un type de mise à jour de l’une des valeurs suivantes :</li>
        <ul>
        <li>Automatique et en cas de modification</li>
        <li>Modification uniquement</li>
        <li>Automatique uniquement</li> 
      </ul>       
    <b>CONSEIL :</b>
    <p>Les projets dont le type de mise à jour est Manuel uniquement ne sont pas affectés par ce paramètre.</p>
    <li> <p><strong>Lorsque la portée d’un projet change</strong>: sélectionnez cette option pour recalculer immédiatement les échéances du projet en cas de changement de portée du projet. Pour plus d’informations sur ce qui constitue un changement de portée d’un projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les calendriers du projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Lorsque plusieurs utilisateurs sont affectés à une tâche, utilisez le planning de]</p> </td> 
   <td> <p>Si un planning n’est pas affecté à un projet ou si un planning n’est pas affecté aux utilisateurs affectés à ses tâches, [!DNL Workfront] utilise la planification par défaut du système pour calculer la chronologie des tâches.</p> <p>Si vous affectez plusieurs utilisateurs à la même tâche dans un projet et que le projet comporte un planning affecté et que les utilisateurs affectés aux tâches disposent également d’un planning, [!UICONTROL Workfront] utilise les plannings suivants :</p> 
    <ul> 
     <li><strong>[!UICONTROL Attribution de Principal]</strong>: [!DNL Workfront] utilise le planning de l’affectation de Principal sur la tâche pour calculer les chronologies.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] utilise le planning du projet pour calculer la chronologie de chaque tâche.</li> 
    </ul> <p>Pour plus d’informations sur les plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Création d’un planning</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Calculs chronologiques] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Heures types par jour de travail]</strong>: définissez le nombre d’heures par jour de travail standard pour les utilisateurs qui travailleront sur des projets. La valeur par défaut est de 8 heures.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Jours de travail standard par semaine]</strong>: définissez la semaine de travail standard pour les utilisateurs qui travaillent sur des projets. La valeur par défaut est de 5 jours.</li> 
    </ul> <p>Ces 2 options convertissent les jours en heures ou les semaines en jours.</p> <p>Par exemple, si vous avez une tâche avec 8 heures planifiées et que la durée est calculée en fonction des heures planifiées, [!DNL Workfront] convertit ces heures en jours afin d’afficher la durée en jours.</p> <p>Dans le champ [!UICONTROL jours ouvrables par semaine] , [!DNL Workfront] calcule la valeur de l’équivalent à temps complet (FTE) de votre système. C'est ce qui [!DNL Workfront] utilise lors du calcul des allocations pour les utilisateurs.</p> <p>Ces valeurs sont utilisées lorsque vous planifiez les calendriers des projets, la planification des ressources ou la journalisation du temps par rapport aux projets. </p> <p>Elles ne sont pas utilisées lorsque vous définissez des feuilles de temps pour les utilisateurs du système, comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configuration des préférences de feuille de temps et d’heure dans [!UICONTROL]</a>.</p> <p><b>REMARQUE</b>:</p> <p>[!DNL Workfront] Les administrateurs ne peuvent pas déverrouiller les préférences [!UICONTROL Calculs chronologiques] .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestres personnalisés]</p> </td> 
   <td> <p>Configurez des trimestres annuels personnalisés pour les utilisateurs qui vont travailler sur des projets. Les trimestres personnalisés sont généralement des trimestres qui ne correspondent pas à la répartition traditionnelle des trimestres au cours d'une année civile. Vous pouvez ajouter plusieurs quartiers personnalisés. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Activation des trimestres personnalisés pour les projets</a>.</p>  <p><b>REMARQUE</b>: </p><p>[!DNL Workfront] Les administrateurs ne peuvent pas déverrouiller les préférences [!UICONTROL Trimestres personnalisés].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Analyses de cas] {#business-cases}

Vous pouvez créer un Business Case pour les projets nouvellement créés dans tout le système afin d’envoyer des demandes de projet. Vous pouvez définir des préférences afin de déterminer les zones visibles sur le **[!UICONTROL Analyse de cas]** formulaire. Nous vous recommandons d’activer ces options afin que d’autres outils, tels que la fonction [!UICONTROL Portfolio Optimizer], mettez à jour correctement. Pour plus d’informations sur ce que chaque champ affiche, voir [Définition d’un cas d’entreprise : index des articles](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Après la [!DNL Workfront] l’administrateur active les sections de la variable [!UICONTROL Analyse de cas], un propriétaire de projet peut alors créer un cas d’entreprise au niveau du projet. Pour plus d’informations sur la création d’un cas d’entreprise, voir [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL La vie après la mort] {#life-after-death}

Configurez l’une des préférences suivantes pour les projets nouvellement créés dans tout le système :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Une fois qu’un projet a été marqué comme terminé, les personnes peuvent toujours le faire] </p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) pour déterminer si une tâche ou un problème peut être supprimé une fois que l’état du projet a été marqué [!UICONTROL Terminé].</p> 
    <ul> 
     <li><strong>[!UICONTROL Tâches De Suppression]</strong>: permet aux utilisateurs de supprimer des tâches d’un projet une fois le projet marqué [!UICONTROL Terminé].<br></li> 
     <li><strong>[!UICONTROL Problèmes de suppression]</strong>: permet aux utilisateurs de supprimer des problèmes d’un projet une fois le projet marqué [!UICONTROL terminé].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Une fois qu’un projet est marqué comme terminé, mort ou en attente d’approbation, les personnes peuvent toujours le faire]</p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) concernant les tâches, les problèmes, les documents et autres objets dans un projet une fois que l’état du projet a été marqué. <strong>[!UICONTROL Terminé]</strong>, <strong>[!UICONTROL Morts]</strong>, ou est <strong>[!UICONTROL Autorisation en attente]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Ajouter et modifier des tâches]</strong> Permet aux utilisateurs de :
      <ul>
       <li>Modifiez les tâches d’un projet une fois que le projet a été marqué [!UICONTROL Terminé], [!UICONTROL Mort] ou est [!UICONTROL En attente d’approbation]. Cela inclut l’ajout d’heures et la modification des entrées de dépenses sur une tâche.</li>
       <li>Ajoutez des tâches à un projet.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Ajouter et modifier des problèmes]</strong>: permet aux utilisateurs de :
      <ul>
       <li>Modifiez les problèmes d’un projet une fois que le projet a été marqué comme [!UICONTROL terminé], [!UICONTROL mort] ou [!UICONTROL En attente d’approbation].</li>
       <li>Ajoutez des problèmes à un projet une fois que le projet a été marqué [!UICONTROL Terminé] ou [!UICONTROL Mort]. (Vous ne pouvez pas ajouter de problèmes à un projet qui est [!UICONTROL Autorisation en attente].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Ajouter des documents au projet et à ses tâches et problèmes]</strong>: permet aux utilisateurs d’ajouter des documents à un projet (ou d’ajouter des documents à des tâches et à des problèmes au sein du projet) une fois le projet marqué [!UICONTROL Terminé] ou [!UICONTROL Mort].</p> <p>Cette option ne s’applique pas aux projets en attente de validation.</p> </li> 
     <li> <p><strong>[!UICONTROL Joindre des modèles]</strong>: permet aux utilisateurs de joindre des modèles à un projet une fois que le projet a été marqué [!UICONTROL Terminé] ou [!UICONTROL Mort].</p> <p>Cette option ne s’applique pas aux projets en attente de validation.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
