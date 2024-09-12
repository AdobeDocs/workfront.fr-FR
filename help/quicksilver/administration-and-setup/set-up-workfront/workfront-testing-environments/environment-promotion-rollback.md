---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Restauration d’un package de promotion d’environnement
description: La fonctionnalité de promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Découvrez comment restaurer un package de promotion installé à partir d’un environnement cible.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7e15301dae4b761d19c85a3581bfdb4540ed40fd
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 17%

---

# Restauration d’un package de promotion d’environnement



Après avoir installé un package, vous pouvez le restaurer. Cette opération supprime les modifications apportées par le package dans l’environnement cible et restaure les objets concernés dans leurs configurations précédentes.

Vous pouvez restaurer un module de promotion dans les 24 heures suivant son installation. Au bout de 24 heures, la fonctionnalité de restauration n’est plus disponible pour cette installation.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Plan <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td> <p>Nouveau : Prime ou Ultimate</p><p>Ou</p><p>Actuel : non disponible</p>
   </td>
  </tr>
  <tr>
   <td>Licences <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td> <p>[!UICONTROL Standard]</p><p>Ou</p><p>Actuel : non disponible</p>
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, voir la section [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

* Un package de promotion d’environnement doit être installé avant de pouvoir être restauré.

  Pour plus d’informations, voir [Installation d’un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Déterminer si un déploiement de package spécifique peut être restauré

Pour savoir si un déploiement de package spécifique peut être restauré, tenez compte des points suivants :

* Moins de 24 heures doivent avoir passé depuis l’installation du package.
* Seul le déploiement de module le plus récent peut être restauré.
* Un déploiement en échec peut être restauré.
* Les restaurations ne peuvent pas être restaurées.


## Restauration d’un package de promotion d’environnement installé

1. Accédez à l’environnement dans lequel le package a été installé.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Promotion de l’environnement** dans le volet de navigation de gauche.
1. Sélectionnez le module à restaurer, puis cliquez sur **Déploiements**.
1. Passez la souris sur le déploiement (installation) que vous souhaitez restaurer, puis cliquez sur Restaurer lorsqu’il apparaît à droite de la ligne du déploiement.

   Ou

   Cliquez sur le déploiement que vous souhaitez restaurer, puis cliquez sur **Restaurer le package** dans le coin supérieur droit de l’écran.

   >[!IMPORTANT]
   >
   >Le déploiement doit avoir eu lieu moins de 24 heures avant de le restaurer. Les installations datant de plus de 24 heures ne peuvent pas être restaurées.

1. (Facultatif) Dans la zone d’aperçu de restauration, affichez les modifications qui se produiront lorsque le déploiement sera restauré.
1. Cliquez sur **Restaurer** dans le coin supérieur droit de l’écran.
