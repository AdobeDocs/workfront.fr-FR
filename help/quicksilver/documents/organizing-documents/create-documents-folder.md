---
product-area: documents
navigation-topic: organize-documents
title: Créer des dossiers de documents
description: Les documents peuvent être organisés en dossiers. Vous pouvez créer des dossiers personnels dans votre zone personnelle Documents.
author: Courtney
feature: Digital Content and Documents
exl-id: 41974d6b-fb00-49b7-9db2-36519994e0fd
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 31%

---

# Créer des dossiers de documents

Les documents peuvent être organisés en dossiers. Workfront comporte actuellement deux versions de la zone Documents : la zone des documents hérités et la zone des nouveaux documents. La version utilisée par votre entreprise dépend du stockage Workfront hérité ou du stockage d’entreprise. Pour plus d’informations sur ces types de stockage, consultez [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les documents à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les documents à l’aide du stockage d’entreprise Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou supérieur</p>
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create document folders in the legacy documents area

If your organization is on legacy Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about legacy Workfront storage, see [Differences between Adobe enterprise storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>L’organisation des documents crée simplement des liens entre les documents et les objets auxquels vous les associez. Cela ne les déplace pas dans le système.

### Afficher des dossiers

Vous pouvez afficher les dossiers dans la vue miniature, standard ou liste. Pour changer de vue, utilisez les options d’affichage dans le coin supérieur droit.

{{step1-to-documents}}

Ou

Lorsqu’un objet Workfront est ouvert, cliquez sur **Documents** dans le panneau de gauche.

1. Cliquez sur les options d’affichage au-dessus du panneau de droite pour modifier l’affichage des documents.

   ![Document view options](assets/screenshot-2016-07-07-12.46.54.png)

### Créer des dossiers et des sous-dossiers

Créez des dossiers pour mieux organiser vos documents. Vous pouvez créer jusqu’à 2 000 dossiers sur un objet et jusqu’à 50 sous-dossiers dans chaque dossier. Les sous-dossiers sont comptabilisés dans le maximum de 2 000 dossiers.

{{step1-to-documents}}

Ou

Lorsqu’un objet Workfront est ouvert, cliquez sur **Documents** dans le panneau de gauche.

1. Pour créer un dossier de niveau supérieur, assurez-vous que rien n’est sélectionné, puis cliquez sur **Ajouter** > **Dossier**.

   Ou

   Pour créer un sous-dossier, sélectionnez le dossier dans lequel vous souhaitez créer le sous-dossier, puis cliquez sur **Ajouter** > **Dossier**.

### Partager des dossiers

Pour plus d’informations sur le partage de dossiers, voir [Partager un dossier de documents](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Create document folders in the new documents area

Si votre entreprise utilise le stockage d’entreprise, la nouvelle zone de documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

### System-generated folders

When you upload a document to a task or issue, Workfront automatically creates a system-generated folder named after the task or issue. This folder is linked to the task or issue and inherits its permissions. System-generated folders are visible in the project-level documents area.

For more information about folder permissions, see [How document permissions work](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

### Create subfolders

You can create subfolders within a system-generated folder to organize documents further. All subfolders inherit permissions from the parent folder.

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.
1. Click into the folder you want to create a subfolder in, then click the **Add folder** ![add folder icon](assets/add-folder-icon.png) icon.
   ![add subfolder](assets/add-subfolder.png)
1. Enter a name for the subfolder, then click **Create**.

### Rename a folder

System-generated folders automatically inherit the name of the task or issue. They can be renamed by clicking the folder name and editing it.

To rename a folder:

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.
1. Find the folder you want to rename, then click the **More** ![more icon](assets/more-icon.png) icon.
1. Click **Rename**, then enter a new name for the folder.

   ![rename folder](assets/rename-folder.png)

1. Click **Rename**.

### Move a folder

System-generated folders can be moved to another project, task, or issue. If a system-generated folder is moved to another location, its linked object is updated to the new object and permissions are inherited from the new parent object. You can also move subfolders to another project, task, or issue.

>[!NOTE]
>
>Only projects, tasks, and issues using the same storage type are available in the move dialog. For example, if you&#39;re moving a folder in an enterprise storage project, only projects, tasks, and issues using enterprise storage are available to move to.


To move a folder:

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.
1. Find the folder you want to move, then click the **More** ![more icon](assets/more-icon.png) icon.
1. Click **Move**, then select the project, task, or issue you want to move the folder to.


   ![move folder](assets/rename-folder.png)

<!-- STEPS PLACEHOLDER: Add steps for moving a folder in the new documents area -->

### Delete a folder

To delete a folder:

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.
1. Find the folder you want to delete, then click the **More** ![more icon](assets/more-icon.png) icon.
1. Cliquez sur **Supprimer**.

   ![delete folder](assets/rename-folder.png)
