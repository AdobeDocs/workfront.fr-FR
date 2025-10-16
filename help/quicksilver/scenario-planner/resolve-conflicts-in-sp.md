---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Résoudre les conflits d’initiative dans le planificateur de scénarios
description: Lorsque des initiatives entrent en conflit les unes avec les autres, elles sont en concurrence pour les mêmes ressources. Les ressources dont vous disposez pour un scénario ne sont pas suffisantes pour couvrir l’ensemble des ressources nécessaires à toutes les initiatives du scénario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '2187'
ht-degree: 92%

---

# Résoudre les conflits d’initiative dans le [!DNL Scenario Planner]

Lorsque des initiatives entrent en conflit les unes avec les autres, elles sont en concurrence pour les mêmes ressources. Les ressources dont vous disposez pour un scénario ne sont pas suffisantes pour couvrir l’ensemble des ressources nécessaires à toutes les initiatives du scénario.

Cela peut se produire dans l’un des cas suivants :

* Le nombre de fonctions requises pour l’initiative est supérieur au nombre de fonctions prévues dans le budget du plan.
* Le coût de l’initiative est supérieur au budget disponible pour le plan.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] paquet</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTE</b></p>
<p>Contactez votre représentant Workfront si vous disposez d’un autre package Workfront.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence</p> </td> 
   <td> <p>[!UICONTROL Light] ou version ultérieure</p> 
   <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
    <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès [!UICONTROL Edit] à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour un plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur l’accès au planificateur de scénarios, voir [ Accès nécessaire pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Documentation sur les exigences d’accès à Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Vue d’ensemble de la résolution des conflits

* Un conflit est également compris comme une suraffectation des fonctions ou du budget d’un scénario.
* Lorsque [!DNL Workfront] détecte un conflit, la barre correspondant au mois du conflit pendant la durée de l’initiative s’affiche en rouge. Cela peut se produire dans l’un des cas suivants :

   * Le nombre de fonctions requises mensuellement pour une initiative est supérieur au nombre de fonctions budgétées pour le plan après que toutes les initiatives précédentes ont utilisé les ressources budgétées pour le plan.
   * Les coûts mensuels de l’initiative sont supérieurs au budget disponible pour le plan après que toutes les initiatives précédentes ont utilisé le budget du plan pour couvrir leurs coûts.

>[!TIP]
>
>Par défaut, le [!DNL Scenario Planner] suppose que vous avez budgétisé 0 fonction et 0 $ ou l’équivalent de 0 $ dans la devise de votre système pour un scénario, sauf si vous avez spécifié le contraire. Le nombre de fonctions indique le nombre de FTE (équivalents temps complet) ou d’heures budgétées pour la fonction.
>
>Pour tous les calculs dans le planificateur de scénarios, Workfront utilise la valeur suivante : 1 FTE = 8 heures.
>
>Pour plus d’informations sur la mise à jour des fonctions disponibles pour un plan et un budget, voir [Créer et modifier des plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* Vous pouvez résoudre un conflit en prenant l’une des mesures suivantes :

   * Ajout automatique des ressources nécessaires manquantes à partir des initiatives du scénario. Cet article décrit comment résoudre les conflits à l’aide de cette option.
   * Ajustement des ressources pour les fonctions et le budget pour le scénario, en modifiant le plan. Pour plus d’informations, voir [Créer et modifier des plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Résoudre les conflits entre les initiatives

1. Accédez à un plan pour lequel vous voulez résoudre des conflits.

   Pour plus d’informations sur la création de plans, voir [Créer et modifier des plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Pour plus d’informations sur la création d’initiatives, voir [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Facultatif) Dans le menu déroulant **[!DNL Initial scenario]**, sélectionnez le scénario que vous souhaitez examiner.

   >[!TIP]
   >
   >Un plan peut comporter plusieurs scénarios. En examinant les conflits du plan, [!DNL Workfront] se réfère aux ressources actuellement disponibles pour le scénario sélectionné et à celles nécessaires pour les initiatives de ce scénario. Pour plus d’informations sur les scénarios, voir [Créer et comparer des scénarios de plan dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Assurez-vous que l’option **[!UICONTROL Afficher les conflits]** est activée. Elle est activée par défaut.

   ![Basculement entre Afficher les scénarios](assets/show-scenarios-toggle-on.png)

   La première initiative en conflit affiche les mois concernés en rouge et une icône d’avertissement s’affiche à côté du nom de l’initiative.

   L’arrière-plan de toutes les initiatives, en commençant par la première initiative conflictuelle, apparaît en rouge sur le graphique du plan.

   Lorsqu’une initiative présente un conflit, cela signifie que le nombre de fonctions pour au moins un rôle spécifique, les coûts encourus, ou les deux, dépassent le nombre de fonctions ou le budget défini pour le plan pour un mois spécifique.

   ![Initiatives sur le plan avec conflit](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Effectuez l’une des opérations suivantes suivantes pour mieux comprendre les conflits qui peuvent exister :

   * Pointez sur l’icône d’avertissement située à côté du nom de l’initiative pour savoir s’il s’agit d’un conflit de fonction ou de budget.

     ![Conflit de fonction budgétaire](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     Lorsque vous pointez sur l’icône d’avertissement, l’une des options suivantes peut s’afficher, selon que les fonctions de votre initiative font l’objet d’une affectation trop importante ou que ses côuts sont surestimés.

      * Afficher les détails de conflit de fonction
      * Afficher les détails de conflit budgétaire
      * Afficher les détails des fonctions et des budgets

   * Pointez sur un mois dans la chronologie du plan lorsque vous consultez le plan par mois, pour afficher les ressources requises pour ce mois et savoir si les conflits du mois sont liés à des personnes ou à des coûts.

     ![Détails des conflits sur la chronologie mensuelle](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     Examinez les informations mensuelles suivantes au niveau du plan :

      * Pour le mois en question, pour toutes les initiatives prévues ce mois-ci, le nombre de fonctions disponibles, requises et affectées de manière excessive est indiqué.
      * Pour le mois en question, pour toutes les initiatives prévues ce mois-ci, les coûts disponibles, requis et affectés de manière excessive.

        >[!TIP]
        >
        >Les coûts [!UICONTROL disponibles] correspondent au budget du scénario pour le mois en question.

   * Pour afficher l’encadré d’informations complémentaires sur le conflit qui se déroule ce mois-là, pointez sur la barre rouge d’une initiative pour un mois donné.

     ![Détails des conflits sur la chronologie de l’initiative](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

     Examinez les champs suivants dans la zone d’informations supplémentaires au niveau de l’initiative :

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Mois au cours duquel le conflit survient</td> 
        <td>S’affiche dans le titre de la zone d’informations complémentaires</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Le nom de l’initiative</td> 
        <td>S’affiche dans le titre de la zone d’informations complémentaires</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Job Roles]</td> 
        <td> <p>Les fonctions associées à cette initiative qui font l’objet d’une affectation trop importante pour le mois sélectionné. Les colonnes suivantes affichent des informations pour chaque fonction requise pour le mois sélectionné en conflit avec le nombre de fonctions disponibles pour ce mois :</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong> : le nombre de chaque fonction disponible dans le scénario pour le mois sélectionné.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong> : le nombre de chaque fonction requise dans le cadre de l’initiative pour le mois sélectionné.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated] :</strong> la différence entre le nombre requis dans le cadre de l’initiative et le nombre disponible dans le scénario. </p> </li> 
         </ul> <p>Conseil : parfois, le nombre de fonctions [!UICONTROL Available] correspond ou est supérieur au nombre de fonctions [!UICONTROL Required], mais le site [!DNL Scenario Planner] affiche toujours une affectation excessive. Cela signifie que des initiatives de niveau supérieur ont déjà utilisé les fonctions disponibles dans le plan pour le même mois. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Coûts</td> 
        <td> <p>Les coûts de l’initiative pour le mois sélectionné. Les colonnes suivantes affichent les informations sur les coûts nécessaires et le budget disponible pour le mois sélectionné :</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong> : le budget disponible du plan pour le mois sélectionné.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong> : les coûts requis pour cette initiative pour le mois sélectionné.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated] :</strong> la différence entre les coûts requis pour l’initiative et le budget disponible dans le plan. </p> </li> 
         </ul> <p>Conseil : parfois, les coûts [!UICONTROL Available] correspondent ou sont supérieurs aux coûts [!UICONTROL Required] pour l’initiative pour le mois sélectionné et le [!DNL Scenario Planner] indique toujours une affectation excessive des coûts. Cela signifie que des initiatives de niveau supérieur utilisent déjà le budget disponible dans le plan pour le même mois. </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. Effectuez l’une des opérations suivantes pour ouvrir le panneau de détails de l’initiative et afficher plus d’informations sur l’emplacement des conflits et pour les résoudre :

   * Cliquez sur l’icône d’avertissement à côté du nom de l’initiative.
   * Cliquez sur la barre d’une initiative.
   * Cliquez sur l’icône **[!UICONTROL Plus]** ![Plus](assets/more-icon.png) à droite du nom de l’initiative, puis cliquez sur **[!UICONTROL Modifier]**.

     Le panneau des détails de l’initiative s’affiche à droite.

     Lorsque vous ne disposez pas d’un nombre de personnes ou d’un budget suffisant pour votre initiative, une icône d’avertissement rouge s’affiche à côté des sections suivantes :

   * [!UICONTROL Fonctions requises]
   * [!UICONTROL Coûts]

1. (Le cas échéant) Pour les initiatives qui ont des conflits de fonctions, accédez à la section **[!UICONTROL Fonctions requises]** pour voir toutes les fonctions requises pour votre initiative. Identifiez les fonctions qui peuvent faire l’objet d’une affectation excessive. Examinez le nombre d’équivalents temps complet ou le nombre d’heures nécessaires pour chaque fonction pour chaque mois de l’initiative. La case contenant le nombre d’équivalents temps complet ou le nombre d’heures pour les mois présentant des affectations excessives s’affiche dans un cadre rouge.

   ![Rôles suraffectés](assets/details-panel-overallocated-roles-350x275.png)

1. (Facultatif) Cliquez sur la flèche pointant vers la droite à côté des mois de la chronologie de l’initiative pour voir quels mois supplémentaires présentent des conflits dans les fonctions.

   ![Flèche droite à l’intérieur de la zone de détails](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Facultatif) Cliquez sur **[!UICONTROL Afficher les détails]** sous la fonction qui affiche un conflit pour voir où les conflits apparaissent et pour surligner les mois en conflit dans la zone du graphique du plan. Des informations supplémentaires s’affichent pour chaque fonction.

   Les champs suivants s’affichent pour chaque fonction :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Le nombre de fonctions disponibles dans le plan pour chaque mois. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>Le nombre de fonctions déjà attribuées à partir du budget du plan à des initiatives de niveau supérieur pour un mois donné. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>La différence entre le nombre de fonctions requises pour l’initiative et le nombre disponible dans le plan après que des initiatives de niveau supérieur ont également utilisé certaines fonctions. Workfront calcule le nombre de fonctions [!UICONTROL Overallocated] à l’aide de la formule suivante :</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Sur le graphique du plan, les mois où les fonctions sont attribuées affichent le nom et le nombre de fonctions nécessaires pour chaque initiative qui en a besoin. Vous devez sélectionner la vue [!UICONTROL Mois] pour voir le nom des fonctions.

   ![Fonctions en conflit](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Faites l’une des opérations suivantes pour résoudre les conflits de fonctions :

   * Baissez manuellement le nombre de fonctions pour chaque mois de l’initiative.
   * Passez la souris sur le nom de la fonction et cliquez sur l’icône **[!UICONTROL supprimer]** ![Supprimer](assets/delete.png) pour supprimer la fonction de l’initiative.
   * Sélectionnez **[!UICONTROL Ajouter des fonctions aux ressources disponibles du scénario]**, puis cliquez sur **[!UICONTROL Appliquer]**.

     Ceci ajoute le nombre manquant d’équivalents temps complet ou le nombre d’heures de fonction au champ [!UICONTROL Disponible] du scénario.

     >[!NOTE]
     >
     >Les fonctions que vous ajoutez pour résoudre les conflits modifient les fonctions [!UICONTROL Disponible] du scénario sélectionné et non pour tous les scénarios du plan.

     Une flèche verte pointant vers le haut ![flèche verte pointant vers le haut](assets/upward-green-arrow.png) s’affiche pour le mois dans le journal du plan afin d’indiquer que davantage de ressources ont été ajoutées au plan ce mois-là. Vous devez sélectionner la vue [!UICONTROL Mois] pour voir cet indicateur.

   * (Le cas échéant) Fermez le panneau de détails et donnez à l’initiative une priorité plus élevée pour recevoir les ressources budgétaires du plan en premier, si possible. Pour plus d’informations sur la mise à jour de la priorité des initiatives, voir [Mettre à jour les priorités des initiatives dans le planificateur de scénarios](../scenario-planner/prioritize-initiatives.md).

1. (Facultatif) Cliquez sur **[!UICONTROL Masquer les détails]** pour fermer la zone de détails supplémentaires, puis cliquez sur **[!UICONTROL Appliquer]** pour enregistrer les modifications apportées aux fonctions.

1. (Le cas échéant) Pour les initiatives qui ont des conflits de coûts, accédez à la section **[!UICONTROL Coûts]** dans le panneau des détails de l’initiative pour examiner les coûts pour chaque mois de la durée de l’initiative. Identifiez les mois pour lesquels le budget du plan pourrait ne pas être suffisant pour couvrir les coûts de l’initiative sélectionnée. La zone où le budget disponible est insuffisant s’affiche avec un contour rouge.
1. (Facultatif) Cliquez sur la flèche pointant vers la droite à côté des mois de la chronologie de l’initiative pour afficher les mois supplémentaires qui ont un budget insuffisant pour couvrir les coûts.

   ![Flèche pour coûts insuffisants](assets/details-panel-insufficient-costs-350x239.png)

1. (Facultatif) Cliquez sur **[!UICONTROL Afficher les détails]** sous les informations relatives aux coûts pour voir où le conflit apparaît et pour surligner les mois en conflit sur le graphique du plan. Les champs supplémentaires suivants s’affichent pour chaque type de coût :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Les coûts disponibles dans le budget du plan pour chaque mois. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>Le montant des fonds déjà affectés du budget du plan à des initiatives de niveau supérieur. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>La différence mensuelle entre les coûts nécessaires à l’initiative et le montant disponible dans le budget du plan après que les initiatives de niveau supérieur ont également utilisé une partie du budget disponible. [!DNL Workfront] calcule le nombre de coûts affectés de manière excessive à l’aide de la formule suivante :</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] calcule les coûts requis pour l’initiative en cours pour chaque mois à l’aide de la formule suivante :</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Sur le graphique du plan, les mois où les coûts sont insuffisants affichent le nom et le nombre de fonctions encore nécessaires pour l’initiative. Vous devez sélectionner la vue Mois pour afficher les montants des coûts.

   ![Conflit de coûts](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Si vous avez désactivé le paramètre [!UICONTROL Inclure les coûts de personnel] pour la zone [!UICONTROL Budget] du plan lorsque vous avez créé le plan, la ligne [!UICONTROL Coûts de personnel] ne s’affiche pour aucune initiative dans aucun scénario. Dans ce cas, Workfront ne prend pas en compte les coûts de personnel dans les calculs pour déterminer les conflits de coûts. Pour plus d’informations sur la création d’un plan, voir [Créer et modifier des plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Faites l’une des opérations suivantes pour résoudre les conflits de coûts :

   * Baissez manuellement le nombre de [!UICONTROL Coûts fixes] pour chaque mois de l’initiative.
   * Dans la section **[!UICONTROL Fonctions requises]**, ajustez manuellement le nombre de fonctions pour le mois avec un budget de coûts de personnel, si possible. Cela permet de réduire les coûts de personnel.

     >[!TIP]
     >
     >Il n’est pas possible d’ajuster manuellement les coûts de personnel.

   * Sélectionnez **[!UICONTROL Ajouter le montant au budget du scénario]**, puis cliquez sur **[!UICONTROL Appliquer]**.

     Le montant insuffisant est ajouté au budget du scénario pour les mois où il manquait, ce qui met également à jour le budget global du scénario.

     >[!NOTE]
     >
     >Le montant que vous ajoutez pour résoudre les conflits de coûts modifie le budget du scénario sélectionné et non de tous les scénarios du plan.

   * (Le cas échéant) Fermez le panneau de détails et donnez à l’initiative une priorité plus élevée pour recevoir les ressources budgétaires du plan en premier, si possible. Pour plus d’informations sur la mise à jour des priorités d’initiative, voir [Mettre à jour les priorités d’initiative dans le  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Cliquez sur **[!UICONTROL Appliquer]** lorsque vous apportez des modifications à la section Coûts.
1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.


