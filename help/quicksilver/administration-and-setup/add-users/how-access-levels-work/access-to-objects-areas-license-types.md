---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Accès aux objets et aux zones par type de licence
description: Le tableau ci-dessous vous indique le niveau d’accès le plus élevé (Modifier ou Afficher) autorisé par chacune des licences Adobe Workfront pour les objets et les zones de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 0e690cf9cd6351ee89e32b8f1625e8493aa0ad4b
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 17%

---

# Accès aux objets et aux zones par type de licence

Le tableau ci-dessous vous indique le niveau d’accès le plus élevé (Modifier ou Afficher) autorisé par chacune des licences Adobe Workfront pour les objets et les zones de Workfront.

* **Affichage**: L’utilisateur peut consulter et partager des éléments.
* **Modifier**: L’utilisateur peut créer, modifier, supprimer et partager des éléments.

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
        <td>Événements</td>
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
        <td>Afficher*</td>
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
* [Accorder l’accès aux filtres, aux vues et aux regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Accorder l’accès aux équipes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Accorder l’accès aux modèles](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Accorder l’accès au planificateur de scénarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Accorder l’accès aux objectifs Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
