---
title: Aperçu du champ
description: Vous pouvez ajouter de nouveaux champs dans Adobe Workfront Planning qui reflètent le cycle de vie de votre entreprise. Les champs sont des attributs des types d’enregistrement.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 85%

---


# Vue d’ensemble des champs

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

Vous pouvez ajouter de nouveaux champs dans Adobe Workfront Planning qui reflètent le cycle de vie de votre entreprise. Les champs sont des attributs des types d’enregistrement.


## Remarques relatives aux champs Adobe Workfront Planning

* Vous ne pouvez créer des champs qu’à partir de la vue de tableau d’une page de type enregistrement. Les champs s’affichent sous forme de colonnes dans la vue de tableau. Tous les champs associés à un type d’enregistrement s’affichent également dans la page d’enregistrement.

  Pour plus d’informations sur la gestion des colonnes de tableau (ou des champs d’enregistrement), voir [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

  Pour plus d’informations sur la gestion des champs, reportez-vous également aux articles suivants :

   * [Modifier les paramètres de champ](/help/quicksilver/planning/fields/edit-fields.md)
   * [Supprimer des champs](/help/quicksilver/planning/fields/delete-fields.md)

* Les champs associés à un type d’enregistrement peuvent être associés à tous les enregistrements de ce type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Les champs associés à un type d’enregistrement ne peuvent pas être ajoutés à un autre type d’enregistrement. <!-- this will change when they open the Field library tab when creating a field-->

* Vous pouvez créer des champs manuellement ou automatiquement des manières suivantes :

   * Manuellement :

      * Lorsque vous ajoutez des colonnes dans la vue Tableau d’une page de type d’enregistrement. Les colonnes du tableau sont les champs associés au type d’enregistrement. Il s’agit des mêmes champs que ceux affichés sur la page d’un enregistrement.

        Vous ne pouvez pas créer de champs à partir de la page de l’enregistrement.

      * Lorsque vous connectez des types d’enregistrements. Vous pouvez créer des champs d’enregistrement liés lorsque vous ajoutez une nouvelle connexion entre deux types d’enregistrement ou un type d’enregistrement et des types d’objet à partir d’autres applications.

        Pour plus d’informations sur la connexion des types d’enregistrement, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

      * Lorsque vous importez des champs existants depuis Workfront.

        Pour plus d’informations, voir [Importer des champs depuis Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


   * Automatiquement :

      * Lorsque vous créez un type d’enregistrement :

         * Nom
         * Description
         * Date de début
         * Date de fin
         * Statut. Les valeurs par défaut des statuts des enregistrements sont les suivantes :
            * Développement
            * Prévu
            * Actif
            * Terminé
            * Suspendu

        Vous pouvez ajouter d’autres valeurs ou renommer les valeurs existantes.

      * Lorsque vous créez un espace de travail à partir d’un modèle.

        Pour plus d’informations, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Lorsque vous importez des types d’enregistrements à l’aide d’un fichier Excel ou CSV.

        Pour plus d’informations, voir la section [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

* Les champs Workfront Planning ne sont pas accessibles à partir de Workfront.

* Les champs Workfront sont accessibles à partir de Workfront Planning uniquement lorsque vous connectez des types d’enregistrement à des types d’objets Workfront et ajoutez des champs liés ou de recherche à partir d’objets Workfront. Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

* Vous pouvez afficher et mettre à jour les paramètres des champs que vous ou toute autre personne avez créés, si vous disposez des autorisations de gestion pour l’espace de travail auquel le champ appartient.

* Vous pouvez avoir jusqu’à 500 champs pour un type d’enregistrement.

* Les noms de champ peuvent contenir jusqu’à 250 caractères.

* Lors de la suppression d’un type d’enregistrement ou d’un espace de travail, tous les champs qui y sont associés, ainsi que les valeurs des champs, sont également supprimés et ne peuvent pas être récupérés. <!-- this might change with a possible recycle bin solution?!-->
