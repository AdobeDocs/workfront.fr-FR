---
product-area: documents
navigation-topic: approvals
title: Créer un workflow d’approbation de document
description: Vous pouvez demander l’approbation d’un document à d’autres utilisateurs et utilisatrices dans Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OoGv4oNg6GkKeo-zoVi5lSxtPK3UE64-EYW21Mz7GRA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 2231
ht-degree: 6%

---

# Créer un workflow d’approbation de document

Vous pouvez demander à d’autres personnes ou équipes d’approuver un document dans Adobe Workfront, ou leur demander de réviser un document sans avoir à l’approuver.

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus d’approbation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les approbations à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les validations à l’aide de l’espace de stockage dans le cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td>  
   <td>
   <p>Contributeur ou supérieur</p>
   <p>Révision ou supérieur</p>
   <p>Si vous utilisez l'intégration Frame.io, vous devez disposer d'une licence Standard pour créer des workflows d'approbation.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Affichage ou accès supérieur pour Projets, Tâches, Problèmes, Modèles, Portfolios, Programmes, Rapports, Tableaux de bord, Calendriers et Documents</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès à l’objet associé à la demande d’accès ou d’approbation </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

## Create an approval workflow in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Select the version of the document you would like to create an approval for in the version dropdown. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)

-->

## Créer un workflow d’approbation dans la zone des documents hérités

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage cloud Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

### Créer un workflow d’approbation de base

Pour créer un workflow d’approbation en une seule étape :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Sélectionnez la version du document pour lequel vous souhaitez créer une approbation dans le menu déroulant Version. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**. La boîte de dialogue **Demander la validation** s’ouvre en mode de base.

1. Renseignez les détails suivants :

   <table>
   <tr>
   <td><strong>Utiliser un modèle de validation (optionnel)</strong></td>
   <td>Sélectionnez un modèle dans le menu déroulant. Si le modèle comporte un chemin d’accès et une étape, il s’applique en mode de base. Si le modèle comporte plusieurs étapes ou plusieurs chemins d’accès, la boîte de dialogue passe automatiquement en mode avancé et toute entrée que vous avez saisie en mode de base est remplacée par le contenu du modèle.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Si vous avez uniquement des réviseurs, ils seront avertis et auront la possibilité de terminer la révision, mais aucune décision ne sera requise ou prise.</td>
   </tr>
   <tr>
   <td><strong>Une seule décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Échéance le (facultatif)</strong></td>
   <td>Définissez une date d’échéance pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance spécifiée.</td>
   </tr>
   <tr>
   <td><strong>Ajouter un message personnalisé (facultatif)</strong></td>
   <td>Saisissez un message dans la zone de texte <strong>Ajouter un message personnalisé</strong>. Le message s’affiche dans l’e-mail de notification de validation et dans l’onglet Validations de Workfront.
   <p>Remarque : si vous modifiez un message personnalisé après la création du workflow d’approbation, une notification par e-mail mise à jour est envoyée à tous les participants existants. Si vous ajoutez un participant ultérieurement, le message personnalisé est inclus dans sa notification par e-mail.</p>
   </td>
   </tr>
   </table>

1. Cliquez sur **Demander l’approbation**.

   ![Demander la validation en mode de base](assets/request-approval-basic.jpeg)

### Création d’un workflow de validation avancée

Le mode avancé prend en charge plusieurs étapes ainsi que des chemins d’accès parallèles. Chaque chemin s’exécute indépendamment et contient une ou plusieurs étapes séquentielles. Lorsque toutes les décisions requises d’une étape sont prises, l’étape suivante de ce chemin commence, l’étape précédente est verrouillée et les réviseurs et approbateurs de la nouvelle étape reçoivent une notification par e-mail.

Une décision « A besoin d’être retravaillée » arrête le chemin qui lui est associé, mais n’affecte pas le workflow d’approbation des autres chemins. Vous pouvez configurer jusqu’à 30 chemins et 100 étapes au total.

Pour créer un workflow de validation avancée :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Sélectionnez la version du document pour lequel vous souhaitez créer une approbation dans le menu déroulant Version. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**.

1. Dans le coin supérieur droit de la boîte de dialogue **Demander l’approbation**, cliquez sur **Aller à l’étape avancée**. Toute entrée entrée entrée en mode de base est conservée et appliquée à **Chemin d’accès 1**, **Étape 1**.

   >[!TIP]
   >
   >Pendant la création de l’approbation, vous pouvez revenir au mode de base en cliquant sur **Accéder au mode de base** dans le coin supérieur droit. Après avoir cliqué sur **Demander l’approbation**, l’option **Accéder à la version de base** n’est plus disponible.

1. Renseignez les détails de l’étape 1 du chemin 1 :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Les étapes sont nommées <em>Étape 1</em>, <em>Étape 2</em>, etc. par défaut. Renommez l’étape en quelque chose de plus explicite, comme <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Si vous avez uniquement des réviseurs, ils seront avertis et auront la possibilité de terminer la révision, mais aucune décision ne sera requise ou prise.<p>Remarque : un réviseur ou un approbateur ne peut être affecté qu’à une seule étape ouverte à la fois sur la même ressource. Si plusieurs étapes parallèles sont ouvertes simultanément, la même personne ne peut pas être ajoutée à plusieurs d’entre elles.</p></td>
   </tr>
   <tr>
   <td><strong>Une seule décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Échéance le (facultatif)</strong></td>
   <td>La première étape de chaque chemin prend en charge une date d’échéance absolue. Chaque étape suivante du chemin prend en charge une date d’échéance relative, à savoir le nombre de jours à partir duquel cette étape s’ouvre. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance.</td>
   </tr>
   <tr>
   <td><strong>Ajouter un message personnalisé (facultatif)</strong></td>
   <td>Saisissez un message dans la zone de texte <strong>Ajouter un message personnalisé</strong>. Le message s’affiche dans l’e-mail de notification de validation et dans l’onglet Validations de Workfront.<p>Lorsque vous ajoutez une deuxième étape, l’option <strong>Afficher ce message sur toutes les étapes</strong> est sélectionnée par défaut. Laissez-la sélectionnée pour utiliser le même message à chaque étape. Pour utiliser un message différent pour chaque étape, désélectionnez <strong>Afficher ce message sur toutes les étapes</strong>, puis saisissez le message spécifique à l’étape dans la zone de texte <strong>Ajouter un message personnalisé</strong> de chaque étape.</p></td>
   </tr>
   </table>

1. (Facultatif) Cliquez sur **Ajouter une étape** pour ajouter une autre étape au chemin d’accès. Les étapes d’un chemin s’exécutent de manière séquentielle dans l’ordre dans lequel elles sont répertoriées. Vous pouvez réorganiser les étapes d’un chemin, mais vous ne pouvez pas déplacer une étape d’un chemin à un autre. Chaque chemin peut avoir un nombre différent d’étapes.

1. (Facultatif) Sous **Chemins parallèles**, cliquez sur **Ajouter un chemin** pour ajouter un autre chemin. Le nouveau chemin commence par une étape vide et devient le chemin sélectionné. Pour renommer un chemin d’accès, pointez sur le libellé du chemin d’accès, cliquez sur l’icône en forme de crayon, puis saisissez un nouveau nom.

1. (Facultatif) Pour supprimer un chemin d’accès, passez le curseur sur le libellé du chemin et cliquez sur l’icône de corbeille. **Le chemin 1** ne peut pas être supprimé et les chemins ne peuvent pas être réorganisés. Les autres chemins ne peuvent être supprimés que si aucune étape du chemin n’est verrouillée ou terminée.

   ![Mode avancé avec chemins parallèles](assets/request-approval-parallel-paths.jpeg)

1. (Facultatif) Pour effacer tous les chemins et toutes les étapes et recommencer, cliquez sur **Réinitialiser** en haut à droite.

1. Cliquez sur **Demander l’approbation**.


<!--

## Create an approval workflow in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)
   
-->

## Créer un workflow d’approbation dans la zone Nouveaux documents

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

La boîte de dialogue **Demander la validation** s’ouvre par défaut en mode **De base**. Le mode de base est une étape unique avec un ensemble d’approbateurs ou de réviseurs. Passez en mode **Avancé** pour configurer les validations à plusieurs étapes ou les chemins d’accès parallèles.

### Créer un workflow d’approbation de base

Pour créer un workflow d’approbation en une seule étape :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Créer un workflow**. La boîte de dialogue **Demander la validation** s’ouvre en mode de base.

1. Renseignez les détails suivants :

   <table>
   <tr>
   <td><strong>Utiliser un modèle de validation (optionnel)</strong></td>
   <td>Le champ Modèles est réduit par défaut. Cliquez sur le champ pour le développer, puis sélectionnez un modèle dans le menu déroulant. Si le modèle comporte un chemin d’accès et une étape, il s’applique en mode de base. Si le modèle comporte plusieurs étapes ou plusieurs chemins d’accès, la boîte de dialogue passe automatiquement en mode avancé et toute entrée que vous avez saisie en mode de base est remplacée par le contenu du modèle.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Si vous avez uniquement des réviseurs, ils seront avertis et auront la possibilité de terminer la révision, mais aucune décision ne sera requise ou prise.</td>
   </tr>
   <tr>
   <td><strong>Une seule décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Échéance le (facultatif)</strong></td>
   <td>Définissez une date d’échéance pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance spécifiée.</td>
   </tr>
   <tr>
   <td><strong>Ajouter un message personnalisé (facultatif)</strong></td>
   <td>Saisissez un message dans la zone de texte <strong>Ajouter un message personnalisé</strong>. Le message s’affiche dans l’e-mail de notification de validation et dans l’onglet Validations de Workfront.</td>
   </tr>
   </table>

1. Cliquez sur **Demander l’approbation**.

   ![Demander la validation en mode de base](assets/request-approval-basic.jpeg)

>[!NOTE]
>
>* La boîte de dialogue **Demander la validation** s’ouvre en mode de base à chaque fois, quelle que soit votre session précédente.
>* Si vous modifiez un message personnalisé après la création du workflow d’approbation, une notification par e-mail mise à jour est envoyée à tous les participants existants. Si vous ajoutez un participant ultérieurement, le message personnalisé est inclus dans sa notification par e-mail.
>* Une fois une approbation enregistrée, vous ne pouvez pas la faire revenir au mode de base. Vous pouvez faire passer une approbation en cours de Base à Avancé tant que l’approbation n’est pas verrouillée ou terminée.

### Création d’un workflow de validation avancée

Le mode avancé prend en charge les chemins d’accès parallèles. Chaque chemin s’exécute indépendamment et contient une ou plusieurs étapes séquentielles. Lorsque toutes les décisions requises d’une étape sont prises, l’étape suivante de ce chemin commence, l’étape précédente est verrouillée et les réviseurs et approbateurs de la nouvelle étape reçoivent une notification par e-mail.

Une décision « A besoin d’être retravaillée » arrête le chemin qui lui est associé, mais n’affecte pas le workflow d’approbation des autres chemins. Vous pouvez configurer jusqu’à 30 chemins et 100 étapes au total.

Pour créer un workflow de validation avancée :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Créer un workflow**.

1. Dans le coin supérieur droit de la boîte de dialogue **Demander l’approbation**, cliquez sur **Aller à l’étape avancée**. Toute entrée entrée entrée en mode de base est conservée et appliquée à **Chemin d’accès 1**, **Étape 1**.

   >[!TIP]
   >
   >Pendant la création de l’approbation, vous pouvez revenir au mode de base en cliquant sur **Accéder au mode de base** dans le coin supérieur droit. Après avoir cliqué sur **Demander l’approbation**, l’option **Accéder à la version de base** n’est plus disponible.

1. Renseignez les détails de l’étape 1 du chemin 1 :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Les étapes sont nommées <em>Étape 1</em>, <em>Étape 2</em>, etc. par défaut. Renommez l’étape en quelque chose de plus explicite, comme <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Si vous avez uniquement des réviseurs, ils seront avertis et auront la possibilité de terminer la révision, mais aucune décision ne sera requise ou prise.<p>Remarque : un réviseur ou un approbateur ne peut être affecté qu’à une seule étape ouverte à la fois sur la même ressource. Si plusieurs étapes parallèles sont ouvertes simultanément, la même personne ne peut pas être ajoutée à plusieurs d’entre elles.</p></td>
   </tr>
   <tr>
   <td><strong>Une seule décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Échéance le (facultatif)</strong></td>
   <td>La première étape de chaque chemin prend en charge une date d’échéance absolue. Chaque étape suivante du chemin prend en charge une date d’échéance relative, à savoir le nombre de jours à partir duquel cette étape s’ouvre. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance.</td>
   </tr>
   <tr>
   <td><strong>Ajouter un message personnalisé (facultatif)</strong></td>
   <td>Saisissez un message dans la zone de texte <strong>Ajouter un message personnalisé</strong>. Le message s’affiche dans l’e-mail de notification de validation et dans l’onglet Validations de Workfront.<p>Lorsque vous ajoutez une deuxième étape, l’option <strong>Afficher ce message sur toutes les étapes</strong> est sélectionnée par défaut. Laissez-la sélectionnée pour utiliser le même message à chaque étape. Pour utiliser un message différent pour chaque étape, désélectionnez <strong>Afficher ce message sur toutes les étapes</strong>, puis saisissez le message spécifique à l’étape dans la zone de texte <strong>Ajouter un message personnalisé</strong> de chaque étape.</p></td>
   </tr>
   </table>

1. (Facultatif) Cliquez sur **Ajouter une étape** pour ajouter une autre étape au chemin d’accès. Les étapes d’un chemin s’exécutent de manière séquentielle dans l’ordre dans lequel elles sont répertoriées. Vous pouvez réorganiser les étapes d’un chemin, mais vous ne pouvez pas déplacer une étape d’un chemin à un autre. Chaque chemin peut avoir un nombre différent d’étapes.


1. (Facultatif) Sous **Chemins parallèles**, cliquez sur **Ajouter un chemin** pour ajouter un autre chemin. Le nouveau chemin commence par une étape vide et devient le chemin sélectionné. Pour renommer un chemin d’accès, pointez sur le libellé du chemin d’accès, cliquez sur l’icône en forme de crayon, puis saisissez un nouveau nom.

1. (Facultatif) Pour supprimer un chemin d’accès, passez le curseur sur le libellé du chemin et cliquez sur l’icône de corbeille. **Le chemin 1** ne peut pas être supprimé et les chemins ne peuvent pas être réorganisés. Les autres chemins ne peuvent être supprimés que si aucune étape du chemin n’est verrouillée ou terminée.

   ![Mode avancé avec chemins parallèles](assets/request-approval-advanced.jpeg)

1. (Facultatif) Pour effacer tous les chemins et toutes les étapes et recommencer, cliquez sur **Réinitialiser** en haut à droite.

1. Cliquez sur **Demander l’approbation**.

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->