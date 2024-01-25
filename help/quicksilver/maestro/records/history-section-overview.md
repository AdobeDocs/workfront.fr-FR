---
title: Présentation de la section Historique
description: Vous pouvez consulter les modifications apportées à l’enregistrement et enregistrées par le système dans le panneau droit d’un enregistrement dans Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 4%

---


# Présentation de la section Historique

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Vous pouvez collaborer sur des enregistrements Adobe Maestro en ajoutant des commentaires ou des réponses dans le panneau droit d’un enregistrement. Vous pouvez également afficher d’autres modifications apportées à l’enregistrement et enregistrées par le système dans cette zone.

Le panneau de droite d’un enregistrement affiche les sections suivantes :

* **Commentaires**: affiche les commentaires et réponses que les utilisateurs ajoutent aux enregistrements. Pour plus d’informations sur la gestion des commentaires dans les enregistrements Maestro, voir [Gestion des commentaires d’enregistrement](/help/quicksilver/maestro/records/manage-record-comments.md).
* **Histoire**: affiche les modifications enregistrées par le système que les utilisateurs apportent aux champs d’enregistrement.

## Recherche de la section Historique d’un enregistrement

{{step1-to-maestro}}

Le dernier espace de travail ouvert par défaut.

1. Choisissez une vue de tableau parmi les **Affichage** menu déroulant.
1. Cliquez sur le nom d’un enregistrement dans la vue de tableau.

   Le record **Détails** s’ouvre. La zone Commentaires s’ouvre par défaut dans le panneau de droite.
1. Cliquez sur le bouton **Afficher l’historique** icon ![](assets/show-history-icon.png). Toutes les modifications apportées aux champs de l’enregistrement s’affichent dans le panneau de droite, en commençant par la plus récente.
1. (Facultatif) Cliquez sur le **Masquer l’historique** icon ![](assets/hide-history-icon.png) pour fermer le panneau de droite.

## Observations relatives à la section Historique

Vous pouvez passer en revue les modifications apportées à l’enregistrement des champs dans la section Historique du panneau droit de la page Détails d’un enregistrement opérationnel ou d’une taxonomie.

![](assets/history-area-in-comments.png)

* Maestro enregistre les informations suivantes dans la section Historique :

   * Toute modification de champ

   * L’ancienne et la nouvelle valeur des champs, lorsque les valeurs changent. Les anciennes valeurs s’affichent au format barré.

   * Nom complet de l’utilisateur qui a apporté la modification.

   * Date et horodatage du moment où la modification s’est produite.

* Les champs des types suivants affichent toujours l’ancienne valeur (au format barré) et la nouvelle valeur :

   * Texte
   * Paragraphe
   * Devise
   * Date
   * Nombre
   * Pourcentage
   * Sélection unique

* Les champs des types suivants affichent l’ancienne valeur au format barré uniquement si au moins l’une des valeurs multiples a été supprimée :

   * Sélection multiple
   * Champs d’enregistrement liés
   * Personnes

  Si la modification ajoute uniquement des valeurs au champ, l’ancienne valeur ne s’affiche pas et seule la nouvelle valeur de champ s’affiche.

* Les champs de type case à cocher n’affichent jamais l’ancienne valeur au format barré. Si le champ est modifié, seul l’état actuel au moment de la modification s’affiche.

  Pour plus d’informations sur les champs Maestro, voir [Créer des champs](/help/quicksilver/maestro/fields/create-fields.md).

* Les modifications apportées aux champs des types suivants ne s’affichent pas dans la section Historique :

   * Champs liés (recherche)
   * Formule
   * Créé par
   * Créé à la date
   * Dernière modification par
   * Date de dernière modification

* Si un champ est supprimé du système, les mises à jour effectuées sur ce champ restent dans la section Historique . Rien n’indique que le champ a été supprimé dans la section Historique d’un enregistrement.