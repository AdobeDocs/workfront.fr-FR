---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Utilisation d’Adobe Cloud Drive
description: Utilisez vos projets de stockage dans le cloud Adobe directement depuis le Finder ou l’Explorateur de fichiers à l’aide d’Adobe Cloud Drive. Ouvrez et modifiez des fichiers dans n’importe quelle application, travaillez hors ligne et résolvez les conflits.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: c16dc2b8b508f71767999aec7029664f5d31f23f
workflow-type: tm+mt
source-wordcount: '3955'
ht-degree: 2%
---
# Utilisation d’Adobe Cloud Drive

Après avoir installé Adobe Cloud Drive, vous pouvez travailler avec vos projets de stockage dans le cloud Adobe directement depuis le Finder ou l’Explorateur de fichiers. Vous pouvez ouvrir et modifier des fichiers dans n’importe quelle application, travailler hors ligne et laisser Adobe Cloud Drive synchroniser vos modifications avec le cloud.

Pour plus d’informations sur l’installation d’Adobe Cloud Drive, voir [Installer Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Version d’Adobe Workfront</td> 
   <td>Workflow Ultimate, avec le stockage dans le cloud Adobe activé</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>
      <p>Afficher l’accès à un projet pour l’afficher dans Adobe Cloud Drive</p>
      <p>Modifier l’accès à un projet pour y ajouter, modifier ou supprimer des fichiers</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accéder à vos projets

1. Ouvrez le Finder (Mac) ou l’Explorateur de fichiers (Windows).
1. Accédez à **Adobe Cloud Drive**.
1. Parcourez la liste des projets auxquels vous avez accès dans Workfront. Ouvrez un dossier de projet pour afficher ses fichiers et sous-dossiers.

   >[!NOTE]
   >
   >* Les dossiers de projet sont en lecture seule au niveau supérieur. Vous ne pouvez pas renommer, supprimer ou déplacer des dossiers de projet eux-mêmes.
   >* Vous pouvez utiliser des fichiers et des dossiers à l’intérieur d’un dossier de projet : ouvrir, modifier, créer, supprimer, etc.
   >* Les projets Workfront hérités n’apparaissent pas dans Adobe Cloud Drive. Seuls les projets stockés dans l’espace de stockage Adobe sont disponibles.

## Indicateurs de statut du fichier

Adobe Cloud Drive utilise des indicateurs visuels pour afficher le statut de la synchronisation des fichiers. Les icônes diffèrent entre Windows et Mac.

### Indicateurs de statut des fichiers sous Windows

| Icône | Statut | Signification du fichier | Signification du dossier |
| --- | --- | --- | --- |
| ![Icône en ligne uniquement](assets/acd-windows-online-only.png) | En ligne uniquement | Le fichier est synchronisé, mais disponible uniquement en ligne. | Tous les fichiers contenus dans sont disponibles en ligne. |
| ![Icône de synchronisation](assets/acd-windows-syncing.png) | Synchronisation | Les dernières mises à jour du fichier sont synchronisées avec le cache local ou l’espace de stockage dans le cloud d’Adobe. | Au moins un fichier du dossier est en cours de synchronisation. |
| ![Icône hors ligne disponible](assets/acd-windows-available-offline.png) | Disponible hors ligne | Le fichier est synchronisé et disponible hors connexion. | Au moins un fichier du dossier est disponible hors connexion. |
| ![Icône épinglée](assets/acd-windows-pinned.png) | Épinglé (toujours conserver sur l’appareil) | Le fichier est synchronisé et toujours conservé hors ligne. Adobe Cloud Drive ne purge pas automatiquement le contenu épinglé. | Tous les fichiers du dossier se trouvent dans le cache local et sont disponibles hors ligne. |
| ![Icône en lecture seule](assets/acd-windows-read-only.png) | Lecture seule | Fichier en lecture seule. | Le dossier est en lecture seule. |
| ![Icône d&#39;erreur de synchronisation](assets/acd-windows-sync-error.png) | Erreur de synchronisation | Impossible de synchroniser le fichier. Pour plus d’informations, pointez sur l’icône. | Impossible de synchroniser le dossier. Pour plus d’informations, pointez sur l’icône. |
| ![Icône de synchronisation exclue](assets/acd-windows-sync-excluded.png) | Synchronisation exclue | Le fichier ne peut pas être synchronisé en raison d&#39;un type ou d&#39;un nom non pris en charge. | Le dossier ne peut pas être synchronisé en raison d’un nom non pris en charge. |

### Indicateurs de statut des fichiers sur Mac

| Icône | Statut | Signification du fichier | Signification du dossier |
| --- | --- | --- | --- |
| (Pas d’icône) | Disponible hors ligne | Le fichier est synchronisé et disponible hors connexion. | Tous les fichiers sont disponibles hors ligne. |
| ![Icône en ligne uniquement](assets/acd-mac-online-only.png) | En ligne uniquement | Le fichier est synchronisé et disponible uniquement en ligne. | Au moins un fichier du dossier est en ligne uniquement. |
| ![Icône de synchronisation](assets/acd-mac-syncing.png) | Synchronisation | Les dernières mises à jour du fichier sont synchronisées avec le cache local ou l’espace de stockage dans le cloud d’Adobe. | Synchronisation du contenu du dossier. |
| ![Icône d&#39;erreur de synchronisation](assets/acd-windows-sync-error.png) | Erreur de synchronisation | Le fichier ne peut pas être mis à jour ni synchronisé. Pour plus d’informations, pointez sur l’icône. | Le dossier ne peut pas être mis à jour ni synchronisé. Pour plus d’informations, pointez sur l’icône. |
| ![Icône de synchronisation exclue](assets/acd-windows-sync-excluded.png) | Synchronisation exclue | Fichier exclu de la synchronisation. | Le dossier est exclu de la synchronisation. |
| ![Icône en lecture seule](assets/acd-mac-read-only.png) | Lecture seule | Fichier en lecture seule. | Le dossier est en lecture seule. |
| ![Icône épinglée](assets/acd-windows-pinned.png) | Épinglé (toujours conserver sur l’appareil) | Le fichier est épinglé pour être disponible hors ligne. Adobe Cloud Drive ne purge pas automatiquement le contenu épinglé. | Le dossier est épinglé pour être disponible hors ligne. |

### Infobulles d’erreur

En cas d’erreur ou de problème de synchronisation, pointez sur l’icône de fichier ou de dossier pour afficher une info-bulle décrivant le problème.

| Catégorie d’erreur | Infobulle | Signification |
|---|---|---|
| Synchronisation exclue | Type de fichier non pris en charge | Le type de fichier n&#39;est pas pris en charge par Adobe Cloud Drive. |
| Synchronisation exclue | Nom de fichier non pris en charge | Le nom de fichier n&#39;est pas pris en charge par Adobe Cloud Drive. |
| Synchronisation exclue | Projet parent supprimé | Le projet Workfront parent a été supprimé. |
| Synchronisation suspendue | Contenu de fichier non pris en charge | Impossible de synchroniser le contenu du fichier (par exemple, un problème de sécurité a été détecté). |
| Synchronisation suspendue | Caractères non valides dans le nom de fichier | Le nom de fichier contient des caractères non valides. |
| Synchronisation suspendue | Chemin complet trop long | Le chemin d&#39;accès au fichier dépasse la longueur maximale autorisée. |
| Synchronisation suspendue | Aucune autorisation d’écriture | Votre accès en écriture à ce fichier ou projet a été révoqué. |
| Erreur de synchronisation | Problème d’authentification | Un problème est survenu avec vos informations de connexion. |
| Erreur de synchronisation | Espace de stockage indisponible | Les services cloud d’Adobe sont temporairement indisponibles. |
| Erreur de synchronisation | Espace de stockage complet | Votre quota de stockage dans le cloud est plein. |
| Erreur de synchronisation | Disque local saturé | Votre disque local ne dispose pas de suffisamment d&#39;espace libre. |
| Erreur de synchronisation | Pas de connexion Internet | Votre appareil n&#39;est pas connecté à Internet. |
| Erreur de synchronisation | Erreur inattendue | Une erreur inattendue s’est produite lors de la synchronisation. |
| Erreur de synchronisation | Compte bloqué | Votre compte a été bloqué par le service. |

>[!NOTE]
>
>Les erreurs au niveau du système, telles que déconnecté, échec d’authentification, réseau indisponible, disque local saturé ou espace de stockage dans le cloud saturé, s’affichent dans la barre d’état système (Windows) ou dans la barre de menus (Mac), et non sur des fichiers individuels.

### Synchroniser la liste d’exclusion

Adobe Cloud Drive exclut de la synchronisation certains fichiers générés par le système, temporaires et de verrouillage. Les types de fichiers et modèles suivants sont exclus :

| Catégorie | Types/modèles de fichiers | Description |
|---|---|---|
| Fichiers système | `.DS_Store`, `Thumbs.db` | Métadonnées du système d’exploitation et fichiers de cache des miniatures. |
| Fichiers de mémoire système et virtuelle | `*.sys` (par exemple, `hiberfil.sys`, `pagefile.sys`, `swapfile.sys`) | Fichiers système volumineux utilisés pour la mémoire virtuelle, la veille ou d’autres fonctions du système d’exploitation. |
| Fichiers d’indexation macOS | `.Spotlight-V100`, `.fseventsd` | Indexation de macOS Spotlight et fichiers de suivi des événements du système de fichiers. |
| Fichiers temporaires et de sauvegarde | `*.tmp`, `*.swp`, `*~`, `*.bak` | Fichiers temporaires, temporaires ou de sauvegarde générés par les applications. |

## Ouvrir un fichier

1. Dans Adobe Cloud Drive, accédez au fichier .
1. Double-cliquez sur le fichier .

   Le fichier s’ouvre dans son application par défaut.

Adobe Cloud Drive prend en charge tout type de fichier qu’une application installée sur votre ordinateur peut ouvrir, notamment :

* Formats Adobe Creative Cloud (PSD, AI, INDD, PRPROJ, AEP, etc.)
* Documents Microsoft Office (DOCX, XLSX, PPTX)
* Images (JPG, PNG, GIF, etc.)
* Fichiers vidéo (MP4, MOV, etc.)

>[!NOTE]
>
>Les formats de documents cloud (PSDC, AIDC, etc.) s’ouvrent en tant qu’équivalents standard (PSD, AI, etc.) lorsque vous y accédez via Adobe Cloud Drive.

## Modifier et enregistrer un fichier

1. Ouvrez un fichier à partir d’Adobe Cloud Drive.
1. Apportez vos modifications dans l’application.
1. Enregistrez le fichier en sélectionnant **Fichier** > **Enregistrer** ou en appuyant sur Ctrl+S (Windows) ou Cmd+S (Mac).

   Vos modifications sont automatiquement synchronisées avec l’espace de stockage dans le cloud d’Adobe.

>[!IMPORTANT]
>
>Enregistrez les fichiers à l’aide de **Fichier** > **Enregistrer** ou du raccourci clavier. Évitez d&#39;utiliser **Enregistrer sous** pour créer des copies, car cela génère des fichiers en double dans le lecteur.

## Créer ou ajouter un nouveau fichier

Vous pouvez créer un nouveau fichier directement dans un projet ou ajouter un fichier existant à partir de votre espace de stockage local.

### Créer un nouveau fichier à partir d&#39;une application

1. Ouvrez l’application que vous souhaitez utiliser pour créer le fichier.
1. Créez le fichier comme vous le feriez normalement.
1. Lors de l’enregistrement, choisissez un emplacement dans un dossier de projet Adobe Cloud Drive.

   Le fichier apparaît dans Adobe Cloud Drive et se synchronise avec l’espace de stockage dans le cloud Adobe.

### Ajouter un fichier existant à un projet

1. Dans le Finder (Mac) ou l’Explorateur de fichiers (Windows), ouvrez le dossier du projet dans Adobe Cloud Drive.
1. Faites glisser ou copiez des fichiers de votre espace de stockage local dans le dossier du projet.

   Les fichiers se synchronisent automatiquement avec l’espace de stockage dans le cloud d’Adobe.

## Rendre les fichiers et les dossiers disponibles hors connexion

Lorsqu’un fichier ou un dossier est disponible hors connexion, vous pouvez l’ouvrir et le modifier sans connexion Internet. Les fichiers hors ligne utilisent l’espace disque local.

### Conserver un fichier ou un dossier sur votre appareil

1. Cliquez avec le bouton droit sur le fichier ou le dossier dans Adobe Cloud Drive.
1. Sélectionnez **Toujours Conserver Sur Cet Appareil**.

   Le fichier ou le dossier est téléchargé dans votre cache local et vous pouvez l’utiliser même lorsque vous êtes hors ligne.

### Supprimer l’accès hors ligne pour libérer de l’espace

1. Cliquez avec le bouton droit sur le fichier ou le dossier hors connexion.
1. Sélectionnez **Libérer De L&#39;Espace**.

   Le fichier ou le dossier reste dans l’espace de stockage cloud, mais il est supprimé de votre cache local.

>[!NOTE]
>
>Les fichiers et dossiers hors ligne utilisent l’espace disque local. Supprimez l’accès hors connexion aux fichiers et dossiers dont vous n’avez plus besoin pour libérer de l’espace.

## Copier un fichier sur le stockage local

Vous pouvez copier un fichier d’Adobe Cloud Drive vers votre lecteur local. L’original reste dans Adobe Cloud Drive, et la copie devient un fichier local indépendant.

1. Cliquez avec le bouton droit sur le fichier dans Adobe Cloud Drive.
1. Sélectionnez **Copier**, puis collez le fichier à l&#39;emplacement souhaité sur votre lecteur local.

   Le fichier est copié vers la destination. L’original reste dans Adobe Cloud Drive.

>[!NOTE]
>
>Les fichiers copiés sur votre espace de stockage local sont des copies indépendantes. Les modifications apportées à une copie locale ne sont pas resynchronisées avec l’espace de stockage dans le cloud d’Adobe.

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## Chargement de fichiers dans le cloud (chargement direct) {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

Le chargement direct envoie les fichiers de votre ordinateur directement vers l’espace de stockage cloud d’Adobe, sans les copier au préalable dans le dossier Adobe Cloud Drive.

<!-- Courtney check me: Removed folder mentions from the Direct Upload section (intro, heading, step 1, 500-file bullet, hidden files bullet, and the Sync Activity link text), per Pulkit: folder support isn't available yet. Confirm nothing else should change. -->

### Charger des fichiers

1. Cliquez avec le bouton droit de la souris sur un fichier dans le Finder (Mac) ou l’Explorateur de fichiers (Windows).
1. Sélectionnez **Charger dans le cloud**.
1. Dans le sélecteur de destination, sélectionnez un emplacement dans l&#39;un des projets d&#39;Adobe Cloud Drive, puis cliquez sur **Télécharger ici**.
1. Surveillez la progression dans la section **Chargement direct** de la fenêtre Activité de synchronisation .

### Informations à connaître sur le chargement direct

* Le chargement direct copie l’élément dans le cloud. L’élément d’origine reste à son emplacement actuel.
* Vous pouvez sélectionner plusieurs éléments à charger simultanément.
* La section Chargement direct répertorie uniquement les fichiers individuels, jusqu’à 500 maximum.
* Vous pouvez charger des éléments à partir de votre répertoire personnel d&#39;utilisateurs ou de tout lecteur externe connecté. Les autres emplacements de stockage dans le cloud, tels qu&#39;iCloud Drive ou `~/Library/CloudStorage`, ne sont pas pris en charge.
* Vous devez être connecté avec un compte Adobe autorisé. Vous n’avez pas besoin de connexion Internet pour démarrer un chargement. Sans connexion , les chargements restent en file d’attente.
* La suspension de la synchronisation annule les chargements en cours. Les chargements mis en file d’attente reprennent automatiquement lorsque vous reprenez la synchronisation.
* Si vous quittez Adobe Cloud Drive pendant un chargement, les chargements en cours sont marqués comme annulés. Les chargements mis en file d’attente reprennent automatiquement lorsque vous redémarrez l’application.
* Les fichiers masqués, les liens symboliques et les alias ne sont pas pris en charge.
* Adobe Cloud Drive contrôle le nombre de téléchargements exécutés en même temps. Les chargements restants restent dans la file d’attente jusqu’à ce qu’un emplacement soit disponible.
* Un nombre réel de chargements, y compris les chargements ayant échoué, s’affiche, par exemple « 3 fichiers en cours de chargement ». Une fois tous les chargements terminés avec succès, le nombre passe à un résumé tel que « 3 fichiers chargés ». Sélectionnez **Ignorer** pour le supprimer.

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### Statut du chargement

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| Icône | Statut | Description | Actions disponibles |
| --- | --- | --- | --- |
| ![Icône en file d’attente](assets/acd-upload-status-queued.png) | En file d’attente | Le chargement est en attente de démarrage. | **Annuler** annule cet élément. |
| ![Icône de chargement](assets/acd-upload-status-uploading.png) | Chargement | Le chargement est en cours. | **Annuler** annule cet élément. |
| ![Icône Terminé](assets/acd-upload-status-completed.png) | Terminé | Le chargement s’est terminé correctement. | **Ouvrir dans Workfront** ouvre la ressource dans l’interface web de Workfront. |
| Icône ![Échec](assets/acd-upload-status-failed.png) | Échec | Le chargement n&#39;a pas pu être terminé. | **Afficher le fichier source** révèle le fichier original. **Réessayer** de relancer le chargement. La reprise n’est disponible que dans certains cas d’échec. |
| ![Icône Annulée](assets/acd-upload-status-cancelled.png) | Annulé | Le chargement a été arrêté, soit par vous, soit par le système. | Aucun. Les chargements annulés ne sont pas repris. Vous devez démarrer un nouveau chargement. |

Pour afficher la raison de l’échec, passez la souris sur l’élément en échec.

### Gestion de la liste de chargement

Chaque action n’est disponible que lorsqu’elle s’applique.

* **Annuler tous les chargements :** Disponible lorsque les chargements sont mis en file d&#39;attente ou en cours. Annule toutes les options.
* **Reprise des chargements ayant échoué :** Disponible lorsque des chargements ayant échoué peuvent être repris existent. Les réessaye tous. Les chargements qui ne peuvent pas être repris restent inchangés.
* **Effacer :** disponible lorsqu&#39;aucun chargement n&#39;est en file d&#39;attente ou en cours. Supprime tous les éléments terminés, en échec et annulés. Les fichiers locaux et le contenu déjà chargé ne sont pas affectés.
* **Effacement automatique :** les éléments terminés, ayant échoué et annulés sont supprimés automatiquement 24 heures après leur dernière mise à jour. Les éléments en file d’attente et en cours ne sont jamais supprimés automatiquement.

## Suspendre et reprendre la synchronisation {#pause-resume-sync}

Vous pouvez suspendre Adobe Cloud Drive lorsque vous ne souhaitez pas qu’il charge ou télécharge des fichiers, par exemple lors d’une connexion Internet lente ou limitée. Lorsque la synchronisation est suspendue, vos modifications ne sont pas envoyées au cloud et les modifications provenant du cloud ne sont pas téléchargées sur votre ordinateur. La synchronisation reste en pause jusqu’à ce que vous la repreniez.

### Suspendre la synchronisation

1. Cliquez sur l’icône Adobe Cloud Drive dans la barre d’état système (Windows) ou dans la barre de menus (Mac).
1. Cliquez sur l’icône **Menu** (≡) dans le coin supérieur droit de la fenêtre Adobe Cloud Drive.
1. Sélectionnez **Mettre en pause la synchronisation**.

   >[!TIP]
   >
   >Une fois la fenêtre Adobe Cloud Drive ouverte, vous pouvez également appuyer sur Ctrl+P (Windows) ou Commande+P (Mac).

   La fenêtre Adobe Cloud Drive indique **La synchronisation est suspendue** et le message **Les fichiers ne seront pas synchronisés tant que vous n&#39;aurez pas repris**. Lorsque vous pointez sur l’icône Adobe Cloud Drive, elle affiche **Adobe Cloud Drive (en pause)**.

>[!NOTE]
>
>La synchronisation Pause n’est disponible que lorsque vous êtes connecté et qu’Adobe Cloud Drive est connecté.

### Reprendre la synchronisation

1. Cliquez sur l’icône Adobe Cloud Drive dans la barre d’état système (Windows) ou dans la barre de menus (Mac).
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **Reprendre**.
   * Cliquez sur l’icône **Menu** (≡), puis sélectionnez **Reprendre la synchronisation**. Une fois la fenêtre ouverte, vous pouvez également appuyer sur Ctrl+R (Windows) ou Commande+R (Mac).

   Adobe Cloud Drive recommence la synchronisation, y compris les modifications que vous avez apportées alors que la synchronisation était en pause.

## Affichage et gestion de l’historique des versions {#version-history}

Vous pouvez utiliser l’historique des versions dans Adobe Cloud Drive pour parcourir les versions cloud enregistrées d’un fichier pris en charge, afficher les détails des versions et les miniatures, et revenir à une version antérieure. Vous pouvez également modifier le nom et la description d’une version si vous disposez des autorisations requises.

### Afficher l’historique des versions

1. Accédez au dossier Adobe Cloud Drive dans le Finder ou l’Explorateur de fichiers.
1. Sélectionnez un fichier pris en charge.
1. Cliquez avec le bouton droit sur le fichier et sélectionnez **Historique des versions**.
1. Sélectionnez une version pour afficher les détails et la miniature disponibles.

   Si le fichier ne comporte aucune version précédente, **Aucune version antérieure** ne s&#39;affiche. Les miniatures peuvent ne pas être disponibles pour chaque fichier ou version.

### Modifier les informations de version

1. Ouvrez Historique des versions pour le fichier.
1. Sélectionnez la version à mettre à jour.
1. Ouvrez le menu des options de la version et sélectionnez **Modifier les informations de la version**.
1. Saisissez un **nom de version** ou une **description**.
1. Sélectionnez **Enregistrer**.

   Les informations mises à jour sont enregistrées et s’affichent lorsque vous rouvrez l’historique des versions.

### Rétablir une version antérieure

1. Ouvrez Historique des versions pour le fichier.
1. Sélectionnez la version à restaurer.
1. Sélectionnez **Revenir à cette version**, le cas échéant.
1. Attendez la fin de la synchronisation.
1. Rouvrez le fichier pour vérifier que le contenu de la version sélectionnée est à jour.

## Gestion du stockage local {#manage-local-storage}

Vous pouvez utiliser Gérer le stockage local dans Adobe Cloud Drive pour surveiller l’utilisation du disque local, définir une limite de stockage et afficher les fichiers marqués comme **Toujours sur cet appareil**.

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### Affichage de l’utilisation du stockage local

1. Sélectionnez l’icône Adobe Cloud Drive et ouvrez son menu d’options.
1. Sélectionnez **Gérer Le Stockage Local**.
1. Passez en revue l&#39;utilisation actuelle du stockage et la liste des fichiers marqués comme **Toujours sur cet appareil**.
1. Triez la liste de fichiers par **Nom** ou **Taille** pour trouver des fichiers spécifiques.

### Modifier la limite de stockage local

1. Ouvrez **Gérer le stockage local** à partir du menu d’options d’Adobe Cloud Drive.
1. Saisissez la limite de stockage souhaitée.
1. Sélectionnez **Enregistrer** pour appliquer la modification.

>[!NOTE]
>
>Assurez-vous que l’espace disque disponible sur votre appareil est suffisant lorsque vous définissez la limite de stockage.

## Afficher l’activité de synchronisation {#sync-activity}

L’activité de synchronisation affiche l’activité récente entre le dossier Adobe Cloud Drive sur votre ordinateur et l’espace de stockage Adobe dans le cloud. Utilisez-le pour surveiller les chargements et les téléchargements, passer en revue les modifications terminées et identifier les éléments qui n’ont pas pu être synchronisés.

### Afficher l’activité de synchronisation

1. Sélectionnez l’icône Adobe Cloud Drive dans la barre de menus (Mac) ou dans la barre d’état système (Windows).
1. Développez la section de l’activité de synchronisation à l’aide de la flèche en regard du résumé de son statut.
1. Passez en revue les éléments répertoriés et leurs indicateurs de statut. Pointez sur un indicateur d’état pour afficher la progression du transfert, l’opération terminée ou un message d’erreur.
1. Sélectionnez le menu Autres actions en regard d’un élément pour afficher les actions disponibles pour cet élément.

### Choses à savoir sur l’activité de synchronisation

* La synchronisation normale effectue le suivi des modifications apportées par le biais du dossier Adobe Cloud Drive, y compris les chargements, les téléchargements, les créations, les renommages, les déplacements et les suppressions.
* La liste de synchronisation normale contient jusqu’à 500 entrées récentes. Les entrées nouvelles ou mises à jour s’affichent en haut. Les entrées plus anciennes peuvent être supprimées lorsque la liste atteint sa limite.
* Une entrée peut initialement afficher **Préparation...** pendant la résolution de son nom ou de ses métadonnées.
* Le résumé affiche le nombre d’éléments en cours de synchronisation. **La synchronisation est terminée**, ce qui signifie qu&#39;aucun élément n&#39;est actif actuellement. Inspectez la liste pour rechercher les éléments ayant échoué ou exclus plutôt que de traiter ce résumé comme une confirmation que chaque élément a réussi.
* Les fichiers et les dossiers exclus de la synchronisation peuvent s’afficher avec une erreur qui explique le nom non pris en charge, le type non pris en charge ou une autre raison d’exclusion.
* L’activité est effacée lorsque vous vous déconnectez. La liste est une vue d’activité, et non un historique d’audit permanent.

### Statut de synchronisation

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| Icône | Statut | Description | Actions disponibles |
| --- | --- | --- | --- |
| Indicateur en attente | En attente de synchronisation | L&#39;élément attend le début de son opération. | **Afficher dans le Finder** (Mac) ou **Afficher dans l&#39;Explorateur** (Windows), le cas échéant. |
| ![Icône de chargement](assets/acd-sync-status-uploading.png) | Chargement / Téléchargement | Transfert du contenu du fichier en cours. Pointez sur l’indicateur pour afficher le sens et le pourcentage de transfert, le cas échéant. À 100 %, l’info-bulle peut afficher **Finalisation en cours...** jusqu’à la fin du traitement. | **Afficher dans le Finder** ou **Afficher dans l&#39;Explorateur**, le cas échéant. |
| ![Icône Terminé](assets/acd-sync-status-completed.png) | Opération synchronisée/terminée | Opération terminée. L’info-bulle peut identifier Téléchargé, Chargé, Créé, Renommé, Renommé sur le cloud, Déplacé, Supprimé ou Supprimé sur le cloud. | **Afficher dans le Finder** ou **Afficher dans l&#39;Explorateur** pour les éléments non supprimés. **Ouvrez dans Workfront** pour les éléments terminés et non supprimés éligibles. |
| Icône ![Échec](assets/acd-sync-status-failed.png) | Échec/exclusion de la synchronisation | L’élément n’a pas pu être synchronisé ou est exclu de la synchronisation. Survolez l’indicateur pour en connaître la raison. | **Afficher dans le Finder** ou **Afficher dans l&#39;Explorateur**, le cas échéant. Résolvez le problème signalé avant d’attendre la synchronisation de l’élément. |

Les éléments supprimés ne peuvent pas être révélés localement ou ouverts dans Workfront à partir de leur entrée d’activité.

### Gestion de la liste des activités

| Action | Description |
| --- | --- |
| Développer ou réduire | Utilisez la flèche en regard du résumé de synchronisation pour afficher ou masquer des entrées individuelles. |
| Afficher dans le Finder / Afficher dans l’Explorateur | Recherchez un élément non supprimé dans le dossier Adobe Cloud Drive. |
| Ouvrir dans Workfront | Ouvrez un élément terminé éligible dans Workfront dans votre navigateur. Cette action n’est pas disponible pour les entrées de synchronisation normale actives, ayant échoué ou supprimées. |
| Effacer | Disponible si aucun élément de synchronisation normale n’est actif. Efface les entrées terminées, y compris les entrées ayant échoué, de la vue d’activité. L’effacement de l’historique ne supprime pas les fichiers locaux ou le contenu cloud et ne résout pas un échec de synchronisation. |
| Ignorer | Une fois un lot terminé, un résumé des éléments synchronisés peut s’afficher. Sélectionnez son bouton Fermer pour ignorer le résumé. |

>[!NOTE]
>
>Les lignes à synchronisation normale ne fournissent pas les actions **Réessayer** ou **Annuler** utilisées par le chargement direct pour chaque élément. Pour plus d&#39;informations sur le chargement direct, voir [Charger des fichiers dans le cloud (chargement direct)](#direct-upload).

## Ouverture d’un élément dans Workfront {#open-in-workfront}

Ouvrir dans Workfront permet de passer d’un élément d’Adobe Cloud Drive à l’emplacement correspondant dans Workfront, dans votre navigateur. Utilisez-le pour continuer à travailler avec l’élément cloud dans Workfront sans le rechercher manuellement.

### Ouvrir un élément à partir du Finder ou de l’Explorateur de fichiers

1. Ouvrez le dossier Adobe Cloud Drive dans le Finder (Mac) ou l’Explorateur de fichiers (Windows).
1. Sélectionnez un seul fichier ou dossier associé à un élément Workfront.
1. Cliquez avec le bouton droit sur l&#39;élément et sélectionnez **Ouvrir dans Workfront**.

   Votre navigateur affiche l’emplacement Workfront correspondant. Si vous y êtes invité, connectez-vous avec un compte ayant accès à cet élément.

### Ouvrir un élément à partir de l’activité de synchronisation

1. Sélectionnez l’icône Adobe Cloud Drive dans la barre de menus (Mac) ou dans la barre d’état système (Windows).
1. Développez la section de l’activité de synchronisation .
1. Pour un élément éligible terminé et non supprimé, ouvrez le menu Autres actions et sélectionnez **Ouvrir dans Workfront**.
1. Pour un fichier téléchargé via Chargement direct, utilisez la même action sur son entrée terminée dans la section **Chargement direct**.

### À savoir sur la fonctionnalité Ouvrir dans Workfront

* Sélectionnez un seul élément à la fois. L’ouverture de plusieurs éléments sélectionnés dans Workfront n’est pas prise en charge.
* Dans l’Explorateur de fichiers, la commande est masquée pour les éléments situés en dehors du dossier Adobe Cloud Drive et pour la racine du lecteur elle-même. Elle est désactivée lorsque plusieurs éléments sont sélectionnés.
* Un élément doit avoir un emplacement Workfront correspondant. Certains dossiers ou autres éléments peuvent ne pas avoir de mappage Workfront, même s’ils sont visibles dans Adobe Cloud Drive.
* Un nouvel élément local qui n’a pas terminé le chargement peut ne pas encore avoir de lien Workfront. Attendez la fin du chargement avant de réessayer.
* Dans une activité de synchronisation normale, l’action n’est proposée que pour les entrées terminées éligibles. Il n’est pas proposé pour les entrées actives, en échec ou supprimées.
* Dans Chargement direct, l’action est proposée pour les chargements terminés, et non pour les entrées mises en file d’attente, en chargement, en échec ou annulées.
* Vous devez être connecté à Adobe Cloud Drive. Workfront peut également vous demander de vous connecter séparément dans le navigateur, et vos autorisations Workfront s’appliquent toujours.
* Vous avez besoin d’une connexion Internet pour récupérer un lien non mis en cache et accéder à Workfront. Un lien précédemment résolu ne fournit pas d’accès hors ligne à Workfront.
* Cette action ouvre Workfront dans un navigateur. Il n’ouvre pas le fichier dans son application de bureau, ne charge pas une autre copie et ne modifie pas sa disponibilité hors connexion locale.

### Disponibilité des ouvertures dans Workfront

| Élément ou état | Comportement d’ouverture dans Workfront | Solution |
| --- | --- | --- |
| Élément éligible unique dans Adobe Cloud Drive | Ouvre l’emplacement Workfront correspondant. | Sélectionnez **Ouvrir dans Workfront**. |
| Plusieurs éléments sélectionnés | L’ouverture de plusieurs éléments n’est pas prise en charge. L’Explorateur de fichiers désactive la commande . | Sélectionnez un seul élément. |
| Nouvel élément en cours de chargement | Le lien Workfront n’est peut-être pas encore disponible. | Patientez jusqu’à la fin du chargement, puis réessayez. |
| Entrée de synchronisation normale terminée | Disponible lorsque l’élément est éligible et n’a pas été supprimé. | Utilisez le menu Autres actions de l’entrée. |
| Entrée de chargement direct terminée | Disponible une fois le chargement terminé. | Utilisez le menu Autres actions de l’entrée. |
| Élément sans mappage Workfront | Un message indique que l’élément n’est pas disponible dans Workfront. | Cochez l’élément directement dans Workfront ou choisissez un autre élément pris en charge. |
| Entrée de synchronisation normale supprimée | L’action n’est pas disponible. | Utilisez Workfront directement si vous devez enquêter sur l’élément supprimé. |

## Déconnexion d’Adobe Cloud Drive

Si vous vous déconnectez d’Adobe Cloud Drive, le lecteur reste visible dans le Finder ou l’Explorateur de fichiers. Toutefois, les modifications que vous apportez à l’intérieur du lecteur lors de la déconnexion et celles qui n’ont pas été synchronisées avant la déconnexion ne sont pas synchronisées dans le cloud.

La suite dépend du compte avec lequel vous vous reconnectez.

### Se reconnecter avec le même compte

Adobe Cloud Drive conserve le dossier monté local lorsque vous vous déconnectez. Si vous vous reconnectez avec les mêmes informations d’identification :

* Adobe Cloud Drive réutilise automatiquement le montage existant.
* Toutes les modifications non synchronisées effectuées avant la déconnexion sont conservées et sont synchronisées une fois la connexion restaurée.
* Aucune action n’est requise de votre part.

### Se connecter avec un autre compte

Si vous vous connectez avec un compte Adobe différent après vous être déconnecté :

* Le dossier monté actuel est automatiquement renommé et sauvegardé. Le nom du dossier de sauvegarde utilise le format suivant : `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`.
* Adobe Cloud Drive mappé au nouveau compte devient disponible dans le Finder ou l’Explorateur de fichiers comme d’habitude.
* Vous pouvez récupérer manuellement toute tâche non synchronisée à partir du dossier de sauvegarde avant de la supprimer.

>[!NOTE]
>
>Les dossiers de sauvegarde sont enregistrés dans `~/Library/CloudStorage` sous Mac et dans `C:\Users\<user>\` sous Windows. Si vous changez de compte plusieurs fois, plusieurs dossiers de sauvegarde horodatés sont créés. Examinez et nettoyez régulièrement les sauvegardes pour libérer de l’espace disque.

## Résoudre les conflits de fichiers

Des conflits peuvent survenir dans l’une des situations suivantes :

* Plusieurs utilisateurs modifient ou suppriment le même fichier en même temps.
* Un fichier est modifié lorsqu&#39;un autre utilisateur l&#39;ouvre.
* Les interruptions réseau entraînent des problèmes de synchronisation.

### Comment Adobe Cloud Drive résout les conflits

Adobe Cloud Drive utilise une stratégie de duplication pour les conflits :

* **Aucun verrouillage de fichier.** Plusieurs utilisateurs peuvent modifier des fichiers en même temps.
* **Duplication automatique.** Lorsqu’Adobe Cloud Drive détecte un conflit, il conserve les deux versions.
* **Effacer le nom.** Les fichiers en conflit incluent le nom d&#39;utilisateur et l&#39;horodatage au format suivant : `filename (Conflicted copy from username on date_time).extension`. Par exemple, `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`.

### Résoudre un conflit manuellement

1. Identifiez le fichier de conflit. Le nom des fichiers en conflit contient une « copie en conflit ».
1. Examinez les deux versions pour déterminer laquelle est correcte.
1. Conservez la version correcte et supprimez l’autre version.
1. Attribuez un nom approprié au fichier conservé.

>[!TIP]
>
>Pour minimiser les conflits :
>
>* Vérifiez le statut de synchronisation avant de modifier les fichiers.
>* Communiquez avec les membres de l’équipe pour savoir qui modifie quels fichiers.
>* Enregistrez fréquemment afin que les modifications soient synchronisées rapidement.
>* Fermez les fichiers lorsque vous avez terminé la modification.
