---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Résolution des problèmes liés à Adobe Cloud Drive
description: Passez en revue les limites, les considérations de performance et les solutions aux problèmes courants d’Adobe Cloud Drive sous Mac et Windows.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# Résolution des problèmes liés à Adobe Cloud Drive

Cet article décrit les limites d’Adobe Cloud Drive, les considérations de performances à garder à l’esprit et les solutions aux problèmes courants que vous pouvez rencontrer.

Pour plus d’informations sur l’utilisation d’Adobe Cloud Drive, voir [Utilisation d’Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Limites

### Opérations sur les fichiers et les dossiers

* Les dossiers de projet sont en lecture seule au niveau supérieur. Vous ne pouvez pas les renommer, les supprimer ou les déplacer depuis Adobe Cloud Drive. Pour créer, renommer ou supprimer un projet, utilisez l’interface web de Workfront.
* Les opérations de fichiers et de dossiers dans un dossier de projet sont entièrement prises en charge.

### Limites de fichier et de chemin d’accès

* Les noms de fichiers ne peuvent pas dépasser 255 caractères sur une plateforme.
* Le chemin d’accès complet au fichier (tous les noms de dossier plus le nom de fichier) ne peut pas dépasser 1 024 caractères. Les fichiers dont le chemin d’accès dépasse cette limite n’apparaissent pas dans Adobe Cloud Drive, même s’ils sont visibles dans l’interface web de Workfront.
* Si une erreur **Chemin d’accès complet trop long** s’affiche sur un fichier, raccourcissez les noms de dossier ou réduisez la profondeur d’imbrication des dossiers pour que le chemin d’accès respecte la limite.

### Stockage

* Les fichiers enregistrés dans Adobe Cloud Drive localement utilisent l’espace disque sur votre appareil.
* Les fichiers cloud uniquement n’utilisent pas le stockage local.
* Supprimez l’accès hors connexion aux fichiers dont vous n’avez plus besoin. Pour plus d’informations, voir [Supprimer l’accès hors ligne pour libérer de l’espace](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space) dans [Utiliser Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Considérations relatives aux performances

* **Taille du fichier :** le temps de synchronisation dépend de la taille du fichier. Les fichiers volumineux prennent généralement plus de temps.
* **Vitesse du réseau :** des connexions plus rapides offrent de meilleures performances de synchronisation. La synchronisation reprend automatiquement après une interruption.
* **Premier accès :** les fichiers sont téléchargés à la demande la première fois que vous y accédez. L’accès ultérieur est plus rapide car le fichier est mis en cache localement.

## Problèmes courants

### Adobe Cloud Drive n’apparaît pas

**Causes possibles :**

* Adobe Cloud Drive n’est pas installé.
* L&#39;installation ne s&#39;est pas terminée correctement.
* Votre organisation ne dispose pas d’une version de Workfront prenant en charge l’espace de stockage dans le cloud Adobe.

**Solutions:**

* Vérifiez qu’Adobe Cloud Drive est installé. Cochez **Applications** (Mac) ou **Programmes** (Windows).
* Lancez Adobe Cloud Drive manuellement.
* Contactez votre administrateur Workfront pour confirmer que votre organisation utilise une version de Workfront prenant en charge l’espace de stockage dans le cloud Adobe.
* Réinstallez Adobe Cloud Drive si nécessaire. Pour plus d’informations, voir [Installation d’Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

### L’icône Adobe Cloud Drive n’est pas visible dans la barre de menus ou dans la barre des tâches

**Causes possibles :**

* La barre de menus (Mac) ou la barre d’état système (Windows) ne dispose pas de suffisamment d’espace pour afficher l’icône.

**Solutions:**

* **Mac:** Maintenez la touche Cmd enfoncée et faites glisser les icônes de barre de menus existantes pour les réorganiser ou les supprimer, créant ainsi de l’espace pour l’icône Adobe Cloud Drive.
* **Windows :** cliquez sur la flèche vers le haut (**Afficher les icônes masquées**) de la barre des tâches pour rechercher l’icône Adobe Cloud Drive, puis faites-la glisser vers la zone visible.

### Les projets ne s’affichent pas ou certains projets sont manquants

**Causes possibles :**

* Vous n’avez accès à aucun projet.
* La synchronisation n&#39;est pas terminée.
* Vous avez un problème de connectivité réseau.

**Solutions:**

* Vérifiez l’accès à votre projet dans l’interface web de Workfront.
* Vérifiez votre connexion réseau.
* Déconnectez-vous d’Adobe Cloud Drive, puis reconnectez-vous.

### Les fichiers ne sont pas synchronisés

**Causes possibles :**

* Vous avez un problème de connectivité réseau.
* Erreur de synchronisation sur le fichier ou le dossier.
* Espace disque insuffisant.

**Solutions:**

* Vérifiez votre connexion Internet.
* Vérifiez que vous disposez de suffisamment d’espace disque.
* Vérifiez les indicateurs de statut du fichier pour détecter les erreurs de synchronisation. Pour plus d’informations, voir [Indicateurs de statut du fichier](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators) dans [Utiliser Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).
* Redémarrez Adobe Cloud Drive.
* Vérifiez l&#39;état d&#39;Adobe Cloud Drive dans la barre d&#39;état système (Windows) ou dans la barre de menus (Mac).

### Vous ne pouvez pas ouvrir un fichier

**Causes possibles :**

* Le fichier est en mode cloud uniquement et le téléchargement a échoué.
* L&#39;application requise pour ouvrir le fichier n&#39;est pas installée.
* Le fichier est corrompu.

**Solutions:**

* Vérifiez l’indicateur de statut du fichier.
* Vérifiez que l’application requise est installée.
* Cliquez avec le bouton droit sur le fichier, sélectionnez **Toujours conserver sur cet appareil**, puis essayez de l&#39;ouvrir à nouveau.
* Vérifiez que le fichier n’est pas corrompu dans l’interface web de Workfront.

### La synchronisation est lente

**Causes possibles :**

* Le fichier est grand.
* Votre connexion réseau est lente.
* De nombreux fichiers se synchronisent en même temps.

**Solutions:**

* Soyez patient avec les fichiers volumineux. La synchronisation peut être reprise, de sorte qu’elle reprend là où elle s’était arrêtée après une interruption.
* Vérifiez la vitesse de votre réseau.
* Limitez le nombre d’opérations de fichiers simultanées.
* Conservez les fichiers volumineux uniquement dans le cloud, sauf si vous avez besoin d’un accès hors ligne.

### Les fichiers hors ligne prennent trop d’espace

**Solutions:**

* Cliquez avec le bouton droit sur les fichiers hors ligne et sélectionnez **Libérer de l’espace**.
* Vérifiez régulièrement votre espace disque.
* Conservez les fichiers volumineux auxquels vous accédez rarement en mode cloud uniquement.

### Vous ne pouvez pas créer, modifier ou supprimer des fichiers ou des dossiers

**Causes possibles :**

* Vous tentez de créer, renommer ou supprimer un dossier de projet. Les dossiers de projet sont en lecture seule au niveau supérieur.
* Le projet est en lecture seule pour vous. Vous ne pouvez donc pas créer, modifier ni supprimer des fichiers ou des dossiers à l’intérieur de celui-ci.

**Solutions:**

* Pour créer, renommer ou supprimer un projet, utilisez l’interface web de Workfront.
* Demandez au propriétaire du projet de partager le projet avec vous avec un accès en modification.

## Obtenir de l’aide

Pour toute question sur les licences, les problèmes d’accès aux projets ou la configuration spécifique à une organisation, contactez votre administrateur Workfront.

Pour partager des journaux avec la prise en charge d’Adobe, suivez les étapes de la section [Exécution de l’outil de collecte de journaux d’Adobe](https://helpx.adobe.com/fr/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html).

## Bonnes pratiques

* **Planifier le travail hors ligne.** Téléchargez des fichiers avant de voyager ou de travailler dans des zones où la connectivité est faible.
* **Statut de synchronisation du moniteur.** Vérifiez les indicateurs de fichier avant de fermer les applications.
* **Suivez la structure de dossiers du projet.** Organisez les fichiers dans des dossiers de projet comme le souhaite le propriétaire du projet.
* **Utiliser des noms de fichier descriptifs.** Aidez les membres de votre équipe à trouver ce dont ils ont besoin.
* **Évitez de créer des doublons.** Ne faites pas de copies inutiles de fichiers.
