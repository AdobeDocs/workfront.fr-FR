---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: FAQ sur la promotion environnementale
description: Consultez les questions fréquentes sur la promotion de l’environnement Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
TQID: 'https://experienceleague.adobe.com/f8iQHTrVCbtK-tIFlCmojM-FQfV0JLCMa6hVfWCEzXY'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 19%
---
# FAQ sur la promotion environnementale

Les questions suivantes sont fréquemment posées sur la promotion de l’environnement :

## La promotion inter-domaines est-elle prise en charge ?

### Réponse

La promotion interdomaines de l’environnement n’est actuellement pas prise en charge. Vous devez effectuer une promotion entre les environnements du même domaine.

## Comment déterminer si notre instance Workfront dispose d’une licence Prime ou Ultimate ?

### Réponse

* Un administrateur Workfront peut localiser la licence de votre entreprise.

  1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche et sélectionnez **[!UICONTROL Configuration]** ![icône Configurer](/help/_includes/assets/gear-icon-setup.png).
  1. Cliquez sur **Système** dans le panneau de gauche.
  1. Pour afficher votre plan Workfront, sélectionnez **Licences**.
Votre plan s’affiche dans le coin supérieur droit de la page.
     ![Localiser le plan](assets/locate-plan.png)

  Ou
* Contactez votre représentant de compte Workfront.

## La promotion de l’environnement est-elle bidirectionnelle ?

### Réponse

Oui. Par exemple, vous pouvez convertir un sandbox en production ou un sandbox en production.

## Le partage est-il pris en charge ?

### Réponse

Non, le partage n’est actuellement pas pris en charge.

## La restauration de package est-elle disponible ?

### Réponse

La restauration des packages est disponible pour le package le plus récent, dans les 24 heures suivant l’installation du package.

## Y aura-t-il une option pour ignorer la promotion de composants individuels ? Où se trouvent les options `Use Existing`, `Overwrite` et `Save with a new Name` », peut-`Skip` être ajouté pour que vous puissiez ignorer la promotion de paramètres individuels ?

### Réponse

* « Utiliser existant » revient à « ignorer » ou à ignorer le déploiement, car il correspond à l’objet existant dans l’environnement cible et n’apporte aucune modification.
* Pour ignorer les objets, nous vous recommandons de supprimer du package de promotion ou directement de l’environnement source les objets que vous ne souhaitez pas installer. Après avoir supprimé les objets, réassemblez le package.
