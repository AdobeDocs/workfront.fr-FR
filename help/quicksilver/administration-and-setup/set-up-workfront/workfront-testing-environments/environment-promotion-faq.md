---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: FAQ sur la promotion de l’environnement
description: Explorez les questions les plus fréquemment posées concernant la promotion de l’environnement Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 4ea4d7d8fd16d4c4d7c2fe5f7adb15c2b44b6705
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 16%

---

# FAQ sur la promotion de l’environnement

Les questions suivantes sont fréquemment posées à propos de la promotion de l’environnement :

## La promotion inter-domaines est-elle prise en charge ?

### Réponse

La promotion de l’environnement inter-domaines n’est actuellement pas prise en charge. Vous devez promouvoir entre les environnements d’un même domaine.

## L’Adobe de Business Platform / IMS est-il un prérequis pour la promotion de l’environnement ?

### Réponse

Non. La promotion de l’environnement est disponible pour les instances Workfront IMS et non IMS.

## Comment savoir si notre instance Workfront est sous une licence Prime ou Ultimate ?

### Réponse

* Un administrateur Workfront peut localiser la licence de votre entreprise.

   1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche et sélectionnez **[!UICONTROL Configuration]** ![icône Configurer](/help/_includes/assets/gear-icon-setup.png).
   1. Cliquez sur **Système** dans le panneau de gauche.
   1. Pour afficher votre formule Workfront, sélectionnez **Licences**.
Votre plan s’affiche près du coin supérieur droit de la page.
      ![](assets/locate-plan.png)

  Ou
* Contactez votre représentant de compte Workfront.

## La promotion de l’environnement est-elle bidirectionnelle ?

### Réponse

Oui. Vous pouvez, par exemple, convertir des environnements de test en environnement de production ou de production en environnement de test.

## Le partage est-il pris en charge ?

### Réponse

Non, le partage n’est actuellement pas pris en charge.

## La restauration de package est-elle disponible ?

### Réponse

La restauration de package est disponible pour le package le plus récent, dans les 24 heures suivant l’installation du package.

## Y aura-t-il une option pour ignorer la promotion de composants individuels ? Là où les options `Use Existing`, `Overwrite` et `Save with a new Name`&quot; existent, peut-on ajouter `Skip` afin que vous puissiez ignorer la promotion de paramètres individuels ?

### Réponse


* &quot;Utiliser existant&quot; est la même chose que &quot;sauter&quot; ou ignorer le déploiement, car il correspond à l’objet existant dans l’environnement cible et n’effectue aucune modification.
* Pour ignorer les objets, il est recommandé de supprimer les
tous les objets que vous ne souhaitez pas installer à partir du package de promotion ou directement depuis l’environnement source. Après avoir supprimé les objets, réassemblez le module.
