---
user-type: administrator
product-area: system-administration;user-management
keywords: manage,group,edit,
navigation-topic: create-and-manage-groups
title: Gérer un groupe
description: En tant qu’administrateur de groupe, vous pouvez gérer un groupe que vous administrez à partir de la zone Groupes dans Configuration. S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 1%

---

# Gérer un groupe

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

En tant qu’administrateur de groupe, vous pouvez gérer un groupe que vous administrez à partir de la zone Groupes dans Configuration. S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>Lorsque vous êtes affecté en tant qu’administrateur d’un groupe, vous héritez du rôle d’administrateur de groupe pour tous les sous-groupes qui se trouvent en dessous. Les seuls utilisateurs pouvant gérer un sous-groupe sont les administrateurs de groupe pour le groupe supérieur et les administrateurs de groupe affectés au sous-groupe.

## Conditions d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Gestion des appartenances à un groupe

Vous pouvez ajouter et supprimer des utilisateurs et d’autres groupes d’un groupe que vous administrez. Vous pouvez également affecter des membres du groupe en tant qu’administrateurs au groupe et gérer les informations de profil utilisateur des membres du groupe.

Pour obtenir des instructions, voir [Affichage et gestion des appartenances d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Gestion des détails d’un groupe

Vous pouvez afficher et modifier la page Détails du groupe pour un groupe ou un sous-groupe que vous gérez. Cette page comprend une description du groupe, les noms des chefs d’entreprise et des administrateurs de groupe, ainsi qu’une option qui vous permet de rendre le groupe et tous ses sous-groupes publics ou privés. Et si votre niveau d’accès vous permet de gérer des formulaires personnalisés, vous pouvez joindre un formulaire personnalisé à un groupe.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Pour obtenir des instructions, voir [Affichage et gestion des détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Modification, copie ou suppression d’un groupe

Sans quitter la page principale d’un groupe que vous affichez, vous pouvez rapidement modifier, copier ou supprimer le groupe.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Sélectionnez le groupe, puis cliquez sur Modifier . ![](assets/edit-icon.png), Copier ![](assets/copy-icon.png)ou Supprimer ![](assets/delete.png) Icône

   Si vous avez besoin d’informations sur l’utilisation de la boîte qui s’affiche, reportez-vous à l’une des options suivantes :

   * **Modifier**: [Affichage et gestion des détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copier**: [Créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) dans l’article [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Supprimer**: [Suppression d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configuration des préférences de projet, de tâche et de problème pour un groupe

Si vous êtes administrateur de groupe et que votre groupe a besoin de différents paramètres de projet, de tâche et de préférences d’émission par rapport à ceux définis au niveau du système, vous pouvez demander à l’administrateur Workfront de déverrouiller une préférence pour tous les groupes de l’entreprise. Une fois déverrouillé, vous (ainsi que les administrateurs de groupe pour tous les autres groupes) pouvez le configurer pour les groupes que vous gérez.

Pour obtenir des instructions, voir [Configuration des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et  [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Liste, ajout et configuration de sous-groupes

Vous pouvez créer, afficher, modifier, copier, renommer, exporter et supprimer des sous-groupes sous un groupe que vous administrez.

## Configurer des notifications d’événement pour un groupe

Si un administrateur Workfront vous offre la possibilité de configurer des notifications d’événement pour les groupes de votre entreprise, vous pouvez les configurer pour un groupe que vous administrez. Pour obtenir des instructions, voir [Affichage et configuration des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Création et personnalisation des états d’un groupe

En tant qu’administrateur de groupe, vous pouvez créer des états personnalisés pour un groupe de niveau supérieur que vous gérez. Cela vous donne l’autonomie de votre groupe et vous aide à éliminer le besoin de dizaines de statuts personnalisés à l’échelle de l’entreprise. (Un administrateur Workfront peut également le faire, pour n’importe quel groupe.)

Vous pouvez également personnaliser les états système d’un groupe de niveau supérieur si un administrateur Workfront les a configurés pour autoriser la personnalisation.

Pour obtenir des instructions, voir [Création ou modification d’un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Utilisation des projets d’un groupe

Dans la zone Groupes de la configuration, lorsque vous affichez la page principale d’un groupe que vous administrez, vous pouvez effectuer les opérations suivantes avec des projets :

* répertorier et utiliser (modifier, copier, supprimer et exporter) les projets associés au groupe et à ses sous-groupes et qui ont été partagés avec vous ;
* Création d’un projet pour le groupe

Pour obtenir des instructions, voir [Création et modification des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Afficher et gérer les processus d’approbation d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et utiliser les processus d’approbation pour lesquels les administrateurs du groupe, ou l’un de ses sous-groupes, ont un accès administratif.

Pour obtenir des instructions, voir [Processus de validation au niveau du groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Affichage et gestion des modèles de disposition d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et utiliser le modèle de mise en page pour lequel les administrateurs du groupe, ou de l’un de ses sous-groupes, disposent d’un accès administratif.

Pour obtenir des instructions, voir [Création et modification des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Affichage et gestion des plannings des membres du groupe

Un administrateur de groupe créant une planification pour un groupe doit spécifier le groupe dont les administrateurs vont gérer la planification. En règle générale, il s’agit du groupe pour lequel la planification est en cours de création, mais il peut s’agir d’un groupe différent si l’administrateur du groupe gère plusieurs groupes et spécifie l’un des autres groupes à la place.

Lorsque vous affichez la page principale d’un groupe que vous gérez, si le groupe est désigné comme celui dont les administrateurs peuvent modifier un planning, vous pouvez afficher et gérer le planning à partir de la page du groupe.

Pour obtenir des instructions, voir [Création et modification des plannings d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Affichage et gestion des profils de feuille de temps des membres du groupe

Lorsque vous affichez la page principale d’un groupe que vous administrez, vous pouvez gérer les profils de feuille de temps que vous et les autres administrateurs du groupe (ou de l’un de ses sous-groupes) êtes autorisés à modifier. Pour obtenir des instructions, voir [Création et gestion des profils de feuille de temps d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Affichage et gestion des membres du sous-groupe d’un groupe

Lorsque vous affichez la page principale d’un groupe que vous administrez, vous pouvez afficher et gérer tous les utilisateurs des sous-groupes du groupe. Pour obtenir des instructions, voir [Affichage et gestion des membres de sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Affichage et gestion des équipes d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et travailler avec les équipes associées au groupe ou à l’un de ses sous-groupes.

Pour obtenir des instructions, voir [Création et modification des équipes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Affichage et gestion des entreprises d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et travailler avec les entreprises associées au groupe ou à l’un de ses sous-groupes. Pour obtenir des instructions, voir [Création et modification d’entreprises d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Affichage et gestion des portefeuilles et des programmes d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et utiliser des portefeuilles et des programmes lorsque les deux conditions suivantes sont vraies :

* Ils sont associés au groupe que vous affichez ou à l’un de ses sous-groupes.
* Vous êtes autorisé à les afficher car vous les avez créés ou ils ont été partagés avec vous.

Pour obtenir des instructions, voir [Création et modification des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) et [Créer, modifier et afficher les programmes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Désactiver ou réactiver un groupe

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Vous pouvez conserver un groupe dans son état actif par défaut ou le désactiver.

La désactivation d’un groupe peut s’avérer utile lorsqu’il n’est actuellement pas utilisé, car les utilisateurs ne le voient plus dans les champs de type avant lorsqu’ils recherchent un groupe qu’ils souhaitent associer à un autre objet.

Pour obtenir des instructions sur la façon de rendre un groupe inactif ou actif, voir [Désactivation ou réactivation d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
