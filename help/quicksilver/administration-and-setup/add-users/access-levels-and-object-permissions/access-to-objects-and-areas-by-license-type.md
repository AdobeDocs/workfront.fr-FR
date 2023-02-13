---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Accès aux objets et aux zones par type de licence
description: Le tableau ci-dessous vous indique le niveau d’accès le plus élevé (Modifier ou Afficher) autorisé par chacune des licences Adobe Workfront pour les objets et les zones de Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 19%

---

# Accès aux objets et aux zones par type de licence

Le tableau ci-dessous vous indique le niveau d’accès le plus élevé (Modifier ou Afficher) autorisé par chacune des licences Adobe Workfront pour les objets et les zones de Workfront.

* **Affichage**: L’utilisateur peut consulter et partager des éléments.
* **Modifier**: L’utilisateur peut créer, modifier, supprimer et partager des éléments.

   >[!NOTE]
   >
   >Lorsqu’un autre utilisateur partage un objet, le responsable du partage peut spécifier des autorisations qui limitent sa capacité de modification. Pour plus d’informations, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | Plan | Travail | Vérifier | Demande | Externe |
|---|---|---|---|---|---|
| Projets | Modifier | Modifier (sans autorisations de création) | Afficher | Afficher (uniquement la page Détails) | Pas d&#39;accès |
| Tâches | Modifier | Modifier | Afficher | Afficher | Afficher |
| Événements | Modifier | Modifier | Modifier | Modifier | Pas d&#39;accès |
| Portefeuilles | Modifier | Afficher | Afficher | Pas d&#39;accès | Pas d&#39;accès |
| Programmes | Modifier | Afficher | Afficher | Pas d&#39;accès | Pas d&#39;accès |
| Rapports, tableaux de bord et calendriers | Modifier | Afficher | Afficher | Afficher&#42; | Affichage (uniquement pour les calendriers, sans autorisation de partage) |
| Filtres, vues et regroupements | Modifier | Modifier | Modifier | Modifier | Accès interdit |
| Documents | Modifier | Modifier | Modifier | Modifier | Affichage (aucune autorisation de partage) |
| Utilisateurs | Modifier | Afficher | Afficher | Afficher | Afficher |
| Équipes | Modifier | Modifier | Afficher | Afficher | Accès interdit |
| Modèles | Modifier | Accès interdit | Accès interdit | Accès interdit | Accès interdit |
| Données financières | Modifier | Afficher (uniquement la zone Finance dans les détails du projet) | Afficher | Accès interdit | Accès interdit |
| Gestion des ressources | Modifier | Afficher | Afficher | Accès interdit | Accès interdit |
| Planificateur de scénarios | Modifier | Modifier | Modifier | Accès interdit | Accès interdit |
| Objectifs Workfront | Modifier | Modifier | Modifier | Modifier | Accès interdit |

&#42; Les utilisateurs disposant d’une licence Request peuvent afficher uniquement les rapports, les tableaux de bord et les calendriers qui sont partagés avec eux.

>[!NOTE]
>
>Les utilisateurs disposant d’une licence de révision ou d’une licence de demande disposent de fonctionnalités de partage limitées. Pour plus d’informations, voir [Présentation des licences Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
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
