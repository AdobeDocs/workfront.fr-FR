---
product-area: documents
navigation-topic: approvals
title: Supprimer des approbateurs ou des réviseurs d’un workflow d’approbation de document
description: Vous pouvez supprimer individuellement des personnes approbatrices ou des personnes réviseuses d’un document.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 42%

---

# Supprimer des approbateurs ou des réviseurs d’un workflow d’approbation de document

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

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
   <td> <p>Tous</p> </td> 
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


## Supprimer des approbateurs ou des réviseurs de la page Détails du document dans votre environnement de production

1. Accédez à la page du document en cliquant sur le nom du document, puis sélectionnez la version du document pour laquelle retirer une approbation dans le menu déroulant de la version. La dernière version est sélectionnée par défaut.

1. Sélectionnez **Validations** dans le panneau de gauche.

1. Passez la souris sur le nom de l’approbateur ou du réviseur que vous souhaitez supprimer, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](../assets/delete.png) qui s’affiche après leur nom.

   La demande d’approbation ou de révision est supprimée et la personne approbatrice reçoit une notification indiquant que son approbation n’est plus nécessaire. L’accès au partage lié à l’approbation est également supprimé.

1. (Facultatif) Pour rétrograder une personne approbatrice en personne réviseuse plutôt que de la supprimer complètement, décochez la case **Approbateur ou approbatrice** en regard de son nom.

1. Répétez l’étape précédente pour supprimer toute personne approbatrice ou réviseuse supplémentaire.

## Supprimer des approbateurs ou des réviseurs du résumé du document dans votre environnement de production

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Sélectionnez la version du document pour laquelle supprimer une personne approbatrice ou une personne réviseuse dans la liste déroulante de la version. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations** du panneau Résumé du document. Passez la souris sur le nom de l’approbateur ou du réviseur que vous souhaitez supprimer, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](../assets/delete.png) qui s’affiche après leur nom.

   La demande d’approbation ou de révision est supprimée et la personne approbatrice reçoit une notification indiquant que son approbation n’est plus nécessaire. L’accès au partage lié à l’approbation est également supprimé.

1. (Facultatif) Pour rétrograder une personne approbatrice en personne réviseuse plutôt que de la supprimer complètement, décochez la case **Approbateur ou approbatrice** en regard de son nom.

1. Répétez l’étape précédente pour supprimer toute personne approbatrice ou réviseuse supplémentaire.


<div class="preview">

## Supprimez des approbateurs ou des réviseurs d’un workflow d’approbation dans votre environnement de prévisualisation dans la zone des documents hérités

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

   La demande d’approbation ou de révision est supprimée et l’approbateur reçoit une notification indiquant que son approbation n’est plus nécessaire.

1. (Facultatif) Pour remplacer le rôle d’approbateur par celui de réviseur ou vice versa, cliquez sur le menu déroulant en regard du nom d’utilisateur et sélectionnez le nouveau rôle.

1. Répétez l’étape précédente pour supprimer toute personne approbatrice ou réviseuse supplémentaire.

   ![supprimer des participants d’une étape](assets/add-or-remove-participants.png)
1. Cliquez sur **Enregistrer**.