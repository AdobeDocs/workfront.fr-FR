---
title: Présentation des champs
description: Vous pouvez ajouter de nouveaux champs dans la planification Adobe Workfront qui reflètent le cycle de vie de votre entreprise. Les champs sont des attributs de types d’enregistrement.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 2%

---

# Présentation des champs

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Vous pouvez ajouter de nouveaux champs dans la planification Adobe Workfront qui reflètent le cycle de vie de votre entreprise. Les champs sont des attributs de types d’enregistrement.


## Observations relatives aux champs de planification Adobe Workfront

* Vous ne pouvez créer des champs qu’à partir de la vue de tableau d’une page de type enregistrement. Les champs s’affichent sous forme de colonnes dans la vue de tableau. Tous les champs associés à un type d&#39;enregistrement s&#39;affichent également dans la page Détails de chaque enregistrement de ce type.

  Pour plus d’informations sur la gestion des colonnes de tableau (ou des champs d’enregistrement), voir [Gestion de la vue de tableau](../views/manage-the-table-view.md).

  Pour plus d’informations sur la gestion des champs, reportez-vous également aux articles suivants :

   * [Modifier les champs](../fields/edit-fields.md)
   * [Supprimer des champs](../fields/delete-fields.md)

* Les champs associés à un type d&#39;enregistrement peuvent être associés à tous les enregistrements de ce type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Les champs associés à un type d’enregistrement ne peuvent pas être ajoutés à un autre type d’enregistrement. <!-- this will change when they open the Field library tab when creating a field-->

* Vous pouvez créer des champs manuellement ou automatiquement de différentes manières :

   * Manuellement :

      * En ajoutant des colonnes dans la vue de tableau d’une page de type enregistrement. Les colonnes du tableau sont les champs associés au type d’enregistrement. Il s’agit des mêmes champs que ceux affichés sur la page Détails d’un enregistrement.

        Vous ne pouvez pas créer de champs à partir de la page Détails d’un enregistrement.

        Cet article décrit comment créer manuellement des champs.

      * En connectant les types d’enregistrement. Vous pouvez créer des champs d’enregistrement liés lorsque vous ajoutez une nouvelle connexion entre deux types d’enregistrement ou un type d’enregistrement et un type d’objet à partir d’autres applications.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Pour plus d’informations sur la connexion des types d’enregistrement, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

      * En important des types d’enregistrement à l’aide d’un fichier Excel ou CSV. Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

   * Automatiquement :

     Voici les champs standard créés par défaut pour chaque nouveau type d&#39;enregistrement :

      * Nom
      * Description
      * Date de début
      * Date de fin
      * État. Les valeurs par défaut des états d’enregistrement sont les suivantes :
         * Développement
         * Prévu
         * Actif
         * Terminé
         * Suspendu

        Vous pouvez ajouter d’autres valeurs ou renommer les valeurs existantes.

     La planification Workfront crée des champs pour les types d’enregistrement lorsque vous créez un espace de travail à partir d’un modèle. Pour plus d’informations, voir [Créer des espaces de travail](../architecture/create-workspaces.md).

* Les champs de planification de Workfront ne sont pas accessibles à partir de Workfront.

* Les champs Workfront sont accessibles à partir de la planification Workfront uniquement lorsque vous connectez des types d’enregistrement à des types d’objets Workfront et ajoutez des champs liés ou de recherche à partir d’objets Workfront. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

* Vous pouvez afficher et mettre à jour les paramètres des champs que vous ou tout autre utilisateur avez créés, si vous disposez des autorisations de gestion pour l’espace de travail auquel le champ appartient.

* Vous pouvez avoir jusqu’à 500 champs pour un type d’enregistrement.

* Les noms de champ peuvent contenir jusqu’à 250 caractères.

* Lors de la suppression d&#39;un type d&#39;enregistrement ou d&#39;un espace de travail, tous les champs qui y sont associés, ainsi que les valeurs des champs, sont également supprimés et ne peuvent pas être récupérés. <!-- this might change with a possible recycle bin solution?!-->
