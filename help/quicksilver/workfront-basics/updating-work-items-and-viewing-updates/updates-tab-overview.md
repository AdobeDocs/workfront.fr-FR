---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Présentation de la section Mises à jour
description: La section Mises à jour répertorie jusqu’à 200 des mises à jour les plus récentes effectuées au cours des 90 derniers jours.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# Présentation de la section Mises à jour

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

La section Mises à jour d’un objet affiche les commentaires que les utilisateurs font sur l’objet ou les mises à jour système qui effectuent le suivi des modifications apportées à l’objet.

## Présentation de la section Mises à jour

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

La section Mises à jour d’un objet affiche jusqu’à 200 des mises à jour les plus récentes effectuées au cours des 90 derniers jours.

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

La section Mises à jour présente les informations suivantes :

* Commentaires des utilisateurs et réponses à ces commentaires.
* Mises à jour système qui sont des messages d’information créés par Workfront pour enregistrer certains événements sur un objet. Vous pouvez, par exemple, capturer les modifications de l’état, du nom ou des champs personnalisés avec des mises à jour du système. Votre administrateur Workfront ou de groupe peut activer les mises à jour système pour vos projets. Pour plus d’informations, voir [Configuration des mises à jour du système](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

La section Mises à jour s’affiche pour les objets suivants :

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

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## Mises à jour qui apparaissent également sur les objets de rang supérieur

Comme illustré dans le tableau suivant, les réponses apportées aux mises à jour de certains objets apparaissent également dans la section Mises à jour des objets de rang supérieur.

Par exemple, lorsque vous ajoutez une mise à jour à une tâche, la mise à jour s’affiche dans la section Mises à jour de la tâche et dans la section Mises à jour du projet contenant la tâche.

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

## Limites de la section Mises à jour

### Limites pour les utilisateurs et les équipes

Vous ne pouvez pas effectuer de mises à jour sur les équipes. La section Mises à jour pour les équipes est renseignée par les mises à jour entrées sur les objets suivants :

* Utilisateurs
* Feuilles de temps
* Histoires
* Itérations

Dans la section Mises à jour pour les utilisateurs et les équipes, vous pouvez afficher les mises à jour qui ont été saisies au cours des 90 derniers jours.

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
