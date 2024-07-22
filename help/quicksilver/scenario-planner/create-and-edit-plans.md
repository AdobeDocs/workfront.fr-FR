---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Créer et modifier de plans dans le planificateur de scénarios
description: Vous pouvez créer des plans dans le cadre de l’utilisation du planificateur de scénario Workfront, lorsque vous définissez la priorité de la stratégie de niveau supérieur de votre entreprise. Pour plus d’informations sur les plans, voir Aperçu des plans dans le planificateur de scénario.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '2389'
ht-degree: 3%

---

# Créez et modifiez des plans dans le [!DNL Scenario Planner]

Vous pouvez créer des plans dans le cadre de l’utilisation de [!DNL Workfront Scenario Planner], lorsque vous définissez la priorité de la stratégie de niveau supérieur de votre entreprise. Pour plus d’informations sur les plans, consultez la [présentation des plans dans le  [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] forfait*</p> </td> 
   <td> <p>Actuel : [!UICONTROL Entreprise] ou version ultérieure</p>
   <p>Nouveau : Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td> <p>Nouveau : Léger ou supérieur</p> 
   <p>Actuel : [!UICONTROL Révision] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td>Produit* </td> 
   <td> 
   <p>Pour les plans Workfront actuels : </p>
   <p>Vous devez acheter une licence supplémentaire pour le [!DNL Adobe Workfront Scenario Planner] afin d’accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’accès et les autorisations pour [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser le [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Niveau d’accès </td> 
   <td> <p>Accès à l’accès à la fonction [!UICONTROL Modifier] [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demander l’accès à un plan dans le [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer ou modifier des plans

Vous pouvez créer entièrement un plan ou en modifier un existant qui a été partagé avec vous.

>[!NOTE]
>
>Après avoir créé un plan, vous êtes considéré comme le créateur et le propriétaire du plan. Lorsqu’un utilisateur est désactivé, le plan n’a pas de propriétaire et n’est visible par personne, sauf s’il a été partagé avec un lien.

Cet article décrit comment créer entièrement un plan ou modifier un plan existant.

Pour toutes les considérations sur les plans, y compris les informations disponibles pour un plan, consultez la [présentation des plans dans le  [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Pour plus d’informations sur la suppression de plans, voir [Suppression de plans dans la  [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Pour créer ou modifier un plan :

{{step1-to-scenario-planner}}

Une liste des plans existants que vous avez créés s&#39;affiche dans le [!DNL Workfront Scenario Planner].

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Filtre]** ![](assets/filter-icon-34x37.png) dans le coin supérieur droit de la liste des plans, puis sélectionnez l’une des options suivantes :

   | Filtre | Description |
   |---|---|
   | [!UICONTROL Tous] | Affiche tous les plans que vous avez créés ou qui ont été partagés avec vous. |
   | [!UICONTROL Mes plans] | Affiche les plans que vous avez créés. |
   | [!UICONTROL Partagé avec moi] | Affiche les plans partagés avec vous. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Facultatif) Cliquez sur l&#39;icône **[!UICONTROL Rechercher]** ![](assets/search-icon.png) pour saisir un mot-clé et localiser rapidement un plan dans la liste.

1. Cliquez sur le nom d&#39;un plan existant pour le modifier et passez à l&#39;étape 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   Ou

   Cliquez sur **[!UICONTROL Nouveau plan]** dans le coin supérieur gauche pour créer un plan et passez à l’étape 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   La zone [!UICONTROL New Plan] s’affiche.

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Conditionnel) Lorsque vous créez un plan, indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Saisissez le nom du plan. Il s’agit d’un champ obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Important : <span style="font-weight: normal;">Vous ne pouvez pas modifier les sélections suivantes après avoir créé et enregistré le plan.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span> FTE ([!UICONTROL équivalent temps plein]) ou [!UICONTROL Hours]</span> </td> 
      <td> <p><span>Sélectionnez l’une des options suivantes pour indiquer comment estimer les informations de rôle de tâche pour ce plan :</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>. Il s’agit de la valeur par défaut </span>. </p> 
      <p><b>IMPORTANT</b></p>  
      <p>Pour tous les calculs dans [!DNL Scenario Planner], [!DNL Workfront] utilise la valeur suivante : 1 ETR = 8 Heures. </p> </li> 
      <li> <p><strong>[!UICONTROL Hours]</strong> </p> </li> 
       </ul> <p><b>IMPORTANT</b></p>

   L’option que vous sélectionnez ici détermine l’affichage des informations sur les rôles de tâche pour le plan, les scénarios du plan et les initiatives.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Date de début]</td> 
      <td> <p>Sélectionnez le mois et l'année auxquels le plan doit commencer. Vous ne pouvez sélectionner que les mois dans ce champ. [!DNL Workfront] suppose que la date de début du forfait est le premier jour du mois sélectionné et que la date de fin est le dernier jour de fin du mois de sa durée. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duration]</td> 
      <td> <p>Dans le menu déroulant, sélectionnez l’une des durées suivantes :</p> 
       <ul> 
        <li>1 an. Il s’agit de la durée par défaut. </li> 
        <li>3 ans</li> 
        <li> <p>5 ans</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. (Conditionnel) Cliquez sur **[!UICONTROL Suivant]**.

   La chronologie du plan s’affiche comme le **[!UICONTROL scénario initial]**.

   Pour plus d’informations sur la création de scénarios supplémentaires, voir [Création et comparaison de scénarios de plan dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Facultatif) Dans le menu déroulant de la frise chronologique, sélectionnez l’une des options du tableau suivant pour modifier l’affichage de la frise chronologique du plan.

   ![](assets/month-dropdown-with-all-options.png)

   | Option de menu déroulant | Description |
   |---|---|
   | [!UICONTROL Mois] | Affiche la chronologie par mois. Il s’agit de la seule option par défaut pour un abonnement d’un an. |
   | [!UICONTROL Trimestre] | Affiche la chronologie par trimestre. Cette option est disponible uniquement lorsque la [!UICONTROL durée] du plan est de 3 ou 5 ans. Il s’agit de l’option par défaut pour un plan sur 3 ans. |
   | [!UICONTROL Year] | Affiche la chronologie par année. Cette option est disponible uniquement lorsque la [!UICONTROL durée] du plan est de 5 ans. Il s’agit de l’option par défaut pour un plan de 5 ans. |

1. (Facultatif) Faites défiler la page de gauche à droite pour afficher toute la durée du plan.
1. (Facultatif) Cliquez sur la ligne d’indicateur **[!UICONTROL Today]** pour revenir à la journée en cours.

   ![](assets/today-indicator-350x160.png)

1. Cliquez sur la zone **[!UICONTROL Rôles de tâche]** dans l’en-tête du plan pour ajouter des rôles de tâche qui seront disponibles pour exécuter le plan.

   Les détails de la zone [!UICONTROL Rôles de tâche] s’affichent.

   >[!TIP]
   >
   >L’unité d’attribution de rôles (ETR ou heures) utilisée par [!DNL Workfront] pour ce plan s’affiche entre parenthèses dans le titre de la boîte.

   ![](assets/adding-people-to-plan-350x206.png)

1. Cliquez sur le champ **[!UICONTROL Commencer à saisir le rôle de tâche]** et sélectionnez un rôle dans la liste ou commencez à saisir le nom d’un rôle de tâche actif.

   Tous les rôles de tâche actifs dans le système sont répertoriés lorsque vous cliquez sur ce champ.

   Le rôle de tâche est alors ajouté à la colonne Rôles de tâche .

1. Mettez à jour ou passez en revue les informations suivantes pour le rôle de tâche :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max disponible] (pour l’éditeur de texte enrichi) </p> <p role="rowheader">ou </p> <p role="rowheader"><span>[!UICONTROL Total disponible] (en heures)</span> </p> </td> 
      <td> <p><span>Selon que vous avez choisi d’utiliser des heures ou l’éditeur de texte enrichi pour votre plan, saisissez </span> le nombre d’heures ou d’heures de travail dans les champs suivants du rôle d’éditeur de texte enrichi <span>ou d’heures</span> disponibles pour exécuter le plan : </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total disponible]</strong> (en heures) : indique le nombre total d’heures pour tous les mois pendant la durée du scénario. Par défaut, [!DNL Workfront] divise uniformément le nombre total disponible sur tous les mois de la durée du scénario. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Si vous saisissez 1 200 heures pour un Designer, cela signifie que le Designer est disponible pendant 100 heures pour chaque mois pendant la durée du plan, lorsque la durée du plan [!UICONTROL] est de 1 an. </p> </li> 
        <li> <p><b>[!UICONTROL Max disponible]</b> (pour l’éditeur de texte enrichi) : indique le nombre d’éditeurs d’texte enrichi disponibles pour chaque mois pendant la durée du plan. Par défaut, <strong>Workfront</strong> attribue le nombre [!UICONTROL Max disponible] à chaque mois pendant la durée du scénario.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>si vous saisissez 1 ETR pour un consultant, cela signifie que le consultant est disponible pour 1 ETR pour chaque mois pendant la durée du plan. </p> <p>Vous pouvez saisir un nombre inférieur à 1 ETR. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Un rôle de consultant 0,5 signifie qu’un consultant consacrerait la moitié de son ETR (généralement, 4 heures, où 8 heures équivalent à 1 ETR) à travailler sur ce plan. Pour tous les calculs dans le planificateur de scénario, Workfront utilise la valeur suivante : 1 ETR = 8 Heures. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max requis] (pour l’éditeur de texte enrichi)</p> <p role="rowheader">ou </p> <p role="rowheader"><span>[!UICONTROL Total requis] (pour les heures)</span> </p> </td> 
      <td> <p><span>Selon que vous avez choisi d’utiliser des heures ou l’éditeur de texte enrichi pour votre plan, passez en revue </span> le nombre d’heures ou d’heures requises pour le rôle d’éditeur de texte enrichi <span> pour terminer les initiatives dans le scénario. </span> Vérifiez les champs suivants :</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total requis]</strong> (en heures) : nombre total d’heures requises pour tous les mois pendant la durée du plan.</p> </li> 
        <li> <p><strong>[!UICONTROL Max requis]</strong> (pour l’éditeur de texte enrichi) : nombre maximal d’éditeur de texte enrichi requis pour n’importe quel mois pendant la durée du plan. </p> </li> 
       </ul> <p>Conseil : Le nombre <span>maximum</span> d’ETR <span> ou le nombre total d’heures</span> requises pour ce rôle de tâche s’affiche une fois que vous avez commencé à ajouter des initiatives. Pour plus d’informations sur l’ajout d’initiatives à un plan, voir <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Créer et modifier des initiatives dans [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL Taux horaire]</td> 
      <td> <p>Il s’agit du taux d’[!UICONTROL Heure de coût] pour le rôle de tâche. Le taux horaire s’affiche dans la devise de votre système. Pour plus d’informations sur la configuration des taux d’Exchange pour votre système, voir <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configuration des taux d’exchange</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Passez la souris sur le nom d’un rôle de tâche ou cliquez sur l’onglet après avoir mis à jour les informations du rôle, puis cliquez sur l’icône **[!UICONTROL corbeille]** ![](assets/delete.png) pour le supprimer du plan.
1. Cliquez sur **[!UICONTROL Distribution de rôles de tâche]**.

   Le panneau de distribution des rôles de tâche s’affiche pour tous les mois de la durée du scénario.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Saisissez le nom d’un rôle de tâche à ajouter au plan dans le **[!UICONTROL champ Commencer à saisir le rôle de tâche]**, puis cliquez sur Entrée lorsqu’il apparaît dans la liste. Cela ajoute le rôle de tâche à la colonne [!UICONTROL Rôles de tâche].
1. Mettez à jour ou passez en revue les informations suivantes pour chaque mois du scénario :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Rôles de tâche] (ETR ou heures)</td> 
      <td>Le rôle de tâche disponible pour le scénario et ceux requis pour les initiatives du scénario s’affichent tous deux dans le panneau de distribution des rôles de tâche. Il existe une indication indiquant si les estimations de rôle de tâche se trouvent dans les ETR ou les heures dans l’en-tête de colonne. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disponible] (max &lt;nombre d’ETR&gt;) </p> 
       <div> 
        <p>ou</p> 
        <p>[!UICONTROL Disponible] (total &lt;nombre d’heures&gt;) </p> 
       </div> </td> 
      <td> <p><span>Selon que vous avez choisi d’utiliser des heures ou l’éditeur de texte enrichi pour votre plan, passez en revue ou mettez à jour</span> le nombre mensuel d’ETR (rôles de tâche) <span>ou d’heures</span> disponibles pour le scénario dans les champs suivants :</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Disponible] (max &lt;nombre d’ETR&gt;)</strong> : le nombre entre parenthèses affiche le nombre maximal de rôles disponibles pour l’un des mois du scénario. Vérifiez ou mettez à jour le nombre d’ETR pour chaque mois du scénario. La modification de l’allocation mensuelle peut mettre à jour le nombre d’ETR entre parenthèses. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Disponible] (total &lt;nombre d’heures&gt;)</strong> : le nombre entre parenthèses affiche le nombre total d’heures disponibles pour tous les mois du scénario. Vérifiez ou mettez à jour le nombre d’heures pour chaque mois du scénario. La modification de l'allocation mensuelle met à jour le nombre d'heures entre parenthèses.</span> </p> </li> 
       </ul> <p>La mise à jour manuelle des affectations mensuelles de rôles de tâche est une autre manière de résoudre les conflits de rôles entre les initiatives dans le scénario. </p> <p>Conseil :   <p><span>Pour mettre à jour la disponibilité mensuelle des rôles pendant plusieurs mois, saisissez le nombre d’heures ou d’ETR dans le champ [!UICONTROL Disponible] d’un mois, puis faites glisser le coin du champ sur les mois adjacents pour copier la même valeur pour chaque mois. Déposez-le pour mettre à jour tous les mois.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Obligatoire] (max &lt;nombre&gt;)</p> 
       <div> 
        <p role="rowheader">ou</p> 
        <p role="rowheader">[!UICONTROL Obligatoire] (total &lt;nombre&gt;)</p> 
       </div> </td> 
      <td> <p><span>Selon que vous avez choisi d’utiliser des heures ou l’éditeur de texte enrichi pour votre plan, passez en revue </span> le nombre mensuel d’heures ou d’heures requises pour le rôle d’éditeur de texte enrichi pour le scénario dans les champs suivants : </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Obligatoire] (max &lt;nombre d’ETR&gt;)</strong> : le nombre entre parenthèses affiche le nombre maximal de rôles requis pour l’un des mois du scénario. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Obligatoire] (total &lt;nombre d’heures&gt;)</strong> : le nombre entre parenthèses affiche le nombre total d’heures requises pour tous les mois du scénario.</span> </p> </li> 
       </ul> <p>Conseil : Vous ne pouvez pas modifier le nombre requis d’ETR <span>ou d’heures</span> pour le rôle de tâche. Ce nombre est renseigné pour le scénario une fois que vous avez commencé à ajouter des initiatives et leurs exigences en termes de rôle professionnel. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Différence]</td> 
      <td> 
       <div> 
        <p>Différence mensuelle entre le nombre de rôles de tâche requis et disponibles pour le scénario. [!DNL Workfront] calcule la différence pour chaque rôle de tâche pour chaque mois à l’aide de la formule suivante :</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (en ETP ou heures) </p> 
        <p>Conseil : Lorsque la différence affiche un nombre négatif, le scénario nécessite davantage de rôles d’emploi que le plan disponible. Vos ressources sont surchargées. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilisation] %</td> 
      <td> 
       <div> 
        <p>Le pourcentage d’utilisation affiche le nombre de rôles de tâche disponibles réellement utilisés (ou requis) sur les initiatives dans le scénario. </p> 
        <p>[!DNL Workfront] calcule l’utilisation par rôle de tâche par mois à l’aide de la formule suivante : </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>Le pourcentage d’utilisation peut s’afficher dans les couleurs suivantes, selon l’allocation de vos ressources :</p> 
        <ul> 
         <li> <p><b>Vert</b> : le nombre de rôles de tâche disponibles et requis correspond. Les ressources sont entièrement allouées et le pourcentage d’utilisation est de 100 %. </p> </li> 
         <li> <p><b>Rouge</b> : il y a plus de rôles de tâche requis que le plan disponible. Les ressources sont surchargées et le pourcentage d’utilisation est supérieur à 100 %.</p> </li> 
         <li> <p><b>Bleu</b> : il existe plus de rôles de tâche disponibles qu’ils ne sont requis. Les ressources sont sous-affectées et le pourcentage d’utilisation est inférieur à 100 %. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Appliquer]** pour enregistrer la distribution mensuelle des rôles de tâche.

   Ou

   Cliquez sur **[!UICONTROL Annuler]** pour fermer la liste de distribution des rôles de tâche et revenir au scénario.

1. Cliquez sur la zone **[!UICONTROL Financial]** dans l&#39;en-tête du plan pour ajouter le budget de ce plan.

   Les détails de la boîte [!UICONTROL Financial] s&#39;affichent.

   >[!TIP]
   >
   >La devise utilisée par [!DNL Workfront] pour ce plan s’affiche entre parenthèses dans le titre de la zone.

1. Spécifiez le **[!UICONTROL budget annuel]**.

   >[!NOTE]
   >
   >Si votre plan s’étend sur plusieurs années, vous devez indiquer un montant budgétaire pour chaque année.

1. Appuyez sur Entrée pour enregistrer le budget annuel, puis sur [!UICONTROL Onglet] pour passer à l’année suivante.

   Le budget annuel est automatiquement réparti à parts égales pour chaque mois de l&#39;année sélectionnée.

1. Cliquez sur **[!UICONTROL Avancé]** pour afficher la distribution budgétaire mensuelle. Les budgets annuel et mensuel sont toujours des nombres arrondis. Lorsque le montant du budget ne peut pas être réparti uniformément sur tous les mois d’une année en raison des décimales, un indicateur **[!UICONTROL Restant]** s’affiche sous la répartition du budget annuel.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Ajustez manuellement les budgets mensuels afin d’éliminer les montants excédentaires.

   Lorsque le total de tous les montants du budget mensuel est supérieur au budget annuel, un indicateur d&#39;avertissement **[!UICONTROL Dépassement]** s&#39;affiche sous la répartition du budget annuel. Ajustez manuellement les montants du budget mensuel jusqu&#39;à ce qu&#39;ils soient égaux ou inférieurs au budget disponible pour le plan.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Désactivez le paramètre **[!UICONTROL Inclure les coûts des personnes]** pour exclure du comptage les coûts associés aux rôles d’emploi par rapport au coût global du plan. Les coûts fixes sont toujours comptabilisés dans le coût global du plan. Ce paramètre est activé par défaut et affecte tous les scénarios du plan.
1. Cliquez n’importe où en dehors de la zone [!UICONTROL Financial] pour la fermer. Les informations que vous avez saisies sont automatiquement enregistrées.

   Vous pouvez maintenant commencer à créer les initiatives sur le plan et ajouter des scénarios.

1. (Recommandé) Cliquez sur **[!UICONTROL Nouvelle initiative]** pour ajouter une nouvelle initiative.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Pour plus d’informations sur l’ajout d’initiatives, consultez l’article [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Facultatif) Effectuez une copie du scénario existant pour créer un nouveau scénario du même plan. Pour plus d’informations sur la création et l’utilisation de plusieurs scénarios, voir [Création et comparaison de scénarios de plan dans le [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Cliquez sur **[!UICONTROL Enregistrer la formule]**.

   Votre plan est créé ou mis à jour.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Favoris]** ![](assets/favorites-icon-small.png) à droite du nom du plan pour ajouter le plan à votre liste de Favoris.

1. (Facultatif) Copiez l’URL du plan et envoyez-la à tout autre utilisateur qui aura besoin de la consulter ou de la mettre à jour. Ils doivent avoir au moins un accès [!UICONTROL Vue] au niveau de leur accès pour pouvoir visualiser le plan. Ils doivent disposer de l’accès [!UICONTROL Edit] pour le modifier. S’ils doivent consulter les informations financières sur le plan, telles que les informations sur les budgets, les coûts et les taux de rôle professionnel, ils doivent également avoir accès aux [!UICONTROL données financières] dans leur niveau d’accès. Pour plus d’informations sur l’accès requis pour [!DNL Scenario Planner], voir [Accès requis pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
