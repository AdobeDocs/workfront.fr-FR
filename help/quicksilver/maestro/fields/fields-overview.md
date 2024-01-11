---
title: Présentation des champs
description: Vous pouvez ajouter de nouveaux champs dans Adobe Manager qui reflètent le cycle de vie de votre entreprise. Les champs sont des attributs de types d’enregistrement.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

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

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez ajouter de nouveaux champs dans Adobe Manager qui reflètent le cycle de vie de votre entreprise. Les champs sont des attributs de types d’enregistrement.


## Observations sur les champs Maestro

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

      * En connectant les types d’enregistrement. Vous pouvez créer des champs d’enregistrement liés lorsque vous ajoutez une nouvelle connexion entre deux types d’enregistrement Maestro ou un type d’enregistrement et un type d’objet à partir d’autres applications.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Pour plus d’informations sur la connexion des types d’enregistrement Maestro, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

      * En important des types d’enregistrement à l’aide d’un fichier Excel ou CSV. Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

   * Automatiquement :

      * Par défaut, chaque fois que vous créez un type d’enregistrement.

        Voici les champs standard créés par défaut pour chaque nouveau type d&#39;enregistrement opérationnel :

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

        Voici les champs standard créés par défaut pour chaque nouveau type d’enregistrement de taxonomie :

         * Nom <!--will more be added? If not, consider rephrasing this bullet-->

      * Lorsque vous créez un espace de travail à partir d’un modèle. Maestro crée des champs pour les types d’enregistrements opérationnels et les taxonomies lorsque vous créez un espace de travail à partir d’un modèle. Pour plus d’informations, voir [Créer des espaces de travail](../architecture/create-workspaces.md).

* Les champs Maestro ne sont pas accessibles à partir de Workfront.

* Les champs Workfront sont accessibles à partir de Maestro uniquement lorsque vous connectez des types d’enregistrements Maestro à des types d’objets Workfront et que vous ajoutez des champs liés ou de recherche à partir d’objets Workfront. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

* Vous pouvez afficher et mettre à jour les paramètres des champs que vous ou tout autre utilisateur avez créés, si vous disposez des autorisations de gestion pour l’espace de travail auquel le champ appartient.

* Vous pouvez avoir jusqu’à 500 champs pour un type d’enregistrement.

* Les noms de champ peuvent contenir jusqu’à 250 caractères.

* Lors de la suppression d&#39;un type d&#39;enregistrement opérationnel, d&#39;une taxonomie ou d&#39;un espace de travail, tous les champs qui y sont associés et les valeurs des champs sont également supprimés et ne peuvent pas être récupérés. <!-- this might change with a possible recycle bin solution?!-->
