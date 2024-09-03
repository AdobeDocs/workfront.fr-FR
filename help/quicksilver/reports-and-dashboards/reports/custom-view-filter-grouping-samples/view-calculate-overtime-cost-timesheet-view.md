---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : calculer le coût des heures supplémentaires dans une vue de feuille de temps »'
description: Les heures supplémentaires ne sont pas calculées par défaut dans Adobe Workfront, mais vous pouvez créer un rapport de feuille de temps qui les calcule.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 100%

---

# Vue : calculer le coût des heures supplémentaires dans une vue de feuille de temps

Les heures supplémentaires ne sont pas calculées par défaut dans Adobe Workfront, mais vous pouvez créer un rapport de feuille de temps qui les calcule.

Si la personne est associée à un taux de Coût par heure dans son profil, vous pouvez également calculer le coût de ses heures supplémentaires.\
Pour plus d’informations sur l’association de personnes à des taux de coût par heure, consultez l’article [Configurer mes paramètres](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Le champ Heures supplémentaires que vous pouvez ajouter à une vue de feuille de temps dans une liste ou un rapport affiche les informations figurant dans le champ Heures supplémentaires de la feuille de temps. Ces informations sont mises à jour manuellement par une personne ayant accès à la modification de la feuille de temps. Pour plus d’informations sur le champ Heures supplémentaires dans une feuille de temps, consultez l’article [Vue d’ensemble de la disposition de la feuille de temps](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Calculer le coût des heures supplémentaires dans une vue de feuille de temps

Pour ajouter une colonne Heures supplémentaires calculée à une vue de feuille de temps, procédez comme suit :

1. Accédez à une liste de feuilles de temps ou créez un rapport de feuille de temps.

   Pour plus d’informations sur la création de rapports, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Cliquez sur **Personnaliser la vue** dans une liste de feuilles de temps.

   Ou

   Sélectionnez l’onglet **Colonnes (vue)** dans un rapport de feuille de temps.

1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Basculer en mode texte**.
1. Dans la zone **Afficher dans cette colonne**, cliquez sur **Cliquez pour modifier le texte**.
1. Copiez et collez le code de mode texte suivant dans la boîte de dialogue **Mode texte**.
   <pre>displayname=Coût des heures supplémentaires calculé<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Ce calcul suppose que la personne effectue généralement une semaine de 40 heures.

1. Cliquez sur **Enregistrer**, puis attribuez un nom à la nouvelle vue et cliquez sur **Enregistrer la vue** dans une liste de feuilles de temps.

   Ou

   Cliquez sur **Enregistrer et fermer** dans un rapport de feuille de temps.

1. (Facultatif et le cas échéant) Si vous créez un rapport de feuille de temps, attribuez-lui un nom, puis cliquez sur **Enregistrer le rapport**.

   Le coût des heures supplémentaires de chaque personne s’affiche dans la colonne **Coût des heures supplémentaires calculé**.

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
