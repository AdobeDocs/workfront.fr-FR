---
content-type: release-notes
title: Activité de planification des versions Adobe Workfront pour la version 25.1
description: Il s’agit de l’activité de publication du produit Adobe Workfront Planning pour le premier trimestre 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 5%

---

# Activité de mise à jour du premier trimestre 2025 pour Adobe Workfront Planning

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Workfront Planning, une nouvelle offre d’Adobe Workfront.
>
>Vous devez acheter un plan de planification Workfront, en plus d’un plan Workfront, pour pouvoir accéder aux fonctionnalités de planification Workfront et les utiliser.
>
>Pour obtenir la liste complète des exigences d’accès à la planification Workfront, consultez la [présentation des accès](/help/quicksilver/planning/access/access-overview.md).
>Pour une présentation de la planification Workfront, consultez la [présentation de la planification Adobe Workfront](/help/quicksilver/planning/general/planning-overview.md).

Cet article décrit les fonctionnalités de la version 2025 du premier trimestre de la planification Workfront.

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning après la mise à disposition de la version générale le 28 août 2024, voir [Activité de mise à jour d’Adobe Workfront Planning : index de l’article](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Nouveaux types d’affichage pour les champs de type pourcentage dans la vue de tableau

>[!NOTE]
>
>Aperçu de la version : 7 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Pour faciliter la lecture des nombres dans la vue du tableau, vous pouvez désormais choisir parmi les choix suivants pour modifier l&#39;affichage d&#39;un champ de type Pourcentage dans la vue du tableau :

* Nombre
* Barres
* Cercle

Ce type d’affichage n’est pris en charge que dans la vue de tableau.

Avant cette amélioration, vous ne pouviez afficher les valeurs en pourcentage que sous forme de nombres.

Pour plus d’informations, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## Les champs de connexion sont désormais pris en charge dans les formulaires de demande

>[!NOTE]
>
>Aperçu de la version : 31 octobre 2024 ; Production pour une version rapide : avec la version 24.11 (14 novembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Vous pouvez désormais ajouter des champs connectés pour les enregistrements de la planification Workfront à un formulaire de demande de type enregistrement.

Vous ne pouvez pas ajouter de champs de recherche de connexion ni de champs connectés pour les objets Workfront dans le formulaire de requête.

Avant cette amélioration, ces types de champs ne pouvaient pas être ajoutés aux formulaires de demande dans la planification Workfront.

Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Avertissement de connexion lors de la connexion d&#39;enregistrements déjà liés à d&#39;autres enregistrements

>[!NOTE]
>
>Aperçu de la version : 31 octobre 2024 ; Production pour une version rapide : avec la version 24.11 (14 novembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Lorsque vous essayez de connecter des enregistrements déjà connectés ailleurs et qui appartiennent à un type d&#39;enregistrement connecté via un type de connexion Un à plusieurs ou Un à un, vous recevez maintenant un avertissement indiquant que les enregistrements sont déjà connectés. Si vous confirmez que vous souhaitez poursuivre la connexion, les enregistrements sélectionnés sont supprimés de l’enregistrement d’origine et ajoutés à l’enregistrement que vous êtes en train de modifier.

Pour plus d’informations sur les types de connexions, voir [Présentation des types d’enregistrements connectés](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Nouvelle icône d’information avec la description des champs dans la page de détails de l’enregistrement.

>[!NOTE]
>
>Aperçu de la version : 30 octobre 2024 ; Production pour une version rapide : avec la version 24.11 (14 novembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Nous avons ajouté une icône d’information à droite des noms de champ dans une page d’enregistrement. Cliquez sur l’icône d’information pour afficher la description du champ, lorsqu’il existe une description. Avant cette amélioration, la description du champ s’affichait lorsque vous survoliez le nom du champ avec la souris.

Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

## Nouveau type de champ Workfront pour la planification des connexions

>[!NOTE]
>
>Aperçu de la version : 24 octobre 2024 ; Production pour une version rapide : avec la version 24.11 (14 novembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Pour continuer à rapprocher les objets Workfront des enregistrements de planification Workfront, nous avons ajouté un nouveau type de champ dans les formulaires personnalisés Workfront appelé Connexion de planification. En ajoutant ce type de champ à un formulaire personnalisé Workfront et, en fin de compte, à un objet Workfront, vous pouvez effectuer les opérations suivantes :

* Afficher les enregistrements liés à un objet Workfront dans le formulaire personnalisé.

* Connectez et déconnectez les enregistrements de planification Workfront d’un objet Workfront.

Vous pouvez ajouter le nouveau champ aux formulaires pour tous les types d’objets. Cependant, vous ne pouvez modifier les informations dans le champ qu’à partir de formulaires associés aux objets Workfront suivants qui peuvent être connectés à partir des types d’enregistrements de la planification Workfront : Portfolio, Programme, Projet, Société, Groupe.

La modification en masse des champs Planification de la connexion pour les objets Workfront n’est pas encore disponible.

Pour plus d’informations, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3435633/){target=_blank}
