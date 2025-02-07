---
title: Affichage et exportation des journaux d’audit
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez afficher tous les journaux d’audit du système ou ceux qui répondent à certains critères de filtrage. Vous pouvez également exporter les journaux d’audit. Les journaux d’audit répertorient les modifications apportées par un utilisateur ou une utilisatrice déclenchées dans le système au cours des 90 derniers jours.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 98%

---

# Afficher et exporter des journaux d’audit

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Vous pouvez afficher tous les journaux d’audit du système ou ceux qui répondent à certains critères de filtrage. Vous pouvez également exporter les journaux d’audit.

Les journaux d’audit répertorient les modifications apportées par un utilisateur ou une utilisatrice déclenchées dans le système au cours des 90 derniers jours.

Pour plus d’informations sur tous les types de journaux d’audit et sur leur génération, consultez l’article [Journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher les journaux d’audit

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système > Journaux d’audit**.
1. Dans le menu déroulant **Type de journal**, sélectionnez le type de journal d’audit à afficher.

   **Tous les types de journaux** est le choix sélectionné par défaut.

   Pour obtenir la liste de tous les types de journaux d’audit que vous pouvez afficher et les informations incluses, consultez l’article [Journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Facultatif) Définissez l’un des filtres disponibles.

   >[!NOTE]
   >
   >Les options du menu déroulant Type d’action varient en fonction du journal d’audit sélectionné.

   ![Journaux d’audit](assets/audit-logs.jpg)

1. Cliquez sur **Appliquer**.
1. (Facultatif) Cliquez sur **Effacer les filtres** pour réinitialiser les modifications apportées aux filtres.

## Exporter des journaux d’audit

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système > Journaux d’audit**.

1. Dans le menu déroulant **Type de journal**, sélectionnez un journal d’audit.

   **Tous les types de journaux** est sélectionné par défaut.

1. Définissez les filtres disponibles, puis cliquez sur **Appliquer**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas exporter plus de 50 000 journaux à la fois. Workfront exporte les journaux en fonction des filtres que vous définissez et non pas du nombre de journaux affichés sur la page. Vous pouvez afficher le nombre total de journaux filtrés dans le coin inférieur droit de la page.

1. Cliquez sur **Exporter**.
