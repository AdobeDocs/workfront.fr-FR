---
product-area: documents
navigation-topic: approvals
title: Charger une nouvelle version du document et demander une approbation
description: Vous pouvez charger une nouvelle version du document et demander l’approbation d’autres utilisateurs dans Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 42fbb40cb8a0f3c70e22fd04bd3d0ce625f58fec
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 28%

---

# Charger une nouvelle version du document et demander une approbation

Si un document marqué a besoin d’être retravaillé lors d’une révision précédente, vous pouvez charger une nouvelle version dans le document d’origine et commencer une nouvelle série d’approbations. Une fois que vous avez chargé une nouvelle version du document, les versions précédentes sont verrouillées.

Si le nom de fichier de la nouvelle version est différent de celui de la version précédente, Workfront affiche le document avec le nom de fichier le plus récent.

Lorsqu&#39;une nouvelle version est ajoutée à un document avec des approbations en attente, l&#39;approbation de la version précédente indique Retiré. Le processus d’approbation précédent se termine, même si certains participants n’ont pas encore pris de décision.

Si la dernière version du document est supprimée, les versions précédentes restent verrouillées. Si vous devez modifier une version précédente, vous devez la déverrouiller manuellement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p>
   <p>Contributeur ou version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès Modifier à l’objet associé au document</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Faire glisser et déposer pour ajouter une nouvelle version

>[!NOTE]
>
>Glisser-déposer ne fonctionne pas avec Internet Explorer.


Si vous avez besoin d’une autre phase de révision et d’approbation d’un document, vous pouvez créer une nouvelle version du document dans Workfront.

Vous pouvez ajouter les participants précédents, de nouveaux participants ou une combinaison des deux. Vous pouvez afficher des informations sur les versions précédentes et les participants sur la page Détails du document .

Pour ajouter une nouvelle version :

1. Accédez au document dans Workfront.
1. Glissez-déposez le nouveau fichier en haut du document précédent. Une nouvelle version est automatiquement créée.

1. Une fois le téléchargement terminé, sélectionnez le document, puis cliquez sur **Détails du document**.
   ![Ouvrir la page des détails du document](assets/open-doc-details.png)


1. Dans le volet de gauche, cliquez sur **Validations**, puis sur **Ajouter**.

1. Pour ajouter tous les participants précédents, cliquez sur **Ajouter tout**. Vous pouvez également ajouter de nouveaux participants ou supprimer des participants précédents selon vos besoins.


1. Pour ajouter un modèle d’approbation existant, cliquez sur le bouton Modèle et commencez à saisir le nom d’un modèle.

   >[!TIP]
   >
   >   Les utilisateurs disposant d&#39;une licence Standard peuvent créer des modèles d&#39;approbation réutilisables à partir de la zone Configuration. Pour plus d’informations, voir [Créer un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Facultatif) Définissez une date limite pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant l’échéance spécifiée.

1. Une fois que vous avez ajouté tous les réviseurs et approbateurs, cliquez sur **Soumettre la demande**. Les participants sont avertis par e-mail.

   ![soumettre la nouvelle version à approbation](assets/add-previous-participants.png)


