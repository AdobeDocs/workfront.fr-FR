---
content-type: release-notes
title: Activité de mise à jour du quatrième trimestre 2025 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le quatrième trimestre 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: f7dcae5e6bcc8674ef37ef94282c50dc9ffe951d
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 10%

---

# Activité de mise à jour du quatrième trimestre 2025 pour Adobe Workfront Planning

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du quatrième trimestre 2025.

<!--keep the sentence below for all future quarterly release pages-->

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Nouvelles limites pour les champs de formule

>[!NOTE]
>
>* Aperçu : 28 août 2025
>* Mise à jour rapide de la production : 11 septembre 2025
>* Version de production pour toute la clientèle : vendredi 16 octobre 2025

Nous avons défini les limites suivantes pour les champs de formule :

* Il existe une limite de 20 champs de formule par type d’enregistrement
* Une expression de formule comporte une limite de 50 000 caractères

Pour plus d&#39;informations, voir [Présentation des champs de formule](/help/quicksilver/planning/fields/formula-fields.md).

## Afficher une erreur lorsque les valeurs de formule ne peuvent pas être résolues

>[!NOTE]
>
>* Aperçu : 28 août 2025
>* Mise à jour rapide de la production : 11 septembre 2025
>* Version de production pour toute la clientèle : vendredi 16 octobre 2025

Pour indiquer qu’il existe un problème lors de la résolution d’un champ de formule, le champ s’affiche désormais sous la forme « #ERROR ! » dans l&#39;un des cas suivants :

* Lorsqu’un champ utilisé dans une formule est supprimé.

* Lorsqu’un champ utilisé dans un champ de recherche agrégé s’affiche sous la forme #ERROR !.

* Lorsqu’une valeur de formule ne peut pas être affichée au format sélectionné.

Pour plus d’informations, consultez [Vue d’ensemble des champs de formule](/help/quicksilver/planning/fields/formula-fields.md).

## Nouvelles expressions ajoutées aux champs de formule dans Planning

>[!NOTE]
>
>Aperçu : 7 août 2025
>&#x200B;>Production pour tous les clients :August 2025
>&#x200B;>[!BADGE Hors programme &#x200B;]{type=Neutral}

Nous avons ajouté de nouvelles expressions avec l’utilisation suivante aux champs de formule dans Workfront Planning et aux champs calculés personnalisés dans Workfront :

* **REMOVEACCENTS(string)** : supprime les signes diacritiques de tous les caractères accentués dans la chaîne d’entrée.
* **REPLACEPATTERN (chaîne, modèle, chaîne de remplacement)** : remplace les correspondances du modèle donné par la chaîne de remplacement.
* **PASCAL(string)** : convertit la chaîne d’entrée en PascalCase en mettant en majuscule la première lettre de chaque mot et en supprimant tous les espaces.

Pour plus d’informations, voir [Vue d’ensemble des expressions de données calculées](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Ajout des boutons Agrandir et Réduire à la fenêtre de création des champs de formule

>[!NOTE]
>
>Aperçu : 31 juillet 2025
>&#x200B;>Production pour tous les clients : 31 juillet 2025
>&#x200B;>[!BADGE Hors programme &#x200B;]{type=Neutral}

Nous avons ajouté un bouton Maximiser pour agrandir le champ de formule lors de la création ou de la modification du champ dans une vue de tableau d&#39;enregistrements. De plus, nous avons ajouté un bouton Réduire dans la nouvelle fenêtre agrandie pour revenir à la zone de création de champ.

Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## La page Enregistrements connectés est désormais disponible dans la zone d’aperçu d’un enregistrement

>[!NOTE]
>
>* Aperçu : 31 juillet 2025
>* Version rapide de production : 14 août 2025
>* Version de production pour toute la clientèle : vendredi 16 octobre 2025

Nous avons à présent fait en sorte que l’expérience de la page Enregistrements connectés dans la zone d’aperçu corresponde à celle de la page dans la page complète de la zone Détails d’un enregistrement.

Avant cette amélioration, l’affichage des enregistrements connectés dans une page d’enregistrements connectés n’était possible que dans la page complète de la zone Détails d’un enregistrement.

Pour plus d’informations, voir [Gérer la mise en page des enregistrements](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## Créer des enregistrements dans la vue chronologique

>[!NOTE]
>
>Aperçu : 24 juillet 2025
>&#x200B;>Version rapide de production : 14 août 2025
>&#x200B;>Version de production pour toute la clientèle : vendredi 16 octobre 2025

Vous pouvez désormais créer des enregistrements dans la vue chronologique d’un type d’enregistrement en double-cliquant n’importe où sur la chronologie.

Vous pouvez sélectionner la période de votre enregistrement ou ouvrir la page de l’enregistrement pour modifier tous ses détails.

Avant cette amélioration, vous ne pouviez ajouter de nouveaux enregistrements qu’à l’aide du bouton Nouvel enregistrement ou sur la ligne en mode Tableau.

Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

## Ajout de l’option Partager dans le menu Plus d’une carte de type enregistrement

>[!NOTE]
>
>Aperçu : 24 juillet 2025
>&#x200B;>Version rapide de production : 14 août 2025
>&#x200B;>Version de production pour toute la clientèle : vendredi 16 octobre 2025

Vous pouvez désormais partager un type d’enregistrement à partir du menu Plus de la carte de type d’enregistrement de la page de l’espace de travail. Avant cette amélioration, l’option Partager n’était disponible que dans la page du type d’enregistrement.

Pour plus d’informations, voir [Partager les types d’enregistrements](/help/quicksilver/planning/access/share-record-types.md).

## Afficher toutes les vues Workfront Planning en mode plein écran

>[!NOTE]
>
>Aperçu : 24 juillet 2025
>&#x200B;>Version rapide de production : 14 août 2025
>&#x200B;>Version de production pour toute la clientèle : vendredi 16 octobre 2025

Vous pouvez désormais afficher toutes les vues Planification de Workfront (tableau, chronologie et calendrier) en mode plein écran. La fonctionnalité d’affichage est conservée et vous pouvez également modifier l’affichage en plein écran.

Avant cette amélioration, cette fonctionnalité n’existait pas.

Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

## Ajout d&#39;équipes en tant qu&#39;approbateurs sur les formulaires de demande Planning

>[!NOTE]
>
>Aperçu : 22 juillet 2025
>&#x200B;>Production pour la version rapide : vendredi 14 août 2025
>&#x200B;>Version de production pour toute la clientèle : vendredi 16 octobre 2025

Pour rendre le processus d&#39;approbation plus flexible, nous avons ajouté la possibilité d&#39;ajouter des équipes en tant qu&#39;approbateurs sur les formulaires de demande Planning. Vous pouvez désormais saisir et sélectionner des noms d’équipe lors de la définition des approbateurs. N’importe quel membre de l’équipe peut prendre une décision, qui compte comme la décision d’approbation de l’ensemble de l’équipe.

Auparavant, seuls des utilisateurs individuels pouvaient être affectés en tant qu’approbateurs.

Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

## Nouveaux champs pour afficher les informations de validation des enregistrements

>[!NOTE]
>
>Aperçu : 17 juillet 2025
>&#x200B;>Production pour la version rapide : vendredi 14 août 2025
>&#x200B;>Version de production pour toute la clientèle : vendredi 16 octobre 2025

Les champs suivants sont introduits afin de capturer les informations d&#39;approbation des enregistrements créés lors de l&#39;envoi d&#39;une demande avec approbation :

* Approbation par
* Date de validation

Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## Renseigner automatiquement les champs en fonction des regroupements appliqués

>[!NOTE]
>
>Aperçu : 10 juillet 2025
>&#x200B;>Version rapide de production : 14 août 2025
>&#x200B;>Version de production pour toute la clientèle : vendredi 16 octobre 2025


Désormais, lorsque des regroupements sont appliqués à une vue Tableau, l’ajout d’un enregistrement au tableau renseigne automatiquement les champs associés aux regroupements auxquels vous ajoutez l’enregistrement.

Si plusieurs regroupements sont appliqués, le système ne renseigne automatiquement les champs associés à tous les regroupements que lorsque vous ajoutez l&#39;enregistrement à la fin de la liste à l&#39;intérieur du dernier critère de regroupement.

Avant cette amélioration, vous deviez mettre à jour manuellement les champs associés aux regroupements.

Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
