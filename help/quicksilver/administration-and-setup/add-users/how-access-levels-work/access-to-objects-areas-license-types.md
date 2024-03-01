---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Accès aux objets et aux zones par de nouvelles licences
description: Le tableau ci-dessous vous indique le niveau d’accès le plus élevé (Modifier ou Afficher) autorisé par chacune des licences Adobe Workfront pour les objets et les zones de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 7a9232f59e4c6f2eac2995be7d7862295b6bab2c
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 18%

---

# Accès aux objets et aux zones par de nouvelles licences

<!-- Audited: 2/2024 -->

Le tableau ci-dessous vous indique le niveau d’accès le plus élevé (Modifier ou Afficher) autorisé par chacune des licences Adobe Workfront pour les objets et les zones de Workfront.

* **Affichage**: l’utilisateur peut passer en revue et partager des éléments.
* **Modifier**: l’utilisateur peut créer, modifier, supprimer et partager des éléments.

  >[!NOTE]
  >
  >Lorsqu’un autre utilisateur partage un objet, le responsable du partage peut spécifier des autorisations qui limitent sa capacité de modification. Pour plus d’informations, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Standard</td>
        <td>Léger</td>
        <td>Contributeur</td>
        <td>Externe</td>
    </tr>
    <tr>
        <td>Projets</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher (uniquement la page Détails)</td>
        <td>Pas d'accès</td>
    </tr>
    <tr>
        <td>Tâches</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher</td>
        <td>Afficher</td>
    </tr>
    <tr>
        <td>Problèmes</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Pas d'accès</td>
    </tr>
    <tr>
        <td>Portefeuilles</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Pas d'accès</td>
        <td>Pas d'accès</td>
    </tr>
    <tr>
        <td>Programmes</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Pas d'accès</td>
        <td>Pas d'accès</td>
    </tr>
    <tr>
        <td>Rapports, tableaux de bord et calendriers</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Vue*</td>
        <td>Affichage (uniquement pour les calendriers, sans autorisation de partage)</td>
    </tr>
    <tr>
        <td>Filtres, vues et regroupements</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Accès interdit</td>
    </tr>
    <tr>
        <td>Documents</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Affichage (aucune autorisation de partage)</td>
    </tr>
    <tr>
        <td>Utilisateurs</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher</td>
        <td>Afficher</td>
    </tr>
    <tr>
        <td>Équipes</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher</td>
        <td>Accès interdit</td>
    </tr>
    <tr>
        <td>Modèles</td>
        <td>Modifier</td>
        <td>Accès interdit</td>
        <td>Accès interdit</td>
        <td>Accès interdit</td>
    </tr>
    <tr>
        <td>Données financières</td>
        <td>Modifier</td>
        <td>Accès interdit</td>
        <td>Accès interdit</td>
        <td>Accès interdit</td>
    </tr>
    <tr>
        <td>Gestion des ressources</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Accès interdit</td>
        <td>Accès interdit</td>
    </tr>
    <tr>
        <td>Planificateur de scénarios</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Accès interdit</td>
        <td>Accès interdit</td>
    </tr>
    <tr>
        <td>Objectifs Workfront</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Accès interdit</td>
    </tr>
</table>

&#42; Les utilisateurs disposant d’une licence de contributeur peuvent uniquement afficher les rapports, les tableaux de bord et les calendriers qui sont partagés avec eux.

>[!NOTE]
>
>Les utilisateurs disposant d’une licence Light ou d’une licence Contributor ont des capacités de partage limitées. Pour plus d’informations, voir [Présentation des licences](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>Les utilisateurs externes ne peuvent pas rechercher des éléments dans Workfront. Ils peuvent afficher des documents et des calendriers qui sont partagés avec eux. Ils peuvent également voir les utilisateurs qui partagent des éléments avec eux.

Vous trouverez des informations détaillées sur les niveaux d’accès autorisés pour chaque objet et zone dans les articles suivants :

* [Accorder l’accès aux projets](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Accorder l’accès aux documents](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Accorder l’accès aux portefeuilles](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Accorder l’accès aux programmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Accorder l’accès aux filtres, vues et regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Accorder l’accès aux équipes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Accorder l’accès aux modèles](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Accorder l’accès au planificateur de scénarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Accorder l’accès aux objectifs Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
