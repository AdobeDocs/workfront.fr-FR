---
title: Présentation des espaces de travail
description: Un espace de travail est une collection de types d’enregistrements utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Adobe Workfront Planning pour les faire correspondre aux workflows de vos entités organisationnelles.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 26%

---

# Vue d’ensemble des espaces de travail

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Un espace de travail est un ensemble de types d’enregistrements utilisés par une entité organisationnelle et représente le cycle de vie et les processus de travail de l’entité. Vous pouvez entièrement personnaliser les espaces de travail dans Adobe Workfront Planning.


![Compte administrateur de la page de destination des espaces de travail](assets/workspaces-landing-page-admin-account.png)

## Considérations sur les espaces de travail

* Vous pouvez créer des espaces de travail pour des unités organisationnelles spécifiques au sein de votre organisation, afin qu’ils correspondent au mode de travail unique de chaque unité.
* Workfront Planning ne comprend aucun espace de travail préconfiguré. Vous devez les créer en fonction des besoins de votre organisation.
* Vous pouvez créer des espaces de travail comme suit :

   * À partir de zéro
   * En utilisant un modèle. Les modèles contiennent un nombre préconfiguré de types d’enregistrements et leurs champs.
   * Utilisation de Planning Designer optimisé par l’IA Cette fonctionnalité est actuellement disponible dans Beta.
   * Utilisation d’un lot de modèle multi-espace de travail.

  Pour plus d’informations, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

* Les espaces de travail sont des structures au sein desquelles vos entités organisationnelles (une équipe, un groupe, un service ou une division) travaillent. Ils ne peuvent pas être associés à des champs. Seuls les types d’enregistrements d’un espace de travail peuvent être associés à des champs.

  Pour plus d’informations, voir [Présentation des types d’enregistrements](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Selon votre licence Workfront, les espaces de travail s&#39;affichent dans les onglets suivants de la zone Planning :

   * Pour les administrateurs système, les espaces de travail s’affichent dans les onglets suivants :

      * **Espaces de travail sur lesquels je me trouve** : affiche les espaces de travail que vous avez créés ou les espaces de travail partagés avec vous.
      * **Autres espaces de travail** : affiche tous les autres espaces de travail du système.

   * Pour tous les autres utilisateurs, les espaces de travail qu’ils ont créés et les espaces de travail que d’autres ont partagés avec eux s’affichent dans la zone Espaces de travail.

* Les types d’enregistrements contenus dans un espace de travail doivent refléter le cycle de vie professionnelle et les concepts d’une entité organisationnelle.

  Par exemple, si les objets de travail d&#39;une unité sont des campagnes, des produits et des régions, l&#39;espace de travail de cette unité doit contenir les types d&#39;enregistrements Campagne, Produit et Région.
* Lorsque vous créez un espace de travail, vous êtes la seule personne à pouvoir y accéder et le gérer. Vous devez le partager avec d’autres utilisateurs afin qu’ils puissent collaborer avec vous dans le même espace.

  Pour plus d’informations, voir [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md).

  Les administrateurs et administratrices système peuvent gérer tous les espaces de travail, même ceux qu’ils ou elles n’ont pas créés.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Il existe des limites au nombre d&#39;objets d&#39;espace de travail que vous pouvez créer dans votre instance de Workfront Planning. Pour plus d&#39;informations, voir Présentation des limites d&#39;objet d&#39;Adobe Workfront Planning [&#128279;](/help/quicksilver/planning/general/limitations-overview.md).
