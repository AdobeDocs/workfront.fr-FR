---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Générer manuellement des feuilles de temps
description: Pour que les modifications que vous avez apportées aux profils de la feuille de temps soient répercutées dans les feuilles de temps actuelles, vous devez d’abord supprimer les feuilles de temps existantes, puis en générer manuellement de nouvelles. Vous pouvez générer manuellement des feuilles de temps à partir des zones « Feuilles de temps » ou « Diagnostics » dans « Configuration », comme expliqué dans cet article.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 100%

---

# Générer manuellement des feuilles de temps

Pour que les modifications que vous avez apportées aux profils de la feuille de temps soient répercutées dans les feuilles de temps actuelles, vous devez d’abord supprimer les feuilles de temps existantes, puis en générer manuellement de nouvelles. Vous pouvez générer manuellement des feuilles de temps à partir des zones « Feuilles de temps » ou « Diagnostics » dans « Configuration », comme expliqué dans cet article.

Pour plus d’informations sur la suppression des feuilles de temps, consultez la section [Supprimer les feuilles de temps dans Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez faire partie de l’administration Workfront ou, si vous travaillez sur des profils de feuille de temps pour un groupe, vous devez être un administrateur ou une administratrice de groupes (ou faire partie de l’administration Workfront). Pour plus d’informations, consultez la section <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupes</a>.</p> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Considérations sur les feuilles de temps générées manuellement

Ce qui suit est vrai lorsque vous générez manuellement des feuilles de temps :

* Elles sont générées en fonction des profils de feuille de temps associés à vos utilisateurs et à vos utilisatrices. Les utilisateurs et les utilisatrices à qui des profils de feuille de temps ne sont pas affectés ne reçoivent pas de feuille de temps. 
* Seules la feuille de temps actuelle et la feuille de temps suivante sont générées. Workfront ne génère pas deux feuilles de temps pour la même période. Si vous disposez déjà d’une feuille de temps pour une période spécifique, une autre feuille de temps ne sera pas générée lorsque vous utilisez le processus manuel pour générer les feuilles de temps.

## Générer manuellement des feuilles de temps à partir de la zone « Feuilles de temps et heures »

Vous pouvez générer manuellement des feuilles de temps au niveau du système ou du groupe à partir de la zone « Feuilles de temps et heures » dans « Configuration ».

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Si vous générez des feuilles de temps utilisées dans tout le système, cliquez sur **Feuilles de temps et heures.**

   Ou

   Si vous générez des feuilles de temps utilisées par un groupe spécifique, cliquez sur **Groupes**, puis cliquez sur le nom du groupe.

1. Cliquez sur **Profils de feuilles de temps**.
1. Cliquez sur **Plus**, puis **Générer des feuilles de temps**.

   De nouvelles feuilles de temps sont créées pour un maximum de deux périodes pour les utilisateurs et les utilisatrices à qui un profil de feuille de temps est affecté.

## Générer manuellement des feuilles de temps au niveau du système à partir de la zone « Diagnostics »

Vous pouvez générer manuellement des feuilles de temps au niveau du système à partir de la zone « Diagnostics » dans « Configuration ».

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Développez **Système**, puis cliquez sur **Diagnostics**.

1. Cliquez sur **Effectuer des diagnostics**.
1. Cliquez sur **Générer des feuilles de temps**.
