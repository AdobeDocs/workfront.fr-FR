---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Accès aux objets et zones par de nouvelles licences
description: Le tableau ci-dessous indique le niveau d’accès le plus élevé (Modifier ou Afficher) que chacune des licences Adobe Workfront autorise pour les objets et les zones de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 3ebff5f28d4142203c6ce5486ce40484d88f0a5d
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 81%

---

# Accéder aux objets et aux zones avec de nouvelles licences

{{highlighted-preview}}

<!-- Audited: 2/2024 -->

>[!NOTE]
>
>Les informations de cet article se rapportent aux niveaux d’accès actuels. Pour plus d&#39;informations sur les niveaux d&#39;accès hérités, voir [Présentation des niveaux d&#39;accès](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Le tableau ci-dessous indique le niveau d’accès le plus élevé (Modifier ou Afficher) que chacune des licences Adobe Workfront autorise pour les objets et les zones de Workfront.

* **Afficher** : la personne peut consulter et partager des éléments.
* **Modifier** : la personne peut créer, modifier, supprimer et partager des éléments.

  >[!NOTE]
  >
  >Lorsqu’une autre personne partage un objet, elle peut spécifier des autorisations qui limitent la capacité des autres à modifier l’objet. Pour plus d’informations, voir [Vue d’ensemble du partage des autorisations sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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
        <td><span class="preview">Modifier **</span></td>
        <td>Afficher</td>
        <td>Pas d’accès
</td>
    </tr>
    <tr>
        <td>Tâches</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Problèmes</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Portefeuilles</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Programmes</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Rapports, tableaux de bord et calendriers</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Afficher*</td>
        <td>Afficher (uniquement pour les calendriers, sans autorisations de partage)</td>
    </tr>
    <tr>
        <td>Filtres, vues et regroupements</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Documents</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Afficher (sans autorisations de partage)</td>
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
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Modèles</td>
        <td>Modifier</td>
        <td>Pas d’accès</td>
        <td>Pas d’accès</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Données financières</td>
        <td>Modifier</td>
        <td>Pas d’accès</td>
        <td>Pas d’accès</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Gestion des ressources</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Pas d’accès</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Planificateur de scénarios</td>
        <td>Modifier</td>
        <td>Afficher</td>
        <td>Pas d’accès</td>
        <td>Pas d’accès</td>
    </tr>
    <tr>
        <td>Objectifs Workfront</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Modifier</td>
        <td>Pas d’accès</td>
    </tr>
</table>

&#42; Les personnes disposant d’une licence Contributeur ne peuvent consulter que les rapports, les tableaux de bord et les calendriers qui sont partagés avec elles.

<span class="preview">&#42;&#42; Les utilisateurs disposant d’une licence light ne peuvent enregistrer le temps au niveau du projet que lorsque l’accès en modification est activé. Ils ne peuvent pas créer, modifier, supprimer ni partager des projets. Le niveau par défaut pour les utilisateurs et utilisatrices légers est Affichage.</span>

>[!NOTE]
>
>* Les personnes disposant d’une licence Light ou d’une licence Contributeur des capacités de partage limitées. Pour plus d’informations, voir [Vue d’ensemble des licences](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>* Les utilisateurs et utilisatrices externes ne peuvent pas rechercher des éléments dans Workfront. Ces personnes peuvent consulter les documents et les calendriers qui sont spécifiquement partagés avec elles. Elles peuvent également voir les utilisateurs et utilisatrices qui partagent des éléments avec elles.
>
>* Les utilisateurs contributeurs et les utilisateurs externes ne peuvent pas voir le contenu partagé à l’échelle du système.  Il doit être partagé explicitement avec eux.

Vous trouverez des informations détaillées sur les niveaux d’accès autorisés pour chaque objet et zone dans les articles suivants :

* [Accorder l’accès aux projets](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Accorder l’accès aux documents](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Accorder l’accès aux portfolios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Accorder l’accès aux programmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Accorder l’accès aux filtres, aux vues et aux regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Accorder l’accès aux équipes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Accorder l’accès aux modèles](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Accorder l’accès au planificateur de scénarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Accorder l’accès à Objectifs Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
