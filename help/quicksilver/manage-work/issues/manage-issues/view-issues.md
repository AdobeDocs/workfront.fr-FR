---
product-area: projects
navigation-topic: manage-issues
title: Afficher les problèmes
description: Vous pouvez afficher les problèmes associés à un projet, à une tâche ou à une itération.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# Afficher les problèmes

Vous pouvez afficher les problèmes associés à un projet, à une tâche ou à une itération.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> <p>Passez en revue la licence ou une licence supérieure pour afficher les problèmes dans la section Problèmes d’un projet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Afficher l’accès aux problèmes</p> <p>Affichage ou accès supérieur à Projets et tâches</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux problèmes de votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations pour le problème</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a></p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher les problèmes en fonction de l’état

Pour afficher les problèmes sur un projet, une tâche ou une itération :

1. Ouvrez un projet, une tâche ou une itération contenant des problèmes, puis cliquez sur **Problèmes** dans le panneau de gauche.

1. Pour afficher tous les problèmes, ouverts ou fermés, cliquez sur l’un des filtres répertoriés ci-dessous dans la **Filtrer** menu déroulant.

>[!TIP]
>
>La liste des filtres varie en fonction de ce que votre administrateur système ou groupe a choisi d’afficher dans celui-ci.

* **Ouvrir :** Affiche les problèmes ouverts.

   Cela inclut les personnes associées à un objet de résolution et celles dont l’état Fermé - En attente d’approbation est .

   Pour plus d’informations sur la résolution d’objets, voir [Présentation de la résolution et des objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Terminé :** Affiche tous les problèmes dont la date de fin est réelle.
* **Tous** Affiche tous les problèmes.

## Comprendre les informations relatives aux problèmes

Vous pouvez afficher des informations sur un problème lorsque vous y accédez.

Pour accéder à un problème et afficher les informations le concernant :

1. Ouvrez un projet, une tâche ou une itération contenant des problèmes, puis cliquez sur **Problèmes** dans le panneau de gauche.
1. Dans la **Filtrer** , sélectionnez le filtre pour afficher les problèmes que vous essayez d’afficher.

   Sélectionnez l’une des options suivantes :

   * Ouvrir
   * Terminé
   * Tout

1. Cliquez sur le nom d’un problème.

   Lorsque vous disposez des autorisations de gestion pour le problème, vous pouvez modifier n’importe quel champ modifiable dans le problème et ajouter des approbations, heures ou documents au problème.

1. Dans le panneau de gauche, cliquez sur l’un des éléments suivants pour afficher plus d’informations sur le problème :

* **Mises à jour**: Vous pouvez effectuer les actions suivantes :

   * Commenter sur le problème ou répondre à un commentaire existant.
   * Temps de journalisation.
   * Modifiez l’état du problème.

      Pour plus d’informations sur la mise à jour du travail dans Workfront, voir [Mise à jour du travail](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documents**: Joindre des documents au problème. Pour plus d’informations sur l’ajout de documents à Workfront, voir [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Détails du problème**: Développez ce lien pour afficher le **Présentation** et **Forms personnalisée** zones.

   Si vous disposez des autorisations de gestion pour le problème et que vous modifiez les droits sur le formulaire personnalisé, vous pouvez modifier certaines des informations ici.

   Affichez ou modifiez les champs suivants dans le **Présentation** area :

   * **Nom**
   * **Chemin**: chemin d’accès à partir duquel le problème a été consigné dans le projet.

      Si un problème a été envoyé en tant que requête dans une file d’attente de requêtes, les noms du projet, du groupe de rubriques et de la rubrique de la file d’attente sont répertoriés ici. Ce champ ne peut pas être modifié.

      Pour plus d’informations sur l’envoi de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Description**
   * **URL**: toute adresse web relative au problème.
   * **Priorité**: un indicateur visuel qui vous permet de hiérarchiser les problèmes.
   * **Gravité**: un indicateur visuel qui indique la gravité du problème décrit dans le problème.
   * **Contact Principal**: le contact Principal par défaut est l’utilisateur qui a créé le problème. Ce champ peut être édité.
   * **Heures planifiées**: affiche le temps nécessaire à quelqu’un pour terminer le problème. La valeur par défaut est de 8 heures. Ce champ peut être édité.
   * **Heures réelles**: affiche le temps nécessaire pour terminer le problème. Il s’agit du temps réel pendant lequel quelqu’un consigne le problème.
   * **Date de début planifiée**: date prévue de début du problème. La valeur par défaut est la date et l’heure auxquelles le problème a été créé.
   * **Date de début réelle**: la date et l’heure auxquelles l’état du problème a été remplacé par En cours.
   * **Date d’achèvement prévue**: date à laquelle le problème doit être terminé.
   * **Date d’achèvement réelle**: date à laquelle le problème est effectivement terminé. Ce champ est renseigné automatiquement lorsque l’état du problème passe à Fermé ou Résolu, ou peut être modifié manuellement.
   * **Coût réel**: le coût basé sur les Heures réelles connectées sur le problème. Ce champ n’est pas modifiable. Le coût réel d’une publication est calculé à partir de la formule suivante, où le taux de coût utilisateur est le taux de coût associé à l’utilisateur qui enregistre le temps jusqu’au problème :

      Problème Coût réel = Heures consignées * Taux de coût utilisateur

   * **Entré par**: il s’agit de l’utilisateur qui a créé le problème. Ce champ n’est pas modifiable.
   * **Dernière mise à jour par**: il s’agit de l’utilisateur qui a mis à jour un champ sur le problème en dernier. Ce champ n’est pas modifiable.

      Dans le **Forms personnalisée** Zone , vue de sélectionner un ou plusieurs formulaires personnalisés à associer au problème.

* **Heures**: Affiche une liste d’entrées d’heure sur le problème.
* **Validations :** Affiche les chemins d’approbation associés au problème.

   Pour plus d’informations sur l’association des approbations à un problème, voir la section [Associer un processus d’approbation à un élément de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) dans [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Afficher les projets et les tâches ayant des problèmes

Vous pouvez ajouter des icônes dans la vue d’un projet, d’un rapport de tâche ou d’une liste pour indiquer si des problèmes sont associés. L’ajout d’icônes à l’affichage d’un rapport ou d’une liste est similaire pour les projets et les tâches.

Pour ajouter des icônes qui indiquent si un projet présente des problèmes dans un rapport de projet :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Reporting** > **Nouveau rapport** > **Rapport de projet**.
1. Dans le **Afficher dans cette colonne** champ, commencer à saisir **Icônes d’état**, puis sélectionnez-le lorsqu’il apparaît dans la liste.

1. Cliquez sur **Enregistrer + Fermer** .

   Les icônes de problème s’affichent sur les projets qui rencontrent des problèmes dans le **Icônes d’état** colonne .

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
