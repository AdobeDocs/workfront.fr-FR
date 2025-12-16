---
title: Présentation de la hiérarchie et du chemin de navigation
description: Vous pouvez créer plusieurs hiérarchies d’espace de travail entre les types d’enregistrements d’un espace de travail.
hide: true
hidefromtoc: true
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '752'
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

Les hiérarchies sont des connexions entre les types d’enregistrements ou entre les types d’enregistrements et un projet Workfront.

Pour plus d’informations sur la création de hiérarchies, voir [Création de hiérarchies d’espace de travail](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

L’utilisation de hiérarchies dans vos espaces de travail présente les avantages suivants :

* Organiser le travail de manière à refléter la manière dont vos équipes planifient, fonctionnent et fournissent les services.
* Pour que les utilisateurs puissent comprendre où ils se trouvent, comment les types d’enregistrements se connectent et comment la stratégie s’exécute en se référant à un ensemble de chemins de navigation qui indiquent leur place dans le système.
* Pour offrir une meilleure navigation et créer de la clarté et de la continuité dans tous les workflows.
* Définir des flux adaptés au fonctionnement de votre organisation, en offrant flexibilité et cohérence à toutes les étapes du travail.

## Remarques concernant l’utilisation des hiérarchies

* Vous pouvez créer plusieurs hiérarchies pour un espace de travail.
* Vous pouvez avoir jusqu&#39;à 4 types d&#39;enregistrements et d&#39;objets connectés dans une seule hiérarchie.
* Vous ne pouvez connecter que les types d&#39;objets suivants dans une hiérarchie d&#39;espace de travail :
   * Types d’enregistrements appartenant à l’espace de travail dans lequel vous créez les hiérarchies.
   * Projets Workfront. Les projets Workfront ne peuvent pas être ajoutés en tant que parents d’autres types d’enregistrements. Ils sont toujours le dernier enfant d&#39;une hiérarchie.
* Vous ne pouvez pas ajouter les types d&#39;objets suivants dans une hiérarchie :
   * Types d’enregistrements d’autres espaces de travail, même s’ils sont définis comme des types d’enregistrements connectables ou globaux. Vous pouvez ajouter des types d&#39;enregistrements globaux aux hiérarchies uniquement lorsqu&#39;ils ont été ajoutés à l&#39;espace de travail à partir duquel vous créez la hiérarchie.
   * Tous les autres objets Workfront.
   * AEM Assets
* Les hiérarchies peuvent inclure à la fois des types d&#39;enregistrements Planning et des projets Workfront.

      Par exemple, vous pouvez avoir un type d’enregistrement Campagne avec les Tactiques de planification et Projets Workfront comme enfants dans la même hiérarchie d’espace de travail.
  * Si une connexion entre les types d&#39;enregistrements sélectionnés existe déjà, le système réutilise la connexion existante.
* S’il n’existe aucune connexion, Workfront en crée une dans le cadre de la configuration de la hiérarchie.
* Le paramètre **Créer le champ correspondant sur le type d&#39;enregistrement lié** doit être activé pour le champ connecté pour les enregistrements et objets que vous souhaitez inclure dans une hiérarchie.
* Voici des règles pour la configuration de la hiérarchie :
   * Un type d’enregistrement ne peut avoir qu’un seul type d’enregistrement parent dans un espace de travail donné.

     Par exemple, un type d’enregistrement Tactique ne peut pas avoir à la fois un type d’enregistrement Campagne et un type d’enregistrement Objectif en tant que parent dans le même espace de travail.
   * Un type d’enregistrement peut être le parent dans plusieurs hiérarchies.

     Par exemple, vous pouvez avoir trois hiérarchies différentes dans un espace de travail et chacune d’elles peut avoir comme type d’enregistrement parent Campagnes .
   * Un enregistrement peut être connecté à plusieurs enregistrements parents du même type, lorsque vous connectez un à plusieurs ou plusieurs à plusieurs types d&#39;enregistrements.
Par exemple, la tactique A peut appartenir à la fois à la campagne X et à la campagne Y.
   * Un type d’enregistrement peut se connecter à plusieurs types d’enregistrement enfants.

     Par exemple, un type d’enregistrement Campaign peut être le parent de plusieurs autres types d’enregistrement, tels que Tactiques, Tests et autres types d’enregistrement.
   * Les types d’enregistrements globaux peuvent apparaître dans plusieurs espaces de travail à l’intérieur de plusieurs hiérarchies, après leur ajout à ces espaces de travail.

     Par exemple, si une campagne est un type d’enregistrement global et fait partie d’une hiérarchie dans Workspace 1, elle peut être ajoutée en tant que type d’enregistrement existant dans Workspace 2 et y faire partie d’une hiérarchie. Cependant, il ne peut pas faire partie d’une hiérarchie dans Workspace 2 uniquement lorsqu’il est désigné comme type d’enregistrement global dans Workspace 1, mais pas ajouté à Workspace 2.


## Remarques concernant l’affichage des chemins de navigation

Lorsque vous créez des hiérarchies entre les types d&#39;enregistrements, elles génèrent des chemins de navigation pour les enregistrements appartenant à ces types d&#39;enregistrements.

Par exemple, si vous créez une hiérarchie et que vous connectez des campagnes aux Tactiques, puis aux Activités et enfin aux Projets, lorsque vous accédez à un enregistrement de l’un des types connectés dans la hiérarchie, vous pouvez voir où l’enregistrement est placé dans la hiérarchie.

Tenez compte des points suivants :

* Si un type d&#39;enregistrement fait partie de plusieurs hiérarchies, vous pouvez basculer entre les hiérarchies à partir du chemin de navigation de l&#39;enregistrement sur la page de l&#39;enregistrement.
* Les chemins de navigation fonctionnent dans Workfront et Planning.

  Par exemple, lorsque vous étudiez un projet lié aux campagnes et tactiques Planning, ainsi qu’aux portfolios et programmes Workfront, vous pouvez basculer entre les deux types d’objets Planning et Workfront à partir du chemin de navigation.

  Pour plus d’informations, voir [Création de hiérarchies d’espaces de travail](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


