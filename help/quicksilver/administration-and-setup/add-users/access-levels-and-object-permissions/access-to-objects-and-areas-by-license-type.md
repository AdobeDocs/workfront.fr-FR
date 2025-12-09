---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Accès aux objets et zones par type de licence
description: Le tableau ci-dessous indique le niveau d’accès le plus élevé (Modifier ou Afficher) que chacune des licences Adobe Workfront autorise pour les objets et les zones de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 78%

---

# Accéder aux objets et zones par type de licence

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>Les informations de cet article font référence aux niveaux d’accès hérités. Pour plus d’informations sur les nouveaux niveaux d’accès, voir [Présentation des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Le tableau ci-dessous indique le niveau d’accès le plus élevé (Modifier ou Afficher) que chacune des licences Adobe Workfront autorise pour les objets et les zones de Workfront.

* Afficher : l’utilisateur peut réviser et partager des éléments.
* Modifier : l’utilisateur peut créer, modifier, supprimer et partager des éléments.

  >[!NOTE]
  >
  >Lorsqu’une autre personne partage un objet, elle peut spécifier des autorisations qui limitent la capacité des autres à modifier l’objet. Pour plus d’informations sur les nouveaux types de licence, consultez [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

  >[!NOTE]
  >
  >Cet article contient des informations sur l’accès aux objets pour les types de licence hérités. Pour plus d’informations sur les nouveaux types de licence, consultez [Présentation des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) et [Présentation des nouvelles licences](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

|   | Plan | Travail | Vérifier | Demande | Externe |
|---|---|---|---|---|---|
| Projets | Modifier | Modifier (sans autorisations Créer) | Afficher | Afficher (uniquement la page des détails) | Pas d’accès |
| Tâches | Modifier | Modifier | Afficher | Afficher | Pas d’accès |
| Problèmes | Modifier | Modifier | Modifier | Modifier | Pas d’accès |
| Portefeuilles | Modifier | Afficher | Afficher | Pas d’accès | Pas d’accès |
| Programmes | Modifier | Afficher | Afficher | Pas d’accès | Pas d’accès |
| Rapports, tableaux de bord et calendriers | Modifier | Afficher | Afficher | Afficher&#42; | Afficher (uniquement pour les calendriers, sans autorisations de partage) |
| Filtres, vues et regroupements | Modifier | Modifier | Modifier | Modifier | Pas d’accès |
| Documents | Modifier | Modifier | Modifier | Modifier | Afficher (sans autorisations de partage) |
| Utilisateurs | Modifier | Afficher | Afficher | Afficher | Afficher |
| Équipes | Modifier | Modifier | Afficher | Afficher | Pas d’accès |
| Modèles | Modifier | Pas d’accès | Pas d’accès | Pas d’accès | Pas d’accès |
| Données financières | Modifier | Afficher (uniquement la zone Finance dans les détails du projet) | Afficher | Pas d’accès | Pas d’accès |
| Gestion des ressources | Modifier | Afficher | Afficher | Pas d’accès | Pas d’accès |
| Planificateur de scénarios | Modifier | Modifier | Modifier | Pas d’accès | Pas d’accès |
| Objectifs Workfront | Modifier | Modifier | Modifier | Modifier | Pas d’accès |

&#42; Les personnes disposant d’une licence Demande ne peuvent consulter que les rapports, les tableaux de bord et les calendriers qui sont partagés avec elles.

>[!NOTE]
>
>Les utilisateurs disposant d’une licence de révision ou de demande disposent de fonctionnalités de partage limitées. Pour plus d’informations, voir [Vue d’ensemble des licences](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Les utilisateurs et utilisatrices externes ne peuvent pas rechercher des éléments dans Workfront. Ces personnes peuvent consulter les documents et les calendriers qui sont spécifiquement partagés avec elles. Elles peuvent également voir les utilisateurs et utilisatrices qui partagent des éléments avec elles.

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
