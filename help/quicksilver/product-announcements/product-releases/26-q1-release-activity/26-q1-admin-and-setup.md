---
title: Améliorations de l’équipe d’aministration au premier trimestre 2026
description: Améliorations de l’équipe d’aministration au premier trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a74d036b-e4fa-49e0-bb10-4baf379e1b1c
TQID: https://experienceleague.adobe.com/IYlqpTdS-pJNpBaCeYywassuOaTQdaSZlctxd1J0NPA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 669
ht-degree: 96%

---

# Améliorations de l’équipe d’aministration au premier trimestre 2026

Cette page décrit toutes les améliorations de l’équipe d’aministration apportées à l’environnement de prévisualisation par la version du premier trimestre 2026. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du premier trimestre 2026, consultez l’article [Vue d’ensemble de la version du premier trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Gérer les priorités dans le modèle de mise en page

>[!NOTE]
>
>Cette fonctionnalité est temporairement indisponible dans l’environnement de prévisualisation>Prévisualisation : 2 décembre 2025>Version rapide de production : 14 janvier 2026>Production pour tous : 15 janvier 2026


Vous pouvez désormais activer ou désactiver les priorités pour des utilisateurs et utilisatrices spécifiques dans le modèle de mise en page. Si les priorités étaient auparavant désactivées pour votre organisation, elles le resteront dans le modèle de mise en page avec cette modification.

Les priorités seront automatiquement incluses pour les types de licence qui ont un accès par défaut aux demandes. Par exemple, une licence de contributeur verra les demandes, les tableaux et les priorités par défaut dans le menu principal, tandis qu’une licence externe ne verra que les documents et les tableaux parce qu’elle n’a pas accès à l’affichage ou à l’envoi des demandes.


Pour plus d’informations, voir [Personnaliser le menu principal à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Rechercher les conflits de formulaires multiples pour les champs personnalisés calculés

>[!NOTE]
>
>Aperçu : 18 décembre 2025>Version rapide de production : 14 janvier 2026>Production pour tous : 15 janvier 2026

Un même champ calculé peut avoir différentes formules lorsqu’il est joint à différents formulaires personnalisés. Si plusieurs formulaires contenant le même champ calculé sont associés à un objet, les formules doivent être identiques sur tous les formulaires. La modification de la formule n’est pas autorisée si elle peut entraîner un conflit.

Pour déterminer les objets susceptibles d’être affectés lors de la modification d’une expression dans des champs personnalisés, nous avons ajouté une option permettant de vérifier les conflits. Cette boîte de dialogue affiche tous les objets qui pourraient être affectés par la modification de la formule, regroupés par type d’objet. Vous pouvez accéder aux détails de chaque objet et consulter les champs pour décider si le champ doit être supprimé de l’un des formulaires ou si l’expression doit rester inchangée.

Pour plus d’informations, voir [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Date de saisie et ID Saisi par stockés dans des objets personnalisés

>[!NOTE]
>
>Aperçu : 13 novembre 2025>Version rapide de production : 13 novembre 2025>Production pour tous : 13 novembre 2025

La date de saisie et l’ID Saisi par sont désormais stockés dans des formulaires, champs et sections personnalisés. Vous pouvez utiliser ces options de données dans les rapports sous la forme de filtres, de vues ou de regroupements. Pour les afficher dans la liste des formulaires, champs ou sections personnalisés de la configuration, ajoutez Date de saisie et Saisi par : nom sous forme de colonnes dans une vue nouvelle ou existante.

>[!NOTE]
>
>La date de saisie et l’ID Saisi par sont disponibles uniquement sur les formulaires, champs et sections personnalisés créés le 13 novembre 2025 ou après cette date.

## Mises à jour des noms de bouton lors de la modification d’un modèle de mise en page

>[!NOTE]
>
>Aperçu : 30 octobre 2025>Version rapide de production : 13 novembre 2025>Production pour tous : 15 janvier 2026

Pour plus de cohérence avec d’autres zones de la configuration telles que le concepteur de formulaire personnalisé, les boutons affichés lors de la modification d’un modèle de mise en page ont été modifiés en **Appliquer**, **Enregistrer et fermer** et **Annuler**. La nouvelle option, **Appliquer**, vous permet d’enregistrer vos modifications dans le modèle de mise en page et de continuer la modification. Auparavant, les options disponibles étaient **Enregistrer** et **Annuler**.

Pour plus d’informations, voir [Créer et gérer des modèles de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Amélioration de la gestion des champs avec l’indicateur Actif sur les champs personnalisés

>[!NOTE]
>
>Aperçu : 30 octobre 2025>Version rapide de production : 13 novembre 2025>Production pour tous : 15 janvier 2026

Lorsque le système comporte un grand nombre de champs personnalisés, la gestion de ces champs dans les formulaires et les rapports personnalisés peut s’avérer difficile. Vous pouvez désormais marquer les champs personnalisés comme inactifs avec le nouvel indicateur **Actif**. Cet indicateur est disponible lors de l’utilisation d’un champ dans un formulaire personnalisé ou lors de l’ajout ou de la modification d’un champ de la liste Champs.

Si vous marquez un champ comme inactif :

* Il est exclu des rapports, filtres, vues ou autres emplacements de Workfront dans lesquels vous pouvez ajouter un champ personnalisé.
* Il n’est pas disponible dans la bibliothèque de champs pour être ajouté à d’autres formulaires personnalisés.

>[!NOTE]
>
>Marquer un champ existant comme inactif le rend indisponible pour une utilisation dans les éléments de rapports et les formulaires personnalisés à partir de ce moment. Si le champ inactif est actuellement utilisé dans un rapport ou un formulaire, le champ et ses données historiques restent en place.

Pour plus d’informations, voir [Ajouter ou modifier un champ personnalisé, un saut de section ou un widget](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md).
