---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Utiliser l’extension Workfront pour Illustrator et InDesign
description: Vous pouvez utiliser l’extension Workfront pour exporter du contenu numérique que vous enregistrez et créez dans Adobe Illustrator et Adobe InDesign vers Workfront. Cela accélère le processus de révision et d’approbation des documents.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '3107'
ht-degree: 98%

---

# Utiliser l’extension Workfront pour Illustrator et InDesign

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Nous remplaçons l’extension Workfront pour Illustrator et InDesign par des [plug-ins Creative Cloud mis à jour](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). À compter de la fin de 2022, cette extension ne sera plus prise en charge et sera disponible en l’état.

Vous pouvez utiliser l’extension Workfront pour exporter du contenu numérique que vous enregistrez et créez dans Adobe Illustrator et Adobe InDesign vers Workfront. Cela accélère le processus de révision et d’approbation des documents.

L’extension Workfront est prise en charge pour Adobe Creative Cloud 2017 et versions ultérieures dans les applications suivantes :

* InDesign
* Illustrator
* Photoshop

  >[!NOTE]
  >
  >Nous vous recommandons d’utiliser le nouveau plug-in [Adobe Workfront pour Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Actuel : Pro ou supérieur</p>
   Ou
   <p>Nouvelle : n’importe quelle formule</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Actuellement : Travail ou licence supérieure</p>
   Ou
   <p>Nouveau : Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’une licence Adobe Creative Cloud en plus d’une licence Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès Modifier à l’objet avec lequel vous souhaitez interagir.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Se connecter à l’extension Workfront depuis Illustrator ou InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

Lorsque vous vous connectez à Workfront à partir de l’une des applications d’Adobe prises en charge, vous vous connectez à toutes les applications d’Adobe prises en charge.

1. Accédez à l’application Adobe dans laquelle vous souhaitez utiliser l’extension Workfront.

   Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. Cliquez sur **Fenêtre** > **Extensions** > Workfront.

1. (Facultatif) Faites glisser le panneau Workfront vers la position où il doit s’afficher dans l’application Adobe.
1. Suivez les invites pour vous connecter à Workfront.

   >[!NOTE]
   >
   >* Workfront se connecte à Adobe Creative Cloud à l’aide d’OAuth 2.0, une norme sécurisée utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs et utilisatrices.
   >* Lorsqu’on vous invite à saisir le [domaine ou l’hôte] de votre compte Workfront, saisissez-le au format suivant : `yourCompany'sDomain.my.workfront.com`. Le domaine de votre entreprise est généralement le nom de votre entreprise.

   Une liste des tâches qui vous sont affectées s’affiche si le projet a le statut Actuel. Si aucune liste ne s’affiche, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

## Charger un fichier vers un projet, une tâche ou un problème Workfront {#upload-a-file-to-a-workfront-project-task-or-issue}

Vous pouvez charger un fichier à partir de votre système de fichiers ou exporter un fichier actuellement ouvert dans une application Adobe Creative Cloud vers un projet, une tâche ou un problème Workfront. 

Tenez compte des points suivants lors du chargement ou de l’export d’un fichier à partir d’Adobe Creative Cloud :

* Votre niveau d’accès doit permettre le chargement de documents vers Workfront. Pour plus d’informations, voir [Accorder l’accès aux documents](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* Vous devez disposer des autorisations nécessaires pour charger des documents vers l’élément qui vous intéresse. Pour plus d’informations, voir [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Le fichier est chargé dans la zone Documents pour l’objet Workfront que vous sélectionnez.
* Vous ne pouvez pas exporter un document vers la zone Documents du menu principal ![icône du menu principal](assets/main-menu-icon.png) à partir d’une application Adobe Creative Cloud.

Les sections suivantes expliquent ce qui suit :

* [Charger un fichier](#upload-a-file)
* [Exporter un fichier actuellement ouvert dans Illustrator ou InDesign](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Charger une nouvelle version d’un fichier à partir d’Illustrator ou InDesign](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### Charger un fichier {#upload-a-file}

Vous pouvez charger vos fichiers vers un projet, une tâche ou u problème sans quitter l’application Adobe Creative Cloud.

1. Si vous ne voyez pas l’extension Workfront lorsque vous ouvrez votre application Adobe Creative Cloud, cliquez sur **Fenêtre** > **Extensions** > **Workfront**.

   Une liste des tâches qui vous sont affectées s’affiche si le projet a le statut Actuel. Si aucune liste ne s’affiche, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le nom de l’élément (projet, tâche ou problème) vers lequel vous souhaitez charger le fichier.

   Pour ce faire, saisissez le nom dans la zone **Rechercher** et sélectionnez **Projet**, **Tâche**, ou **Problème** à partir du menu déroulant à droite de la zone **Rechercher**. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous pouvez afficher.

1. Cliquez sur **Sélectionner** dans le coin inférieur droit de l’extension Workfront.
1. Dans le menu déroulant **Cliquer pour sélectionner le format**, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. (Le cas échéant) Si l’élément de travail sur lequel vous souhaitez charger le fichier contient des dossiers de documents, sélectionnez un dossier de documents dans le champ **Cliquer pour sélectionner un dossier de documents**, puis cliquez sur **Sélectionner**.

1. Cliquez sur **Charger un fichier local**.
1. Dans la case **Ouvrir le fichier** recherchez le fichier dans votre système de fichiers, puis cliquez sur **Ouvrir**.

1. (Facultatif) Saisissez un nouveau nom pour le fichier.

   ![Renommer le fichier](assets/rename-file-uploading.png)

1. Cliquez sur **Charger**.

   Dans Workfront, le document est maintenant répertorié dans la zone Documents pour l’élément (projet, tâche ou problème) que vous avez sélectionné.

1. (Facultatif) Cliquez sur le nom du document pour ouvrir sa page Détails du document dans Workfront.

   Workfront s’ouvre dans un nouvel onglet du navigateur.

### Exporter un fichier actuellement ouvert dans Illustrator ou InDesign {#export-a-file-currently-open-in-illustrator-or-indesign}

1. Dans une application Adobe Creative Cloud prise en charge, ouvrez un fichier que vous souhaitez exporter vers Workfront.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > **Workfront**.

   Une liste des tâches qui vous sont affectées s’affiche si le projet a le statut Actuel. Si aucune liste ne s’affiche, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le nom de l’élément (projet, tâche ou problème) vers lequel vous souhaitez exporter le fichier.

   Pour ce faire, saisissez le nom dans la zone **Rechercher** et sélectionnez **Projet**, **Tâche**, ou **Problème** à partir du menu déroulant à droite de la zone **Rechercher**. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous pouvez afficher.

1. Dans le menu déroulant **Cliquer pour sélectionner le format**, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. (Le cas échéant) Si l’élément de travail sur lequel vous souhaitez charger le fichier contient des dossiers de documents, sélectionnez un dossier de documents dans le champ **Cliquer pour sélectionner un dossier de documents**, puis cliquez sur **Sélectionner**.
1. (Facultatif) Pour renommer le document, cliquez sur le nom du document et saisissez un nouveau nom.

   ![Renommer le document à l’exportation](assets/rename-doc-exporting.png)

1. Cliquez sur **Exporter**.

   Un message s’affiche pour confirmer que le document a bien été exporté vers Workfront.

   Dans Workfront, le document est répertorié dans la zone Documents de l’objet que vous avez spécifié dans Workfront.

1. (Facultatif) Cliquez sur le nom du document pour y accéder dans Workfront.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront s’ouvre dans un nouvel onglet du navigateur.

### Charger une nouvelle version d’un fichier à partir d’Illustrator ou InDesign {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. Si vous souhaitez exporter un fichier sur lequel vous travaillez dans une application d’Adobe prise en charge en tant que nouvelle version d’un fichier dans Workfront, ouvrez-le dans l’application Adobe.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > **Workfront**.

   Une liste des tâches qui vous sont affectées s’affiche si le projet a le statut Actuel. Si aucune liste ne s’affiche, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le nom du projet, de la tâche ou du problème où le document existant est répertorié.

   Pour ce faire, saisissez le nom dans la zone **Rechercher** et sélectionnez **Projet**, **Tâche**, ou **Problème** depuis le menu déroulant à droite de la zone **Rechercher**. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous pouvez afficher.

   Tous les documents chargés sur des projets, des tâches ou des problèmes s’affichent dans une liste, qu’ils aient été chargés à partir de l’application Adobe ou non.

1. Dans le menu déroulant **Cliquer pour sélectionner le format**, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   C’est obligaoire si vous exportez un fichier que vous avez ouvert dans l’application Adobe. Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. Si vous exportez un fichier que vous avez ouvert dans l’application Adobe en tant que nouvelle version du document Workfront que vous avez sélectionné, cliquez sur **Exporter**.

   Ou

   Si vous souhaitez charger un fichier à partir de votre système de fichiers d’ordinateur en tant que nouvelle version du document Workfront que vous avez sélectionné, cliquez sur **Charger un fichier local**, recherchez le fichier dans la zone qui s’affiche, puis cliquez sur **Ouvrir** et sur **Charger**.

1. (Facultatif) Cliquez sur le nom du document pour afficher sa nouvelle version dans Workfront.

   >[!NOTE]
   >
   >Le nom du document dans Workfront est renseigné par défaut et ne peut pas être modifié. Cela ne change pas non plus le nom du fichier que vous chargez ou exportez en tant que nouvelle version.
   >
   >
   >![Le nom du document ne peut pas être modifié](assets/doc-name-cant-be-changed.png)

## Commenter un document Workfront à partir d’Illustrator ou InDesign {#comment-on-a-workfront-document-from-illustrator-or-indesign}

Vous pouvez ajouter des commentaires directement à un document Workfront dans une application Adobe. Dans Workfront, vos commentaires s’affichent dans les zones Mises à jour du document et Mises à jour de l’élément Workfront dans lequel le document est enregistré.

1. Ouvrez l’une des applications Adobe prises en charge.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > **Workfront**.

   Une liste des tâches qui vous sont affectées s’affiche si le projet a le statut Actuel. Si aucune liste ne s’affiche, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur l’élément (projet, tâche ou problème) dans lequel le document existant est répertorié.

   Pour ce faire, saisissez le nom dans la zone **Rechercher** et sélectionnez **Projet**, **Tâche**, ou **Problème** à partir du menu déroulant à droite de la zone **Rechercher**. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous pouvez afficher.

1. Cliquez sur le nom du document existant, puis sur **Sélectionner** dans le coin inférieur droit de l’extension Workfront.
1. Cliquez sur l’onglet **Commenter**, puis saisissez votre mise à jour dans la zone.

1. (Facultatif) Pour inclure d’autres utilisateurs et utilisatrices ou équipes Workfront sur le commentaire, commencez à saisir le nom d’un utilisateur, d’une utilisatrice ou d’une équipe dans la zone **Notifier des personnes ou des équipes**, puis cliquez sur le nom qui apparaît dans la liste déroulante.
1. (Facultatif) Pour demander l’approbation du document, sélectionnez **Effectuer une demande d’approbation**.
1. Cliquez sur **Mettre à jour**.

   Une mise à jour est publiée dans l’onglet Mises à jour du document. Les utilisateurs et utilisatrices Workfront que vous incluez dans le commentaire reçoivent une notification in-app et, selon la manière dont Workfront est configuré, peuvent également recevoir une notification par e-mail.

   Pour plus d’informations sur les notifications dans Workfront, voir [Afficher et gérer des notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

   Pour plus d’informations sur la réception de notifications par e-mail, voir [Notifications Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Demander l’approbation d’un document à partir d’Illustrator ou InDesign

Vous pouvez demander l’approbation d’un document Workfront directement à partir d’une application Adobe.

Vous pouvez demander l’approbation d’un document auprès des entités suivantes :

* Un utilisateur ou une utilisatrice Workfront
* Un utilisateur ou une utilisatrice externe sans compte Workfront

Vous pouvez demander l’approbation d’un document depuis une application Adobe de la manière suivante :

* En joignant un approbateur ou une approbatrice au document.
* En commentant un document, en informant la personne lorsque vous faites un commentaire et en la joignant en tant qu’approbateur ou approbatrice au document.

  Pour plus d’informations sur la demande d’approbation lors de l’ajout de commentaires sur un document, voir la section [Commenter un document Workfront à partir d’Illustrator ou InDesign](#comment-on-a-workfront-document-from-illustrator-or-indesign) dans cet article.

Pour demander l’approbation d’un document depuis une application Adobe, procédez comme suit :

1. Ouvrez l’une des applications Adobe prises en charge.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > **Workfront**.

   Une liste des tâches qui vous sont affectées s’affiche si le projet a le statut Actuel. Si aucune liste ne s’affiche, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le projet, la tâche ou le problème où le document existant est répertorié, puis cliquez sur le nom du document existant.

   Pour ce faire, saisissez le nom dans la zone **Rechercher** et sélectionnez **Projet**, **Tâche**, ou **Problème** dans le menu déroulant à droite de la zone **Rechercher**. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront pour lesquels vous possédez un accès en affichage.

1. Cliquez sur le nom du document existant, puis sur **Sélectionner** en bas à droite de l’extension Workfront.
1. Cliquez sur l’onglet **Approbation**.
1. Pour ajouter un approbateur ou une approbatrice, effectuez l’une des opérations suivantes dans la zone **Commencer à saisir un nom** :

   * Saisissez le nom d’un approbateur ou d’une approbatrice, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

     ![Ajouter un approbateur de document](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * Saisissez l’adresse e-mail d’une personne externe.

1. Cliquez sur **Demander une approbation**.

   Les utilisateurs et utilisatrices Workfront que vous incluez dans le commentaire ou ajoutez en tant qu’approbateurs et approbatrices reçoivent une notification in-app et, selon la configuration de Workfront, peuvent également recevoir une notification par e-mail.\
   Les personnes externes reçoivent une notification par e-mail leur permettant de prendre une décision concernant l’approbation.

   Pour plus d’informations sur les notifications dans Workfront, voir la section [Afficher et gérer des notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). Pour plus d’informations sur la réception de notifications par e-mail, voir la section [Notifications Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Générer une épreuve à partir d’Illustrator ou d’InDesign {#generate-a-proof-from-illustrator-or-indesign}

Si votre organisation utilise des modèles de workflows automatisés, vous pouvez générer une épreuve pour un document que vous créez dans une application Adobe sans quitter l’application. Pour plus d’informations sur la création d’épreuves, voir la section [Créer des épreuves](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md). Pour plus d’informations sur les modèles de workflows automatisés, voir la section [Modèles de workflows automatisés](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) dans [Vue d’ensemble des workflows automatisés](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. Ouvrez l’une des applications Adobe prises en charge.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > Workfront.

   Une liste des tâches qui vous sont affectées s’affiche si le projet a le statut Actuel. Si aucune liste ne s’affiche, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Si le document est déjà chargé dans Workfront, sélectionnez le projet, la tâche ou le problème dans l’extension Workfront où le document est répertorié, puis cliquez sur le nom du document.

   Ou

   Chargez un document Adobe dans un objet Workfront, comme décrit dans la section [Charger un fichier dans un projet, une tâche ou un problème Workfront](#upload-a-file-to-a-workfront-project-task-or-issue) dans cet article, puis cliquez sur le nom du document.

1. Dans le menu déroulant **Cliquer pour sélectionner le format**, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   Certains formats ne sont plus disponibles une fois que vous avez activé la fonctionnalité de relecture à l’étape suivante. Pour plus d’informations, voir la section [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. Cliquez sur **Charger en tant que nouvelle épreuve** pour l’activer.
1. Sélectionnez le **Modèle de workflow** que les personnes devront utiliser lors de la révision du document.

   Votre équipe d’administration Workfront configure des modèles de workflows automatisés, comme décrit dans la section [Créer et gérer des modèles de workflows automatisés](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). Pour toute question, contactez votre équipe d’administration.

   1. Ajoutez au moins une **Nouvelle personne destinataire** à chaque étape du modèle de workflow.

      Vous pouvez commencer à saisir un nom et le sélectionner lorsque vous le voyez dans la liste déroulante qui s’affiche.

   1. Spécifiez le **Rôle d’épreuve** et la fréquence des **Alertes par e-mail** pour chaque personnes destinataire que vous ajoutez.

   1. (Facultatif) Dans la section **Notification par e-mail**, indiquez si vous souhaitez envoyer une notification par e-mail avec un message personnalisé facultatif concernant l’épreuve à toutes les personnes destinataires de l’épreuve que vous avez ajoutées.

1. Cliquez sur **Créer une épreuve**.

   Vous pouvez afficher la progression du processus de création de l’épreuve. Une alerte s’affiche une fois la création terminée. Vous pouvez ouvrir la tâche dans laquelle vous avez créé l’épreuve, qui y est alors répertoriée.

## Charger une nouvelle version d’une épreuve sans quitter Illustrator ou InDesign

1. Cliquez sur un document existant contenant une épreuve, puis sur **Sélectionner** en bas à droite.
1. Cliquez sur **Charger en tant que nouvelle version d’épreuve** pour l’activer.
1. (Facultatif) Sélectionnez le **modèle de workflow** que les personnes doivent utiliser lors de la révision de la nouvelle version.

   Si vous ne sélectionnez pas de modèle différent, le modèle sélectionné pour la version précédente reste actif. En outre, si vous avez modifié le modèle pour la version précédente, les modifications sont appliquées sur la nouvelle version.

   Votre équipe d’administration Workfront configure des modèles de workflows automatisés, comme décrit dans la section [Créer et gérer des modèles de workflows automatisés](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). Pour toute question, contactez votre équipe d’administration.

   1. Ajoutez au moins une **Nouvelle personne destinataire** à chaque étape du modèle de workflow.

      Vous pouvez commencer à saisir un nom et le sélectionner lorsque vous le voyez dans la liste déroulante qui s’affiche.

   1. Spécifiez le **Rôle d’épreuve** et la fréquence des **Alertes par e-mail** pour chaque personnes destinataire que vous ajoutez.
   1. (Facultatif) Dans la section **Notification par e-mail**, indiquez si vous souhaitez envoyer une notification par e-mail avec un message personnalisé facultatif concernant l’épreuve à toutes les personnes destinataires de l’épreuve que vous avez ajoutées.

1. Cliquez sur **Créer une version d’épreuve**.

   Vous pouvez afficher la progression du processus de création de l’épreuve. Une alerte s’affiche une fois la création terminée. Vous pouvez ouvrir la tâche dans laquelle vous avez créé l’épreuve, qui y est alors répertoriée.

## Se déconnecter de l’extension Workfront

1. Dans l’application Adobe, cliquez sur **Fenêtre** > **Extensions** > **Workfront**.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit du panneau.

1. (Facultatif) Cliquez sur **Commentaires** pour ouvrir une enquête rapide et envoyer vos commentaires sur Workfront pour Adobe Creative Cloud à Workfront.
1. Cliquez sur **Déconnexion**.\
   L’écran Connexion s’affiche. Pour plus d’informations sur la connexion, voir [Se connecter à l’extension Workfront à partir d’Illustrator ou InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) dans cet article.

## Formats de fichiers exportés pris en charge {#supported-exported-file-formats}

* [Formats de fichiers exportés pris en charge pour Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [Formats de fichiers exportés pris en charge pour Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### Formats de fichiers exportés pris en charge pour Adobe InDesign {#supported-exported-file-formats-for-adobe-indesign}

Workfront prend en charge les formats de fichiers suivants pour exporter un fichier d’InDesign vers Workfront :

* EPS - PostScript encapsulé
* EPUB - Publication électronique à disposition fixe
* EPUB - Publication électronique redistribuable &#42;
* HTML - Langage de balisage hypertexte
* IDML - InDesign Markup Language &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PDF - Fichier Adobe Portable Document
* PNG - Portable Network Graphics
* SWF - Flash Player &#42;
* XML - Langage de balisage extensible &#42;

&#42; Ce format de fichier n’est pas disponible lorsque l’option **Charger une nouvelle épreuve** est activée (pour plus d’informations sur cette option, voir [Générer une épreuve à partir d’Illustrator ou d’InDesign](#generate-a-proof-from-illustrator-or-indesign) dans cet article). Si ce format de fichier est déjà sélectionné avant l’activation de l’option **Charger une nouvelle épreuve**, le système remplace le format de fichier par PDF. Vous pouvez sélectionner un autre format dans la liste.

### Formats de fichiers exportés pris en charge pour Adobe Illustrator {#supported-exported-file-formats-for-adobe-illustrator}

Workfront prend en charge les formats de fichiers suivants pour exporter un fichier d’Illustrator vers Workfront :

* DWG - AutoCAD Drawing, fichier d’échange AutoCAD &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PNG - Portable Network Graphics
* PSD - Document Photoshop
* SWF - Flash Player &#42;
* TIFF - Tagged Image File Format

&#42; Ce format de fichier n’est pas disponible lorsque l’option **Charger une nouvelle épreuve** est activée (pour plus d’informations sur cette option, voir [Générer une épreuve à partir d’Illustrator ou d’InDesign](#generate-a-proof-from-illustrator-or-indesign) dans cet article). Si ce format de fichier est déjà sélectionné avant l’activation de l’option **Charger une nouvelle épreuve**, le système remplace le format de fichier par PNG. Vous pouvez sélectionner un autre format dans la liste.
