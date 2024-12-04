---
content-type: release-notes
title: Activité de planification des versions Adobe Workfront pour la version 25.1
description: Il s’agit de l’activité de publication du produit Adobe Workfront Planning pour le premier trimestre 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: 5db940b197364e30ef6e1ea3e3c94ae3bda5b20c
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 3%

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


## Importation de champs Workfront existants dans des types d’enregistrement Workfront Planning

>[!NOTE]
>
>Aperçu de la version : 27 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Désormais, lorsque vous ajoutez des champs à un type d’enregistrement, vous avez la possibilité d’importer des champs personnalisés ou natifs Workfront existants et de les associer au type d’enregistrement que vous avez sélectionné. L’importation de champs existants crée une copie des champs Workfront dans Workfront Planning. Les champs copiés sont indépendants de leurs versions d’origine.

Avant cette amélioration, vous deviez créer manuellement tous les champs et les associer aux types d’enregistrement.

Les champs calculés ne sont pas pris en charge pour le moment.

Pour plus d’informations, voir [Importation de champs à partir d’Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## Créer des types d’enregistrement, des enregistrements et des champs en important un fichier CSV ou Excel

>[!NOTE]
>
>Aperçu de la version : 27 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Vous pouvez désormais importer de nouveaux types d’enregistrements en important un fichier CSV ou Excel.

Les informations importées sont les suivantes :

* Le nom de la feuille ou du fichier est importé en tant que nom de type d’enregistrement.

* La première ligne de chaque colonne est importée en tant que nouveau champ. Chaque feuille importée peut contenir jusqu’à 500 champs.

* Chaque ligne est importée en tant que nouvel enregistrement. Chaque feuille peut contenir jusqu’à 10 000 enregistrements.

Pour plus d’informations, voir la section [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

## Éviter les références circulaires dans les formules

>[!NOTE]
>
>Aperçu de la version : 27 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Nous avons ajouté un message d’avertissement lors de l’édition ou de la création d’un champ de formule qui peut créer une référence circulaire à lui-même ou à des champs partagés. Vous ne pouvez pas enregistrer un champ de formule qui se réfère à lui-même ou aux éléments référencés dans son calcul.

Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## Ajout de pages de vue Connexion à une page d’enregistrement pour afficher les enregistrements connectés dans une vue de tableau

>[!NOTE]
>
>Aperçu de la version : 27 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Vous pouvez ajouter des pages à la zone de détails d’un enregistrement pour afficher les enregistrements connectés dans une vue de tableau. Vous pouvez ajouter une page par enregistrement connecté.

Les pages ajoutées sont en lecture seule.

Pour plus d’informations, voir [Gestion de la mise en page de la page d’enregistrement](/help/quicksilver/planning/records/manage-the-record-page.md).

## Nouveaux onglets Workfront et Planification dans la section Envoyé de la zone Demandes

>[!NOTE]
>
>Aperçu de la version : 27 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Vous trouverez désormais les requêtes de planification Workfront dans la section Envoyés de la zone Demandes de Workfront. La section Envoyé affiche désormais les onglets suivants :

* Workfront : affiche les requêtes envoyées dans Workfront.
* Planification : affiche les demandes envoyées à l’aide d’un formulaire de demande de planification Workfront.

Vous devez utiliser un lien vers le formulaire de requête pour pouvoir ajouter des requêtes à un type d’enregistrement Workfront Planning. L’envoi d’une demande de planification Workfront à partir de la zone Demandes de Workfront sera disponible ultérieurement.

Votre entreprise doit acheter un package de planification Workfront avant que l’onglet Planification ne soit disponible dans la zone Demandes .

Pour plus d’informations, voir [Soumettre des demandes de planification Adobe Workfront pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## D’autres types de champ sont désormais pris en charge dans les formulaires de demande.

>[!NOTE]
>
>Aperçu de la version : 27 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Vous pouvez maintenant ajouter les types de champ suivants à un formulaire de demande de type enregistrement dans Workfront Planning :

* Personnes
* Connexions Workfront

Avant cette amélioration, ces types de champs ne pouvaient pas être ajoutés aux formulaires de demande dans la planification Workfront.

Pour plus d’informations, voir Création et gestion d’un formulaire de demande dans Adobe Workfront Planning (/help/quicksilver/planning/requests/create-request-form.md).

## Limiter le partage public des formulaires de requête contenant certains types de champs

>[!NOTE]
>
>Aperçu de la version : 27 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Vous ne pouvez plus partager un formulaire de demande publiquement si le formulaire contient l’un des types de champs suivants :

* Formule
* Connexions Workfront et AEM Assets
* Champs de recherche
* Personnes

Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


## Afficher les enregistrements dans la vue Calendrier par semaine

>[!NOTE]
>
>Aperçu de la version : 26 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Vous pouvez désormais afficher les enregistrements dans la vue Calendrier par semaine. Avant cette amélioration, vous ne pouviez afficher le calendrier que par mois.

Pour plus d’informations, voir [Gestion de la vue Calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Restaurer les enregistrements supprimés

>[!NOTE]
>
>Aperçu de la version : 22 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Une fois les enregistrements supprimés, ils sont désormais temporairement déplacés dans une corbeille Récemment supprimés pendant 30 jours. Vous pouvez accéder à la corbeille Récemment supprimés de la page du type d&#39;enregistrement et elle ne contient que les enregistrements d&#39;un type spécifique.

Les gestionnaires de Workspace peuvent restaurer les enregistrements de la corbeille pendant 30 jours au maximum après leur suppression. Les enregistrements connectés et leurs informations de champ sont également restaurés.

Avant cette amélioration, les enregistrements supprimés ne pouvaient pas être restaurés.

Pour plus d’informations, voir [Restaurer les enregistrements supprimés](/help/quicksilver/planning/records/records-information.md).

## Assistant d’Adobe de l’IA disponible dans les zones de détails des enregistrements

>[!NOTE]
>
>Aperçu de la version : 21 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Afin de vous faciliter la tâche, nous avons ajouté l’assistant d’Adobe AI à l’aperçu des détails ou à la page d’enregistrement d’un enregistrement. Vous pouvez utiliser l’assistant d’IA situé dans une page d’enregistrement pour mettre à jour les informations sur l’enregistrement.

Pour plus d’informations, reportez-vous à la section [Présentation de l’assistant de planification Adobe Workfront AI](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## Nouvelle expérience lors de l’ajout d’une miniature et d’une image de couverture à une page d’enregistrement

>[!NOTE]
>
>Aperçu de la version : 20 novembre 2024 ; Production pour une version rapide : avec la version 24.12 (décembre 2024) ; Production pour une version trimestrielle : avec la version 25.1 (janvier 2025)

Lorsque vous ouvrez l’aperçu ou la page d’un enregistrement et que l’enregistrement ne comporte pas de miniature ou d’image de couverture, vous devez maintenant pointer sur la zone située au-dessus du nom de l’enregistrement dans l’en-tête pour afficher les options permettant d’ajouter une couverture et une image de miniature à l’enregistrement. Avant cette amélioration, les images d’espace réservé vides pour la miniature et la couverture s’affichaient au-dessus du nom de l’enregistrement.

Pour plus d’informations, consultez les articles suivants :

* [Ajouter une image de couverture à un enregistrement](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Ajout d’une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

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
