---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: La zone Documents
description: Dans la zone Documents, vous pouvez organiser, gérer et afficher les métadonnées des documents chargés dans Adobe Workfront. Vous pouvez également voir le statut de décision de l’épreuve.
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ed7944fe4934ac5ab52b1eed3e144309de9781c4
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 34%

---

# La zone Documents

Dans la zone Documents, vous pouvez organiser, gérer et afficher les métadonnées des documents chargés dans Adobe Workfront. Vous pouvez également voir le statut de décision de l’épreuve.

Workfront comporte actuellement deux versions de la zone Documents : la zone des documents hérités et la zone des nouveaux documents. La version utilisée par votre entreprise dépend du stockage Workfront hérité ou du stockage d’entreprise. Pour plus d’informations sur ces types de stockage, consultez [Présentation du stockage d’entreprise ](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Zone des documents hérités

Il existe deux types de zones Documents. Les fonctionnalités sont les mêmes pour les deux :

* **Zone Documents dans un programme, un portefeuille, un projet, une tâche ou un événement :** répertorie tous les documents auxquels vous avez accès pour un projet, une tâche ou un événement spécifique. Pour accéder à cette zone, cliquez sur **Documents** ![icône Documents](assets/document-icon-12x14.png) dans le panneau de gauche lors de l’affichage d’un projet, d’une tâche ou d’un événement.

* **Zone Documents générale :** répertorie tous les documents auxquels vous avez accès dans Workfront. Pour accéder à cette zone, cliquez sur **Documents** ![icône Documents](assets/document-icon.png) dans le menu principal ![icône du menu principal](assets/main-menu-icon.png).

Pour plus d’informations sur le chargement de documents vers Workfront, voir [Ajouter des documents à Adobe Workfront à partir de votre système de fichiers](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).


La zone des documents enregistre un décompte des éléments suivants :

* Dossiers Workfront
* Fichiers téléchargés à partir du système de fichiers
* Fichiers ajoutés à Workfront à partir des intégrations
* Experience Manager Assets lié

### Panneau Résumé

Lorsque vous sélectionnez un document dans la zone des documents, vous pouvez utiliser le résumé à droite pour afficher les détails du document, gérer les mises à jour et les approbations du document, afficher les versions du document, et ajouter et modifier des Forms personnalisées pour le document.

Si la relecture est configurée pour le document, la section Détails contient des informations telles que la date d’échéance de la relecture et la progression actuelle de la relecture.

Vous pouvez cliquer sur l’en-tête Détails pour accéder à la zone Détails du document complète lorsque vous avez besoin de toutes les informations sur un document.

![Zone Documents](assets/documents-area-v2-350x199.png)

Pour plus d’informations sur le résumé, voir [Vue d’ensemble du résumé des documents](../../documents/managing-documents/summary-for-documents.md).

### Décision concernant l&#39;épreuve

Une fois qu’un statut de décision de l’épreuve a été pris, il apparaît dans la liste des documents.

![Décision sur l&#39;épreuve dans la liste de documents](assets/proof-decision---doc-list-350x168.png)

### Dossiers

Sur un projet, une tâche ou un problème où des documents sont chargés, vous pouvez configurer des dossiers pour organiser les documents. Pour plus d’informations, voir [Créer des dossiers de documents](../../documents/organizing-documents/create-documents-folder.md).

Dans la zone Documents générale, vous pouvez configurer deux types de dossiers pour organiser les documents auxquels vous avez accès :

* **Dossiers intelligents :** affichez uniquement les documents que vous souhaitez voir. Pour plus d’informations, voir [Créer et gérer des dossiers intelligents](../../documents/organizing-documents/create-manage-smart-folders.md).

* **Mes dossiers :** organisez les documents comme vous le souhaitez. Pour plus d’informations, voir [Créer des dossiers de documents](../../documents/organizing-documents/create-documents-folder.md).

### Détails du document développés

La page Détails du document fournit une version plus complète des Détails du document dans le résumé à droite.

## Zone du nouveau document

La nouvelle zone de documents n’est disponible que si votre entreprise utilise un espace de stockage d’entreprise. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise ](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Utilisation du panneau de résumé

Lorsque vous sélectionnez un document dans la zone des documents, vous pouvez utiliser le panneau Résumé à droite pour afficher des détails sur le document, ajouter et modifier des formulaires personnalisés joints, créer et gérer des workflows d’approbation, afficher des versions du document, etc.

#### Vérifier et approuver avec Frame.io

Vous pouvez réviser et approuver des documents dans la zone des nouveaux documents à l&#39;aide de la visionneuse Frame.io.

Pour plus d’informations, voir [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Gestion des versions

Vous pouvez charger de nouvelles versions d’un document dans la zone des nouveaux documents. Lorsque vous chargez une nouvelle version, la version précédente est conservée et est accessible à partir du panneau Résumé . Les versions sont automatiquement nommées avec la date et l’heure du chargement, mais peuvent être renommées selon les besoins.

Vous pouvez également lancer un nouveau workflow d’approbation pour une version spécifique d’un document.

#### Afficher l’historique des documents

Vous pouvez afficher l&#39;historique d&#39;un document dans la zone des nouveaux documents. L’historique comprend les types d’informations suivants :

* Date de chargement du document
* Lorsque de nouvelles versions ont été chargées
* Quand les workflows d’approbation ont été lancés pour le document
* Et plus encore

### Dossiers au niveau du système pour les autorisations de document

Workfront crée automatiquement un dossier au niveau du système lorsque le premier document est chargé sur une tâche ou un événement. Ces dossiers héritent des autorisations de la tâche ou de l’événement et sont visibles dans la zone des documents au niveau du projet. Tous les documents chargés vers cette tâche ou cet événement sont stockés dans ce dossier et y héritent des autorisations. Il s’agit de la principale méthode de gestion des autorisations pour les documents dans la zone des nouveaux documents. Pour plus d’informations, voir [Présentation des autorisations d’objet et des niveaux d’accès pour le modèle de stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Considérations

* La nouvelle zone de documents est optimisée pour les écrans d’une largeur de 1 024 pixels ou plus. Si votre écran est plus petit, vous risquez de rencontrer des problèmes pour accéder au panneau Résumé .

* La zone de documents globale n’est pas disponible dans la nouvelle expérience de zone de documents. Vous pouvez uniquement accéder aux documents d&#39;un programme, d&#39;un portefeuille, d&#39;un projet, d&#39;une tâche ou d&#39;un événement.
