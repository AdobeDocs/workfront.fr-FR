---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Liaison de documents à partir d’applications externes
description: 'Vous pouvez lier des documents et des dossiers à Adobe Workfront à partir des sources suivantes : EDIT ME.'
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: 0ecee45183f5bc77a1c4a489013e486d8c26094c
workflow-type: tm+mt
source-wordcount: '2586'
ht-degree: 0%

---

# Liaison de documents à partir d’applications externes

Vous pouvez lier des documents et des dossiers à Adobe Workfront à partir des sources suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Fournisseurs de documents cloud tiers existants</td> 
   <td>Il s’agit notamment des éléments suivants : 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Épreuve Workfront </td> 
   <td>Vous pouvez rendre les bons à tirer créés à l’origine dans Workfront BAT disponibles dans Workfront. Pour utiliser cette fonctionnalité, vous devez disposer d’un abonnement Pro Workfront ou d’une version ultérieure. Pour plus d’informations sur les différents plans disponibles, voir <a href="https://www.workfront.com/plans">Formules Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader"> dʼExperience Manager Assets Essentials </td> 
   <td>Vous pouvez lier des documents à Workfront à partir de Experience Manager Assets Essentials. Pour plus d’informations, voir <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront pour Experience Manager Assets Essentials</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>Cela nécessite un achat supplémentaire. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autres fournisseurs de documents (par le biais d’intégrations de documents personnalisées)</td> 
   <td> <p class="workfront_plans">Pour utiliser cette fonctionnalité, vous devez disposer d’un abonnement Pro Workfront ou d’une version ultérieure. Pour plus d’informations sur les différents plans disponibles, voir <a href="https://www.workfront.com/plans">Formules Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Avant de lier des documents ou des dossiers, votre administrateur Workfront doit activer cette fonctionnalité pour chaque fournisseur de documents ou pour une intégration de documents personnalisée, comme décrit dans la section [Configuration des intégrations de documents](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

Vous pouvez tester et approuver les documents liés à un fournisseur cloud externe de la même manière que vous le faites avec les documents téléchargés directement vers Workfront. 

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Stockage de documents

Les documents liés à Workfront à partir d’une application externe sont stockés avec le fournisseur cloud externe et non dans Workfront.

Les exceptions suivantes s’appliquent :

* Lorsqu’il est fourni par le service de document, les miniatures et les images d’aperçu peuvent être stockées sur les serveurs Workfront.
* Lorsque vous utilisez le correctif dans Workfront, le document est copié et ajouté aux serveurs de vérification. 

## Liaison d’un document d’une application externe à Workfront

Vous pouvez lier des documents existants à un fournisseur cloud externe. Cela inclut tous les documents partagés.

* [Conditions préalables](#prerequisites)
* [Liaison d’un document externe à Workfront](#link-an-external-document-to-workfront)
* [Ajouter une nouvelle version d’un document lié](#add-a-new-version-of-a-linked-document)
* [Lier des documents Workfront BAT](#link-workfront-proof-documents)
* [Création d’un document Google dans Workfront](#create-a-google-document-from-within-workfront)

### Conditions préalables {#prerequisites}

Avant de lier des documents ou des dossiers, votre administrateur Workfront doit activer cette fonctionnalité pour chaque fournisseur de documents ou pour une intégration de documents personnalisée, comme décrit dans la section [Configuration des intégrations de documents](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Liaison d’un document externe à Workfront {#link-an-external-document-to-workfront}

Vous pouvez lier des documents à Workfront à partir d’une application externe telle que Google et Microsoft OneDrive.

>[!IMPORTANT]
>
>Dropbox stocke des documents en fonction du chemin d’accès au fichier. Ainsi, si un fichier lié à partir d’un Dropbox est déplacé, renommé ou supprimé, il devient inaccessible dans Workfront.

1. Accédez au **Documents** dans Workfront où vous souhaitez obtenir le document.
1. Cliquez sur **Ajouter**, puis cliquez sur le fournisseur de documents externe dans lequel vous souhaitez lier des documents à Workfront.

   Par exemple, pour lier des documents depuis Dropbox, cliquez sur **De Dropbox**.

   Les fournisseurs externes que vous avez déjà autorisés apparaissent en haut de la liste.

1. (Conditionnel) Si vous êtes invité à vous connecter au service externe, saisissez vos informations de connexion pour le service dans la zone qui s’affiche, puis cliquez sur **Se connecter**.
1. (Conditionnel) Si vous êtes invité à autoriser l’application externe, cliquez sur le bouton **Autoriser** bouton .

   Tu n&#39;as besoin de faire ça qu&#39;une seule fois.

1. Dans la zone de recherche du **Lier des fichiers et des dossiers externes** s’affiche, saisissez le nom de l’élément à rechercher, puis appuyez sur **Entrée** pour afficher tous les résultats de l’application externe, quel que soit le dossier dans lequel ils sont stockés.

   Ou

   Recherchez et sélectionnez les documents à lier.

   Bien que vous puissiez sélectionner plusieurs documents, seuls les documents sélectionnés dans la vue actuelle sont liés. Par exemple, si vous sélectionnez un document, puis accédez à un dossier, le document que vous avez initialement sélectionné n’est pas lié.

1. (Conditionnel) Si vous êtes un client DAM Workfront, cliquez sur le bouton **Miniature** pour afficher les fichiers sous forme d’images miniatures.

   >[!NOTE]
   Les clients DAM Workfront peuvent afficher des miniatures lors de la liaison de documents à partir de la gestion des actifs numériques Workfront. Des miniatures peuvent également s’afficher pour les clients DAM Workfront pour d’autres services tels que Dropbox et Box. Toutefois, l’affichage de miniatures pour des services autres que Workfront DAM dans Workfront n’est pas pris en charge et les miniatures ne s’affichent jamais lors de la liaison de documents à partir de SharePoint ou de Google Drive.

1. Cliquez sur **Lien**.

   Dans Workfront, l’icône du fournisseur de cloud s’affiche en regard des documents.

   >[!NOTE]
   Dans le cas des documents liés à une boîte, le lien vers le document dans la boîte ne s’affiche pas tant que vous n’avez pas actualisé la page.

### Ajouter une nouvelle version d’un document lié {#add-a-new-version-of-a-linked-document}

Vous pouvez ajouter une nouvelle version d’un document lié à Workfront à partir d’une application externe.

1. Accédez au **Documents** zone de liaison du document, puis sélectionnez le document associé.

   >[!IMPORTANT]
   Le document doit se trouver en dehors d’un dossier lié pour créer une version.

1. Cliquez sur **Ajouter** > **Version**, puis cliquez sur le fournisseur de documents externe.

   Par exemple, pour lier une nouvelle version d’un document à partir d’un Dropbox, cliquez sur **De Dropbox**.

   Les fournisseurs externes que vous avez déjà autorisés apparaissent en haut de la liste.

1. (Conditionnel) Si vous êtes invité à vous connecter au service externe, saisissez vos informations de connexion pour le service dans la zone qui s’affiche, puis cliquez sur **Se connecter**.
1. (Conditionnel) Si vous êtes invité à autoriser l’application externe, cliquez sur **Autoriser**.

   Tu n&#39;as besoin de faire ça qu&#39;une seule fois.

1. Dans la zone de recherche du **Lier des fichiers et des dossiers externes** s’affiche, saisissez le nom de l’élément à rechercher, puis appuyez sur **Entrée** pour afficher tous les résultats de l’application externe, quel que soit le dossier dans lequel ils sont stockés.

   Ou

   Recherchez et sélectionnez les documents à lier.

   Vous pouvez sélectionner plusieurs documents ; toutefois, seuls les documents sélectionnés dans la vue active sont liés. Par exemple, si vous sélectionnez un document, puis accédez à un dossier, le document que vous avez initialement sélectionné n’est pas lié.

1. (Conditionnel) Si vous êtes un client DAM Workfront, cliquez sur le bouton **Miniature** pour afficher les fichiers sous forme d’images miniatures.

   >[!NOTE]
   Les clients DAM Workfront peuvent afficher des miniatures lors de la liaison de documents à partir de la gestion des actifs numériques Workfront. Des miniatures peuvent également s’afficher pour les clients DAM Workfront pour d’autres services tels que Dropbox et Box. Toutefois, l’affichage de miniatures pour des services autres que Workfront DAM dans Workfront n’est pas pris en charge et les miniatures ne s’affichent jamais lors de la liaison de documents à partir de SharePoint ou de Google Drive.

1. Cliquez sur **Lien**.

   Dans Workfront, l’icône du fournisseur de cloud s’affiche en regard des documents, indiquant qu’ils sont liés au fournisseur de cloud externe.

   >[!NOTE]
   Dans le cas des documents liés à une boîte, le lien vers le document dans la boîte ne s’affiche pas tant que vous n’avez pas actualisé la page.

Pour plus d’informations sur l’ajout d’une nouvelle version d’un document que vous avez téléchargé vers Workfront à partir de votre système de fichiers, voir [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#adding-new-versions-of-documents) in [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Lier des documents Workfront BAT {#link-workfront-proof-documents}

Vous pouvez lier des bons à tirer à Workfront qui existaient à l’origine dans le bon à tirer Workfront. Lorsque vous liez un BAT à partir d’un BAT Workfront, tous les commentaires et autres métadonnées associés au BAT sont disponibles dans Workfront. 

Vous pouvez lier uniquement les BAT pour lesquels vous disposez de l’accès Affichage dans le BAT Workfront.

1. Accédez au **Documents** dans Workfront où vous souhaitez obtenir le document.
1. Cliquez sur **Ajouter**, puis cliquez sur **A partir du bon à tirer Workfront**.

   >[!NOTE]
   Les options de ce menu peuvent varier en fonction des fournisseurs tiers configurés dans votre environnement.

1. Dans le **Lien** proofs **de** Zone Bon à tirer de Workfront qui s’affiche, commencez à saisir le nom du BAT que vous souhaitez rendre disponible dans Workfront.

   La liste est filtrée au fur et à mesure que vous tapez.

1. Sélectionnez jusqu’à 10 bons à tirer à lier.

   Un nom de BAT grisé n’est pas disponible pour la liaison, car le BAT est déjà associé à un document dans Workfront.

1. Cliquez sur **Lien**.

   La version la plus récente du BAT est liée à Workfront. Lorsque vous ouvrez le BAT, toutes les versions sont disponibles dans la visionneuse de vérification.

### Création d’un document Google dans Workfront {#create-a-google-document-from-within-workfront}

Vous pouvez créer un document Google dans Workfront. Vous ne pouvez pas créer de documents à partir de Workfront pour d’autres fournisseurs cloud.

1. Accédez au **Documents** dans Workfront où vous souhaitez obtenir le document.
1. Cliquez sur **Ajouter** > **Fichier Google**, puis sélectionnez le type de document Google que vous souhaitez créer.

1. Sélectionnez le type de document Google que vous souhaitez créer.
1. Si la variable **Ajout d’un compte de lecteur Google** s’affiche, cliquez sur **Autoriser Google Drive**.

   Un document Google est ajouté à la variable **Documents** .

   >[!NOTE]
    Mon lecteur et Partagé avec moi affichent deux résultats différents. Si vous ne parvenez pas à localiser un fichier dans Mon lecteur, archivez le dossier Partagé avec moi .

## Mise à jour et liaison d’un document de Workfront à un fournisseur cloud externe

Vous pouvez charger et lier un document de Workfront à un fournisseur cloud externe. Cette opération déplace le stockage du document de Workfront vers le fournisseur cloud externe. Lorsque le document est modifié dans l’application externe, il est automatiquement mis à jour dans Workfront.

Les utilisateurs n’ayant pas accès à Workfront peuvent voir le document dans l’application externe s’ils ont accès à l’application.

1. Sélectionnez un document téléchargé dans Workfront.
1. Cliquez sur **Plus** >**Envoyer à**, puis sélectionnez le fournisseur de cloud que vous souhaitez utiliser pour le stockage du document lié.

   Vous pouvez également utiliser le menu Plus ![](assets/more-icon.png) sur la page Détails du document pour effectuer cette opération.

1. Sélectionnez le dossier dans l’application du fournisseur où vous souhaitez stocker le document.

   Il peut s’agir de n’importe quel dossier de l’application du fournisseur, y compris un dossier partagé.

1. Cliquer sur **Enregistrer**.

   Le logo du fournisseur externe s’affiche en regard du nom du document pour indiquer que le document est désormais lié à Workfront et stocké par le fournisseur cloud externe.

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## Lier des dossiers

Lorsque vous liez un dossier entre Workfront et un fournisseur de cloud externe, le dossier et tout son contenu sont liés. Si les utilisateurs n’ayant pas accès à Workfront ajoutent, suppriment et modifient des fichiers à partir de l’application de document externe, leurs modifications sont synchronisées avec Workfront. Les sections suivantes décrivent comment lier des dossiers et des sous-dossiers :

* [Droits d’accès au dossier](#folder-access-rights)
* [Lier un ou plusieurs dossiers externes](#link-one-or-more-external-folders)
* [Ajout de sous-dossiers à un dossier lié](#add-subfolders-to-a-linked-folder)

### Droits d’accès au dossier {#folder-access-rights}

Lors de la synchronisation du contenu du dossier à partir d’une application de document externe, Workfront utilise les informations d’identification de l’utilisateur qui a initialement lié le dossier. Cela entraîne l’expérience utilisateur suivante :

* Si les utilisateurs n’ont pas accès à l’affichage des fichiers et des dossiers dans l’application externe, mais qu’ils ont accès à l’affichage du dossier lié via Workfront, ils ne peuvent afficher que les noms des fichiers et des dossiers dans Workfront, et non leur contenu.
* Lorsqu’un utilisateur accède au contenu d’un dossier lié dans Workfront (tel qu’un sous-dossier dans un dossier lié) lié à Workfront par un autre utilisateur, le contenu se synchronise avec Workfront à l’aide des informations d’identification de connexion Workfront de l’utilisateur qui a initialement lié le dossier, et non des informations d’identification de l’utilisateur accédant au contenu.

>[!IMPORTANT]
* Si l’utilisateur qui a initialement lié le dossier est supprimé du système Workfront, il ne peut plus accéder au contenu du dossier lié via Workfront. Dans ce cas, le dossier doit être relationné par un utilisateur Workfront principal disposant des droits sur le dossier dans l’application externe.
* Si l’utilisateur qui a lié un dossier n’a plus accès à l’application externe, Workfront ne peut plus accéder au contenu du dossier. Cela peut se produire, par exemple, si l’utilisateur qui avait initialement lié le dossier quitte la société. Pour garantir un accès continu, un utilisateur ayant accès au dossier doit lier à nouveau le dossier.


### Lier un ou plusieurs dossiers externes {#link-one-or-more-external-folders}

1. Accédez à la zone Workfront dans laquelle vous souhaitez placer le dossier, puis cliquez sur  **Documents** ![](assets/document-icon.png) dans le panneau de gauche .

1. Cliquez sur **Ajouter**, puis cliquez sur le fournisseur de documents externe à partir duquel vous souhaitez lier un dossier à Workfront.
1. (Conditionnel) Si vous n’avez pas encore autorisé le service externe, spécifiez vos informations de connexion pour le fournisseur externe, puis cliquez sur **Se connecter**.

   Les fournisseurs externes que vous avez déjà autorisés apparaissent en haut de la liste.

1. Dans le **Lier des fichiers et des dossiers externes** qui s’affiche, recherchez et sélectionnez les dossiers à lier.

   Ou

   Saisissez le nom du dossier à rechercher, puis appuyez sur **Entrée**.

   Vous pouvez sélectionner plusieurs dossiers ; toutefois, seuls les dossiers sélectionnés dans la vue actuelle sont liés. Par exemple, si vous sélectionnez un dossier, puis accédez à un dossier, le dossier que vous avez initialement sélectionné n’est pas lié.

   >[!NOTE]
   Lors de la liaison de dossiers à partir de Google Drive, vous ne pouvez lier que les dossiers qui se trouvent sur votre disque personnel (My Drive) et dans Team Drive. Vous ne pouvez pas lier des dossiers à partir de la zone Partagé avec moi .

1. Cliquez sur **Lien**.

   Dans Workfront, le logo du fournisseur de cloud s’affiche en regard du dossier, indiquant qu’il est lié au fournisseur de cloud externe.

1. (Facultatif) Pour renommer le dossier de sorte que le nom du dossier dans Workfront soit différent de celui de l’application de document externe, sélectionnez le dossier dans la **Dossiers** , cliquez sur le menu Plus ![](assets/more-icon.png)  qui s’affiche en regard du nom du dossier, puis cliquez sur **Renommer**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

Cela ne renomme pas le dossier dans l’application externe.

### Ajout de sous-dossiers à un dossier lié  {#add-subfolders-to-a-linked-folder}

Vous pouvez créer un dossier dans un dossier lié existant. Vous pouvez également faire glisser un autre dossier vers un dossier lié existant.

1. Pour créer un dossier dans un dossier lié existant, accédez au dossier existant, puis créez le nouveau dossier comme décrit dans la section [Création de dossiers de document](../../documents/organizing-documents/create-documents-folder.md).

   Ou

   Pour faire glisser un dossier existant dans un dossier lié existant, accédez à la zone Documents dans laquelle vous souhaitez placer le sous-dossier, puis faites-le glisser dans le dossier lié.

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   Les restrictions suivantes s’appliquent lorsque vous faites glisser un dossier Workfront existant dans un dossier lié :
   * Le dossier que vous faites glisser ne peut pas déjà être lié et ne peut pas contenir de contenu déjà lié.
   * Le dossier (y compris son contenu) que vous faites glisser ne peut pas dépasser 50 Mo.


## Ajouter un document à un dossier lié

Lorsque vous ajoutez un document à un dossier lié via Workfront, il est automatiquement ajouté en tant que document lié.

1. Dans le **Documents** à l’endroit où vous souhaitez obtenir le document, faites-le glisser dans un dossier lié.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode"> <img src="assets/documents-linked-document-move-nwe-350x126.png" style="width: 350;height: 126;">Selection box is wonky on the left<br></p>
   -->

   Ou

   Sélectionnez le dossier lié dans lequel vous souhaitez obtenir le document, puis cliquez sur **Ajouter > Document**, puis accédez au document et ajoutez-le au dossier .

   Une nouvelle version de votre document est automatiquement créée dans l’application externe et liée à Workfront.

## Suppression d’un document ou d’un dossier lié

Lorsque vous supprimez un document ou un dossier lié de l’application externe, le document ou le dossier reste dans le système Workfront jusqu’à ce que vous le supprimiez également de Workfront.

1. Sélectionnez le document ou le dossier lié, puis cliquez sur **Supprimer**.
1. Dans la boîte de confirmation qui s’affiche, cliquez sur **Oui, dissociez-le**.

   Le document n’est plus lié au site Workfront. Elle n’est pas affectée dans l’application externe.

## À propos du changement de nom des documents et dossiers liés

Lorsque vous renommez un document ou un dossier lié, le changement n’est visible que dans l’application dans laquelle il est créé. Par exemple, si vous renommez un document lié dans Workfront, le nouveau nom n’est visible que dans Workfront.

Si vous souhaitez que le nom corresponde dans Workfront et dans l’application externe, vous devez le renommer aux deux endroits.

>[!IMPORTANT]
Ne renommez pas un document Workfront lié à Dropbox ; ce faisant, le fichier dans Workfront est inaccessible. Renommez plutôt le fichier dans Dropbox, puis resynchronisez-le, comme décrit dans la section [Liaison de documents à partir d’applications externes](#synchronizing-changes-made-on-a-linked-document).
