---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Création et gestion des profils de feuille de temps d’un groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et utiliser les profils de feuille de temps pour lesquels les administrateurs du groupe, ou l’un de ses sous-groupes, ont un accès administratif.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 32%

---

# Création et gestion des profils de feuille de temps d’un groupe

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et utiliser les profils de feuille de temps pour lesquels les administrateurs du groupe, ou l’un de ses sous-groupes, ont un accès administratif.

S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

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
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur de groupe du groupe.</p>  <p>Vous devez également disposer d’un accès administratif aux feuilles de calcul. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones</a>.</p>  <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Création et modification de profils de feuille de temps au niveau du groupe

Vous pouvez créer et modifier des profils de feuille de temps à utiliser dans un groupe que vous gérez. Pour obtenir des instructions, voir [Créer, modifier et affecter des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Suppression de profils de feuille de temps au niveau du groupe

Vous pouvez supprimer les profils de feuille de temps utilisés par un groupe que vous gérez. Pour obtenir des instructions, voir [Suppression des profils de la feuille de temps](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Génération manuelle de feuilles de temps de groupe

Pour activer les modifications que vous avez apportées pour regrouper les profils de feuille de temps à refléter dans les feuilles de temps de groupe actuelles, vous devez d’abord supprimer les feuilles de temps existantes, puis en générer manuellement de nouvelles. Pour plus d’informations, voir [ Génération manuelle de feuilles de temps à partir de la zone Heures et heures](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) dans [ Génération manuelle de feuilles de temps](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Pour plus d’informations sur la suppression des feuilles de temps de groupe, voir [Suppression des feuilles de temps dans Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exportation de profils de feuille de temps au niveau du groupe

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).
1. Cliquez sur **Groups**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe avec les profils de la feuille de temps à exporter.
1. Cliquez sur **Profils de feuille de temps**.
1. Cliquez sur **Exporter** pour exporter la liste des profils de feuille de temps pour le groupe.
