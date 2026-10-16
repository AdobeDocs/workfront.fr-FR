---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Créer une feuille de temps à usage unique
description: Vous pouvez créer manuellement une feuille de temps à usage unique si vous souhaitez qu’elle ne soit pas récurrente. Lorsque la date de fin de la feuille de temps est atteinte et que vous avez besoin d’autres feuilles de temps, vous devez en créer de nouvelles.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
TQID: https://experienceleague.adobe.com/6ngmKzkpxxHYM7L9Z16JsJKcEW7CdFjJcdp6B6hgTtc
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
source-wordcount: '1048'
ht-degree: 79%
---
# Créer une feuille de temps à usage unique

<!--Audited: 6/2025-->

Vous pouvez créer manuellement une feuille de temps à usage unique si vous souhaitez qu’elle ne soit pas récurrente. Lorsque la date de fin de la feuille de temps est atteinte et que vous avez besoin d’autres feuilles de temps, vous devez en créer de nouvelles.

Pour plus d’informations sur la création d’un profil de feuille de temps qui génère des feuilles de temps récurrentes pour vos utilisateurs et utilisatrices sans intervention de votre part (recommandé), voir [Créer, modifier et affecter des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Pour plus d&#39;informations sur la génération manuelle de feuilles de temps pour tous les utilisateurs du système associés à un profil de feuille de temps, voir [Génération manuelle de feuilles de temps](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

>[!NOTE]
>
>* Il n’est pas possible de créer des feuilles de temps à usage unique pour les groupes.
>* Lors de la création d’une feuille de temps à usage unique, vous ne pouvez pas sélectionner de types d’heures généraux spécifiques à inclure dans votre feuille de temps. Tous les types d’heures généraux activés dans votre système s’affichent dans les feuilles de temps créées manuellement.
>
>Si vous souhaitez sélectionner uniquement certains types d’heures généraux à afficher dans vos feuilles de temps, utilisez un profil de feuille de temps. Pour plus d’informations sur les profils de feuille de temps, voir [Créer, modifier et affecter des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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

## Créer une feuille de temps à usage unique

{{step1-to-timesheets}}

Toutes les feuilles de temps que vous êtes autorisé à consulter s&#39;affichent par défaut.

![Liste des feuilles de temps](assets/list-of-all-timesheets.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez,

     Ou

     Sélectionnez **Mes feuilles de temps** pour afficher uniquement vos feuilles de temps.

     Cette action applique les filtres **Mes approbations de feuille de temps** ou **Ma feuille de temps** à la liste des feuilles de temps.

   * Cliquez sur l’icône **Filtre** ![Icône Filtre](assets/filter-nwepng.png) pour appliquer un filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste de feuille de temps ni dans la liste des filtres si votre administrateur ou administratrice Workfront ou un administrateur ou une administratrice de groupes a supprimé les filtres Mes approbations de feuille de temps et Mes feuilles de temps des contrôles de liste de la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, consultez la section [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Facultatif) Cliquez sur l’icône **Rechercher** ![Icône Rechercher](assets/search-icon.png) pour saisir un mot-clé et rechercher une feuille de temps spécifique. Par exemple, vous pouvez rechercher une période de feuille de temps avec le nom du ou de la propriétaire.

1. (Facultatif) Cliquez sur les icônes **Affichage** ![Icône Affichage](assets/view-icon.png) ou **Regroupement** ![Icône Regroupement](assets/grouping.png) pour appliquer une vue ou un regroupement ou en créer un nouveau.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, voir les articles suivants :

   * [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Cliquez sur **Nouvelle feuille de temps** en haut de la liste des feuilles de temps.

   Saisissez les informations suivantes :

   | Nom du champ | Description |
   | --------- | ---------- |
   | Créer une feuille de temps pour | Commencez à saisir le nom de l’utilisateur ou de l’utilisatrice, une fonction ou une équipe pour lesquels vous créez la feuille de temps, puis cliquez dessus lorsqu’ils s’affichent dans la liste. |
   | Date de début | Il s’agit de la date de début de la feuille de temps. |
   | Date de fin | Il s’agit de la date de fin de la feuille de temps. |
   | Approbateurs | <p>Les approbateurs et approbatrices sont des utilisateurs et utilisatrices qui approuvent la feuille de temps pour les utilisateurs et utilisatrices associés à la feuille de temps. Seules les personnes disposant de droits d’administration sur les feuilles de temps peuvent être définies comme approbateurs ou approbatrices. Pour plus d’informations sur les droits d’administration des feuilles de temps, voir [Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Commencez à saisir les noms des approbateurs et approbatrices de la feuille de temps et sélectionnez-les lorsqu’ils apparaissent dans la liste.</p> <p>Vous pouvez avoir plusieurs approbateurs et approbatrices pour une feuille de temps. Dans ce cas, une fois que l’un des approbateurs ou l’une des approbatrices a approuvé la feuille de temps, celle-ci est marquée comme **Fermée** et disparaît de la liste des approbations de tous les autres approbateurs et approbatrices.</p> |
   | Peut modifier l’heure | <p>Sélectionnez cette option si vous souhaitez permettre aux approbateurs et approbatrices de modifier les heures de la feuille de temps.</p><p>Cette option fonctionne avec le paramètre **Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration** dans la zone Configuration > Feuille de temps et heures > Préférences. Pour plus d’informations, voir [Configurer les préférences en matière de feuilles de temps et d’heures](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).</p><p>Les scénarios suivants sont possibles :</p><p>Lorsque l’option **Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration** est activée :</p><ul><li>Les approbateurs peuvent uniquement approuver et rejeter des feuilles de temps, que l&#39;option **Peut modifier l&#39;heure** soit activée ou non.</li><li>Les personnes responsables des personnes propriétaires de feuilles de temps peuvent consulter uniquement les feuilles de temps de leurs personnes subordonnées directes.</li></ul><p>Lorsque l’option **Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration** est désactivée :</p><ul><li>Lorsque l’option **Peut modifier l’heure** est activée, les approbateurs peuvent envoyer, rouvrir ou fermer la feuille de temps et modifier l’heure.</li><li>Lorsque l’option **Peut modifier l’heure** est désactivée, les approbateurs ne peuvent pas envoyer, rouvrir ou fermer la feuille de temps et ne peuvent pas modifier l’heure. Les approbateurs et approbatrices ne peuvent qu’approuver ou rejeter la feuille de temps.</li><li>Les personnes responsables des personnes propriétaires de feuilles de temps peuvent soumettre, rappeler, rouvrir et modifier les feuilles de temps de leurs personnes subordonnées directes.</li></ul><p>**REMARQUE**</br> Une fois que vous avez soumis une feuille de temps pour approbation, vous ne pouvez plus modifier les heures. Pour remettre une feuille de temps soumise à l’état modifiable, rappelez la feuille de temps ou demandez à l’approbateur ou à l’approbatrice de rejeter la feuille de temps. Pour plus d’informations, voir [Soumettre une feuille de temps pour approbation](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) et [Approuver une feuille de temps](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md). |
   | Hrs supp | Vous pouvez choisir de masquer la case **Heures sup.** sur la feuille de temps. Cette option est désactivée par défaut. |

1. Cliquez sur **Créer une feuille de temps**.

## Lorsque des tâches et des problèmes apparaissent sur les feuilles de temps des utilisateurs et utilisatrices

Une tâche ou un problème attribué à un utilisateur ou à une utilisatrice apparaît automatiquement sur sa feuille de temps si la tâche ou le problème répond à l’un des critères suivants :

* L’utilisateur ou l’utilisatrice a consigné des heures dans la tâche ou le problème.
* Les dates prévues de la tâche ou du problème sont comprises dans les dates de la feuille de temps.
* La tâche ou le problème a une date de début effectif (le statut de la tâche ou du problème est En cours).
* La tâche ou le problème est épinglé à la feuille de temps.
* La date d’achèvement prévue est comprise dans la période de la feuille de temps et le statut est En cours.

Si les préférences de **Préremplir les feuilles de temps avec...** (situées dans les préférences en matière de feuilles de temps et d’heures) sont désélectionnées, la feuille de temps affiche les problèmes et les tâches dont le statut est En cours. Pour plus d’informations sur les préférences en matière de feuilles de temps et d’heures, voir [Configurer les préférences en matière de feuilles de temps et d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
