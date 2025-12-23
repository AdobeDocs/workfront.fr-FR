---
title: Présentation de la hiérarchie et du chemin de navigation
description: Vous pouvez créer plusieurs hiérarchies d’espaces de travail entre les types d’enregistrements d’un espace de travail, après avoir connecté les types d’enregistrements.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 1%

---



# Présentation de la hiérarchie et du chemin de navigation

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

En tant que gestionnaire d&#39;espace de travail, vous pouvez définir des hiérarchies flexibles mais structurées entre les types d&#39;enregistrements connectés et d&#39;autres types d&#39;objets dans Adobe Workfront Planning.

Les hiérarchies sont des connexions entre les types d’enregistrements ou entre les types d’enregistrements et un projet Workfront.

Pour plus d’informations sur la création de hiérarchies, voir [Création de hiérarchies d’espace de travail](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

L’utilisation de hiérarchies dans vos espaces de travail présente les avantages suivants :

* Organiser le travail de manière à refléter la manière dont vos équipes planifient, fonctionnent et fournissent les services.
* Pour que les utilisateurs puissent comprendre où ils se trouvent, comment les types d’enregistrements se connectent et comment la stratégie s’exécute en se référant à un ensemble de chemins de navigation qui indiquent leur place dans le système.
* Pour offrir une meilleure navigation et créer de la clarté et de la continuité dans tous les workflows.
* Définir des flux adaptés au fonctionnement de votre organisation, en offrant flexibilité et cohérence à toutes les étapes du travail.

## Remarques concernant l’utilisation des hiérarchies

* Vous pouvez créer jusqu’à 5 hiérarchies pour un espace de travail.
* Vous pouvez avoir jusqu&#39;à 4 types d&#39;enregistrements et d&#39;objets connectés dans une seule hiérarchie.
* Vous ne pouvez connecter que les types d&#39;objets suivants dans une hiérarchie d&#39;espace de travail :
   * Types d’enregistrements appartenant à l’espace de travail dans lequel vous créez les hiérarchies.
   * Projets Workfront. Les projets Workfront ne peuvent pas être ajoutés en tant que parents d’autres types d’enregistrements. Il s&#39;agit toujours du dernier type d&#39;objet d&#39;une hiérarchie.
* Vous ne pouvez pas ajouter les types d&#39;objets suivants dans une hiérarchie :
   * Types d’enregistrements d’autres espaces de travail, même s’ils sont définis comme des types d’enregistrements connectables ou globaux. Vous pouvez ajouter des types d&#39;enregistrements globaux aux hiérarchies uniquement lorsqu&#39;ils ont été ajoutés à l&#39;espace de travail à partir duquel vous créez la hiérarchie.
   * Tous les autres objets Workfront.
   * AEM Assets.
* Les hiérarchies peuvent inclure à la fois des types d&#39;enregistrements Planning et des projets Workfront.

  Par exemple, vous pouvez avoir un type d’enregistrement Campagne avec les Tactiques de planification et Projets Workfront comme enfants dans la même hiérarchie d’espace de travail.

* Si une connexion entre les types d&#39;enregistrements sélectionnés existe déjà, le système réutilise la connexion existante.
* S’il n’existe aucune connexion, Workfront en crée une dans le cadre de la configuration de la hiérarchie.
* Le paramètre **Créer le champ correspondant sur le type d’enregistrement lié** doit être activé pour le champ connecté pour les enregistrements et les types d’objet que vous souhaitez inclure dans une hiérarchie.
* Vous ne pouvez pas supprimer un type d&#39;enregistrement s&#39;il fait partie d&#39;une hiérarchie.
* Vous ne pouvez pas supprimer un champ de connexion si le type d’enregistrement référencé dans le champ fait partie d’une hiérarchie. Vous devez d&#39;abord supprimer le type d&#39;enregistrement de la hiérarchie ou supprimer la hiérarchie avant de pouvoir supprimer le type d&#39;enregistrement.
* Vous pouvez supprimer un champ de recherche d’un type d’enregistrement connecté. Les informations du champ ne peuvent pas être récupérées.
* Voici des règles pour la configuration de la hiérarchie :
   * Un type d’enregistrement ne peut avoir qu’un seul type d’enregistrement parent dans un espace de travail donné.

     Par exemple, un type d’enregistrement Tactique ne peut pas avoir à la fois un type d’enregistrement Campagne et un type d’enregistrement Objectif en tant que parent dans le même espace de travail.
   * Un type d’enregistrement peut être le parent dans plusieurs hiérarchies.

     Par exemple, vous pouvez avoir trois hiérarchies différentes dans un espace de travail et chacune d’elles peut avoir comme type d’enregistrement parent Campagnes .
   * Un enregistrement peut être connecté à plusieurs enregistrements parents du même type, lorsque vous connectez un à plusieurs ou plusieurs à plusieurs types d&#39;enregistrements.

     Par exemple, la tactique A peut appartenir à la fois à la campagne X et à la campagne Y.
   * Un type d’enregistrement ne peut se connecter qu’à un seul type d’enregistrement enfant à la fois. Un type d’enregistrement enfant peut également être un parent pour un autre type d’enregistrement.

     Par exemple, un type d’enregistrement Campagne peut être le parent d’un seul autre type d’enregistrement dans la même hiérarchie (Tactiques), et les tactiques peuvent à leur tour être le parent de programmes qui peuvent être un parent de projets.
   * Un type d’enregistrement ne peut pas être le parent dans une hiérarchie et l’enfant dans une autre hiérarchie du même espace de travail.
   * Les types d’enregistrements globaux peuvent apparaître dans plusieurs espaces de travail à l’intérieur de plusieurs hiérarchies, après leur ajout à ces espaces de travail.

     Par exemple, si une campagne est un type d’enregistrement global et fait partie d’une hiérarchie dans Workspace 1, elle peut être ajoutée en tant que type d’enregistrement existant dans Workspace 2 et y faire partie d’une hiérarchie. Cependant, il ne peut pas faire partie d’une hiérarchie dans Workspace 2 uniquement lorsqu’il est désigné comme type d’enregistrement global dans Workspace 1, mais pas ajouté à Workspace 2.
   * Lorsque les types d&#39;enregistrements connectés font partie des hiérarchies, vous pouvez connecter un enregistrement d&#39;un type d&#39;enregistrement enfant à un maximum de 10 enregistrements d&#39;un type d&#39;enregistrement parent.

     Par exemple, si vous créez une hiérarchie entre Campagnes comme enregistrement parent et Persona comme enregistrement enfant, vous pouvez connecter la même persona à un maximum de 10 campagnes.

## Remarques concernant l’affichage des chemins de navigation

Lorsque vous créez des hiérarchies entre les types d&#39;enregistrements, elles génèrent des chemins de navigation pour les enregistrements appartenant à ces types d&#39;enregistrements.

Par exemple, si vous créez une hiérarchie et que vous connectez des campagnes aux Tactiques, puis aux Activités et enfin aux Projets, lorsque vous accédez à un enregistrement de l’un des types connectés dans la hiérarchie, vous pouvez voir où l’enregistrement est placé dans la hiérarchie.

![Chemin de navigation](assets/breadcrumbs-on-project.png)

Tenez compte des points suivants :

* Si un type d&#39;enregistrement fait partie de plusieurs hiérarchies, vous pouvez basculer entre les hiérarchies à partir du chemin de navigation de l&#39;enregistrement sur la page de l&#39;enregistrement.
* Si le type d’enregistrement dans une hiérarchie comporte plusieurs enregistrements, vous pouvez sélectionner des enregistrements dans le chemin de navigation.
* Les chemins de navigation fonctionnent dans Workfront et Planning.

  Par exemple, lorsque vous étudiez un projet lié aux campagnes et tactiques Planning, ainsi qu’aux portfolios et programmes Workfront, vous pouvez basculer entre les deux types d’objets Planning et Workfront à partir du chemin de navigation.

  Pour plus d’informations, voir [Création de hiérarchies d’espaces de travail](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* Lorsque vous modifiez un enregistrement, les modifications sont visibles à partir de tous les espaces de travail et de toutes les hiérarchies dont l&#39;enregistrement fait partie.


