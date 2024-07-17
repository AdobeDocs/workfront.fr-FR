---
title: Afficher et exporter les journaux d’audit
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez afficher tous les journaux d’audit du système ou ceux qui répondent à certains critères de filtrage. Vous pouvez également exporter les journaux d’audit. Les journaux d’audit répertorient les modifications utilisateur déclenchées dans le système au cours des 90 derniers jours.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 21%

---

# Afficher et exporter les journaux d’audit

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Vous pouvez afficher tous les journaux d’audit du système ou ceux qui répondent à certains critères de filtrage. Vous pouvez également exporter les journaux d’audit.

Les journaux d’audit répertorient les modifications utilisateur déclenchées dans le système au cours des 90 derniers jours.

Pour plus d’informations sur tous les types de journaux d’audit et sur leur génération, voir [Journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Afficher les journaux d’audit

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Système > Journaux d’audit**.
1. Dans le menu déroulant **Type de journal**, sélectionnez le type de journal d’audit à afficher.

   **Tous les types de journaux** est sélectionné par défaut.

   Pour obtenir la liste de tous les types de journaux d’audit que vous pouvez afficher et les informations qu’ils incluent, voir [Journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Facultatif) Définissez l’un des filtres disponibles.

   >[!NOTE]
   >
   >Les options du menu déroulant Type d’action varient en fonction du journal d’audit sélectionné.

   ![](assets/audit-logs.jpg)

1. Cliquez sur **Appliquer**.
1. (Facultatif) Cliquez sur **Effacer les filtres** pour réinitialiser les modifications apportées aux filtres.

## Exportation des journaux d’audit

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Système > Journaux d’audit**.

1. Dans le menu déroulant **Type de journal**, sélectionnez un journal d’audit.

   **Tous les types de journaux** est sélectionné par défaut.

1. Définissez les filtres disponibles, puis cliquez sur **Appliquer**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas exporter plus de 50 000 logs à la fois. Workfront exporte les journaux en fonction des filtres que vous définissez, et non du nombre de journaux affichés sur la page. Vous pouvez afficher le nombre total de journaux filtrés dans le coin inférieur droit de la page.

1. Cliquez sur **Export**.
