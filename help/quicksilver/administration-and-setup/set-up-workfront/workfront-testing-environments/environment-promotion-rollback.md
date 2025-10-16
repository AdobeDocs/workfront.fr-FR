---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Restaurer un package de promotion d’environnement
description: La fonctionnalité de promotion d’environnement est destinée à fournir la possibilité de déplacer des objets liés à la configuration d’un environnement à un autre. Découvrez comment restaurer un package de promotion installé à partir d’un environnement cible.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 15%

---

# Restaurer un package de promotion d’environnement



Après avoir installé un package, vous pouvez le restaurer. Cela supprime les modifications apportées par le package dans l’environnement cible et restaure les objets affectés à leurs configurations précédentes.

Vous pouvez restaurer un package de promotion dans les 24 heures suivant son installation. Au bout de 24 heures, la fonctionnalité de restauration n’est plus disponible pour cette installation.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Licences Workfront</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td><p>Vous devez être un administrateur ou une administratrice Workfront.</p>
   </td>
  </tr>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

* Un package de promotion d’environnement doit être installé avant de pouvoir être restauré.

  Pour obtenir des instructions, voir [Installation d’un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Déterminer si un déploiement de package spécifique peut être restauré

Pour savoir si un déploiement de package spécifique peut être restauré, tenez compte des points suivants :

* Moins de 24 heures doivent s’être écoulées depuis l’installation du package.
* Seul le déploiement de package le plus récent peut être restauré.
* Un déploiement ayant échoué peut être restauré.
* Les restaurations ne peuvent pas être restaurées.


## Restaurer un package de promotion d’environnement installé

1. Accédez à l’environnement dans lequel le package a été installé.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Promotion de l’environnement** dans le volet de navigation de gauche.
1. Sélectionnez le package à restaurer, puis cliquez sur **Déploiements**.
1. Pointez sur le déploiement (installation) à restaurer, puis cliquez sur Restaurer lorsqu’il apparaît à droite de la ligne de ce déploiement.

   Ou

   Cliquez sur le déploiement à restaurer, puis cliquez sur **Restaurer le package** dans le coin supérieur droit de l’écran.

   >[!IMPORTANT]
   >
   >Le déploiement doit s’être produit moins de 24 heures avant que vous ne le restauriez. Les installations de plus de 24 heures ne peuvent pas être restaurées.

1. (Facultatif) Dans la zone Aperçu de la restauration , affichez les modifications qui se produiront lorsque le déploiement sera restauré.
1. Cliquez sur **Restaurer** dans le coin supérieur droit de l’écran.
