---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: "Afficher : calculer le coût des heures supplémentaires dans une vue de feuille de temps"
description: Les heures supplémentaires ne sont pas calculées par défaut dans Adobe Workfront, mais vous pouvez créer un rapport de feuille de temps qui les calcule.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 76%

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

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
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

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Calculer le coût des heures supplémentaires dans une vue de feuille de temps

Pour ajouter une colonne Heures supplémentaires calculée à une vue de feuille de temps, procédez comme suit :

1. Accédez à une liste de feuilles de temps.

1. Cliquez sur le menu déroulant **Afficher**, puis sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**, puis sur **Modifier le mode Texte**.
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

1. Cliquez sur **Terminé**, puis nommez la nouvelle vue et cliquez sur **Enregistrer la vue** dans une liste de feuilles de temps.

   Le coût des heures supplémentaires de chaque personne s’affiche dans la colonne **Coût des heures supplémentaires calculé**.


