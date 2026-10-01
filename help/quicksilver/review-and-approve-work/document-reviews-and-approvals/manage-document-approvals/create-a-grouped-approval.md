---
product-area: documents
navigation-topic: approvals
title: Créer une validation groupée
description: Vous pouvez regrouper plusieurs ressources dans un seul workflow d’approbation afin qu’elles passent par les mêmes étapes.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: f55042154ac3d93544c152b7b1ad26746a209772
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 3%
---

# Créer une validation groupée

<span class="preview">Les informations de cette page ne sont pas disponibles dans l’environnement de sandbox de prévisualisation, car l’intégration Frame.io n’y est pas disponible. Cette fonctionnalité sera disponible dans les environnements de production les 14 et 15 octobre 2026.</span>

Une approbation groupée regroupe plusieurs ressources dans un seul workflow d’approbation. Vous pouvez utiliser le mode de base et avancé, plusieurs étapes et des chemins d’accès parallèles avec des approbations groupées, comme vous le pouvez avec des approbations de ressources uniques.

Les approbations groupées sont disponibles uniquement dans la zone Nouveaux documents, qui s’affiche lorsque votre organisation utilise l’espace de stockage dans le cloud d’Adobe. Pour plus d’informations, voir [Présentation de l’espace de stockage dans le cloud ](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Package Adobe Workfront</td>
   <td> <p>Tout package de workflow pour gérer les validations à l’aide de l’espace de stockage dans le cloud Adobe</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Licence Adobe Workfront</td>
   <td>
   <p>Contributeur ou supérieur</p>
   <p>Révision ou supérieur</p>
   <p>Pour les objets utilisant l’espace de stockage dans le cloud Adobe, vous devez disposer d’une licence Standard pour créer des workflows d’approbation.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configurations des niveaux d’accès</td>
   <td> <p>Accédez en lecture seule ou à un accès plus étendu aux projets, tâches, événements, modèles, portefeuilles, programmes, rapports, tableaux de bord, calendriers et documents</p></td>
  </tr>
  <tr>
   <td role="rowheader">Autorisations d’objet</td>
   <td> <p>Gérer l’accès à l’objet associé à la demande ou à l’approbation</p></td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une validation groupée de base

Pour créer une validation groupée en une seule étape :

1. Accédez au projet, à la tâche ou à l’événement contenant les documents, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur la première ressource à inclure, puis utilisez la combinaison Maj+clic sur les ressources supplémentaires pour en sélectionner plusieurs.

1. Une fois les ressources sélectionnées, cliquez sur **Demander l’approbation** dans le menu inférieur. La boîte de dialogue **Demander la validation** s’ouvre en mode de base.

   ![créer une validation groupée](assets/requeset-grouped-approval.png)

1. Renseignez les détails suivants :

   <table>
   <tr>
   <td><strong>Utiliser un modèle de validation (optionnel)</strong></td>
   <td>Le champ Modèles est réduit par défaut. Cliquez sur le champ pour le développer, puis sélectionnez un modèle dans le menu déroulant. Si le modèle comporte un chemin d’accès et une étape, il s’applique en mode de base. Si le modèle comporte plusieurs étapes ou plusieurs chemins d’accès, la boîte de dialogue passe automatiquement en mode avancé et toute entrée que vous avez saisie en mode de base est remplacée par le contenu du modèle.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des personnes ou des équipes dans l’aperçu</strong></td>
   <td><p>Commencez à saisir un nom d’utilisateur, une équipe ou une adresse e-mail, puis choisissez s’il s’agit d’un <strong>approbateur</strong> ou d’un <strong>réviseur</strong>. Workfront ajoute individuellement chaque membre actif d’une équipe.</p>
   <p>Remarque : si un utilisateur ou une utilisatrice est déjà ajouté(e) ou appartient à plusieurs équipes que vous ajoutez, il ou elle est inclus(e) une fois.</p></td>
   </tr>
   <tr>
   <td><strong>Une seule décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Échéance le (facultatif)</strong></td>
   <td>Définissez une date d’échéance pour l’approbation. Les utilisateurs sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance spécifiée.</td>
   </tr>
   <tr>
   <td><strong>Ajouter un message personnalisé (facultatif)</strong></td>
   <td>Saisissez un message dans la zone de texte <strong>Ajouter un message personnalisé</strong>. Le message s’affiche dans l’e-mail de notification de validation et dans l’onglet Validations de Workfront.</td>
   </tr>
   </table>

1. (Facultatif) Cliquez sur l’onglet **Documents** pour passer en revue les ressources incluses dans cette approbation.

1. Cliquez sur **Demander l’approbation**.

   ![validation groupée de base](assets/basic-group-approval.png)

## Créer une validation groupée avancée

Le mode avancé prend en charge les chemins d’accès parallèles. Chaque chemin s’exécute indépendamment et contient une ou plusieurs étapes séquentielles. Lorsque toutes les décisions requises d’une étape sont prises, l’étape suivante de ce chemin commence, l’étape précédente est verrouillée et les réviseurs et approbateurs de la nouvelle étape reçoivent une notification par e-mail.

Une décision « A besoin d’être retravaillée » arrête le chemin sur lequel elle se trouve, mais n’affecte pas le workflow d’approbation sur d’autres chemins.

<!--
You can configure up to 30 paths and 100 stages total.
-->

Pour créer une approbation groupée avancée :

1. Accédez au projet, à la tâche ou à l’événement contenant les documents, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur la première ressource à inclure, puis utilisez la combinaison Maj+clic sur les ressources supplémentaires pour en sélectionner plusieurs.

1. Une fois les ressources sélectionnées, cliquez sur **Demander l’approbation** dans le menu inférieur.

   ![créer une validation groupée](assets/requeset-grouped-approval.png)

1. Dans le coin supérieur droit de la boîte de dialogue **Demander l’approbation**, cliquez sur **Aller à l’étape avancée**. Toute entrée entrée entrée en mode de base est conservée et appliquée à **Chemin d’accès 1**, **Étape 1**.

   >[!TIP]
   >
   >Pendant la création de l’approbation, vous pouvez revenir au mode de base en cliquant sur **Accéder au mode de base** dans le coin supérieur droit. Une fois la demande d’approbation soumise, l’option **Accéder à la version de base** n’est plus disponible.

1. Renseignez les détails de l’étape 1 du chemin 1 :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Les étapes sont nommées <em>Étape 1</em>, <em>Étape 2</em>, etc. par défaut. Renommez l’étape en quelque chose de plus explicite, comme <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des personnes ou des équipes dans l’aperçu</strong></td>
   <td><p>Commencez à saisir un nom d’utilisateur, une équipe ou une adresse e-mail, puis choisissez s’il s’agit d’un <strong>approbateur</strong> ou d’un <strong>réviseur</strong>. Workfront ajoute individuellement chaque membre actif d’une équipe.</p>
   <p>Remarque : si un utilisateur ou une utilisatrice est déjà ajouté(e) ou appartient à plusieurs équipes que vous ajoutez, il ou elle est inclus(e) une fois.</p></td>
   </tr>
   <tr>
   <td><strong>Une seule décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Échéance le (facultatif)</strong></td>
   <td>La première étape de chaque chemin prend en charge une date d’échéance absolue. Chaque étape suivante du chemin d’accès prend en charge une date d’échéance relative (nombre de jours à partir duquel cette étape s’ouvre). Les utilisateurs sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance.</td>
   </tr>
   <tr>
   <td><strong>Ajouter un message personnalisé (facultatif)</strong></td>
   <td>Saisissez un message dans la zone de texte <strong>Ajouter un message personnalisé</strong>. Le message s’affiche dans l’e-mail de notification de validation et dans l’onglet Validations de Workfront.<p>Lorsque vous ajoutez une deuxième étape, l’option <strong>Afficher ce message sur toutes les étapes</strong> est sélectionnée par défaut. Laissez-la sélectionnée pour utiliser le même message à chaque étape. Pour utiliser un message différent pour chaque étape, désélectionnez <strong>Afficher ce message sur toutes les étapes</strong>, puis saisissez le message spécifique à l’étape dans la zone de texte <strong>Ajouter un message personnalisé</strong> de chaque étape.</p></td>
   </tr>
   </table>

1. (Facultatif) Ajoutez des étapes supplémentaires au chemin d’accès 1 :
   1. Cliquez sur **Ajouter une étape** pour ajouter une autre étape au chemin d’accès actuel. Les étapes d’un chemin s’exécutent de manière séquentielle dans l’ordre dans lequel elles sont répertoriées.
   1. Renseignez les détails de la nouvelle étape, puis répétez cette étape pour ajouter d’autres étapes si nécessaire.

      >[!NOTE]
      >
      >Vous pouvez réorganiser les étapes d’un chemin, mais vous ne pouvez pas déplacer une étape d’un chemin à un autre. Chaque chemin peut avoir un nombre différent d’étapes.


1. (Facultatif) Ajoutez un chemin d’accès parallèle :
   1. Sous **Chemins parallèles** sur le côté gauche de l’écran, cliquez sur **Ajouter un chemin** pour ajouter un autre chemin.
   1. Suivez les mêmes étapes pour ajouter des étapes et des participants au nouveau chemin. Chaque chemin s’exécute indépendamment. Vous pouvez donc avoir un nombre différent d’étapes et différents participants dans chaque chemin.

1. (Facultatif) Pour supprimer un chemin d’accès, passez le curseur sur le libellé du chemin et cliquez sur l’icône de corbeille. **Le chemin 1** ne peut pas être supprimé et les chemins ne peuvent pas être réorganisés. Les autres chemins ne peuvent être supprimés que si aucune étape du chemin n’est verrouillée ou terminée.

1. (Facultatif) Pour effacer tous les chemins et toutes les étapes et recommencer, cliquez sur **Réinitialiser** dans le coin supérieur droit.

1. (Facultatif) Cliquez sur l’onglet **Documents** pour passer en revue les ressources incluses dans cette approbation.

1. Cliquez sur **Demander l’approbation**.

   ![validation avancée groupée](assets/advanced-group-approval.png)


<!--

## Add additional documents to a grouped approval

You can add additional documents to a grouped approval after the approval has been created as long as the first stage has not been completed. 

To add an additional document to a grouped approval:

1. Click any document in the grouped approval, then click **Manage Approval** in the bottom menu.
1. Click **Documents on this approval**, then click **Add**.

   ![add document grouped approval](assets/add-document-to-grouped-approval.png)
1. Choose the documents you want to add, then click **Add to approval**. 
1. Once you add all of the documents, click **Edit approval**. The new documents are added to the grouped approval and all participants are notified of the change.

-->

## Limites connues

* Actuellement, vous ne pouvez pas ajouter ou supprimer des documents d’un workflow d’approbation groupé une fois qu’il a été créé. Cette fonctionnalité est prévue pour une version ultérieure.
* Les validations groupées sont temporairement limitées à 3 chemins d’accès et 25 ressources par groupe.