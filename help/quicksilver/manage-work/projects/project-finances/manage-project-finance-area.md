---
product-area: projects
navigation-topic: financials
title: Gestion des informations dans la zone de financement des projets
description: Vous pouvez afficher ou modifier les informations financières d’un projet en accédant à la zone Finances de la section Détails du projet .
author: Lisa
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: f01ce9bcbb795097d39e276a734300f5059e35c4
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 88%

---

# Gérer les informations dans la zone Finances d’un projet

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Vous pouvez afficher ou modifier les données financières d’un projet en accédant à la zone Finances de la section Détails du projet. Il existe un nombre limité de champs que vous pouvez afficher ou modifier dans cette zone. Pour plus d’informations sur la modification de toutes les informations d’un projet, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td>
   <td>
   <p>Léger ou supérieur</p>
   <p>Révision ou supérieur</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou accès supérieur aux projets et aux données financières</p> <p>Accès en modification aux projets et aux données financières pour modifier les données financières du projet</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou autorisations supérieures pour le projet, comprenant des autorisations d’affichage de finances</p> <p>Autorisations de gestion du projet qui incluent la gestion des finances pour modifier les données financières du projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble de la zone Finances

Tenez compte des points suivants lors de l’affichage ou de la modification de données dans la zone Finances :

* Les informations financières que vous pouvez trouver dans la zone Finances des Détails du projet représentent les valeurs qui sont cumulées au niveau du projet à partir des tâches, ainsi que les informations saisies directement dans le projet. Certaines données financières peuvent être gérées au niveau du projet ainsi qu’au niveau de la tâche.
* Vous devez disposer des autorisations d’affichage sur le projet ainsi que de l’accès aux données financières à partir de votre niveau d’accès afin de pouvoir afficher la zone Finances sur un projet.
* Vous devez disposer des autorisations de gestion sur le projet ainsi que de l’accès aux données financières à partir de votre niveau d’accès afin de pouvoir modifier les informations de la zone Finances. Cependant, nous recommandons que seules les personnes propriétaires du projet modifient les informations dans cette zone.

## Afficher les données financières sur un projet

1. Accédez à un projet.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Finance**.

   ![Zone Finance dans la vue détaillée](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur ou administratrice Workfront a configuré votre modèle de mise en page, la section Vue d’ensemble peut ne pas être répertoriée en premier, auquel cas elle est réduite. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Affichez les champs suivants dans la zone Finances du projet :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Méthode d'indice de performances</td> 
      <td> Contrôle la méthode utilisée par Workfront pour calculer les mesures de la Valeur acquise. Elle peut être basée sur les heures ou basée sur les coûts. <br>Pour plus d’informations sur le PIM, voir l’article <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Définir la méthode d’indice de performances (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">ICP/SPI/CSI</td> 
      <td> <p>Il s’agit de mesures de performances de projet qui indiquent les performances de votre projet à un moment donné. Leurs valeurs sont calculées selon la méthode d’indice de performances.<br>Pour plus d’informations, voir les articles suivants : </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calculer l’Indice Coûts Performances (ICP)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calculer l’Indice Horaire Performances (IHP) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calculer l’Indice Coûts Horaire Performances (ICH)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimation à l'achèvement</td> 
      <td> Coût total prévisionnel de votre projet, représenté en heures si la méthode d’indice de performances (PIM) est basée sur les heures et représenté avec une valeur monétaire si la méthode d’indice de performances (PIM) est basée sur les coûts.<br>Pour plus d’informations sur le calcul de l’estimation à l’achèvement, consultez l’article <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calculer l’estimation à l’achèvement (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Il s’agit du budget défini pour le projet. Il est spécifié manuellement par la personne propriétaire du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts fixes</td> 
      <td>Il s’agit des coûts fixes du projet indépendamment des autres activités du projet. Ils sont saisis manuellement par la personne propriétaire du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts prévus</td> 
      <td>Coût estimé du projet en fonction du nombre d’heures prévues et des taux associés aux personnes affectées à la tâche (fonctions ou utilisateurs et utilisatrices).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts réels</td> 
      <td>Tous les coûts du projet. Le coût réel est la somme de tous les coûts réels : le coût de la main-d’œuvre (basé sur les heures effectives et les taux associés aux fonctions ou aux utilisateurs et utilisatrices qui les enregistrent), les dépenses et les coûts fixes, qui peuvent être associés à un projet ou à une tâche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus fixes</td> 
      <td>Recettes définies attendues en fonction du planning du projet. Les revenus fixes sont spécifiées manuellement par la personne propriétaire du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus prévus</td> 
      <td>Recettes projetées attendues selon le nombre d’heures prévues et les taux associés aux personnes affectées la tâche (fonctions ou utilisateurs et utilisatrices).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenu réel</td> 
      <td>Recettes réelles du projet basées sur le nombre d’heures effectives et les taux associés aux personnes affectées à la tâche (fonctions ou utilisateurs et utilisatrices).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus facturés</td> 
      <td> <p>Revenus facturés aux clients ou à d’autres parties capturées dans les enregistrements de facturation. Pour plus d’informations sur les enregistrements de facturation, voir l’article <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Créer des enregistrements de facturation</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Modifier des informations financières sur un projet

En tant que personne propriétaire de projet, vous pouvez modifier les informations du sous-onglet Finances d’un projet.

Pour modifier les informations sur le sous-onglet Finances du projet :

1. Accédez à un projet dont vous êtes la personne propriétaire.

   >[!NOTE]
   >
   >Pour effectuer les étapes suivantes, vous devez disposer des autorisations de gestion sur le projet. Nous recommandons également que seule la personne propriétaire du projet modifie le sous-onglet Finances du projet.

1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Finance**. La zone Finances s’ouvre alors pour modification.
1. Modifier un champ qui peut être modifié en cliquant sur le champ ou cliquez sur **+Ajouter** pour ajouter des informations dans un champ vide.

   >[!TIP]
   >
   >Les champs ne peuvent pas être modifiés s’ils sont automatiquement calculés par Workfront ou si vous ne disposez pas d’autorisations de modification.

   ![Modifier la zone financière](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Mettez à jour l’un des champs ci-dessous.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront a configuré votre modèle de mise en page, les champs de la section Détails du projet peuvent être différents dans votre environnement. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Méthode d'indice de performances</td> 
      <td> <p>Contrôle la méthode utilisée par Workfront pour calculer les mesures de performances du projet. Elle est configurée au niveau du système par votre administrateur ou administratrice, mais vous pouvez également la modifier au niveau du projet. Choisissez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Basé sur les heures :</strong> Workfront utilise le nombre d’heures prévues pour calculer le CPI et l’EAC du projet, et l’EAC du projet s’affiche sous forme de nombre, en heures. </li> 
        <li><strong>Basé sur les coûts</strong> : Workfront utilise le coût prévu de la main-d’œuvre pour calculer le CPI et l’EAC du projet, et l’EAC s’affiche sous forme de valeur monétaire. Lorsque vous sélectionnez cette option, assurez-vous que les personnes assignées à la tâche (fonctions ou utilisateurs et utilisatrices) sont associées aux taux de coûts.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimation à l'achèvement</td> 
      <td> <p>Représente le coût total projeté de votre tâche ou de votre projet lorsqu’il sera achevé. Elle est configurée au niveau du système par votre administrateur ou administratrice, mais vous pouvez également la modifier au niveau du projet. Choisissez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Calculer au niveau du projet</strong> : l’EAC pour la tâche parent et le projet est déterminée à l’aide des heures effectives/du coût réel de main-d’œuvre dans les formules de l’EAC. Ce calcul inclut les heures effectives/les coûts et les dépenses ajoutés directement à la tâche parent ou au projet.</li> 
        <li><strong>Regrouper depuis tâches/sous-tâches</strong> : l’EAC pour la tâche parent et le projet est déterminée en additionnant les EAC de chaque tâche enfant. Ce calcul inclut les heures effectives/les coûts et les dépenses ajoutés directement à la tâche ou au projet parent.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Indiquez le budget de ce projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts fixes</td> 
      <td>Indiquez le coût fixe de ce projet. Cela ne doit pas inclure de coûts de main-d’œuvre ou de dépenses.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus fixes</td> 
      <td> <p>Indiquez les revenus fixes de ce projet. Cela ne doit pas inclure les revenus provenant d’enregistrements de facturation facturés à des partenaires ou à des tiers.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Devise du projet</td> 
      <td> <p>Indiquez une devise pour ce projet, si elle diffère de la devise par défaut de votre système. La devise par défaut de votre système est définie par votre équipe d’administration Workfront. Pour plus d’informations sur la configuration des taux de change dans Workfront, consultez l’article <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer les modifications**.
