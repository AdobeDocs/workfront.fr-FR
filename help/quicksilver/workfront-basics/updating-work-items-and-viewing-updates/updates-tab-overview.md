---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Onglet Mises à jour - Aperçu
description: L’onglet Mises à jour répertorie jusqu’à 200 des mises à jour les plus récentes effectuées au cours des 90 derniers jours.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 19872953e847921c0fee6d383026641c05012ead
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 7%

---

# Onglet Mises à jour - Aperçu

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only for a limited number of objects when you opt in to the new commenting experience Beta.</span> -->

<!-- for preview commenting beta: at the release of commenting beta: change the title to: Updates section overview - also update ALL articles from which this is linked-->

L’onglet Mises à jour répertorie jusqu’à 200 des mises à jour les plus récentes effectuées au cours des 90 derniers jours.

Vous pouvez faire des commentaires et répondre aux mises à jour sur les objets suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Documents</li> 
     <li>Objectifs</li> 
     <li>Événements</li> 
     <li>Itérations</li> 
     <li>Projets</li> 
     <li>Programmes</li> 
     <li>Portefeuilles</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Histoires</li> 
     <li>Tâches</li> 
     <li>Modèles</li> 
     <li>Tâches de modèles</li> 
     <li>Feuilles de temps</li> 
     <li>Utilisateurs</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Mises à jour qui apparaissent également sur les objets de rang supérieur

Comme illustré dans le tableau suivant, les réponses apportées aux mises à jour de certains objets apparaissent également dans l’onglet Mises à jour des objets de rang supérieur.

Par exemple, lorsque vous ajoutez une mise à jour à une tâche, la mise à jour s’affiche dans l’onglet Mises à jour de la tâche et dans l’onglet Mises à jour du projet contenant la tâche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objet où la mise à jour d’origine a été ajoutée</strong> </th> 
   <th> <p><strong>Objet de classement supérieur où la mise à jour d’origine apparaît également</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Problème</td> 
   <td>Projet</td> 
  </tr> 
  <tr> 
   <td>Tâche</td> 
   <td>Projet</td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Programme, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Document </td> 
   <td>Objet où le document est joint, projet </td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>Portfolio</td> 
  </tr> 
  <tr> 
   <td>Utilisateur</td> 
   <td>Équipe</td> 
  </tr> 
  <tr> 
   <td>Feuille de temps</td> 
   <td>Utilisateur, Équipe</td> 
  </tr> 
  <tr> 
   <td>Tâche de modèle</td> 
   <td>Modèle</td> 
  </tr> 
  <tr> 
   <td>Histoire</td> 
   <td>Itération, Équipe</td> 
  </tr> 
  <tr> 
   <td>Itération</td> 
   <td>Équipe</td> 
  </tr>

<tr> 
   <td>Objectifs</td> 
   <td>Résultat, activité</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les réponses ajoutées aux mises à jour système ne sont pas cumulées à l’objet parent. Seules les réponses directes sur un objet enfant et les réponses ajoutées aux mises à jour existantes sont cumulées aux objets parents.
>
>Pour plus d’informations sur la hiérarchie d’objets dans Adobe Workfront, voir [Présentation des objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## Limites de l’onglet Mises à jour

### Limites pour les utilisateurs et les équipes

Vous ne pouvez pas effectuer de mises à jour sur les équipes. L’onglet Mises à jour pour les équipes est renseigné par les mises à jour renseignées sur les objets suivants :

* Utilisateurs
* Feuilles de temps
* Histoires
* Itérations

Dans l’onglet Mises à jour pour les utilisateurs et les équipes, vous pouvez afficher les mises à jour qui ont été saisies au cours des 90 derniers jours.

Si vous souhaitez afficher toutes les mises à jour effectuées sur un utilisateur ou une équipe, au-delà de la limite de 90 jours, vous pouvez créer un rapport pour les notes. Le rapport ne doit pas comporter de filtre horaire qui affiche toutes les mises à jour effectuées pour les utilisateurs ou les équipes. Pour plus d’informations, voir [Création d’un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Restrictions lors de la saisie de commentaires au nom d’un autre utilisateur

Les administrateurs d’Adobe Workfront et les administrateurs de groupe peuvent se connecter en tant qu’autres utilisateurs et effectuer des actions dans Workfront, comme saisir des commentaires. (Pour plus d’informations, voir [Connexion en tant qu’autre utilisateur](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) Tout commentaire fait au nom d’un autre utilisateur est indiqué sur le commentaire.

Un administrateur de groupe peut commenter au nom d’une autre personne, mais ne peut pas supprimer ce commentaire. Seul un administrateur Adobe Workfront peut supprimer un commentaire qu’il a fait au nom d’un autre utilisateur.

## Afficher les mises à jour du système sur les tâches avec le rapport Entrée de journal

Le rapport Entrée de journal répertorie les mises à jour système de la zone Mises à jour des projets, tâches et problèmes.

Le rapport vous permet de voir :

* Nombre de modifications d’état survenues
* Lorsqu’une tâche ou un problème a été supprimé
* Modification des valeurs de champs personnalisés importants au cours d’un projet
* Quelles dates importantes ont changé au cours d’un projet ?
* Si la priorité a changé au cours d’un projet
* Si le propriétaire d’un projet a changé

Pour plus d’informations, voir [Rapport sur la zone Mises à jour](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
