---
content-type: release-notes
title: Activité de mise à jour du troisième trimestre 2025 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le troisième trimestre 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 6761f5af-2501-4487-8114-2751f1e4fe69
source-git-commit: ccd0f65f064b5e55b6b5b94b27e25facfe50502f
workflow-type: tm+mt
source-wordcount: '2078'
ht-degree: 4%

---

# Activité de mise à jour du troisième trimestre 2025 pour Adobe Workfront Planning

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du troisième trimestre 2025.

<!--keep the sentence below for all future quarterly release pages-->

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Renseigner automatiquement les champs en fonction des regroupements appliqués

Aperçu : 10 juillet 2025
Version rapide de production : 14 août 2025
Production pour tous : 16 octobre 2025

Désormais, lorsque des regroupements sont appliqués à une vue Tableau, l’ajout d’un enregistrement au tableau renseigne automatiquement les champs associés aux regroupements auxquels vous ajoutez l’enregistrement.

Si plusieurs regroupements sont appliqués, le système ne renseigne automatiquement les champs associés à tous les regroupements que lorsque vous ajoutez l&#39;enregistrement à la fin de la liste à l&#39;intérieur du dernier critère de regroupement.

Avant cette amélioration, vous deviez mettre à jour manuellement les champs associés aux regroupements.

Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

## Bouton de partage commun pour les affichages et les types d’enregistrements

>[!NOTE]
>
>* Aperçu : 9 juillet 2025
>* Production pour tous : 17 juillet 2025

Vous pouvez désormais partager une vue ainsi qu’un type d’enregistrement à partir du même bouton sur la page du type d’enregistrement. Avant cette amélioration, vous pouviez uniquement partager le type d’enregistrement à partir du bouton Partager sur la page du type d’enregistrement et une vue à partir de l’onglet de la vue.

Pour plus d’informations, consultez les articles suivants :

* [Partager des vues](/help/quicksilver/planning/access/share-views.md)

* [Partage des types d’enregistrements](/help/quicksilver/planning/access/share-record-types.md)

<!--## Add teams as approvers on Planning request forms

>[!NOTE]
>
>* Preview: July 9, 2025 
>* Production for everyone: October 16, 20025 

To make the approval process more flexible, we've added the ability to add teams as approvers on Planning request forms. Now, you can enter and select team names when setting approvers. Any of the team members can make a decision, which counts as the approval decision for the entire team.

Previously, only individual users could be assigned as approvers. 

For more information, see [Add an approval to a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).-->

## Mise à jour de l’expérience lors du partage d’un formulaire de demande

>[!NOTE]
>
>* Aperçu : 9 juillet 2025
>* Production pour tous : 17 juillet 2025

Pour rendre plus sûr et plus simple le partage d’un formulaire de demande dans Workfront Planning, nous avons apporté les modifications suivantes :

* Nous avons supprimé les autorisations héritées. Désormais, le formulaire de demande n’est partagé qu’avec ceux que vous sélectionnez.
* Nous avons supprimé les options de gestion et de contribution pour les utilisateurs avec lesquels vous partagez le formulaire de demande. Désormais, les utilisateurs ajoutés peuvent uniquement envoyer le formulaire.
* L’onglet Partage public affiche désormais le lien et le champ de date d’expiration uniquement une fois que l’option Créer un lien public a été activée.

Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-requests/create-request-form).

## Développer et réduire tous les regroupements dans la vue Tableau

>[!NOTE]
>
>* Prévisualisation : vendredi 26 juin 2025
>* Production pour tous : 17 juillet 2025

Vous pouvez désormais réduire et développer les regroupements dans une vue Tableau à l’aide des zones suivantes :

* Zone Regroupement, accessible à partir de la barre d’outils de la vue Tableau

* En-tête d’un regroupement, en cliquant dessus avec le bouton droit

Vous pouvez réduire ou développer simultanément un ou tous les regroupements.

Avant cette amélioration, vous ne pouviez réduire ou développer qu’un seul regroupement à la fois, à partir de chaque en-tête de regroupement.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

## Nouvelle fonctionnalité d’agrégation pour les champs de formule

>[!NOTE]
>
>* Prévisualisation : vendredi 26 juin 2025
>* Production pour tous : 26 juin 2025

Désormais, lorsque vous connectez des types d’enregistrements et importez un champ de formule en tant que recherche, vous pouvez appliquer les fonctions d’agrégat (SOMME, MOYENNE, MIN, MAX, etc.) en fonction du format du champ de formule. Par exemple, si le champ de formule est numérique, vous pouvez utiliser des fonctions telles que SUM ou AVG ; si le champ de formule est formaté en tant que texte, les fonctions d&#39;agrégat telles que SUM ne s&#39;appliqueront pas.

Auparavant, lorsque vous connectiez des types d’enregistrement et importiez des champs de recherche à partir des enregistrements connectés, vous pouviez appliquer des fonctions d’agrégation uniquement aux champs standard, mais pas aux champs de formule.

Pour plus d&#39;informations, voir [Présentation des champs de formule](/help/quicksilver/planning/fields/formula-fields.md).

## Disponibilité des trimestres personnalisés pour la vue chronologique de Workfront Planning

>[!NOTE]
>
>* Prévisualisation : vendredi 12 juin 2025
>* Version rapide de production : 17 juillet 2025
>* Production pour tous les clients : 17 juillet 2025

Avec cette mise à jour, lorsque vous configurez des trimestres personnalisés dans les Préférences du projet de la Configuration, les trimestres personnalisés sont disponibles pour la vue Chronologie dans Workfront Planning.

Avant cette mise à jour, les trimestres personnalisés n’étaient disponibles que pour les fonctionnalités de création de rapports de Workfront.

Grâce à cette amélioration, les clients qui ont acheté Workfront Planning verront une expérience mise à jour pour la définition des trimestres personnalisés. Cette mise à jour comprend les améliorations suivantes :

Les écarts et les chevauchements entre les trimestres ne sont plus acceptés.

Vous pouvez configurer jusqu’à 100 trimestres personnalisés. Avant cette mise à jour, vous ne pouviez configurer que 8 trimestres personnalisés

L’expérience du trimestre personnalisé reste inchangée pour les clients qui n’ont pas acheté Workfront Planning.

Pour plus d’informations, voir [Activer des trimestres personnalisés pour les projets](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Calculer simultanément toutes les formules dépendantes

>[!NOTE]
>
>* Prévisualisation : vendredi 12 juin 2025
>* Version rapide de production : 12 juin 2025
>* Production pour tous les clients : 12 juin 2025

Nous avons introduit une amélioration qui met à jour tous les champs de formule qui dépendent les uns des autres en même temps après la mise à jour manuelle d’un champ référencé. Les champs de formule situés à 2, 3 ou 4 du champ dont la valeur a été modifiée manuellement et qui se référent entre eux seront désormais automatiquement mis à jour en même temps.

Avant cette amélioration, seuls les champs de formule directement dépendants étaient mis à jour lorsque la valeur d’un champ de références était mise à jour manuellement.

Pour plus d’informations, consultez [Vue d’ensemble des champs de formule](/help/quicksilver/planning/fields/formula-fields.md).

## Nouvelles expressions ajoutées aux champs de formule

>[!NOTE]
>
>* Prévisualisation : samedi 6 juin 2025
>* Version rapide de production : 6 juin 2025
>* Production pour tous les clients : 6 juin 2025

Nous avons ajouté les expressions suivantes aux champs de formule :

* ARRAYCONTAINS

* SORTASCARRAY

* SORTDESCARRAY

Avant cette amélioration, ces expressions n’étaient prises en charge que dans les champs calculés personnalisés de Workfront.

Pour plus d’informations, consultez [Vue d’ensemble des champs de formule](/help/quicksilver/planning/fields/formula-fields.md).

## Filtres, colonnes et champs supplémentaires ajoutés à l&#39;onglet Planification dans la zone Demandes

>[!NOTE]
>
>* Prévisualisation : vendredi 29 mai 2025
>* Version rapide de production : 12 juin 2025
>* Production pour tous les clients : 17 juillet 2025

Nous avons ajouté la fonctionnalité suivante à une liste de demandes dans l’onglet Planification de la zone des Demandes :

* Colonne « Entré par » pour indiquer la personne qui a ajouté une demande
* Filtres permettant de limiter le nombre de demandes affichées dans l&#39;onglet Planification. Vous pouvez filtrer la liste selon les éléments suivants :

   * Workspace d’où provient le formulaire de demande
   * type d’enregistrement associé au formulaire de demande
   * la date d’entrée de la demande
   * nom du formulaire de demande
   * le statut des requêtes ;
   * nom de la personne qui a saisi la demande.

* Les colonnes permettent d&#39;afficher ou de masquer des champs (ou des colonnes) dans la liste des demandes Planning.

Pour plus d’informations, voir [Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Nouvelle expérience lors de la répartition des enregistrements en mode compact dans la vue chronologique

>[!NOTE]
>
>* Prévisualisation : vendredi 22 mai 2025
>* Version rapide de production : 12 juin 2025
>* Production pour tous les clients : 17 juillet 2025

Nous avons modifié l’expérience lors de la répartition des enregistrements dans la vue Chronologie et la vue Compacte est maintenant appliquée.
Avec la nouvelle mise à jour, lorsque vous définissez vos objets de répartition et que vous affichez la chronologie en mode Compact, vous êtes invité à passer à la vue Standard une fois la configuration des conditions de répartition terminée.

Avant cette amélioration, il n’était pas possible de définir les conditions de répartition lors de l’affichage de la vue chronologique en mode Compact.

Avec cette mise à niveau, l’option Standard est le choix par défaut. Auparavant, le mode Compact était la valeur par défaut.

Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Mettez à jour les paramètres de la vue chronologique pour définir l’aspect des barres des enregistrements connectés lors de l’utilisation de l’option Répartition

>[!NOTE]
>
>* Prévisualisation : vendredi 15 mai 2025
>* Version rapide de production : 12 juin 2025
>* Production pour tous les clients : 17 juillet 2025

Vous pouvez maintenant formater l’aspect des barres d’enregistrement dans la vue chronologique pour les enregistrements de la répartition. Vous pouvez mettre à jour les paramètres suivants pour les barres de ces enregistrements :

* Style de barre
* Couleur

Avant cette amélioration, vous ne pouviez formater que les barres des enregistrements principaux telles qu&#39;elles s&#39;affichaient dans la vue chronologique et vous ne pouviez pas formater les barres des enregistrements connectés.\
 
Pour plus d’informations, voir [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).  

## Exporter la vue du tableau vers un fichier CSV ou Excel 

>[!NOTE]
>
>* Prévisualisation : vendredi 15 mai 2025
>* Version rapide de production : 12 juin 2025
>* Production pour tous les clients : 17 juillet 2025

Nous avons ajouté une nouvelle fonctionnalité à Workfront Planning, qui vous permet d’exporter des informations visibles dans la vue Tableau au format CSV ou Excel.  

Tenez compte des points suivants lors de l’exportation d’informations à partir de la vue Tableau :  

* Les informations exportées prennent en compte les filtres, regroupements et tris appliqués à la vue Tableau dans Workfront Planning.
* Les miniatures et les couleurs de ligne personnalisées ne sont pas prises en charge dans le fichier exporté.  
* Seuls les champs rendus visibles dans l’interface de Workfront sont exportés. Les champs masqués ne sont pas exportés.  

Pour plus d&#39;informations, voir [Gérer la vue du tableau](/help/quicksilver/planning/views/manage-the-table-view.md). 

## Les champs connectés Workfront Planning sont désormais pris en charge lors de l&#39;import d&#39;enregistrements au moyen d&#39;un fichier CSV ou Excel

>[!NOTE]
>
>* Prévisualisation : vendredi 15 mai 2025
>* Version rapide de production : 12 juin 2025
>* Production pour tous les clients : 17 juillet 2025

Vous pouvez désormais remplir les valeurs des champs connectés lorsque vous ajoutez des enregistrements à un type d’enregistrement à l’aide d’un fichier CSV ou Excel.  Seuls les champs d&#39;enregistrement Planning connectés sont pris en charge. Les champs affichant des connexions à d&#39;autres applications ne sont pas pris en charge.

Cette modification est prise en charge lors de l’importation d’un fichier CSV et Excel pour créer un type d’enregistrement et des enregistrements pour un type d’enregistrement existant.

Avant cette amélioration, les champs de connexion ne pouvaient pas être renseignés lorsque vous avez importé des enregistrements.

Pour plus d’informations, voir les articles suivants :

* [Créez des enregistrements en important des informations à partir d’un fichier CSV ou Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).

* [Créez des types d’enregistrements en important des informations à partir d’un fichier CSV ou Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

## Modification en ligne dans la page Enregistrements connectés d’un enregistrement

>[!NOTE]
>
>* Aperçu : 30 avril 2025
>* Version rapide de production : 15 mai 2025
>* Production pour tous les clients : 17 juillet 2025

Vous pouvez désormais modifier des enregistrements dans la page Enregistrements connectés d’un enregistrement. Avec cette mise à jour, nous avons introduit les éléments suivants :

* Le nom de la page a été modifié de « Vue de la connexion » en « Page des enregistrements connectés ».
* Les enregistrements connectés affichés sur cette page sont modifiables en ligne en mode Tableau. Les objets Workfront connectés continuent de s’afficher dans un tableau en lecture seule.

Avant cette amélioration, le tableau de la page d’affichage Connexion était en lecture seule pour les connexions aux enregistrements.

Pour plus d’informations, voir [Gérer la mise en page des enregistrements](/help/quicksilver/planning/records/manage-the-record-page.md).

## Zone Planning visible par défaut dans le menu principal pour les utilisateurs disposant d&#39;une licence standard

>[!NOTE]
>
>* Aperçu : 30 avril 2025
>* Version rapide de production : 15 mai 2025
>* Production pour tous les clients : 17 juillet 2025

Les utilisateurs de Standard et de System Administrator peuvent désormais trouver la zone Planning dans le menu principal par défaut, sans être affectés à un modèle de mise en page qui l&#39;inclut. Pour y accéder, tous les autres utilisateurs doivent disposer d&#39;un modèle de mise en page qui inclut la zone Planning qui leur est affectée.

Avant cette amélioration, les utilisateurs de tous les niveaux de licence devaient être affectés à un modèle de mise en page modifié pour inclure la zone Planning dans le menu principal afin d&#39;accéder à cette zone.

>[!NOTE]
>
>Cette modification sera visible pour tous les utilisateurs nouveaux et existants disposant d’une licence d’administrateur système et standard.
>>Les utilisateurs et utilisatrices existants affectés à un modèle de mise en page continueront à tout voir en fonction des paramètres définis dans le modèle de mise en page.

Pour plus d’informations, consultez [Présentation d’Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

## Formatage des couleurs au niveau des lignes en mode Tableau

>[!NOTE]
>
>* Aperçu : 30 avril 2025
>* Version rapide de production : 15 mai 2025
>* Production pour tous les clients : 17 juillet 2025

Pour une meilleure visibilité des informations importantes de vos enregistrements, nous avons introduit une mise en forme des couleurs au niveau des lignes pour la vue Tableau. Vous pouvez désormais choisir une couleur pour chaque ligne après avoir défini des conditions pour chaque choix.  Il s’agit d’une nouvelle fonctionnalité qui n’existait pas avant cette mise à jour.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

## Nouveau paramètre pour tronquer les noms d’enregistrement longs dans la vue chronologique standard

>[!NOTE]
>
>* Aperçu : 23 avril 2025
>* Version rapide de production : 15 mai 2025
>* Production pour tous les clients : 17 juillet 2025

Vous pouvez désormais activer un paramètre dans l’onglet Style de barre de la zone Paramètres d’une vue chronologique pour tronquer les noms d’enregistrement plus longs lors de leur affichage en vue standard. Le paramètre est désactivé par défaut et ne peut être activé que lorsque vous affichez la vue chronologique en mode Standard. Lorsque ce paramètre est désactivé, les informations des barres d’enregistrement sont développées par défaut. Avant cette amélioration, les informations sur les barres d’enregistrement étaient tronquées par défaut.

Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Autorisations de partage pour les types d’enregistrements


>[!NOTE]
>
>* Aperçu : 17 avril 2025
>* Version rapide de production : 17 juillet 2025
>* Production pour tous les clients : 17 juillet 2025

Pour mieux contrôler qui peut consulter ou gérer les enregistrements dans chaque type d&#39;enregistrement et s&#39;assurer que seules des personnes autorisées peuvent gérer les informations de chaque type d&#39;enregistrement en fonction de leurs rôles et responsabilités, nous avons introduit des autorisations au niveau du type d&#39;enregistrement.

Avant cette amélioration, vous ne pouviez partager que des espaces de travail avec d’autres personnes et l’autorisation qui leur était accordée à un espace de travail appliqué à tous les types d’enregistrements de l’espace de travail.

Nous avons introduit les mises à jour suivantes :

* Les autorisations Workspace sont automatiquement partagées avec tous les types d’enregistrements de l’espace de travail.
* Le niveau des autorisations accordées pour l’espace de travail s’affiche sous la forme d’autorisations héritées pour le type d’enregistrement.
* Vous ne pouvez pas partager un type d’enregistrement avec un niveau d’autorisation supérieur à celui des utilisateurs sur l’espace de travail.
* Vous pouvez désactiver les autorisations héritées sur le type d’enregistrement pour le rendre en lecture seule pour toutes les personnes dans l’espace de travail. Ensuite, vous pouvez ajouter des personnes, des équipes, des groupes, des entreprises ou des rôles individuels et leur accorder l’autorisation de niveau Contribution au type d’enregistrement.

Pour plus d’informations, voir [Partage de types d’enregistrements](/help/quicksilver/planning/access/share-record-types.md).


