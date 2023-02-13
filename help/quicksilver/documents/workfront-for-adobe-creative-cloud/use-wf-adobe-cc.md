---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Utilisation de l’extension Workfront pour Illustrator et InDesign
description: Vous pouvez utiliser l’extension Workfront pour exporter du contenu numérique que vous enregistrez et créez dans Adobe Illustrator et Adobe InDesign vers Workfront. Cela accélère le processus de révision et d’approbation des documents.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: 147a5b5d508e1ea01d18d981f9157439a643cf55
workflow-type: tm+mt
source-wordcount: '3056'
ht-degree: 0%

---

# Utilisation de l’extension Workfront pour Illustrator et InDesign

>[!IMPORTANT]
>
>Nous remplaçons l’extension Workfront pour Illustrator et InDesign par [modules externes de Creative Cloud mis à jour](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). À compter de la fin de 2022, cette extension ne sera plus prise en charge et sera disponible en l’état.


Vous pouvez utiliser l’extension Workfront pour exporter du contenu numérique que vous enregistrez et créez dans Adobe Illustrator et Adobe InDesign vers Workfront. Cela accélère le processus de révision et d’approbation des documents.

L’extension Workfront est prise en charge pour Adobe Creative Cloud 2017 et versions ultérieures dans les applications suivantes :

* InDesign
* Illustrator
* Photoshop

   >[!NOTE]
   >
   >Nous vous recommandons d’utiliser la nouvelle [Adobe Workfront pour Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) module externe

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’une licence Adobe Creative Cloud en plus d’une licence Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modifiez l’accès à l’objet avec lequel vous souhaitez interagir.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Connexion à l’extension Workfront depuis Illustrator ou InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

Lorsque vous vous connectez à Workfront à partir de l’une des applications d’Adobe prises en charge, vous êtes connecté à toutes les applications d’Adobe prises en charge.

1. Accédez à l’application Adobe dans laquelle vous souhaitez utiliser l’extension Workfront.

   Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. Cliquez sur **Fenêtre** > **Extensions** > Workfront.

1. (Facultatif) Faites glisser le panneau Workfront vers l’emplacement où il doit s’afficher dans l’application d’Adobe.
1. Suivez les invites pour vous connecter à Workfront.

   >[!NOTE]
   >
   >* Workfront se connecte à Adobe Creative Cloud à l’aide d’OAuth 2.0, une norme sécurisée utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs.
   >* Lorsque vous êtes invité à saisir la variable [domaine ou hôte] de votre compte Workfront, saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.


   Une liste des tâches qui vous sont affectées s’affiche si le projet est à l’état actuel. Si une liste ne s’affiche pas, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

## Télécharger un fichier vers un projet, une tâche ou un problème Workfront {#upload-a-file-to-a-workfront-project-task-or-issue}

Vous pouvez télécharger un fichier à partir de votre système de fichiers ou exporter un fichier actuellement ouvert dans une application Adobe Creative Cloud vers un projet, une tâche ou un problème Workfront. 

Tenez compte des points suivants lors du téléchargement ou de l’exportation d’un fichier à partir de Adobe Creative Cloud :

* Votre niveau d’accès doit permettre le téléchargement de documents vers Workfront. Pour plus d’informations, voir [Accorder l’accès aux documents](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* Vous devez disposer des autorisations nécessaires pour télécharger des documents vers l’élément qui vous intéresse. Pour plus d’informations, voir [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Le fichier est téléchargé dans la zone Documents pour l’objet Workfront que vous sélectionnez.
* Vous ne pouvez pas exporter un document vers la zone Documents du menu principal. ![](assets/main-menu-icon.png) à partir d’une application Adobe Creative Cloud.

Cette section explique ce qui suit :

* [Chargement d’un fichier](#upload-a-file)
* [Exporter un fichier actuellement ouvert dans Illustrator ou InDesign](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Télécharger une nouvelle version d’un fichier depuis Illustrator ou InDesign](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### Chargement d’un fichier {#upload-a-file}

Vous pouvez charger vos fichiers vers un projet, une tâche ou une question sans quitter l’application Adobe Creative Cloud.

1. Si vous ne voyez pas l’extension Workfront lorsque vous ouvrez votre application Adobe Creative Cloud, cliquez sur **Fenêtre** > **Extensions** > Workfront.

   Une liste des tâches qui vous sont affectées s’affiche si le projet est à l’état actuel. Si une liste ne s’affiche pas, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le nom du projet, de la tâche ou du problème auquel vous souhaitez charger le fichier.

   Pour ce faire, saisissez le nom dans la variable **Rechercher** et sélection **Projet**, **Tâche** ou **Problème** depuis le menu déroulant à droite de l’objet **Rechercher** de la boîte. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous avez accès à afficher.

1. Cliquez sur **Sélectionner** dans le coin inférieur droit de l’extension Workfront.
1. Dans le **Cliquez pour sélectionner le format** dans le menu déroulant, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. (Conditionnel) Si l’élément de travail sur lequel vous souhaitez charger le fichier contient des dossiers de documents, sélectionnez un dossier de documents dans la **Cliquez pour sélectionner un dossier de document.** , puis cliquez sur **Sélectionner**.

1. Cliquez sur **Chargement d’un fichier local**.
1. Dans le **Ouvrir le fichier** qui s’affiche, recherchez le fichier dans votre système de fichiers, puis cliquez sur **Ouvrir**.

1. (Facultatif) Saisissez un nouveau nom pour le fichier. 

   ![](assets/rename-file-uploading.png)

1. Cliquez sur **Télécharger**.

   Dans Workfront, le document est maintenant répertorié dans la zone Documents pour le projet, la tâche ou le problème que vous avez spécifié.  

1. (Facultatif) Cliquez sur le nom du document pour ouvrir sa page Détails du document dans Workfront.

   Workfront s’ouvre dans un nouvel onglet du navigateur.

### Exporter un fichier actuellement ouvert dans Illustrator ou InDesign {#export-a-file-currently-open-in-illustrator-or-indesign}

1. Dans une application Adobe Creative Cloud prise en charge, ouvrez un fichier que vous souhaitez exporter vers Workfront. 
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > Workfront.

   Une liste des tâches qui vous sont affectées s’affiche si le projet est à l’état actuel. Si une liste ne s’affiche pas, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le nom du projet, de la tâche ou du problème auquel vous souhaitez exporter le fichier.

   Pour ce faire, saisissez le nom dans la variable **Rechercher** et sélection **Projet**, **Tâche** ou **Problème** depuis le menu déroulant à droite de l’objet **Rechercher** de la boîte. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous avez accès à afficher.

1. Dans le **Cliquez pour sélectionner le format** dans le menu déroulant, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. (Conditionnel) Si l’élément de travail sur lequel vous souhaitez charger le fichier contient des dossiers de documents, sélectionnez un dossier de documents dans la **Cliquez pour sélectionner un dossier de document.** , puis cliquez sur **Sélectionner**.
1. (Facultatif) Pour renommer le document, cliquez sur le nom du document et saisissez un nouveau nom.

   ![](assets/rename-doc-exporting.png)

1. Cliquez sur **Exporter**. 

   Un message s’affiche pour confirmer que le document a bien été exporté vers Workfront.

   Dans Workfront, le document est répertorié dans la zone Documents de l’objet que vous avez spécifié dans Workfront.

1. (Facultatif) Cliquez sur le nom du document auquel accéder dans Workfront.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront s’ouvre dans un nouvel onglet du navigateur.

### Télécharger une nouvelle version d’un fichier depuis Illustrator ou InDesign {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. Si vous souhaitez exporter un fichier sur lequel vous travaillez dans une application d’Adobe prise en charge en tant que nouvelle version d’un fichier dans Workfront, ouvrez-le dans l’application d’Adobe. 
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > Workfront.

   Une liste des tâches qui vous sont affectées s’affiche si le projet est à l’état actuel. Si une liste ne s’affiche pas, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le nom du projet, de la tâche ou du problème où le document existant est répertorié.

   Pour ce faire, saisissez le nom dans la variable **Rechercher** et sélection **Projet**, **Tâche** ou **Problème** depuis le menu déroulant à droite de l’objet **Rechercher** de la boîte. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous avez accès à afficher.

   Tous les documents chargés sur des projets, des tâches ou des problèmes s’affichent dans une liste, qu’ils aient été téléchargés à partir de l’application Adobe ou non.

1.  
1. Dans le **Cliquez pour sélectionner le format** dans le menu déroulant, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   Cela est nécessaire si vous exportez un fichier que vous avez ouvert dans l’application Adobe. Pour obtenir la liste des formats pris en charge pour chaque application prise en charge, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. Si vous exportez un fichier que vous avez ouvert dans l’application Adobe en tant que nouvelle version du document Workfront que vous avez sélectionné, cliquez sur **Exporter**.

   Ou

   Si vous souhaitez charger un fichier à partir de votre système de fichiers d’ordinateur en tant que nouvelle version du document Workfront que vous avez sélectionné, cliquez sur **Chargement d’un fichier local**, recherchez le fichier dans la zone qui s’affiche, puis cliquez sur **Ouvrir**, puis cliquez sur **Télécharger**.

1. (Facultatif) Cliquez sur le nom du document pour afficher sa nouvelle version dans Workfront. 

   >[!NOTE]
   >
   >Le nom du document dans Workfront est renseigné par défaut et ne peut pas être modifié. Il ne change pas non plus le nom du fichier que vous téléchargez ou exportez en tant que nouvelle version.
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## Commentaire sur un document Workfront à partir d’Illustrator ou d’un InDesign {#comment-on-a-workfront-document-from-illustrator-or-indesign}

Vous pouvez ajouter des commentaires directement à un document Workfront dans une application Adobe. Dans Workfront, vos commentaires s’affichent dans les zones Mises à jour du document et Mises à jour de l’élément Workfront dans lequel le document est enregistré. 

1. Ouvrez l’une des applications d’Adobe prises en charge.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > Workfront.

   Une liste des tâches qui vous sont affectées s’affiche si le projet est à l’état actuel. Si une liste ne s’affiche pas, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le projet, la tâche ou le problème où le document existant est répertorié.

   Pour ce faire, saisissez le nom dans la variable **Rechercher** et sélection **Projet**, **Tâche** ou **Problème** depuis le menu déroulant à droite de l’objet **Rechercher** de la boîte. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous avez accès à afficher.

1. Cliquez sur le nom du document existant, puis sur **Sélectionner** dans le coin inférieur droit de l’extension Workfront.
1. Cliquez sur le bouton **Commentaire** puis saisissez la mise à jour dans la zone qui s’affiche.

1. (Facultatif) Pour inclure d’autres utilisateurs ou équipes Workfront sur le commentaire, commencez à saisir le nom d’un utilisateur ou d’une équipe dans le champ **Notifier les personnes ou les équipes** puis cliquez sur le nom qui apparaît dans la liste déroulante.
1. (Facultatif) Pour demander l’approbation du document, sélectionnez **Effectuer une demande d’approbation**.
1. Cliquez sur **Mettre à jour**.

   Une mise à jour est publiée dans l’onglet Mises à jour du document. Les utilisateurs Workfront que vous incluez dans le commentaire reçoivent une notification in-app et, selon la manière dont Workfront est configuré, peuvent également recevoir une notification électronique.

   Pour plus d’informations sur les notifications dans Workfront, voir [Affichage et gestion des notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 

   Pour plus d’informations sur la réception de notifications par courrier électronique, voir [Notifications Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Demande d’approbation de document auprès d’Illustrator ou d’un InDesign

Vous pouvez demander l’approbation d’un document Workfront directement auprès d’une application Adobe.

Vous pouvez demander la validation d&#39;un document auprès des entités suivantes :

* Un utilisateur Workfront
* Un utilisateur externe sans compte Workfront

Vous pouvez demander une validation sur un document à une application d&#39;Adobe de la manière suivante :

* En joignant un approbateur au document.
* En commentant un document, informez la personne lorsque vous faites un commentaire. et les joindre en tant qu’approbateur au document.

   Pour plus d’informations sur la demande d’approbation lors de la création de commentaires sur un document, voir [Commentaire sur un document Workfront à partir d’Illustrator ou d’un InDesign](#comment-on-a-workfront-document-from-illustrator-or-indesign) dans cet article.

Pour demander la validation d&#39;un document à une application d&#39;Adobe :

1. Ouvrez l’une des applications d’Adobe prises en charge.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > Workfront.

   Une liste des tâches qui vous sont affectées s’affiche si le projet est à l’état actuel. Si une liste ne s’affiche pas, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Cliquez sur le projet, la tâche ou le problème où le document existant est répertorié, puis cliquez sur le nom du document existant.

   Pour ce faire, saisissez le nom dans la variable **Rechercher** et sélection **Projet**, **Tâche** ou **Problème** depuis le menu déroulant à droite de l’objet **Rechercher** de la boîte. Si le nom de l’élément de travail n’apparaît pas dans la liste, appuyez sur **Entrée** pour rechercher tous les éléments Workfront que vous avez accès à afficher.

1. Cliquez sur le nom du document existant, puis sur **Sélectionner** dans le coin inférieur droit de l’extension Workfront.
1. Cliquez sur le bouton **Validation** .
1. Pour ajouter un approbateur, dans la variable **Commencer à saisir un champ de nom** effectuez l’une des opérations suivantes :

   * Saisissez le nom d’un approbateur, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

      ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * Saisissez l’adresse électronique d’un utilisateur externe.

1. Cliquez sur **Demande d’approbation**.

   Les utilisateurs Workfront que vous incluez dans le commentaire ou ajoutez en tant qu’approbateurs reçoivent une notification in-app et, selon la configuration de Workfront, peuvent également recevoir une notification par e-mail.\
   Les utilisateurs externes reçoivent une notification par e-mail leur permettant de prendre une décision concernant l’approbation.

   Pour plus d’informations sur les notifications dans Workfront, voir [Affichage et gestion des notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). Pour plus d’informations sur la réception de notifications par courrier électronique, voir [Notifications Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Générer un BAT à partir d’Illustrator ou d’InDesign {#generate-a-proof-from-illustrator-or-indesign}

Si votre entreprise utilise des modèles de processus automatisés, vous pouvez générer un BAT pour un document que vous créez dans une application Adobe sans quitter l’application. Pour plus d’informations sur la création de BAT, voir [Créer un bon à tirer](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md). Pour plus d’informations sur les modèles de processus automatisés, voir [Modèles de workflow automatisés](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) in [Présentation des processus automatisés](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. Ouvrez l’une des applications d’Adobe prises en charge.
1. Si l’extension Workfront n’est pas affichée, cliquez sur **Fenêtre** > **Extensions** > Workfront.

   Une liste des tâches qui vous sont affectées s’affiche si le projet est à l’état actuel. Si une liste ne s’affiche pas, connectez-vous à Workfront.

   Les tâches personnelles sont répertoriées sous **Aucun projet**.

1. Si le document est déjà téléchargé vers Workfront, sélectionnez le projet, la tâche ou le problème dans l’extension Workfront où le document est répertorié, puis cliquez sur le nom du document.

   Ou

   Télécharger un document d’Adobe vers un objet Workfront, comme décrit dans la section [Télécharger un fichier vers un projet, une tâche ou un problème Workfront](#upload-a-file-to-a-workfront-project-task-or-issue) dans cet article, cliquez sur le nom du document.

1. Dans le **Cliquez pour sélectionner le format** dans le menu déroulant, cliquez sur le format dans lequel vous souhaitez enregistrer le fichier dans Workfront.

   Certains formats ne sont pas disponibles une fois que vous avez activé la fonctionnalité de vérification à l’étape suivante. Pour plus d’informations, voir [Formats de fichiers exportés pris en charge](#supported-exported-file-formats) dans cet article.

1. Cliquez sur **Chargement en tant que nouveau BAT** pour l’activer.
1. Sélectionnez la **Modèle de workflow** vous souhaitez que les personnes utilisent lors de la révision du document.

   Votre administrateur Workfront configure des modèles de workflow automatisés, comme décrit dans la section . Si vous avez des questions, contactez l’administrateur.

   1. Ajouter au moins un **Nouveau destinataire** à chaque étape du modèle de workflow.

      Vous pouvez commencer à saisir un nom et le sélectionner lorsque vous le voyez dans la liste déroulante qui s’affiche.

   1. Spécifiez la variable **Rôle BAT** et la fréquence **Alertes par email** pour chaque destinataire que vous ajoutez.

   1. (Facultatif) Dans le **Notification par email** , indiquez si vous souhaitez envoyer une notification par email avec un message personnalisé facultatif concernant le BAT à tous les destinataires du BAT que vous avez ajoutés.

1. Cliquez sur **Créer un BAT**.

   Vous pouvez afficher la progression du processus de création du BAT. Une alerte s’affiche une fois la génération terminée. Vous pouvez ouvrir la tâche dans laquelle vous avez créé le BAT, qui est alors répertoriée.

## Télécharger une nouvelle version d&#39;un BAT sans quitter Illustrator ou InDesign

1. Cliquez sur un document existant contenant un BAT, puis cliquez sur **Sélectionner** dans le coin inférieur droit.
1. Cliquez sur **Télécharger en tant que nouvelle version du BAT** pour l’activer.
1. (Facultatif) Sélectionnez le **Modèle de workflow** vous souhaitez que les utilisateurs utilisent lors de la révision de la nouvelle version.

   Si vous ne sélectionnez pas de modèle différent, le modèle sélectionné pour la version précédente reste en vigueur. En outre, si vous avez modifié le modèle pour la version précédente, les modifications sont appliquées pour la nouvelle version.

   Votre administrateur Workfront configure des modèles de workflow automatisés, comme décrit dans la section . Si vous avez des questions, contactez l’administrateur.

   1. Ajouter au moins un **Nouveau destinataire** à chaque étape du modèle de workflow.

      Vous pouvez commencer à saisir un nom et le sélectionner lorsque vous le voyez dans la liste déroulante qui s’affiche.

   1. Spécifiez la variable **Rôle BAT** et la fréquence **Alertes par email** pour chaque destinataire que vous ajoutez.
   1. (Facultatif) Dans le **Notification par email** , indiquez si vous souhaitez envoyer une notification par email avec un message personnalisé facultatif concernant le BAT à tous les destinataires du BAT que vous avez ajoutés.

1. Cliquez sur **Créer une version de BAT**.

   Vous pouvez afficher la progression du processus de création du BAT. Une alerte s’affiche une fois la génération terminée. Vous pouvez ouvrir la tâche dans laquelle vous avez créé le BAT, qui est alors répertoriée.

## Déconnexion de l’extension Workfront

1. Dans l’application Adobe, cliquez sur **Fenêtre** > **Extensions** > Workfront.

1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit du panneau.

1. (Facultatif) Cliquez sur **Commentaires** pour ouvrir une enquête brève et envoyer vos commentaires sur Workfront for Adobe Creative Cloud à Workfront. 
1. Cliquez sur **Déconnexion**.\
   L’écran Connexion s’affiche. Pour plus d’informations sur la connexion, voir [Connexion à l’extension Workfront depuis Illustrator ou InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) dans cet article.

## Formats de fichiers exportés pris en charge {#supported-exported-file-formats}

* [Formats de fichiers exportés pris en charge pour Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [Formats de fichiers exportés pris en charge pour Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### Formats de fichiers exportés pris en charge pour Adobe InDesign  {#supported-exported-file-formats-for-adobe-indesign}

Workfront prend en charge les formats de fichiers suivants pour exporter un fichier d’InDesign vers Workfront :

* EPS - PostScript encapsulé
* EPUB - Publication électronique à mise en page fixe
* EPUB : publication électronique redistribuable &#42;
* HTML - Langage de balisage HyperText
* IDML - Langage de balisage d’InDesign &#42;
* JPG, JPEG - Groupe d&#39;experts photographiques communs
* PDF - Adobe de fichier de document portable
* PNG - Graphiques réseau mobiles
* SWF - Flash Player &#42;
* XML - Extensible Markup Language &#42;

&#42; Ce format de fichier n’est pas disponible lorsque **Télécharger un nouveau BAT** est activé (pour plus d’informations sur cette option, voir [Générer un BAT à partir d’Illustrator ou d’InDesign](#generate-a-proof-from-illustrator-or-indesign) dans cet article). Si ce format de fichier est déjà sélectionné avant l’activation **Télécharger un nouveau BAT**, le système remplace le format de fichier par PDF. Vous pouvez sélectionner un autre format dans la liste.

### Formats de fichiers exportés pris en charge pour Adobe Illustrator  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront prend en charge les formats de fichiers suivants pour exporter un fichier d’Illustrator vers Workfront :

* DWG - Dessin AutoCAD, fichier d’échange AutoCAD &#42;
* JPG, JPEG - Groupe d&#39;experts photographiques communs
* PNG - Graphiques réseau mobiles
* PSD - Document Photoshop
* SWF - Flash Player &#42;
* TIFF : format de fichier image balisé

&#42; Ce format de fichier n’est pas disponible lorsque **Télécharger un nouveau BAT** est activé (pour plus d’informations sur cette option, voir [Générer un BAT à partir d’Illustrator ou d’InDesign](#generate-a-proof-from-illustrator-or-indesign) dans cet article). Si ce format de fichier est déjà sélectionné avant l’activation **Télécharger un nouveau BAT**, le système remplace le format de fichier par PNG. Vous pouvez sélectionner un autre format dans la liste.
