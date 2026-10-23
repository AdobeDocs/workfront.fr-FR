---
product-area: documents
navigation-topic: approvals
title: Gérer les validations groupées
description: Vous pouvez ajouter ou supprimer des participants et des documents dans une approbation groupée sans interrompre le processus pour le reste du groupe.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: e62ae215bcc7ea42701d6eb92cf43f531a6afc0d
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 5%
---

# Gérer les validations groupées

Une approbation groupée regroupe plusieurs documents sous un seul workflow d’approbation, de sorte que tous les documents passent par les mêmes étapes au lieu d’exiger une approbation distincte par document. Vous pouvez ajouter ou supprimer des participants et des documents dans une approbation groupée active sans recréer le workflow.

Les approbations groupées prennent en charge les modes De base et Avancé, les étapes multiples et les chemins d’accès parallèles de la même manière que les approbations de ressources uniques. Pour plus d’informations, voir [Créer un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Les validations groupées ne sont disponibles que dans la zone des nouveaux documents. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
   <p>Si vous utilisez l'intégration Frame.io, vous devez disposer d'une licence Standard pour créer des workflows d'approbation.</p>
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

## Ajouter des participants à une approbation groupée active

Vous pouvez ajouter des approbateurs ou des réviseurs à une approbation groupée lorsqu&#39;une étape est active, sans interrompre les approbations déjà en cours.

Pour ajouter des participants à une approbation groupée active :

1. Accédez au projet, à la tâche ou à l’événement contenant l’approbation groupée, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur un document du groupe, puis sur l&#39;icône **Validations** située sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Modifier le workflow**.

1. Saisissez l’utilisateur, l’équipe ou l’e-mail dans le champ **Ajouter des noms ou des e-mails** de l’étape active.

1. Pour chaque personne que vous ajoutez, choisissez s’il s’agit d’un approbateur ou d’un réviseur.

1. Cliquer sur **Enregistrer**.

   Les nouveaux participants voient chaque approbation ouverte dans le groupe dans leur file d&#39;attente. Ils ne voient pas les décisions qui ont été prises avant qu&#39;elles ne soient ajoutées, alors ils doivent quand même terminer toutes les approbations actuellement ouvertes eux-mêmes.

## Supprimer des participants d&#39;une approbation groupée active

Vous pouvez supprimer des approbateurs ou des réviseurs d’une approbation groupée lorsqu’une étape est active. Les participants supprimés cessent immédiatement de voir les approbations du groupe dans leur file d’attente, mais les décisions qu’ils ont déjà prises sont conservées et ne sont pas réinitialisées.

Pour supprimer des participants d&#39;une approbation groupée active :

1. Accédez au projet, à la tâche ou à l’événement contenant l’approbation groupée, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur un document du groupe, puis sur l&#39;icône **Validations** située sur le côté droit de la page.

   ![Supprimer des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Modifier le workflow**.

1. Recherchez le participant que vous souhaitez supprimer de l’étape active, puis cliquez sur l’icône **Supprimer** en regard de son nom.

1. Cliquer sur **Enregistrer**.

## Ajouter des documents à une validation groupée

Vous pouvez ajouter des documents à une approbation groupée jusqu&#39;à ce que sa première étape soit verrouillée. Une fois la première étape verrouillée, vous ne pouvez plus ajouter de documents.

Pour ajouter un document à une approbation groupée :

1. Accédez au projet, à la tâche ou à l’événement contenant l’approbation groupée, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur un document du groupe, puis sur l&#39;icône **Validations** située sur le côté droit de la page.

1. Cliquez sur **Modifier le workflow**, puis sur l’onglet **Documents**.

1. Sélectionnez le ou les documents à ajouter au groupe.

1. Cliquer sur **Enregistrer**.

   Tous les participants du groupe sont avisés qu&#39;un document supplémentaire a été ajouté pour qu&#39;ils puissent l&#39;examiner.

## Supprimer des documents d&#39;une approbation groupée

Vous pouvez supprimer un document d’une approbation groupée à tout moment dans le workflow. Le document supprimé devient sa propre approbation autonome et conserve l’ensemble de ses décisions, commentaires et historiques existants sans redémarrer. Étant donné que le document comporte déjà une décision d’approbation, vous ne pouvez pas le rajouter à une approbation groupée par la suite.

Pour supprimer un document d&#39;une approbation groupée :

1. Accédez au projet, à la tâche ou à l’événement contenant l’approbation groupée, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document à supprimer, puis sur l&#39;icône **Validations** sur le côté droit de la page.

1. Cliquez sur **Modifier le workflow**, puis sur l’onglet **Documents**. Le document que vous avez sélectionné est épinglé en haut de la liste et est déjà vérifié.

1. Effacez la sélection du document que vous souhaitez supprimer du groupe.

1. Cliquer sur **Enregistrer**.

   >[!NOTE]
   >
   >Le statut d’approbation du document reste visible et inchangé à partir du moment où il a été supprimé. La vue d’approbation groupée est mise à jour pour refléter les documents restants dans le groupe.


## Résoudre une décision « Travail nécessaire » sur un seul document dans une approbation groupée à plusieurs étapes

Dans une approbation groupée en plusieurs étapes, tous les documents d’une étape doivent parvenir à une décision avant que le groupe puisse passer à l’étape suivante. Si un document est marqué **nécessite un travail**, il ne peut pas être déplacé avec le reste du groupe. Il doit donc être supprimé manuellement du groupe pour que l’étape puisse progresser.

Lorsque vous supprimez le document du groupe, il devient sa propre approbation autonome et conserve toutes ses décisions, commentaires et historiques existants sans redémarrer. Vous pouvez ajouter le document révisé en tant que nouvelle version à l&#39;approbation autonome ou créer une nouvelle approbation groupée avec celle-ci.

Pour résoudre une décision « Un travail est nécessaire » :

1. Supprimez du groupe le document marqué **A besoin d’être retravaillé**. Pour plus d&#39;informations, voir [Supprimer des documents d&#39;une approbation groupée](#remove-documents-from-a-grouped-approval). Le document supprimé devient sa propre approbation autonome et conserve ses décisions, commentaires et historiques existants.

1. Une fois le document mis à jour, chargez-le en tant que nouvelle version et demandez à nouveau son approbation ou ajoutez-le dans le cadre d’un nouveau groupe.

   Pour plus d’informations, consultez les ressources suivantes :

   * [Charger une nouvelle version du document et demander une approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)
   * [Créer un workflow d’approbation de document](create-a-document-approval.md)
   * [Créer une validation groupée](create-a-grouped-approval.md)


## Limites connues

Il existe un problème temporaire de synchronisation avec Frame.io lorsque vous ajoutez ou supprimez des documents dans une approbation groupée. Les modifications ne seront pas répercutées dans Frame.io avant la prochaine synchronisation du document.