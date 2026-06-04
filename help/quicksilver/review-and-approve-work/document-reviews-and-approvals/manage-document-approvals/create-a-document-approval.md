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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1473
ht-degree: 12%

---

# Créer un workflow d’approbation de document

{{highlighted-preview}}

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

## Créez un workflow d’approbation à partir du panneau Résumé dans la zone des documents hérités de l’environnement de production

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage cloud Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Pour créer un workflow de validation :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Sélectionnez la version du document pour laquelle vous souhaitez créer une approbation dans le menu déroulant de la version. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**.


1. Renseignez les détails suivants :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Ajoutez un nom d’étape. Vous pouvez remplacer le nom par un nom plus explicite, tel que <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Si vous avez uniquement des réviseurs, ils seront avertis et auront la possibilité de terminer la révision, mais aucune décision ne sera requise ou prise.</td>
   </tr>
   <tr>
   <td><strong>Une décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Date d’échéance (facultatif)</strong></td>
   <td>Définissez une date d’échéance pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance spécifiée.</td>
   </tr>
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres étapes si nécessaire.

   >[!NOTE]
   >
   >Si vous ajoutez plusieurs étapes, le workflow d’approbation se poursuit dans l’ordre dans lequel elles sont répertoriées. Lorsque toutes les décisions requises sont prises, l’étape suivante commence et l’étape précédente est verrouillée.

   ![&#x200B; Détails du document &#x200B;](assets/new-stage.png)


<div class="preview">

## Créez un workflow d’approbation à partir du panneau Résumé dans la zone des documents hérités de l’aperçu

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage cloud Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Pour créer un workflow de validation :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Sélectionnez la version du document pour lequel vous souhaitez créer une approbation dans le menu déroulant Version. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**.

1. Renseignez les détails suivants :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Ajoutez un nom d’étape. Vous pouvez remplacer le nom par un nom plus explicite, tel que <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
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
   <p>Lorsque vous ajoutez une deuxième étape, l’option <strong>Afficher ce message sur toutes les étapes</strong> est sélectionnée par défaut. Laissez-la sélectionnée pour utiliser le même message à chaque étape. Pour utiliser un message différent pour chaque étape, désélectionnez <strong>Afficher ce message sur toutes les étapes</strong>, puis saisissez le message spécifique à l’étape dans la zone de texte <strong>Ajouter un message personnalisé</strong> de chaque étape, si nécessaire.</p></td>
   </tr>
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres étapes si nécessaire.

   >[!NOTE]
   >
   >* Si vous ajoutez plusieurs étapes, le workflow d’approbation se poursuit dans l’ordre dans lequel elles sont répertoriées. Lorsque toutes les décisions requises sont prises, l’étape suivante commence et l’étape précédente est verrouillée.
   >* Si vous modifiez un message personnalisé après la création du workflow d’approbation, une notification par e-mail mise à jour est envoyée à tous les participants existants. Si vous ajoutez un participant ultérieurement, le message personnalisé est inclus dans sa notification par e-mail.

   ![Ajouter un message personnalisé à une étape](assets/add-custom-message.jpeg)

</div>


## Créez un workflow d’approbation à partir du panneau Résumé dans la nouvelle zone Documents de l’environnement de production

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Pour créer un workflow de validation :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Créer un workflow**, puis renseignez les informations suivantes :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Ajoutez un nom d’étape. Vous pouvez remplacer le nom par un nom plus explicite, tel que <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Si vous avez uniquement des réviseurs, ils seront avertis et auront la possibilité de terminer la révision, mais aucune décision ne sera requise ou prise.</td>
   </tr>
   <tr>
   <td><strong>Une décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Date d’échéance (facultatif)</strong></td>
   <td>Définissez une date d’échéance pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date d’échéance spécifiée.</td>
   </tr>
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres étapes si nécessaire.

   >[!NOTE]
   >
   >Si vous ajoutez plusieurs étapes, le workflow d’approbation se poursuit dans l’ordre dans lequel elles sont répertoriées. Lorsque toutes les décisions requises sont prises, l’étape suivante commence et l’étape précédente est verrouillée.

   ![&#x200B; Détails du document &#x200B;](assets/new-stage.png)


<div class="preview">

## Créez un workflow d’approbation à partir du panneau Résumé dans la nouvelle zone Documents de l’aperçu

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Pour créer un workflow de validation :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Créer un workflow**, puis renseignez les informations suivantes :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Ajoutez un nom d’étape. Vous pouvez remplacer le nom par un nom plus explicite, tel que <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
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
   <p>Lorsque vous ajoutez une deuxième étape, l’option <strong>Afficher ce message sur toutes les étapes</strong> est sélectionnée par défaut. Laissez-la sélectionnée pour utiliser le même message à chaque étape. Pour utiliser un message différent pour chaque étape, désélectionnez <strong>Afficher ce message sur toutes les étapes</strong>, puis saisissez le message spécifique à l’étape dans la zone de texte <strong>Ajouter un message personnalisé</strong> de chaque étape.</p></td>
   </tr>
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres étapes si nécessaire.

   >[!NOTE]
   >
   >* Si vous ajoutez plusieurs étapes, le workflow d’approbation se poursuit dans l’ordre dans lequel elles sont répertoriées. Lorsque toutes les décisions requises sont prises, l’étape suivante commence et l’étape précédente est verrouillée.
   >* Si vous modifiez un message personnalisé après la création du workflow d’approbation, une notification par e-mail mise à jour est envoyée à tous les participants existants. Si vous ajoutez un participant ultérieurement, le message personnalisé est inclus dans sa notification par e-mail.

   ![Ajouter un message personnalisé à une étape](assets/add-custom-message.jpeg)

</div>



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
