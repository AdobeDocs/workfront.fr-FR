---
title: Octroi de l’accès aux filtres, vues et regroupements
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: En tant que personne membre de l’administration Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur ou d’une utilisatrice aux contrôles de filtrage, d’affichage et de regroupement pour les listes et les rapports.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 97%

---

# Accorder l’accès aux filtres, aux vues et aux regroupements

En tant que personne membre de l’administration Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur ou d’une utilisatrice aux contrôles de filtrage, d’affichage et de regroupement pour les listes et les rapports, comme expliqué dans [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Pour plus d’informations sur les contrôles de filtrage, d’affichage et de regroupement, consultez la section [Éléments de création de rapports : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer l’accès des utilisateurs et des utilisatrices aux filtres, aux vues et aux regroupements à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou à modifier le niveau d’accès, comme expliqué dans la section [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur les boutons **Vue** ou **Modifier** à droite des filtres, puis sélectionnez les capacités que vous souhaitez accorder sous **Ajuster vos paramètres**.

   ![](assets/gear-icon-filters-dashboards-groupings.png)

   Par défaut, les utilisateurs et les utilisatrices disposant d’une licence Plan, Travail, Révision ou Demande disposent de toutes les capacités de visualisation et de modification. Les utilisateurs et les utilisatrices disposant d’une licence d’utilisation externe n’ont pas accès aux filtres, aux vues et aux regroupements.

   <!--If this changes, undraft section with table below
   -->

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et domaines dans le niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles listés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’attribuer à un utilisateur ou à une utilisatrice. Pour plus d’informations, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

Ce tableau détaille les actions que les utilisateurs et les utilisatrices de chaque catégorie de licence peuvent effectuer avec les filtres, les vues et les regroupements, selon les permissions accordées par une personne membre de l’administration Workfront. Pour plus d’informations sur les types de licences Workfront, consultez la section [Vue d’ensemble des licences Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> Action </th>
<th> Planificateur </th>
<th> Employé </th>
<th> Réviseur </th>
<th> Demandeur ou demandeuse </th>
</tr>
</thead>
<tbody>
<tr>
<td>Modifier des filtres, des vues et des regroupements</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Créer des filtres, des vues et des regroupements</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Afficher des filtres, des vues et des regroupements</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Supprimer des filtres, des vues et des regroupements</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Partager des filtres, des vues et des regroupements</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Partager des filtres, des vues et des regroupements au niveau du système</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>
