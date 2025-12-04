---
title: Présentation de la hiérarchie et du chemin de navigation
description: Vous pouvez créer plusieurs hiérarchies d’espace de travail entre les types d’enregistrements d’un espace de travail.
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Présentation de la hiérarchie et du chemin de navigation

En tant que gestionnaire d&#39;espace de travail, vous pouvez définir des hiérarchies flexibles mais structurées entre les types d&#39;enregistrements et d&#39;autres types d&#39;objets dans Adobe Workfront Planning.

L’utilisation de hiérarchies dans vos espaces de travail présente les avantages suivants :

* Organiser le travail de manière à refléter la manière dont vos équipes planifient, fonctionnent et fournissent les services.
* Les utilisateurs comprennent où ils se trouvent, comment les types d’enregistrements se connectent et comment la stratégie s’exécute en se référant à un ensemble de chemins de navigation qui indiquent leur place dans le système.
* proposer une meilleure navigation et créer de la clarté et de la continuité dans tous les workflows ;
* Les hiérarchies n’imposent pas de structure rigide définie par le système et vous permettent plutôt de définir des flux adaptés au fonctionnement de votre organisation, ce qui offre flexibilité et cohérence à toutes les étapes du travail.

## Remarques concernant l’utilisation des hiérarchies

* En tant que responsable d’espace de travail, vous pouvez créer plusieurs hiérarchies pour un espace de travail.
* Si une connexion entre les types d&#39;enregistrements sélectionnés existe déjà, le système réutilise la connexion existante.
* S’il n’existe aucune connexion, Workfront en crée automatiquement une dans le cadre de la configuration de la hiérarchie.
* Voici des règles pour la configuration de la hiérarchie :
   * Un type d’enregistrement ne peut avoir qu’un seul type d’enregistrement parent dans un espace de travail donné.

     Par exemple, un type d’enregistrement Tactique ne peut pas avoir à la fois un type d’enregistrement Campagne et un type d’enregistrement Objectif en tant que parent dans le même espace de travail.
   * Un enregistrement peut être connecté à plusieurs enregistrements parents du même type, lorsque vous connectez un à plusieurs ou plusieurs à plusieurs types d&#39;enregistrements.
Par exemple, la tactique A peut appartenir à la fois à la campagne X et à la campagne Y.
   * Un type d’enregistrement peut se connecter à plusieurs types d’enregistrement enfants.

     Par exemple, un type d’enregistrement Campaign peut être le parent de plusieurs autres types d’enregistrement, tels que Tactiques, Tests et autres types d’enregistrement.
   * Les hiérarchies peuvent inclure à la fois des types d&#39;enregistrements Planning et des types d&#39;objets Workfront.

     Par exemple, vous pouvez avoir un type d’enregistrement Campagne avec les Tactiques de planification et Projets Workfront comme enfants.
   * Les types d’enregistrements globaux peuvent apparaître dans plusieurs espaces de travail au sein de plusieurs hiérarchies.
   * Les types d’objets Workfront peuvent également apparaître dans plusieurs hiérarchies et dans différents espaces de travail.
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * Les types d’enregistrements avec des connexions qui ne créent pas de champ correspondant sur leurs types d’enregistrements liés peuvent également faire partie de hiérarchies. Les nouvelles connexions créées lors de la configuration de la hiérarchie créent toujours un champ correspondant sur les types d’enregistrements liés, par défaut.

## Remarques concernant l’affichage des chemins de navigation


