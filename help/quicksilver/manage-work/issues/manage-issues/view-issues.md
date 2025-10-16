---
product-area: projects
navigation-topic: manage-issues
title: Afficher les problèmes
description: Vous pouvez afficher les problèmes associés à un projet, une tâche ou une itération.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: dc4b6dc284c59281206a457395765e634067ba91
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 94%

---

# Afficher les problèmes

<!--Audited: 10/2025-->

Vous pouvez afficher les problèmes associés à un projet, une tâche ou une itération.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <ul><li><p>Contributeur ou version ultérieure</p></li> <li><p>Licence légère ou supérieure pour afficher les événements dans la section Événements d'un projet.</p></li>

Ou

<ul><li><p>Requête ou supérieure</p></li> <li><p>Licence de révision ou une licence supérieure pour afficher les problèmes dans la section Problèmes d’un projet.</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage aux problèmes</p> <p>Affichage ou accès supérieur aux Projets et aux Tâches</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations relatives au problème</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to view issues in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Afficher les problèmes en fonction de leur statut

Pour afficher les problèmes sur un projet, une tâche ou une itération, procédez comme suit :

1. Ouvrez un projet, une tâche ou une itération contenant des problèmes, puis cliquez sur **Problèmes** dans le panneau de gauche.

1. Pour afficher tous les problèmes, ouverts ou fermés, cliquez sur l’un des filtres répertoriés ci-dessous dans le menu déroulant **Filtre**.

>[!TIP]
>
>La liste des filtres varie en fonction de ce que votre administrateur ou administratrice système ou de groupes a choisi d’y afficher.

* **Ouverts :** affiche les problèmes ouverts.

  Cela inclut les problèmes associés à un objet de résolution et ceux dont le statut est Fermé - Approbation en attente.

  Pour plus d’informations sur les objets de résolution, consultez [Vue d’ensemble des objets de résolution et des objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Terminés :** affiche tous les problèmes avec une date d’achèvement effective.
* **Tous :** affiche tous les problèmes.

## Comprendre les informations relatives aux problèmes

Vous pouvez afficher des informations sur un problème lorsque vous y accédez.

Pour accéder à un problème et afficher les informations le concernant,procédez comme suit :

1. Ouvrez un projet, une tâche ou une itération contenant des problèmes, puis cliquez sur **Problèmes** dans le panneau de gauche.
1. Dans le menu déroulant **Filtre**, sélectionnez le filtre permettant d’afficher les problèmes que vous essayez de voir.

   Sélectionnez l’une des options suivantes :

   * Ouvertes
   * Terminé
   * Tout

1. Cliquez sur le nom d’un problème.

   Lorsque vous disposez des autorisations de gestion pour le problème, vous pouvez modifier n’importe quel champ modifiable dans le problème et ajouter des approbations, heures ou documents au problème.

1. Dans le panneau de gauche, cliquez sur l’un des éléments suivants pour afficher plus d’informations sur le problème :

* **Mises à jour** : vous pouvez effectuer les actions suivantes :

   * Commenter le problème ou répondre à un commentaire existant.
   * Consigner le temps.
   * Modifier le statut du problème.

     Pour plus d’informations sur la mise à jour du travail dans Workfront, voir [Mettre à jour le travail](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documents** : vous pouvez joindre des documents au problème. Pour plus d’informations sur l’ajout de documents à Workfront, voir [Ajouter des documents à Adobe Workfront à partir de votre système de fichiers](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Détails du problème** : développez ce lien pour afficher les zones **Vue d’ensemble** et **Formulaires personnalisés**.

  Si vous disposez des autorisations de gestion pour le problème et que vous modifiez les droits sur le formulaire personnalisé, vous pouvez modifier certaines des informations ici.

  Affichez ou modifiez les champs suivants dans la zone **Vue d’ensemble** :

   * **Nom**
   * **Chemin** : chemin d’accès à partir duquel le problème a été consigné dans le projet.

     Si un problème a été envoyé en tant que demande dans une file d’attente des demandes, les noms du projet, du groupe de rubriques et de la rubrique de la file d’attente sont répertoriés ici. Ce champ ne peut pas être modifié.

     Pour plus d’informations sur l’envoi de demandes, voir [Créer et envoyer des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Description**
   * **URL** : toute adresse web relative au problème.
   * **Priorité** : indicateur visuel qui vous permet de hiérarchiser les problèmes.
   * **Gravité** : indicateur visuel qui indique la gravité du problème décrit dans le problème.
   * **Contact principal** : le contact principal par défaut est la personne qui a créé le problème. Ce champ peut être modifié.
   * **Nombre d’heures prévues** : affiche le temps nécessaire à quelqu’un pour terminer le problème. La valeur par défaut est de 8 heures. Ce champ peut être modifié.
   * **Heures effectives** : affiche le temps nécessaire qu’il a fallu pour terminer le problème. Il s’agit du temps effectif que quelqu’un consigne pour le problème.
   * **Date de début prévue** : date de début prévue du problème. La valeur par défaut est la date et l’heure auxquelles le problème a été créé.
   * **Date de début effective** : date et heure auxquelles le statut du problème a été remplacé par En cours.
   * **Date d’achèvement prévue** : date à laquelle le problème devrait être terminé.
   * **Date d’achèvement effective** : date à laquelle le problème est réellement terminé. Ce champ est renseigné automatiquement lorsque le statut du problème passe à Clôturé ou Résolu, ou peut être modifié manuellement.
   * **Coût réel** : coût basé sur les Heures effectives consignées sur le problème. Ce champ n’est pas modifiable. Le coût réel d’un problème est calculé à partir de la formule suivante, où le taux de coût utilisateur est le taux de coût associé à la personne qui consigne le temps passé sur ce problème :

     Coût réel du problème = Heures consignées * Taux de coût utilisateur

   * **Entré par** : il s’agit de la personne ayant créé le problème. Ce champ n’est pas modifiable.
   * **Dernière mise à jour par** : il s’agit de la personne qui a mis à jour en dernier un champ sur le problème. Ce champ n’est pas modifiable.

     Dans la zone **Formulaires personnalisés**, affichez ou sélectionnez un ou plusieurs formulaires personnalisés à associer au problème.

* **Heures** : affiche une liste des entrées d’heure sur le problème.
* **Approbations :** affiche les chemins d’approbation associés au problème.

  Pour plus d’informations sur l’association des approbations à un problème, voir la section [Associer un processus d’approbation à un élément de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) dans [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Afficher les projets et les tâches ayant des problèmes

Vous pouvez ajouter des icônes dans l&#39;affichage d&#39;un rapport ou d&#39;une liste de projet ou de tâche pour indiquer si des problèmes sont associés.

L’ajout d’icônes à la vue de rapport ou de liste est similaire pour les projets et les tâches.

Pour ajouter des icônes qui indiquent si un projet présente des problèmes dans un rapport de projet :

{{step1-click-main-menu}}

1. Cliquez sur **Rapports** > **Nouveau rapport** > **Rapport de projet**.
1. Dans le champ **Afficher dans cette colonne**, commencer à saisir **Icônes de statut**, puis sélectionnez-la lorsqu’elle apparaît dans la liste.

1. Cliquez sur **Enregistrer + Fermer**.

   Les icônes de problème s’affichent sur les projets qui rencontrent des problèmes dans la colonne **Icônes de statut**.

   ![Liste de projets avec icône événement](assets/project-list-with-issue-icon-350x132.png)
