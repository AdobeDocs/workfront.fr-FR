---
product-area: home
navigation-topic: use-the-home-area
title: Gérer votre travail avec le widget Mon travail
description: Le widget Mon travail affiche à un seul endroit toutes les tâches, tous les problèmes et toutes les requêtes qui vous sont assignés. Ici, vous pouvez filtrer et organiser votre travail, consigner le temps, effectuer des mises à jour et marquer les tâches comme terminées.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 20791e9f2cc0716b9b0ddd8f98c31ae0bea7ff45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 15%

---


# Gérer votre travail avec le widget Mon travail

Le widget Mon travail affiche à un seul endroit toutes les tâches, tous les problèmes et toutes les requêtes qui vous sont assignés. Ici, vous pouvez filtrer et organiser votre travail, consigner le temps, effectuer des mises à jour et marquer les tâches comme terminées.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence</strong></td> 
   <td> <p>Actuel : Contribute</p>
   <p>Ou</p> 
   <p>Nouveau :[!UICONTROL Lumière] ou version ultérieure<p> 
  </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>Accès en [!UICONTROL View] ou de niveau supérieur aux projets, tâches, problèmes et documents</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations Contribute ou supérieures aux tâches et problèmes sur lesquels vous devez travailler</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Recherche de votre travail avec des filtres

Vous pouvez affiner les filtres Mon travail pour vous concentrer sur des éléments spécifiques de votre liste de travail :

![](assets/filter-my-work-widget.png)

### Détails du filtre

<table>
  <tbody>
    <tr>
      <td>Utilisation de</td>
      <td>Affiche les éléments sur lesquels vous travaillez actuellement</td>
    </tr>
    <tr>
      <td>Démarrage possible</td>
      <td>Affiche les éléments avec 
      <ul>
      <li>Pas de prédécesseurs incomplets ou de contraintes de tâche</li>
      <p>et</p>
      <li>La date de début planifiée se situe au-delà ou jusqu’à deux semaines à l’avenir.</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>À préparer</td>
      <td>Affiche les éléments qui ont
       <ul>
      <li>Des prédécesseurs incomplets ou des contraintes de tâche qui empêchent l’utilisation de l’élément</li>
      <p>ou</p>
      <li>La date de début planifiée de plus de deux semaines à l’avenir</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Demandé</td>
      <td>Affiche les problèmes sur lesquels vous n’avez pas commencé à travailler.</td>
    </tr>
    <tr>
      <td>Délégué par moi-même</td>
      <td>Affiche les éléments que vous avez délégués à d’autres utilisateurs</td>
    </tr>
    <tr>
      <td>M’a été délégué</td>
      <td>Affiche les éléments que les utilisateurs vous ont délégués.</td>
    </tr>
    <tr>
      <td>Terminé</td>
      <td>Affiche le travail terminé au cours des deux dernières semaines. Cette option de filtre n’inclut pas les validations.</td>
    </tr>
  </tbody>
</table>

>[!TIP]
>
>Si vous recherchez des options de filtrage plus spécifiques, vous pouvez utiliser les widgets Ma tâche ou Mon problème . Pour plus d’informations sur les filtres Ma tâche et Mon problème, consultez la [présentation des filtres de widget New Home](/help/quicksilver/workfront-basics/using-home/new-home/widget-filter-overview-new-home.md).

## Organiser votre travail

Vous pouvez utiliser les fonctions de tri et de groupe du widget Mon travail pour organiser votre travail d’une manière qui vous semble logique.

### Trier

Vous pouvez trier la liste de travail en fonction des

* Date d’échéance
Les éléments en retard affichent une icône d’avertissement en regard de la date. Workfront utilise la date d’achèvement prévue pour déterminer si les tâches et les problèmes sont en retard.
* Nom
* Pourcentage d’achèvement
* Statut

>[!TIP]
>
>Pour créer une liste qui affiche tous les éléments en retard dans la partie supérieure du widget Mon travail, triez-les par date d’échéance et n’appliquez pas de regroupement.


![](assets/sort-my-work-widget.png)

### Groupe

Vous pouvez regrouper la liste de travail par

* Projet
* Statut
* Date d’échéance
La date d’échéance est déterminée par la date d’achèvement planifiée.

>[!NOTE]
>
>Lorsque vous appliquez un groupement, votre sélection dans le menu Tri détermine l’ordre dans lequel il se trouve.


![](assets/group-my-work-widget.png)

## Mise à jour des informations sur les éléments de travail dans le résumé

Vous pouvez ouvrir le panneau Résumé pour mettre rapidement à jour les informations d’une tâche ou d’un problème. Dans le résumé, vous pouvez :

* Mettre à jour le pourcentage terminé
* Ajouter une mise à jour
* Accédez à la zone Document pour télécharger un document.
* Affichage des détails de l’élément de travail et mise à jour des champs personnalisés
Les administrateurs de Workfront peuvent personnaliser les champs qui apparaissent dans le modèle de mise en page Résumé. Pour plus d’informations, voir [Personnaliser l’accueil et le résumé à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Modification de l’état de l’élément de travail
* Afficher les sous-tâches
* Enregistrer des heures
* Afficher les processus d’approbation joints

Pour ouvrir le résumé, passez la souris sur l’élément de travail, puis cliquez sur l’icône **Résumé** ![](assets/open-summary-new-home.png).

Pour plus d’informations sur l’utilisation du panneau Résumé, voir [Aperçu du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

## Utilisation d’actions rapides pour mettre à jour des tâches

Vous pouvez utiliser le menu des actions rapides pour

* Enregistrer des heures
* Ajouter une mise à jour
* Mettre à jour un formulaire personnalisé
* Charger un fichier

Pour localiser le menu des actions rapides, passez la souris sur l’élément de travail . La liste des actions rapides s’affiche près du bouton **Travailler dessus** ou **Terminé** .

![](assets/quick-actions-new-home.png)


## Afficher les approbations et les demandes de l’équipe

Les approbations et les demandes de l’équipe ne s’affichent pas dans le widget Mon travail. Si vous travaillez régulièrement avec les approbations et les demandes de l’équipe, nous vous recommandons d’ajouter les widgets suivants à votre page d’accueil :

* En attente de mon approbation
* Toutes les approbations
* Demandes de l’équipe

Pour plus d’informations sur l’ajout de widgets à votre nouvelle page d’accueil, voir [Ajout, modification ou suppression de widgets dans la nouvelle page d’accueil](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).




