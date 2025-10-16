---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : Calculer le coût des heures supplémentaires dans une vue Feuille de temps'
description: Les heures supplémentaires ne sont pas calculées par défaut dans Adobe Workfront, mais vous pouvez créer un rapport de feuille de temps qui les calcule.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 74%

---

# Vue : calculer le coût des heures supplémentaires dans une vue de feuille de temps

<!--Audited: 11/2024-->

Les heures supplémentaires ne sont pas calculées par défaut dans Adobe Workfront, mais vous pouvez créer un rapport de feuille de temps qui les calcule.

Si la personne est associée à un taux de Coût par heure dans son profil, vous pouvez également calculer le coût de ses heures supplémentaires.\
Pour plus d’informations sur l’association de personnes à des taux de coût par heure, consultez l’article [Configurer mes paramètres](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Le champ Heures supplémentaires que vous pouvez ajouter à une vue de feuille de temps dans une liste ou un rapport affiche les informations figurant dans le champ Heures supplémentaires de la feuille de temps. Ces informations sont mises à jour manuellement par une personne ayant accès à la modification de la feuille de temps. Pour plus d’informations sur le champ Heures supplémentaires dans une feuille de temps, consultez l’article [Vue d’ensemble de la disposition de la feuille de temps](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Calculer le coût des heures supplémentaires dans une vue de feuille de temps

Pour ajouter une colonne Heures supplémentaires calculée à une vue de feuille de temps, procédez comme suit :

1. Accédez à une liste de feuilles de temps.

1. Cliquez sur le menu déroulant **Affichage**, puis sur **Nouvel affichage**.

1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Basculer en mode texte**, puis sur **Modifier le mode texte**.
1. Dans la zone **Modifier le mode texte**, supprimez le texte de la zone, puis copiez et collez le code de mode texte suivant :

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >Ce calcul suppose que la personne effectue généralement une semaine de 40 heures.

1. Cliquez sur **Terminé**, puis attribuez un nom à la nouvelle vue et cliquez sur **Enregistrer la vue** dans une liste de feuilles de temps.

   Le coût des heures supplémentaires de chaque personne s’affiche dans la colonne **Coût des heures supplémentaires calculé**.


