---
product-area: documents
navigation-topic: approvals
title: Gérer les validations groupées
description: Vous pouvez ajouter ou supprimer des participants et des ressources dans une approbation groupée sans interrompre le workflow pour le reste du groupe.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 8250a95bec88df91e3422c8da7c05ac802b3cb22
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 8%
---

# Gérer les validations groupées

{{highlighted-preview-article-level}}

Une approbation groupée regroupe plusieurs ressources sous un seul workflow d’approbation, de sorte que toutes les ressources passent par les mêmes étapes au lieu d’exiger une approbation distincte par ressource. Vous pouvez ajouter ou supprimer des participants et des ressources dans une approbation groupée active sans recréer le workflow.

Les approbations groupées prennent en charge les modes De base et Avancé, les étapes multiples et les chemins d’accès parallèles de la même manière que les approbations de ressources uniques. Pour plus d’informations, voir [Créer un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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

1. Cliquez sur **Modifier le workflow**.

1. Recherchez le participant que vous souhaitez supprimer de l’étape active, puis cliquez sur l’icône **Supprimer** en regard de son nom.

1. Cliquer sur **Enregistrer**.

   Le statut d&#39;approbation des participants restants est réévalué pour tenir compte de la modification.

## Ajout de ressources à une approbation groupée

Vous pouvez ajouter des ressources à une approbation groupée jusqu’à ce que sa première étape soit verrouillée. Une fois la première étape verrouillée, vous ne pouvez plus ajouter de ressources, car les participants à cette étape n’auraient pas eu la possibilité de les examiner.

Pour ajouter une ressource à une approbation groupée :

1. Accédez au projet, à la tâche ou à l’événement contenant l’approbation groupée, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur un document du groupe, puis sur l&#39;icône **Validations** située sur le côté droit de la page.

1. Cliquez sur **Modifier le workflow**, puis sur l’onglet **Documents**.

1. Sélectionnez la ou les ressources à ajouter au groupe.

1. Cliquer sur **Enregistrer**.

   Tous les participants du groupe sont avertis qu’une ressource supplémentaire a été ajoutée pour qu’ils puissent la réviser.

## Supprimer des ressources d’une approbation groupée

Vous pouvez supprimer une ressource d’une approbation groupée à tout moment dans le workflow. La ressource supprimée devient sa propre approbation autonome et conserve l’ensemble de ses décisions, commentaires et historiques existants sans redémarrer. Étant donné que la ressource fait déjà l’objet d’une décision d’approbation, vous ne pouvez pas la réajouter à une approbation groupée par la suite.

Pour supprimer une ressource d’une approbation groupée :

1. Accédez au projet, à la tâche ou à l’événement contenant l’approbation groupée, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document à supprimer, puis sur l&#39;icône **Validations** sur le côté droit de la page.

1. Cliquez sur **Modifier le workflow**, puis sur l’onglet **Documents**. Le document que vous avez sélectionné est épinglé en haut de la liste et est déjà vérifié.

1. Effacez la sélection du document que vous souhaitez supprimer du groupe.

1. Cliquer sur **Enregistrer**.

   Le statut d’approbation de la ressource reste visible et inchangé à partir du moment où elle a été supprimée. La vue d’approbation groupée est mise à jour pour refléter les ressources restantes dans le groupe.

## Résoudre une décision « Travail nécessaire » dans une approbation groupée à plusieurs étapes

Dans une approbation groupée à plusieurs étapes, toutes les ressources d’une étape doivent parvenir à une décision avant que le groupe puisse passer à l’étape suivante. Si une ressource est marquée **Nécessite un travail**, elle ne peut pas avancer avec le reste du groupe, elle doit donc être supprimée du groupe pour que l’étape puisse progresser.

Pour résoudre une décision « Un travail est nécessaire » :

1. Supprimez du groupe la ressource marquée **A besoin d’être retravaillée**. Pour plus d’informations, voir [Supprimer des ressources d’une approbation groupée](#remove-assets-from-a-grouped-approval). La ressource supprimée devient sa propre approbation autonome et conserve ses décisions, commentaires et historiques existants.

1. Une fois la ressource mise à jour, demandez à nouveau son approbation, soit en tant que ressource unique, soit en tant que partie d’un nouveau groupe. Étant donné que la ressource comporte déjà une décision d’approbation, vous ne pouvez pas la réajouter au groupe d’origine.

   Pour plus d’informations, voir [Création d’un processus d’approbation de document](create-a-document-approval.md) et [Création d’une approbation groupée](create-a-grouped-approval.md).
