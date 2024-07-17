---
title: Accorder l’accès aux filtres, vues et regroupements
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux contrôles de filtrage, d’affichage et de regroupement pour les listes et les rapports.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 24%

---

# Accorder l’accès aux filtres, vues et regroupements

En tant qu&#39;administrateur Adobe Workfront, vous pouvez utiliser un niveau d&#39;accès pour définir l&#39;accès d&#39;un utilisateur aux contrôles de filtrage, d&#39;affichage et de regroupement pour les listes et les rapports, comme expliqué dans la [Présentation des niveaux d&#39;accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Pour plus d’informations sur les contrôles de filtrage, d’affichage et de regroupement, voir [Éléments de reporting : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer l’accès des utilisateurs aux filtres, aux vues et aux regroupements à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d&#39;accès, comme expliqué dans la section [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de Filtres, puis sélectionnez les fonctionnalités que vous souhaitez accorder sous **{Affiner vos paramètres**.

   ![](assets/gear-icon-filters-dashboards-groupings.jpg)

   Par défaut, les utilisateurs disposant d’une licence Plan, Travail, Réviseur ou Demande disposent de fonctionnalités d’affichage et de modification complètes. Les utilisateurs disposant d’une licence d’utilisateur externe n’ont pas accès aux filtres, aux vues et aux regroupements.

   <!--If this changes, undraft section with table below
   -->

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, passez à l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

Ce tableau répertorie ce qu’un administrateur Workfront peut permettre aux utilisateurs de chaque type de licence de faire avec les filtres, les vues et les regroupements. Pour plus d’informations sur les types de licence Workfront, voir [Présentation des licences Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

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
<th> Demandeur </th>
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
<td>Affichage des filtres, des vues et des regroupements</td>
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
<td>Partage de filtres, de vues et de regroupements</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Partage des filtres, vues et regroupements à l’échelle du système</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>
