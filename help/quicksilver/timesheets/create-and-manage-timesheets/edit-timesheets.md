---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Modifier les informations de la feuille de temps
description: Les utilisateurs disposant d’un accès administratif aux feuilles de temps peuvent modifier les informations des feuilles de temps existantes dans Adobe Workfront. Vous pouvez par exemple modifier la personne propriétaire, les approbateurs et approbatrices ou la période de la feuille de temps.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 69%
---
# Modifier les informations de la feuille de temps

Les utilisateurs disposant d’un accès administratif aux feuilles de temps peuvent modifier les informations des feuilles de temps existantes dans Adobe Workfront. Vous pouvez par exemple modifier la personne propriétaire, les approbateurs et approbatrices ou la période de la feuille de temps.

Vous pouvez modifier les informations d’une seule feuille de temps ou modifier plusieurs feuilles de temps en masse.

>[!IMPORTANT]
>
>Si des utilisateurs et utilisatrices sont associés aux profils de feuille de temps et que les feuilles de temps sont générées automatiquement, les modifications que vous apportez aux feuilles de temps existantes ne se répercutent pas sur les feuilles de temps qui seront générées pour les dates futures. Les paramètres de toutes les feuilles de temps générées automatiquement sont définis dans les profils de feuille de temps. Pour plus d’informations, voir [Créer des profils de feuille de temps](../create-and-manage-timesheets/create-timesheet-profiles.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td><p>Accès administratif aux feuilles de temps</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier les feuilles de temps

{{step1-to-timesheets}}

Toutes les feuilles de temps que vous êtes autorisé à consulter s&#39;affichent par défaut.

![Liste des feuilles de temps](assets/list-of-all-timesheets.png)

1. (Facultatif) Cliquez sur l’icône **rechercher** ![Icône Rechercher](assets/search-icon.png) et saisissez un mot-clé pour rechercher une feuille de temps spécifique. Par exemple, vous pouvez rechercher une période de la feuille de temps ou le nom de la personne propriétaire.

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez,

     Ou

     Sélectionnez **Mes feuilles de temps** pour afficher uniquement vos feuilles de temps.

     Cette action applique les filtres **Mes approbations de feuille de temps** ou **Ma feuille de temps** à la liste des feuilles de temps.

   * Cliquez sur l’icône **Filtre** ![Icône Filtre](assets/filter-nwepng.png) pour appliquer un filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste des feuilles de temps ou dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé ces filtres des contrôles de liste dans la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, consultez la section [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Facultatif) Cliquez sur les icônes **Affichage** ![Icône Affichage](assets/view-icon.png) ou **Regroupement** ![Icône Regroupement](assets/grouping.png) pour appliquer une vue ou un regroupement ou en créer un nouveau.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, voir les articles suivants :

   * [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Sélectionnez une ou plusieurs feuilles de temps, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) en haut de la liste des feuilles de temps.
1. Affichez ou saisissez les informations suivantes :

   | Nom du champ | Description |
   | --------- | ---------- |
   | Propriétaire | <p>Il s’agit du nom de la personne pour laquelle la feuille de temps a été créée. Vous ne pouvez pas modifier ce champ.</p><p>Ce champ ne s’affiche pas lorsque vous sélectionnez plusieurs feuilles de temps.</p> |
   | Date de début | Il s’agit de la date de début de la feuille de temps. |
   | Date de fin | Il s’agit de la date de fin de la feuille de temps. |
   | Statut | <p>Il s’agit du statut de la feuille de temps. Voici les options de statut possibles de la feuille de temps :</p><ul><li>**Ouverte** : la feuille de temps est ouverte et les entrées d’heure peuvent être modifiées.</li><li>**Envoyée** : la feuille de temps est soumise pour approbation aux approbateurs et approbatrices désignés.</li><li>**Rejetée** : la feuille de temps n’a pas été approuvée par les approbateurs et approbatrices et est à nouveau disponible pour que l’utilisateur ou l’utilisatrice puisse modifier les entrées de temps.</li><li>**Fermée** : la feuille de temps est fermée par l’utilisateur ou l’utilisatrice,ou approuvée par l’approbateur ou l’approbatrice ; elle est donc maintenant fermée. Vous ne pouvez pas ajouter d’heures à une feuille de temps fermée.</li></ul> |
   | Approbateurs | <p>Les approbateurs et approbatrices sont des utilisateurs et utilisatrices qui approuvent la feuille de temps pour les utilisateurs et utilisatrices associés à la feuille de temps. Seules les personnes disposant de droits d’administration sur les feuilles de temps peuvent être définies comme approbateurs ou approbatrices. Pour plus d’informations sur les droits d’administration des feuilles de temps, voir [Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Commencez à saisir les noms des approbateurs et approbatrices de la feuille de temps et sélectionnez-les lorsqu’ils apparaissent dans la liste.</p> <p>Vous pouvez avoir plusieurs approbateurs et approbatrices pour une feuille de temps. Dans ce cas, une fois que l’un des approbateurs ou l’une des approbatrices a approuvé la feuille de temps, celle-ci est marquée comme **Fermée** et disparaît de la liste des approbations de tous les autres approbateurs et approbatrices.</p> |
   | Peut modifier l’heure | <p>Sélectionnez cette option si vous souhaitez permettre aux approbateurs et approbatrices de modifier les heures de la feuille de temps.</p><p>Cette option n’est pas disponible lorsque vous sélectionnez plusieurs feuilles de temps.</p> |
   | Hrs supp | <p>Vous pouvez choisir de masquer la zone Heures supplémentaires sur la feuille de temps.</p><p>Cette option est désactivée par défaut.</p> |

1. Cliquer sur **Enregistrer**.
