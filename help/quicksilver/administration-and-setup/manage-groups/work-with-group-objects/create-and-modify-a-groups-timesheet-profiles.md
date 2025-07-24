---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Créer et gérer des profils de feuilles de temps d’un groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et utiliser les profils de feuille de temps pour lesquels les administrateurs et administratrices du groupe, ou l’un de ses sous-groupes, disposent d’un accès administratif.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 90%

---

# Créer et gérer des profils de feuille de temps d’un groupe

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et utiliser les profils de feuille de temps pour lesquels les administrateurs et administratrices du groupe, ou l’un de ses sous-groupes, disposent d’un accès administratif.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td>
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td><p>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</p>
   <p>Vous devez également disposer d’un accès administratif aux feuilles de temps.</p></td>
  </tr>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer et modifier des profils de feuille de temps à l’échelle du groupe

Vous pouvez créer et modifier des profils de feuille de temps à utiliser dans un groupe que vous gérez. Pour obtenir des instructions, voir [Créer, modifier et attribuer des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Supprimer des profils de feuille de temps à l’échelle du groupe

Vous pouvez supprimer les profils de feuille de temps utilisés par un groupe que vous gérez. Pour obtenir des instructions, voir [Supprimer des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Générer manuellement des feuilles de temps de groupe

Pour que les modifications apportées aux profils de feuille de temps de groupe se reflètent dans les feuilles de temps de groupe actuelles, vous devez d’abord supprimer les feuilles de temps existantes, puis en générer de nouvelles manuellement. Pour obtenir des instructions, voir [Générer manuellement des feuilles de temps à partir de la zone Feuilles de temps et heures](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) dans [Générer manuellement des feuilles de temps](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Pour plus d’informations sur la suppression des feuilles de temps de groupe, voir [Supprimer des feuilles de temps dans Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exporter des profils de feuille de temps à l’échelle du groupe

{{step-1-to-setup}}

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe contenant les profils de feuille de temps à exporter.
1. Cliquez sur **Profils de feuille de temps**.
1. Cliquez sur **Exporter** pour exporter la liste des profils de feuille de temps du groupe.
