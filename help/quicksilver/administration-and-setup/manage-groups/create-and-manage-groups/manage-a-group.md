---
user-type: administrator
product-area: system-administration;user-management
keywords: gérer,regrouper,modifier,
navigation-topic: create-and-manage-groups
title: Gestion d’un groupe
description: En tant qu’administrateur ou administratrice de groupe, vous pouvez gérer un groupe que vous administrez à partir de la zone Groupes dans Configuration. S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 99%

---

# Gérer un groupe

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

En tant qu’administrateur ou administratrice de groupe, vous pouvez gérer un groupe que vous administrez à partir de la zone Groupes dans Configuration. S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>Lorsque vous devenez administrateur ou administratrice d’un groupe, vous héritez du rôle d’administrateur ou administratrice de groupes pour tous les sous-groupes qui lui sont subordonnés. Les seuls personnes qui peuvent gérer un sous-groupe sont les administrateurs et administratrices de groupes du groupe supérieur et les administrateurs et administratrices de groupes affectés au sous-groupe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

+++

## Gérer les membres d’un groupe

Vous pouvez ajouter et supprimer des personnes et d’autres groupes d’un groupe que vous administrez. Vous pouvez également désigner des membres du groupe comme des administrateurs et administratrices du groupe et gérer les informations du profil d’utilisateur ou d’utilisatrice des membres du groupe.

Pour plus d’informations, voir [Afficher et gérer les membres d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Gérer les détails d’un groupe

Vous pouvez afficher et modifier la page Détails du groupe d’un groupe ou d’un sous-groupe que vous gérez. Cette page comprend une description du groupe, les noms de la personne responsable d’entreprise et des administrateurs et administratrices du groupe, ainsi qu’une option permettant de rendre le groupe et tous ses sous-groupes publics ou privés. Et, si votre niveau d’accès vous permet de gérer des formulaires personnalisés, vous pouvez joindre un formulaire personnalisé à un groupe.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Pour plus d’informations, voir [Afficher et gérer les détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Modifier, copier ou supprimer un groupe

Sans quitter la page principale d’un groupe que vous consultez, vous pouvez rapidement modifier, copier ou supprimer le groupe.

{{step-1-to-setup}}

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Sélectionnez le groupe, puis cliquez sur l’icône Modifier ![](assets/edit-icon.png), Copier ![](assets/copy-icon.png) ou Supprimer ![](assets/delete.png).

   Si vous avez besoin d’informations sur l’utilisation de la boîte qui s’affiche, consultez l’un des documents suivants :

   * **Modifier** : [afficher et gérer les détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copier** : [créez un groupe de premier niveau en copiant un groupe ou un sous-groupe existant](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) dans l’article [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

   * **Supprimer** : [supprimer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Configurer les préférences d’un groupe en matière de projets, de tâches et de problèmes

Si vous gérez un groupe et que votre groupe a besoin de paramètres de préférences pour les projets, les tâches et les problèmes différents de ceux définis au niveau du système, vous pouvez demander à l’administrateur ou administratrice Workfront de déverrouiller une préférence pour tous les groupes dans l’ensemble de l’organisation. Une fois déverrouillée, vous (et les administrateurs et administratrices de groupes pour tous les autres groupes) pouvez la configurer pour les groupes que vous gérez.

Pour plus d’informations, voir [Configurer les préférences d’un projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Configurer les préférences d’une tâche ou d’un problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Répertorier, ajouter et configurer des sous-groupes

Vous pouvez créer, afficher, modifier, copier, renommer, exporter et supprimer des sous-groupes sous un groupe que vous gérez.

## Configurer les notifications d’événements pour un groupe

Si un administrateur ou une administratrice Workfront déverrouille la possibilité de configurer les notifications d’événements pour les groupes de votre organisation, vous pouvez les configurer pour un groupe que vous gérez. Pour plus d’informations, voir [Afficher et configurer les notifications d’événements pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Créer et personnaliser des statuts pour un groupe

En tant qu’administrateur ou administratrice de groupes, vous pouvez créer des statuts personnalisés pour un groupe de niveau supérieur que vous gérez. Cela donne de l’autonomie à votre groupe et contribue à éliminer le besoin de dizaines de statuts personnalisés à l’échelle de l’entreprise. (Un administrateur ou une administratrice Workfront peut également effectuer cette opération pour n’importe quel groupe).

Vous pouvez également personnaliser les statuts du système pour un groupe de niveau supérieur si un administrateur ou une administratrice Workfront les a configurés pour permettre la personnalisation.

Pour plus d’informations, voir [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Travailler sur les projets d’un groupe

Dans la zone Groupes de Configuration, lorsque vous affichez la page principale d’un groupe que vous gérez, vous pouvez effectuer les opérations suivantes avec les projets :

* Répertorier et utiliser (modifier, copier, supprimer et exporter) les projets qui sont associés au groupe et à ses sous-groupes et qui ont été partagés avec vous.
* Créer un projet pour le groupe

Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Afficher et gérer les processus d’approbation d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et utiliser les processus d’approbation pour lesquels les administrateurs et administratrices du groupe, ou l’un de ses sous-groupes, ont un accès administratif.

Pour plus d’informations, voir [Processus d’approbation au niveau du groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Afficher et gérer les modèles de mise en page d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et utiliser le modèle de disposition pour lequel l’équipe d’administration du groupe, ou de l’un de ses sous-groupes, dispose d’un accès administratif.

Pour plus d’informations, voir [Créer et modifier les modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Afficher et gérer les plannings des membres du groupe

Un administrateur ou une administratrice de groupes qui crée un planning pour un groupe doit spécifier le groupe dont les administrateurs et administratrices gèreront le planning. Il s’agit généralement du groupe pour lequel le planning est créé, mais il peut s’agir d’un groupe différent si l’administrateur ou administratrice de groupes gère plusieurs groupes et indique l’un d’entre eux à la place.

Lorsque vous affichez la page principale d’un groupe que vous gérez, si le groupe est désigné comme celui dont les administrateurs et administratrices peuvent modifier un planning, vous pouvez afficher et gérer le planning à partir de la page du groupe.

Pour plus d’informations, voir [Créer et modifier les plannings d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Afficher et gérer les profils de feuilles de temps des membres du groupe

Lorsque vous affichez la page principale d’un groupe que vous gérez, vous pouvez gérer les profils de feuilles de temps que vous et les autres administrateurs et administratrices du groupe, ou de l’un de ses sous-groupes, avez l’autorisation de modifier. Pour plus d’informations, voir [Créer et gérer les profils de feuilles de temps d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Afficher et gérer les membres des sous-groupes d’un groupe

Lorsque vous affichez la page principale d’un groupe que vous gérez, vous pouvez afficher et gérer toutes les personnes des sous-groupes du groupe. Pour plus d’informations, voir [Afficher et gérer les personnes membres d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Afficher et gérer les équipes d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez consulter et travailler avec les équipes associées au groupe ou à l’un de ses sous-groupes.

Pour plus d’informations, voir [Créer et modifier les équipes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Afficher et gérer les entreprises d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez consulter et travailler avec les entreprises associées au groupe ou à l’un de ses sous-groupes. Pour plus d’informations, voir [Créer et modifier les entreprises d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Afficher et gérer les portfolios et les programmes d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et travailler avec des portfolios et des programmes lorsque les deux conditions suivantes sont remplies :

* Ils sont associés au groupe que vous consultez ou à l’un de ses sous-groupes.
* Vous disposez des autorisations de les consulter parce que vous les avez créés ou qu’ils ont été partagés avec vous.

Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) et [Créer, modifier et afficher les programmes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Désactiver ou réactiver un groupe

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Vous pouvez conserver un groupe dans son statut actif par défaut ou le désactiver.

La désactivation d’un groupe peut être utile lorsqu’il n’est pas utilisé actuellement, car les personnes ne le voient plus dans les champs de saisie semi-automatique lorsqu’elles recherchent un groupe qu’elles veulent associer à un autre objet.

Pour savoir comment rendre un groupe inactif ou actif, voir [Désactiver ou réactiver un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
