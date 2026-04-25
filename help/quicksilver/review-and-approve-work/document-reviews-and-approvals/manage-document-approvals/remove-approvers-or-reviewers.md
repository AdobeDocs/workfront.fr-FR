---
product-area: documents
navigation-topic: approvals
title: Supprimer des approbateurs ou des réviseurs d’un workflow d’approbation de document
description: Vous pouvez supprimer individuellement des personnes approbatrices ou des personnes réviseuses d’un document.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 33%

---

# Supprimer des approbateurs ou des réviseurs d’un workflow d’approbation de document

Vous pouvez supprimer des approbateurs ou des réviseurs d’une ressource ou d’un document après leur affectation.

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
<p>Tout package de workflow pour gérer les approbations à l’aide du stockage d’entreprise Adobe</p>  </td> 
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
   <td> <p>Gérer l’accès à l’objet associé à la demande d’accès ou d’approbation </p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Supprimer des approbateurs ou des réviseurs d’un workflow d’approbation dans la zone des documents hérités

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, consultez la section [Stockage Workfront par rapport au stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Pour supprimer des approbateurs ou des réviseurs d’un workflow d’approbation :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Faites défiler l’écran jusqu’à la section **Validations** du panneau Résumé du document.

1. Cliquez sur **Modifier le workflow**.

1. Recherchez le participant que vous souhaitez supprimer, puis cliquez sur l’icône **Supprimer** en regard de son nom.

   La demande d’approbation ou de révision est supprimée et la personne approbatrice reçoit une notification indiquant que son approbation n’est plus nécessaire. L’accès au partage lié à l’approbation est également supprimé.

   ![modifier le workflow d’approbation](assets/edit-approval-in-legacy.png)

1. (Facultatif) Pour remplacer le rôle d’approbateur par celui de réviseur ou vice versa, cliquez sur le menu déroulant en regard du nom d’utilisateur et sélectionnez le nouveau rôle.

1. Répétez l’étape précédente pour supprimer toute personne approbatrice ou réviseuse supplémentaire.

</div>


## Supprimer des approbateurs ou des réviseurs à un workflow d’approbation dans la zone du nouveau document

Si votre entreprise utilise le stockage d’entreprise, la nouvelle zone de documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise](/help/quicksilver/review-and-approve-work/esm-overview.md).

Pour créer un workflow de validation :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)


1. Cliquez sur **Modifier le workflow**.

1. Recherchez le participant que vous souhaitez supprimer, puis cliquez sur l’icône **Supprimer** en regard de son nom.

   La demande d’approbation ou de révision est supprimée et la personne approbatrice reçoit une notification indiquant que son approbation n’est plus nécessaire.

1. (Facultatif) Pour remplacer le rôle d’approbateur par celui de réviseur ou vice versa, cliquez sur le menu déroulant en regard du nom d’utilisateur et sélectionnez le nouveau rôle.

1. Répétez l’étape précédente pour supprimer toute personne approbatrice ou réviseuse supplémentaire.

   ![remove participants from a stage](assets/add-or-remove-participants.png)

1. Cliquez sur **Enregistrer**.