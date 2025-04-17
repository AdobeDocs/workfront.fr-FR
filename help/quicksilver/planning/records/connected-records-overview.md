---
title: Présentation des enregistrements connectés
description: Après avoir créé des connexions entre les types d’enregistrements, vous pouvez connecter des enregistrements individuels les uns aux autres. Cet article décrit les points à prendre en compte lors de la connexion des enregistrements dans Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 19%

---

# Présentation des enregistrements connectés

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, consultez la section [Activer ou désactiver les versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Vous pouvez connecter des enregistrements d’Adobe Workfront Planning les uns aux autres ou aux objets d’autres applications.

Cet article décrit les points à prendre en compte lors de la connexion des enregistrements dans Adobe Workfront Planning.

Pour plus d&#39;informations sur la façon de connecter des enregistrements entre eux ou à un autre objet, voir [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).


## Remarques concernant la connexion des enregistrements

* Une fois que vous avez connecté les types d’enregistrement, les types d’enregistrement connectés s’affichent sous forme de champs d’enregistrement liés dans les tableaux des types d’enregistrement à partir desquels ils sont liés et sur les pages des enregistrements.
* Vous pouvez parcourir et ajouter des enregistrements et des objets de l’enregistrement et des types d’objets liés à partir des champs d’enregistrement liés.
* Vous pouvez ajouter des champs (champs de recherche) des types d’enregistrements liés dans la table du type d’enregistrement à partir duquel vous effectuez le lien.

  En outre, vous pouvez ajouter des champs (champs de recherche) des types d’enregistrements à partir desquels vous établissez un lien dans la table du type d’enregistrement auquel vous établissez un lien.

  Par exemple, si vous liez le type d’enregistrement Produit au type d’enregistrement Campagne, vous pouvez afficher les champs de produit pour les campagnes, ainsi que les champs de campagne pour les produits.
* Vous ne pouvez pas mettre à jour manuellement les valeurs des champs de recherche des enregistrements à partir desquels vous établissez un lien.

  Les valeurs des champs de recherche renseignent l’enregistrement Workfront Planning à partir duquel vous établissez automatiquement la liaison après leur mise à jour dans l’enregistrement ou l’objet d’origine.

* Toute personne ayant accès à Workfront Planning and View ou à des autorisations supérieures de l’espace de travail <span class="preview">et un type d’enregistrement</span> peut voir les connexions que vous établissez entre les enregistrements ou entre les enregistrements et les objets d’autres applications. Elle peut afficher les enregistrements et les objets connectés, quelles que soient ses autorisations dans les applications auxquelles vous vous connectez.
* Vous pouvez afficher et modifier les connexions de tous les autres utilisateurs, si vous disposez des autorisations de niveau Gérer sur l’espace de travail <span class="preview">et le type d’enregistrement</span> où se trouvent les enregistrements connectés.
* Vous pouvez connecter un enregistrement à un ou plusieurs objets depuis une autre application. Cela dépend du type de connexion que vous avez sélectionné lors de la connexion des types d&#39;enregistrement. Pour plus d’informations, consultez la section « Types de connexions » dans l’article [Présentation des types d’enregistrements connectés](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Zones de connexion des enregistrements

Vous pouvez connecter des enregistrements à d&#39;autres enregistrements ou à des objets à partir d&#39;une autre application dans les domaines suivants :

* Vous pouvez connecter des enregistrements de Workfront Planning à des objets Workfront ou Experience Manager Assets dans les zones suivantes d&#39;un enregistrement Planning :

   * Champs d&#39;enregistrement connectés dans la vue Table d&#39;un type d&#39;enregistrement dans Planning.
   * L&#39;aperçu ou la page de l&#39;enregistrement dans les champs d&#39;enregistrement connectés sur l&#39;onglet Détails.
   * L&#39;aperçu ou la page de l&#39;enregistrement dans l&#39;onglet Connexions.
   * Page de l’enregistrement dans un onglet Affichage des connexions d’un enregistrement connecté.

* Vous pouvez connecter des objets Workfront à des enregistrements Workfront Planning dans les zones suivantes de Workfront :

   * Section Planning d’un objet Workfront.
   * Champ de connexion Planning dans un formulaire personnalisé d’objet Workfront.

  Pour plus d’informations, voir [Gérer les connexions d’enregistrement à partir d’objets Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
