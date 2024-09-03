---
product-area: projects
navigation-topic: manage-tasks
title: Gérer les finances des tâches dans la section Détails de la tâche
description: Gérer les finances des tâches dans la section Détails de la tâche
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 100%

---

# Gérer les finances des tâches dans la section Détails de la tâche

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Vous pouvez afficher ou modifier les informations financières d’une tâche en accédant à la zone Vue d’ensemble de la section Détails de la tâche. Il existe un nombre limité de champs que vous pouvez afficher ou modifier dans cette zone. Pour plus d’informations sur la modification de toutes les informations financières d’une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets et tâches</p> <p>Accès Afficher ou supérieur aux données financières</p> <p>Vous devez disposer d’un accès Modifier aux données financières pour modifier les informations financières sur les tâches.</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher pour la tâche qui incluent l’autorisation Afficher les finances ou supérieure.</p> <p>Vous devez disposer des autorisations Gérer sur la tâche qui incluent Modifier les finances pour modifier les informations financières sur les tâches.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Modifier les finances de la tâche dans la section Détails de la tâche

1. Accédez à un projet dans lequel vous souhaitez afficher une tâche.

   >[!NOTE]
   >
   >Pour trouver une tâche, vous pouvez également la rechercher, puis cliquer sur le nom pour accéder à la tâche. Pour plus d’informations sur la recherche d’objets dans Workfront, voir [Rechercher dans Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Cliquez sur le nom de la tâche que vous souhaitez afficher.
1. Cliquez sur **Détails de la tâche**.
1. (Facultatif) Cliquez sur l’icône **Réduire tout** en haut à droite de la page Détails de la tâche.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Selon la façon dont votre administrateur ou administratrice Workfront ou de groupes configure notre modèle de mise en page, les champs de la section Détails de la tâche peuvent être réorganisés ou ne pas s’afficher. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Cliquez sur **Finances** pour développer et afficher les informations financières de la tâche.

   Cliquez sur l’icône **Modifier**![](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Finances**.

1. Modifiez un champ qui peut être modifié en cliquant sur le champ ou en cliquant sur **+Ajouter** pour ajouter des informations à un champ vide.
1. Examinez ou modifiez les informations suivantes dans la section **Finances** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Type de coût</td> 
      <td> <p>Indiquez le type de coût de la tâche. Cela détermine comment le coût de la tâche est calculé, en fonction du nombre d’heures passées sur les tâches. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p>Aucun coût</p> </li> 
        <li> <p>Fixe par heure </p> </li> 
        <li> <p> Utilisateur, par heure </p> </li> 
        <li> <p> Rôle par heure</p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>. L’administration de Workfront ou de groupes sélectionne le paramètre « Type de coût » par défaut pour les tâches de votre système ou de votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences de projet à l’échelle du système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de revenus</td> 
      <td> <p>Indiquez le type de revenu de la tâche. Cela détermine comment le revenu de la tâche est calculé en fonction du nombre d’heures passées sur les tâches. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p> Non facturable </p> </li> 
        <li> <p>Utilisateur, par heure </p> </li> 
        <li> <p>Rôle par heure </p> </li> 
        <li> <p>Fixe par heure </p> </li> 
        <li> <p>Utilisateur par heure avec limite </p> </li> 
        <li> <p>Rôle par heure avec limite </p> </li> 
        <li> <p>Utilisateur, par heure plus fixe </p> </li> 
        <li> <p>Rôle par heure plus fixe </p> </li> 
        <li> <p>Revenus fixes </p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des revenus, voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>. </p> <p>L’administration de Workfront ou de groupes sélectionne le paramètre « Type de revenu » par défaut pour les tâches de votre système ou de votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences du projet à l’échelle du système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts prévus</td> 
      <td> <p>Il s’agit d’un calcul qui affiche le coût de la tâche en fonction du nombre d’heures prévues, du type de coût et du taux horaire des utilisateurs et utilisatrices ou des fonctions. Pour plus d’informations sur le suivi des coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts réels</td> 
      <td> <p> Il s’agit d’un calcul qui affiche le coût de la tâche en fonction des heures effectives, du type de coût et du taux horaire pour des utilisateurs et utilisatrices ou des fonctions. Pour plus d’informations sur le suivi des coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus prévus</td> 
      <td> <p>Il s’agit d’un calcul qui affiche les revenus associées à la tâche en fonction du nombre d’heures prévues, du type de revenu et du taux horaire des utilisateurs et utilisatrices ou des fonctions. Pour plus d’informations sur le suivi des coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenu réel</td> 
      <td> <p>Il s’agit d’un calcul qui affiche les revenus associés à la tâche en fonction des heures effectives, du type de revenu et du taux horaire des utilisateurs et utilisatrices ou des fonctions. Pour plus d’informations sur le suivi des coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suive les coûts</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ICP/SPI/CSI</strong> </td> 
      <td> <p>Il s’agit de mesures des performances de votre tâche à un moment donné. Leurs valeurs sont calculées en fonction de la méthode d’indice de performances du projet.<br>Pour plus d’informations, voir les articles suivants :</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calculer l’Indice Coûts Performances (ICP)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calculer l’Indice Horaire Performances (IHP) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calculer l’Indice Coûts Horaire Performances (CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimation à l’achèvement (EAC)</td> 
      <td> <p>Il s’agit d’un calcul qui affiche le coût total de votre tâche à la fin de celle-ci. Pour plus d’informations sur l’estimation à l’achèvement, voir <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calculer l’estimation à l’achèvement (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Le cas échéant) Si vous modifiez les champs de la section Finance, cliquez sur **Enregistrer****les modifications**.
