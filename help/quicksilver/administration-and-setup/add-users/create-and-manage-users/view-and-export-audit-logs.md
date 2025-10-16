---
title: Affichage et exportation des journaux d’audit
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez afficher tous les journaux d’audit du système ou ceux qui répondent à certains critères de filtrage. Vous pouvez également exporter les journaux d’audit. Les journaux d’audit répertorient les modifications apportées par un utilisateur ou une utilisatrice déclenchées dans le système au cours des 90 derniers jours.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 57%

---

# Afficher et exporter des journaux d’audit

<!--Audited: 08/2025-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Vous pouvez afficher tous les journaux d’audit du système ou ceux qui répondent à certains critères de filtrage. Vous pouvez également exporter les journaux d’audit dans un fichier CSV.

Les journaux d’audit répertorient les modifications apportées par un utilisateur ou une utilisatrice déclenchées dans le système au cours des 90 derniers jours.

Pour plus d’informations sur tous les types de journaux d’audit et sur ce qui les génère, voir [Présentation des journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td><p>Administrateur ou administratrice système</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>System Administrator</p></td>
  </tr> 
 </tbody> 
</table>-->

## Afficher les journaux d’audit

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système > Journaux d’audit**.
1. Dans le menu déroulant **Type d’action**, sélectionnez le type d’audit à afficher.

   >[!NOTE]
   >
   >Les options du menu déroulant Type d’action varient en fonction du journal d’audit sélectionné.

1. Dans le menu déroulant **Type de journal**, sélectionnez le type de journal d’audit à afficher.

   **Tous les types de journaux** est le choix sélectionné par défaut.

   Pour obtenir la liste de tous les types de journaux d’audit que vous pouvez afficher et les informations qu’ils incluent, voir [Présentation des journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Facultatif) Définissez l’un des filtres disponibles pour les champs suivants :

   * **Utilisateurs** : saisissez le nom de l’utilisateur qui a effectué la modification.
   * **De** : date de début de la période au cours de laquelle la modification a été apportée.
   * **À** : date de fin de la période au cours de laquelle la modification a été apportée.

   ![Journaux d’audit](assets/audit-logs.png)

1. Cliquez sur **Appliquer**.
1. (Facultatif) Cliquez sur **Effacer** pour réinitialiser les modifications apportées aux filtres.

## Exporter des journaux d’audit

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Journaux d’audit**.

1. Dans le menu déroulant **Type de journal**, sélectionnez un journal d’audit.

   **Tous les types de journaux** est sélectionné par défaut.

1. Définissez les filtres disponibles, puis cliquez sur **Appliquer**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas exporter plus de 50 000 journaux à la fois. Workfront exporte les journaux en fonction des filtres que vous définissez et non pas du nombre de journaux affichés sur la page. Vous pouvez afficher le nombre total de journaux filtrés dans le coin inférieur droit de la page.

1. Cliquez sur **Exporter**.

   La boîte de dialogue Enregistrer le fichier s’ouvre et vous pouvez enregistrer le fichier exporté sur votre ordinateur.

   Vous ne pouvez enregistrer les journaux d’audit qu’au format CSV.

   Terminez d’enregistrer le fichier exporté. Vous pouvez maintenant le trouver sur votre ordinateur et le partager avec d&#39;autres personnes.
