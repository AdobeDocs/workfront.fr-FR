---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Utilisation d’Adobe Cloud Drive
description: Utilisez vos projets de stockage dans le cloud Adobe directement depuis le Finder ou l’Explorateur de fichiers à l’aide d’Adobe Cloud Drive. Ouvrez et modifiez des fichiers dans n’importe quelle application, travaillez hors ligne et résolvez les conflits.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d5dd769447e81d5d95b4907f8a01016b118f2322
workflow-type: tm+mt
source-wordcount: 1723
ht-degree: 2%

---

# Utilisation d’Adobe Cloud Drive

Après avoir installé Adobe Cloud Drive, vous pouvez travailler avec vos projets de stockage dans le cloud Adobe directement depuis le Finder ou l’Explorateur de fichiers. Vous pouvez ouvrir et modifier des fichiers dans n’importe quelle application, travailler hors ligne et laisser Adobe Cloud Drive synchroniser vos modifications avec le cloud.

Pour plus d’informations sur l’installation d’Adobe Cloud Drive, voir [Installation d’Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

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
| ![Icône Hors ligne disponible](assets/acd-windows-available-offline.png) | Disponible hors ligne | Le fichier est synchronisé et disponible hors connexion. | Au moins un fichier du dossier est disponible hors connexion. |
| ![&#x200B; Icône épinglée &#x200B;](assets/acd-windows-pinned.png) | Épinglé (toujours conserver sur l’appareil) | Le fichier est synchronisé et toujours conservé hors ligne. Adobe Cloud Drive ne purge pas automatiquement le contenu épinglé. | Tous les fichiers du dossier se trouvent dans le cache local et sont disponibles hors ligne. |
| ![Icône Lecture seule](assets/acd-windows-read-only.png) | Lecture seule | Fichier en lecture seule. | Le dossier est en lecture seule. |
| ![&#x200B; Icône d’erreur de synchronisation &#x200B;](assets/acd-windows-sync-error.png) | Erreur de synchronisation | Impossible de synchroniser le fichier. Pour plus d’informations, pointez sur l’icône. | Impossible de synchroniser le dossier. Pour plus d’informations, pointez sur l’icône. |
| ![Icône Synchronisation exclue](assets/acd-windows-sync-excluded.png) | Synchronisation exclue | Le fichier ne peut pas être synchronisé en raison d&#39;un type ou d&#39;un nom non pris en charge. | Le dossier ne peut pas être synchronisé en raison d’un nom non pris en charge. |

### Indicateurs de statut des fichiers sur Mac

| Icône | Statut | Signification du fichier | Signification du dossier |
| --- | --- | --- | --- |
| (Pas d’icône) | Disponible hors ligne | Le fichier est synchronisé et disponible hors connexion. | Tous les fichiers sont disponibles hors ligne. |
| ![Icône en ligne uniquement](assets/acd-mac-online-only.png) | En ligne uniquement | Le fichier est synchronisé et disponible uniquement en ligne. | Au moins un fichier du dossier est en ligne uniquement. |
| ![Icône de synchronisation](assets/acd-mac-syncing.png) | Synchronisation | Les dernières mises à jour du fichier sont synchronisées avec le cache local ou l’espace de stockage dans le cloud d’Adobe. | Synchronisation du contenu du dossier. |
| ![&#x200B; Icône d’erreur de synchronisation &#x200B;](assets/acd-windows-sync-error.png) | Erreur de synchronisation | Le fichier ne peut pas être mis à jour ni synchronisé. Pour plus d’informations, pointez sur l’icône. | Le dossier ne peut pas être mis à jour ni synchronisé. Pour plus d’informations, pointez sur l’icône. |
| ![Icône Synchronisation exclue](assets/acd-windows-sync-excluded.png) | Synchronisation exclue | Fichier exclu de la synchronisation. | Le dossier est exclu de la synchronisation. |
| ![Icône Lecture seule](assets/acd-mac-read-only.png) | Lecture seule | Fichier en lecture seule. | Le dossier est en lecture seule. |
| ![&#x200B; Icône épinglée &#x200B;](assets/acd-windows-pinned.png) | Épinglé (toujours conserver sur l’appareil) | Le fichier est épinglé pour être disponible hors ligne. Adobe Cloud Drive ne purge pas automatiquement le contenu épinglé. | Le dossier est épinglé pour être disponible hors ligne. |

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
>Enregistrez les fichiers à l’aide de **Fichier** > **Enregistrer** ou du raccourci clavier. Évitez d’utiliser **Enregistrer sous** pour créer des copies, car cela génère des fichiers en double dans le lecteur.

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
1. Sélectionnez **Libérer de l’espace**.

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
>Les dossiers de sauvegarde sont enregistrés dans `~/Library/CloudStorage` sous Mac et `C:\Users\<user>\` sous Windows. Si vous changez de compte plusieurs fois, plusieurs dossiers de sauvegarde horodatés sont créés. Examinez et nettoyez régulièrement les sauvegardes pour libérer de l’espace disque.

## Résoudre les conflits de fichiers

Des conflits peuvent survenir dans l’une des situations suivantes :

* Plusieurs utilisateurs modifient ou suppriment le même fichier en même temps.
* Un fichier est modifié lorsqu&#39;un autre utilisateur l&#39;ouvre.
* Les interruptions réseau entraînent des problèmes de synchronisation.

### Comment Adobe Cloud Drive résout les conflits

Adobe Cloud Drive utilise une stratégie de duplication pour les conflits :

* **Aucun verrouillage de fichier.** Plusieurs utilisateurs peuvent modifier des fichiers en même temps.
* **Duplication automatique.** Lorsqu’Adobe Cloud Drive détecte un conflit, il conserve les deux versions.
* **Effacer le nom.** Les fichiers en conflit incluent le nom d’utilisateur et l’horodatage au format suivant : `filename (Conflicted copy from username on date_time).extension`. Par exemple, `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`.

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
