---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : calculer le coût des heures supplémentaires dans une vue de feuille de calcul'
description: Les heures supplémentaires ne sont pas calculées par défaut dans Adobe Workfront, mais vous pouvez créer un rapport de feuille de temps qui calcule les heures supplémentaires.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Afficher : calculer le coût des heures supplémentaires dans une vue de feuille de temps ;

Les heures supplémentaires ne sont pas calculées par défaut dans Adobe Workfront, mais vous pouvez créer un rapport de feuille de temps qui calcule les heures supplémentaires.

Si l&#39;utilisateur est associé à un taux Coût par heure dans son profil, vous pouvez également calculer le coût des heures supplémentaires de cet utilisateur.\
Pour plus d’informations sur l’association des utilisateurs aux taux de coût par heure, consultez l’article . [Configurer mes paramètres](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Le champ Heure de fin que vous pouvez ajouter à une vue de feuille de temps dans une liste ou un rapport affiche les informations figurant dans le champ Heure de fin de la feuille de temps. Ces informations sont mises à jour manuellement par un utilisateur ayant accès à la modification de la feuille de temps. Pour plus d’informations sur le champ Heure de dépassement dans une feuille de temps, consultez l’article . [Présentation de la disposition de la feuille de calcul](../../../timesheets/timesheets/timesheet-layout.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Calcul du coût des heures supplémentaires dans une vue de feuille de temps

Pour ajouter une colonne Heure de dépassement de délai calculée à une vue de feuille de temps :

1. Accédez à une liste de feuilles de temps ou créez un rapport de feuille de temps.

   Pour plus d’informations sur la création de rapports, voir l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Cliquez sur **Vue Personnaliser** dans une liste de feuilles de temps.

   Ou

   Sélectionnez la **Colonnes (affichage)** dans un rapport de feuille de calcul.

1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**.
1. Dans le **Afficher dans cette colonne** zone, cliquez sur **Cliquer pour modifier le texte**.
1. Copiez et collez le code de mode texte suivant dans le **Mode texte** de la boîte de dialogue
   <pre>displayname=Coût des heures supplémentaires calculé<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Ce calcul suppose que l’utilisateur travaille généralement une semaine de 40 heures.

1. Cliquez sur **Enregistrer**, puis attribuez un nom à la nouvelle vue et cliquez sur **Enregistrer la vue** dans une liste de feuilles de temps.

   Ou

   Cliquez sur **Enregistrer + Fermer** dans un rapport de feuille de calcul.

1. (Facultatif et conditionnel) si vous créez un rapport de feuille de calcul, nommez-le, puis cliquez sur **Enregistrer le rapport**.

   Le coût des heures supplémentaires de chaque utilisateur s’affiche dans la variable **Coût des heures supplémentaires calculé** colonne .

   ![calculate_supplémentaires_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
