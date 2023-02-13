---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Génération manuelle de feuilles de temps
description: Pour que les modifications que vous avez apportées aux profils de la feuille de temps soient répercutées dans les feuilles de temps actuelles, vous devez d’abord supprimer les feuilles de temps existantes, puis en générer manuellement de nouvelles. Vous pouvez générer manuellement des feuilles de temps à partir de la zone Feuilles de temps ou la zone Diagnostics dans Configuration, comme expliqué dans cet article.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Génération manuelle de feuilles de temps

Pour que les modifications que vous avez apportées aux profils de la feuille de temps soient répercutées dans les feuilles de temps actuelles, vous devez d’abord supprimer les feuilles de temps existantes, puis en générer manuellement de nouvelles. Vous pouvez générer manuellement des feuilles de temps à partir de la zone Feuilles de temps ou la zone Diagnostics dans Configuration, comme expliqué dans cet article.

Pour plus d’informations sur la suppression des feuilles de temps, voir [Suppression de feuilles de temps dans Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un administrateur Workfront ou, si vous travaillez sur des profils de feuille de temps pour un groupe, vous devez être un administrateur de groupe (ou un administrateur Workfront). Pour plus d’informations, voir <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a>.</p> <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Observations relatives aux feuilles de temps générées manuellement

Lorsque vous générez manuellement des feuilles de temps :

* Ils sont générés en fonction des profils de la feuille de temps associés à vos utilisateurs. Les utilisateurs qui ne sont pas associés à des profils de feuille de temps ne reçoivent pas de feuille de temps. 
* Seule la feuille de temps actuelle et celle à suivre sont générées. Workfront ne génère pas deux feuilles de temps pour la même période. Si vous disposez déjà d’une feuille de temps pour une période spécifique, une autre feuille de temps ne sera pas générée lorsque vous utilisez le processus manuel pour générer les feuilles de temps.

## Générer manuellement des feuilles de temps à partir de la zone Heures et heures

Vous pouvez générer manuellement des feuilles de temps au niveau du système ou du groupe à partir de la zone Heures et heures dans Configuration.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Si vous générez des feuilles de temps utilisées dans tout le système, cliquez sur **Fiches horaires et heures.**

   Ou

   Si vous générez des feuilles de temps utilisées par un groupe spécifique, cliquez sur **Groupes**, puis cliquez sur le nom du groupe.

1. Cliquez sur **Profils de feuille de temps**.
1. Cliquez sur **Plus**, puis **Générer des feuilles de calcul**.

   De nouvelles feuilles de temps sont créées pendant deux périodes au maximum pour les utilisateurs associés aux profils de la feuille de temps.

## Générer manuellement des feuilles de calcul au niveau du système à partir de la zone Diagnostics

Vous pouvez générer manuellement des feuilles de temps au niveau du système à partir de la zone Diagnostics dans Configuration.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Développer **Système**, puis cliquez sur **Diagnostics**.

1. Cliquez sur **Diagnostics d’exécution**. 
1. Cliquez sur **Générer des feuilles de calcul**.
