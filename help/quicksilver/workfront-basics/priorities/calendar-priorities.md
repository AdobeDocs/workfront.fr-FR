---
navigation-topic: get-started-with-workfront
title: Gérer votre travail dans le calendrier des priorités
description: Suivez votre travail grâce à un calendrier visuel clair.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: d24ad7d1-3a88-479e-beaf-69f8264c9a6b
source-git-commit: 20cb2237a534b51ab5c75e393369bdd92c233efb
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 17%

---

# Gérer votre travail dans le calendrier des priorités

Suivez facilement votre travail grâce à un calendrier visuel clair. Avec le calendrier Priorités, vous pouvez :

* Utiliser des filtres pour trouver votre travail
* Appliquer des champs personnalisés tels que le statut et le niveau de focus pour identifier le travail hautement prioritaire
* Appliquer des couleurs pour une organisation rapide

>[!IMPORTANT]
>
>Les projets doivent avoir le statut Actuel ou un statut équivalent au statut actuel pour afficher les projets ainsi que leurs tâches et événements enfants.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> 
   <p>Current : Reviewer ou supérieur</p>
   <p>Nouveau : Light ou supérieur</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>Accès Afficher ou Modifier à l’objet mis à jour</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Accès Afficher à l’objet</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher votre travail dans le calendrier

Priorités affiche les éléments de travail qui vous sont affectés. Vous ne pouvez pas voir les éléments de travail affectés à votre équipe dans le calendrier Priorités.

{{step1-to-priorities}}

1. Cliquez sur l’icône Calendrier en haut de la liste de travail.
   ![icône de calendrier](assets/calendar-tab.png)
1. Sélectionnez un ou plusieurs filtres pour affiner vos éléments de travail.

   +++Développer pour afficher des informations détaillées sur les filtres disponibles
   <table>
    <tbody>
    <tr>
    <th>Filtre</th>
    <th>Description</th>
    </tr>
        <tr>
        <td>Travail en cours</td>
        <td>Affiche les éléments sur lesquels vous travaillez actuellement</td>
        </tr>
        <tr>
        <td>Démarrage possible</td>
        <td>Affiche les éléments avec 
        <ul>
        <li>Aucune contrainte de tâches ou de prédécesseurs incomplète</li>
        <p>et</p>
        <li>La date de début prévue est dans le passé ou peut être dans les deux semaines à venir</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>À préparer</td>
        <td>Affiche les éléments qui ont
        <ul>
        <li>Prédécesseurs incomplets ou contraintes de tâche empêchant le traitement de l'élément</li>
        <p>ou</p>
        <li>La date de début prévue est dans le futur depuis plus de deux semaines</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Demandé</td>
        <td>Affiche les problèmes sur lesquels vous n'avez pas encore commencé à travailler</td>
        </tr>
        <td>Terminé</td>
        <td>Affiche le travail effectué au cours des deux dernières semaines. Cette option de filtre n’inclut pas les validations.</td>
        </tr>
        <tr>
        <td>Projet</td>
        <td>Affiche les projets contenant des tâches ou des événements qui vous ont été affectés</td>
        </tr>
        <tr>
        <td>Date d’échéance</td>
        <td>Affiche le travail par date d'achèvement prévue</td>
        </tr>
        <tr>
        <td>Statut</td>
        <td>Affiche les tâches ou les événements dont le statut est nouveau, en cours ou terminé</td>
        </tr>
        <tr>
        <td>Mon focus</td>
        <td>Affiche les tâches ou les événements dans auxquels des niveaux de focus ont été affectés. Les niveaux de focus sont attribués et gérés par l’utilisateur individuel.</td>
        </tr>
    </tbody>
    </table>

   +++

1. Cliquez sur la barre d’éléments de travail du calendrier pour ouvrir le résumé latéral. Le résumé latéral vous permet d’effectuer les opérations suivantes :

* Afficher et modifier les détails des projets et des éléments de travail
* Ajouter et afficher des commentaires
* Affichage et chargement de documents
* Créer une épreuve
* Accédez à la page du projet dans Workfront
* Accédez à la page Détails de l’élément de travail dans Priorités
* Enregistrer des heures
* Ajout de liens rapides

1. (Facultatif) Cliquez sur **Créer** pour ajouter un nouvel élément de travail au calendrier. Pour plus d’informations, voir [Créer une nouvelle tâche ou un nouvel événement dans Priorités](/help/quicksilver/workfront-basics/priorities/create-task-issue-priorities.md).

## Configurer le calendrier

{{step1-to-priorities}}

1. Cliquez sur l’icône Calendrier en haut de la liste de travail.
   ![icône de calendrier](assets/calendar-tab.png)
1. Cliquez sur l’icône **Paramètres** dans le coin droit du calendrier.

1. Dans l’onglet **Style de barre**, choisissez jusqu’à 5 champs à afficher dans la barre d’éléments de travail du calendrier.
   ![exemple de barre](assets/sample-task-for-field-config.png)

1. Dans l’onglet **Couleur**, choisissez comment vous souhaitez que vos éléments de travail s’affichent. Par exemple, si vous choisissez Projet, vos éléments de travail s’affichent en fonction de la couleur affectée au projet dans la liste de travail.
   ![exemple de projet de couleur](assets/sample-calendar-projects.png)
