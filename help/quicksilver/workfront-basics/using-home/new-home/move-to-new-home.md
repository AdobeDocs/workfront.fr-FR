---
product-area: home
navigation-topic: use-the-home-area
title: Passage de la page d’accueil héritée à la nouvelle page d’accueil
description: La page d’accueil héritée sera supprimée de Workfront le 10/17 avec la version Q4. Cet article fournit des informations sur les fonctionnalités qui seront disponibles dans la nouvelle page d’accueil, ainsi que des recommandations pour déplacer les utilisateurs vers l’expérience de nouvelle page d’accueil.
author: Courtney
feature: Get Started with Workfront
source-git-commit: b34de7dc66d69b030e313ee891a7404e1d5470e8
workflow-type: tm+mt
source-wordcount: '1596'
ht-degree: 34%

---


# Passage de la page d’accueil héritée à la nouvelle page d’accueil

La page d’accueil héritée sera supprimée de Workfront le 10/17 avec la version Q4. Cet article fournit des informations sur les fonctionnalités qui seront disponibles dans la nouvelle page d’accueil, ainsi que des recommandations à l’intention des administrateurs de Workfront qui déplacent les utilisateurs vers la nouvelle expérience d’accueil.

Pour plus d’informations sur l’obsolescence de la page d’accueil héritée, consultez le [Guide de l’obsolescence de la page d’accueil héritée](/help/quicksilver/product-announcements/announcements/legacy-home-deprecation.md).


## Comprendre ce qui change de la page d’accueil héritée à la nouvelle page d’accueil

### Liste de travail

#### Organisation du travail avec le widget Mon travail

Le widget Mon travail a été créé sous forme de widget pour refléter autant que possible la liste de travail Hérité de l’accueil. Les utilisateurs peuvent regrouper et filtrer leur liste de tâches dans le widget Mon travail avec des filtres et des regroupements similaires :

| **Filtre** | **Regroupement** |
|------------|-----------|
| - Travail sur <br> - Prêt à démarrer <br> - Non prêt <br> - Demandé <br> - Délégué <br> - Terminé | - Projet <br> - État <br> - Date d’échéance <br> - Rien |


**Regroupements d&#39;hôtes hérités non disponibles dans Nouvelle page d&#39;accueil**

* Date d’achèvement prévue - renommée Date d’échéance dans la nouvelle page d’accueil
* Démarrage planifié
* Date d’engagement
* Ma priorité

| **Page d’accueil héritée** | **New Home** |
|------------|-----------|
| ![](assets/filter-list-legacy.png) | ![](assets/filter-list-my-work.png) |

#### Déléguer le travail

Les utilisateurs peuvent toujours déléguer du travail à partir de la nouvelle page d’accueil dans les widgets suivants :

* Mon travail
* Mes tâches
* Mes problèmes
* En attente de mes approbations

Les utilisateurs peuvent trouver du travail qui leur est délégué dans les widgets suivants :

* Mon widget de travail à l’aide du filtre Délégué à moi
* En attente de mes validations à l’aide du filtre des validations déléguées

| **Page d’accueil héritée** | **New Home** |
|------------|-----------|
| ![](assets/delegate-legacy.png) | ![](assets/delegate-my-work.png) |

#### Utilisation de la vue Calendrier

La vue Calendrier n’est plus disponible dans Nouvelle page d’accueil. Cependant, un remplacement du calendrier figure sur la feuille de route des priorités.

#### Créer une tâche personnelle

Les utilisateurs ne peuvent plus créer de tâche personnelle exactement comme ils l’ont fait dans la page d’accueil héritée. Au lieu de cela, ils peuvent créer des tâches.

#### Afficher les validations que j’ai envoyées

Les utilisateurs ne peuvent pas afficher les validations qu’ils ont envoyées dans New Home. Si les utilisateurs de votre entreprise ont besoin de cette fonctionnalité, vous pouvez créer un rapport d’approbation comme solution de contournement, modifier ou publier un commentaire ici dans les publications de la communauté suivantes :

* [ Ajoutez le widget &quot;Approbations que j’ai envoyées&quot; à la nouvelle page d’accueil ](https://experienceleaguecommunities.adobe.com/t5/workfront-ideas/add-quot-approvals-i-submitted-quot-widget-to-new-home/idc-p/704664#M25269)
* [ Ajoutez &quot;Approbations que j’ai envoyées&quot; au nouvel accueil ](https://experienceleaguecommunities.adobe.com/t5/workfront-ideas/add-quot-approvals-i-submitted-quot-widget-to-new-home/idc-p/704664#M25269)

#### Ajout d’éléments à ma priorité

Les utilisateurs n’ont plus accès à une fonctionnalité Ma priorité dans la nouvelle page d’accueil. Nous introduisons une nouvelle colonne Mon point de mires avec des priorités qui la remplaceront.

Si vous le souhaitez, les utilisateurs peuvent utiliser le widget Panoramas pour effectuer le suivi des éléments de priorité élevée.

### Mise à jour des éléments de travail

Dans la page d’accueil héritée, les utilisateurs peuvent utiliser le panneau approprié pour mettre à jour leur travail. Dans Nouvelle page d’accueil, les utilisateurs utilisent désormais le panneau Résumé pour mettre à jour le travail. Il s’agit du même panneau Résumé disponible dans les Projets, tâches, problèmes et documents.

#### Utilisation du panneau Résumé

Dans le résumé, les utilisateurs peuvent

* Mettre à jour le pourcentage terminé
* Ajouter une mise à jour
* Accédez à la zone Documents pour télécharger un document.
* Affichage des détails de l’élément de travail et mise à jour des champs personnalisés
Les administrateurs de Workfront peuvent personnaliser les champs qui apparaissent dans le modèle Résumé de la mise en page. Pour plus d’informations, voir [Personnaliser l’accueil et le résumé à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Modification de l’état de l’élément de travail
* Afficher les sous-tâches
* Enregistrer des heures
* Afficher les processus d’approbation joints
* Chargement de fichiers - Cette fonctionnalité est nouvelle

| **Page d’accueil héritée** | **New Home** |
|------------|-----------|
| ![](assets/right-panel-legacy.png) | ![](assets/summary-new-home.png) |


#### Ouvrir le panneau de résumé

Les utilisateurs peuvent ouvrir le panneau Résumé en survolant l’élément de travail, puis en cliquant sur l’icône **Résumé** ![](assets/open-summary-new-home.png).

Pour plus d’informations sur l’utilisation du panneau Résumé, voir [Aperçu du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

#### Utilisation d’actions rapides

Outre le panneau Résumé, les utilisateurs peuvent également utiliser des actions rapides pour

* Enregistrer des heures
* Ajouter une mise à jour
* Mettre à jour un formulaire personnalisé
* Charger un fichier

Pour localiser le menu des actions rapides, passez la souris sur l’élément de travail . La liste des actions rapides s’affiche près du bouton **Travailler dessus** ou **Terminé** .

![](assets/quick-actions-new-home.png)


### Afficher les approbations et les demandes de l’équipe

Les utilisateurs peuvent toujours gérer les approbations et les demandes de l’équipe dans la nouvelle page d’accueil à l’aide des widgets suivants :

* En attente de mon approbation
* Toutes les approbations
* Demandes de l’équipe

Pour plus d’informations sur l’ajout de widgets à votre nouvelle page d’accueil, voir [Ajout, modification ou suppression de widgets dans la nouvelle page d’accueil](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).

## Découvrez les widgets disponibles

Les widgets sont la base de la Nouvelle Maison. En ajoutant des widgets à la page d’accueil, les utilisateurs peuvent choisir le type d’informations qui s’affiche pour répondre le mieux à leurs besoins. Certains widgets ne sont disponibles que pour des types de licences spécifiques, car les objets qu’ils suivent ne sont disponibles que pour ces licences.

Les administrateurs de Workfront peuvent personnaliser les widgets disponibles dans la nouvelle page d’accueil à l’aide d’un modèle de mise en page. Pour plus d’informations, consultez la section [Personnaliser la nouvelle page d’accueil à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md).

+++ Développer pour afficher une liste détaillée des widgets disponibles
Vous trouverez ci-dessous les 11 widgets actuellement disponibles, ainsi qu’un résumé des informations qu’ils affichent :

* **Mes tâches**\
   Affiche toutes les tâches, problèmes et requêtes affectés au même endroit. Vous pouvez cliquer sur le bouton Travailler sur ce projet pour commencer à travailler sur un élément ou sur le bouton Terminé pour le marquer comme terminé. Vous pouvez également mettre à jour des informations (statut, condition, pourcentage terminé) sur les tâches et les problèmes, consigner des heures et ajouter des mises à jour à partir du widget Mon travail.

* **Panoramas**\
    Affiche tous les panoramas que vous avez créés ou que vous avez été invité à utiliser. Vous pouvez également créer un panorama à partir des modèles suivants : Panorama de base, Panorama Kanban, Panorama rétrospectif, Panorama dynamique.

* **Mes projets**\
    Affiche les _projets que vous possédez_ ou les _projets sur lesquels vous êtes_ dans une liste. Vous pouvez utiliser les filtres, les vues ou les regroupements existants pour personnaliser la liste, ou vous pouvez créer un projet directement à partir du widget.

* **Mes tâches**\
    Affiche les tâches qui vous sont affectées dans une liste. Vous pouvez utiliser les filtres, les vues ou les regroupements existants pour personnaliser la liste, ou vous pouvez créer une tâche directement à partir du widget. Vous pouvez également déléguer vos tâches lorsque vous n’êtes pas au bureau.

* **Mes problèmes**\
    Affiche les problèmes qui vous sont attribués dans une liste. Vous pouvez utiliser des filtres, des vues ou des regroupements existants pour personnaliser la liste, ou créer un problème directement à partir du widget. Ce widget comprend uniquement les problèmes dont les projets associés sont définis sur Actuel et n’incluent pas les projets terminés. Vous pouvez également déléguer vos problèmes lorsque vous n’êtes pas au bureau.

* **Mes demandes**\
    Affiche toutes les requêtes que vous avez envoyées, un filtre permettant d’afficher uniquement les requêtes ouvertes et un bouton permettant d’ouvrir le panneau de résumé d’une requête.

* **Demandes de l’équipe**\
    Affiche toutes les demandes en attente classées par équipe pour les équipes dont vous faites partie, ainsi que des boutons permettant d’attribuer directement une demande à un utilisateur ou à une utilisatrice ou d’y travailler soi-même.

* **En attente de mon approbation**\
    Affiche toutes les approbations affectées ou déléguées en attente, un bouton pour déléguer des approbations et des boutons pour prendre des décisions d’approbation directement dans le widget.

* **Toutes les approbations**\
        Affiche 2 graphiques avec des informations sur le temps d’approbation moyen et les décisions, ainsi que des listes de vues des approbations en attente et en retard. <span style="color: #ff0000;">Cette fonctionnalité fait partie d’une version progressive et n’est actuellement disponible que pour certains clientes et clients.</span>

* **Mentions**\
    Affiche les fils de commentaires récents provenant de Workfront, comme sur la page Mes mises à jour . Vous pouvez utiliser le bouton de réponse pour rédiger une réponse dans le widget. Ce widget affiche également les commentaires sur les tâches et les problèmes qui vous sont affectés, que vous avez affectés à un autre utilisateur ou une autre utilisatrice, qui vous appartiennent, dont vous êtes le contact principal ou que vous avez créés, à condition que l’élément ait été mis à jour au cours des 30 derniers jours.

* **À faire**\
    Ce widget unique vous permet d’ajouter des éléments à une liste de contrôle personnelle que vous pouvez modifier librement. Les tâches À faire sont suivies en tant que tâches dans votre projet personnel et restent jusqu’à deux semaines après leur achèvement.

  >[!NOTE]
  >
  >Vous devez disposer des autorisations nécessaires pour créer des tâches afin de créer des tâches dans le widget À faire. Seules les tâches personnelles saisies par l’utilisateur ou utilisatrice actuel apparaîtront dans le widget.

+++

  ![](assets/widgets-menu.png)

### Afficher les widgets disponibles pour chaque type de licence

Par défaut, la page d’accueil contient quelques widgets spécifiques en fonction de votre type de licence. Les tableaux ci-dessous indiquent les widgets que les utilisateurs et utilisatrices de chaque type de licence voient lorsqu’ils naviguent pour la première fois dans la nouvelle page d’accueil.

<table border="1" class="inlineTable">
    <tr>
        <td><b>Nouveau type de licence</b></td>
        <td><b>Widgets par défaut</b></td>
    </tr>
    <tr>
        <td>Standard</td>
        <td>Mes projets, Mon travail, Mentions, À faire</td>
    </tr>
    <tr>
        <td>Léger</td>
        <td>Mon travail, En attente de mon approbation</td>
    </tr>
    <tr>
        <td>Contributeur</td>
        <td>Mes demandes, Mentions, En attente de mon approbation, Panoramas</td>
    </tr>
    <tr>
        <td>Externe</td>
        <td>En attente de mon approbation</td>
    </tr>
</table>

<table border="1" class="inlineTable">
    <tr>
        <td><b>Type de licence actuel</b></td>
        <td><b>Widgets par défaut</b></td>
    </tr>
    <tr>
        <td>Plan</td>
        <td>Mes projets, Mentions, À faire</td>
    </tr>
    <tr>
        <td>Travail</td>
        <td>Mon travail, Mentions, À faire</td>
    </tr>
    <tr>
        <td>Vérifier</td>
        <td>Mon travail, Mentions</td>
    </tr>
    <tr>
        <td>Demande</td>
        <td>Mes projets, En attente de mon approbation</td>
    </tr>
    <tr>
        <td>Contribuer</td>
        <td>Mon travail, Mentions</td>
    </tr>
    <tr>
        <td>Externe</td>
        <td>En attente de mon approbation</td>
    </tr>
</table>

## Préparation de l’obsolescence

Afin de minimiser les perturbations pour vous et votre organisation, vous trouverez ci-dessous quelques recommandations qui aideront à faciliter la transition.

### Commencer la transition vers la nouvelle page d’accueil

Notre recommandation principale est de commencer la transition vers le nouveau domicile dès que possible. Sur le plan organisationnel, cela signifie que votre administrateur personnalise les expériences des utilisateurs par le biais de modèles de mise en page (semblables à la page d’accueil héritée) afin de s’assurer que chaque utilisateur dispose de ce dont il a besoin.

Nous recommandons aux administrateurs :

1. Créez une mise en page de page d’accueil par défaut à l’aide de modèles de mise en page (ou, éventuellement, créez-en un pour chaque utilisateur, équipe, groupe ou rôle de tâche qui nécessite une mise en page unique). Pour plus d’informations, voir [Personnaliser la nouvelle page d’accueil à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md) .

1. Affectez vos nouveaux modèles de mise en page à un petit nombre d’utilisateurs de test, qui peuvent vérifier que leurs widgets et paramètres généraux répondent à leurs besoins.

1. Réaffectez le reste de vos utilisateurs à la disposition Nouvelle page d’accueil.

Cela donnera dès que possible à vos utilisateurs le temps de s’adapter à la nouvelle expérience et de personnaliser leurs pages d’accueil en fonction de leurs besoins. Voir [Suppression, ajout et réorganisation de widgets dans la nouvelle page d’accueil](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md) pour plus d’informations sur la manière dont un utilisateur peut personnaliser les widgets sur sa propre nouvelle page d’accueil.