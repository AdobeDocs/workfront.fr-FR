---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurez la variable [!UICONTROL Experience Manager Assets as a Cloud Service] integration
description: Vous pouvez connecter votre travail à votre contenu dans [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 821e31b8c6023a9ec4e017cc5548bb9fd930983c
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# Configurez la variable [!UICONTROL Experience Manager Assets as a Cloud Service] integration

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les organisations qui ont été intégrées au [!DNL Adobe Admin Console].

Vous pouvez connecter votre travail à votre contenu dans [!DNL Experience Manager Assets]&#x200B; :

* Purge des ressources et des métadonnées à partir de [!DNL Adobe Workfront] to [!DNL Experience Manager Assets]&#x200B;
* Lier des ressources depuis [!DNL Experience Manager Assets] à vos projets et tâches dans [!DNL Workfront&#x200B;]
* Faciliter les cas d’utilisation de contrôle de version
* Création de dossiers liés à [!DNL Experience Manager Assets]
* Suivi des métadonnées pour les ressources et les dossiers
* Synchronisation des métadonnées de projet entre [!DNL Workfront] et [!DNL Experience Manager Assets]

>[!NOTE]
>
>Vous pouvez également connecter plusieurs [!DNL Experience Manager Assets] référentiels sur un [!UICONTROL Workfront] ou plusieurs [!DNL Workfront] environnements à un [!DNL Experience Manager Assets] référentiel dans les ID d’organisation. Suivez les instructions de configuration de cet article pour chaque intégration que vous souhaitez configurer.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td>Quelconque
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licences</strong>
   </td>
   <td>Actuel : formule [!UICONTROL] <br>
   Nouveau : [!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] license</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td>Vous devez avoir [!DNL Experience Manager Assets as a Cloud Service], et vous devez être ajouté au produit en tant qu’utilisateur.
   </td>
  </tr>
  <tr>
   <td>Paramétrages du niveau d'accès*
   </td>
   <td>Vous devez être un [!DNL Workfront] administrateur.
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Conditions préalables

Avant de commencer,

* Vous devez avoir [!DNL Workfront] et [!DNL Adobe Experience Manager Assets] associé à un ID d’organisation dans la variable [!DNL Adobe Admin Console]. Pour plus d’informations, voir [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configuration des informations d’intégration

{{step-1-to-setup}}

1. Sélectionner **[!UICONTROL Documents]** dans le panneau de gauche, puis sélectionnez **[!UICONTROL [!DNL Experience Manager]Intégration]**.

   >[!NOTE]
   >
   >Cette zone de configuration s’affiche uniquement si votre [!DNL Workfront] est inclus sous un [!DNL Adobe Admin Console].

1. Sélectionner **[!UICONTROL Ajouter [!DNL Experience Manager] Intégration]**.
1. Dans le **[!UICONTROL Nom]** , saisissez le nom que les utilisateurs doivent voir lorsqu’ils interagissent avec cette intégration dans Workfront et Experience Manager Assets.
1. Dans le **[!UICONTROL URL de navigation]** , le système renseigne automatiquement l’URL de navigation. Cette URL en lecture seule est utilisée pour créer un lien vers le [!DNL Experience Manager] de l’instance [!UICONTROL Menu Principal] pour un accès rapide.
1. Sélectionnez un référentiel dans la **[!UICONTROL [!DNL Experience Manager]Référentiel de ressources]** menu déroulant. Le système renseigne automatiquement les variables [!DNL Experience Manager] référentiels associés à l’ID d’organisation auquel votre profil utilisateur est affecté.
   ![choix du référentiel experience manager](assets/setup-information.png)

1. Cliquez sur **[!UICONTROL Enregistrer]** ou passez à la [Configuration des métadonnées (facultatif)](#set-up-metadata-optional) dans cet article.

   >[!NOTE]
   >
   >En raison de la complexité de l’intégration, vous ne pouvez pas modifier le référentiel après avoir enregistré la configuration initiale.

## Configuration des métadonnées (facultatif)

Vous pouvez mapper [!DNL Workfront] données d’objet aux champs de média de ressources dans [!DNL Experience Manager] Ressources.

>[!IMPORTANT]
>
>Vous ne pouvez mapper les métadonnées que dans une seule direction : à partir de [!DNL Workfront] to [!DNL Experience Manager]. Métadonnées pour les documents liés à [!DNL Workfront] de [!DNL Experience Manager] ne peut pas être transféré vers [!DNL Workfront].

### Configuration des champs de métadonnées

Avant de commencer à mapper les champs de métadonnées, vous devez configurer les champs de métadonnées dans Workfront et Experience Manager Assets.

Pour configurer les champs de métadonnées :

1. Configurer un schéma de métadonnées dans [!DNL Experience Manager Assets] comme expliqué dans [Configuration du mappage des métadonnées de ressource entre les Adobes [!DNL Workfront] et [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Configurez les champs de formulaire personnalisés dans Workfront. [!DNL Workfront] comporte de nombreux champs personnalisés intégrés que vous pouvez utiliser. Cependant, vous pouvez également créer vos propres champs personnalisés, en suivant la procédure décrite à la section [Création ou modification d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Développer pour afficher plus d’informations sur les champs Workfront et Experience Manager Assets pris en charge**

**Balises Experience Manager Assets**

Vous pouvez mapper n’importe quel champ pris en charge par Workfront à une balise dans Experience Manager Assets. Pour ce faire, vous devez vous assurer que les valeurs de balise dans Experience Manager Assets correspondent à Workfront.

* Les balises et les valeurs de champ Workfront doivent correspondre exactement à l’orthographe et au format.
* Les valeurs de champ Workfront mappées aux balises de ressources Experience Manager doivent être toutes en minuscules, même si la balise dans Experience Manager Assets semble comporter des lettres majuscules.
* Les valeurs de champ Workfront ne doivent pas inclure d’espaces.
* La valeur de champ dans Workfront doit également inclure la structure de dossiers de la balise Experience Manager Assets.
* Pour mapper plusieurs champs de texte d’une seule ligne à des balises, saisissez une liste séparée par des virgules des valeurs de balise dans le côté Workfront du mappage de métadonnées, et `xcm:keywords` côté Experience Manager Assets. Chaque valeur de champ correspond à une balise distincte. Vous pouvez utiliser un champ calculé pour combiner plusieurs champs Workfront en un seul champ de texte séparé par des virgules.
* Vous pouvez mapper des valeurs à partir de champs de liste déroulante, de bouton radio ou de case à cocher en saisissant une liste des valeurs disponibles dans ce champ, séparées par des virgules.


>[!INFO]
>
>**Exemple**: pour correspondre à la balise affichée dans la structure de dossiers ici, la valeur de champ dans Workfront est `landscapes:trees/spruce`. Notez les minuscules dans la valeur du champ Workfront.
>
>Si vous souhaitez que la balise soit située le plus à gauche dans l’arborescence des balises, elle doit être suivie d’un signe deux-points. Dans cet exemple, pour mapper la balise paysage, la valeur de champ dans Workfront est `landscapes:`.
>
>![Structure de dossiers dans AEM](assets/aem-folder-structure-with-red-boxes.png)


Une fois les balises créées dans Experience Manager Assets, elles s’affichent dans la liste déroulante Balises de la section Métadonnées . Pour lier un champ à une balise, sélectionnez `xcm:keywords` dans la liste déroulante du champ Experience Manager Assets de la zone de mappage des métadonnées.

Pour plus d’informations sur les balises dans Experience Manager Assets, notamment sur la création et la gestion des balises, voir [Administration des balises](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Champs de schéma de métadonnées personnalisés Experience Manager Assets**

Vous pouvez mapper des champs Workfront intégrés et personnalisés à des champs de schéma de métadonnées personnalisés dans Experience Manager Assets.

Les champs de métadonnées personnalisés créés dans Experience Manager Assets sont organisés dans leur propre section dans la zone de configuration des métadonnées.

![section de métadonnées personnalisées](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Champs Workfront**

Vous pouvez mapper des champs Workfront intégrés et personnalisés à Experience Manager Assets. Les valeurs de champ suivantes doivent correspondre dans les deux cas et dans l’orthographe entre Workfront et Experience Manager Assets :

* Champs de liste déroulante
* Champs à sélection multiple

>[!TIP]
>
> Pour vérifier si les valeurs de champ correspondent exactement, accédez à
>
> * Configuration > Forms personnalisée dans Workfront ou le champ dans l’objet
> * Ressources > schémas de métadonnées dans Experience Manager Assets

+++

### Mappage des métadonnées des ressources

Mappages de métadonnées lorsqu’une ressource est transférée à partir de [!DNL Workfront] pour la première fois. Les documents contenant des champs intégrés ou personnalisés sont automatiquement associés aux champs spécifiés lors de la première envoi d’une ressource à [!DNL Experience Manager Assets].

Pour mapper les métadonnées des ressources :

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Dans le **[!UICONTROL [!DNL Workfront]field]** , choisissez un champ Workfront intégré ou personnalisé.

   >[!NOTE]
   >
   >Vous pouvez mapper une seule [!DNL Workfront] champ à plusieurs [!UICONTROL Experience Manager Assets] des champs. Vous ne pouvez pas mapper plusieurs [!DNL Workfront] à un seul champ [!DNL Experience Manager Assets] champ .
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Dans le [!DNL Experience Manager Assets] , recherchez dans les catégories prérenseignées ou saisissez au moins deux lettres dans le champ de recherche pour accéder à d’autres catégories.
1. Répétez les étapes 2 et 3 si nécessaire.
   ![Champs de métadonnées](assets/metadata-no-asset-toggle.png)
1. Cliquez sur [!UICONTROL Enregistrer] ou passez à la [Configuration des workflows](#set-up-workflows-optional) dans cet article.

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## Configuration des workflows (facultatif)

Un workflow est un ensemble d’actions qui connectent Workfront à Adobe Experience Manager as a Cloud Service. En tant qu’administrateur Workfront, vous pouvez configurer des workflows dans Workfront, puis les affecter à des modèles de projet. Lorsqu’un projet est créé à l’aide d’un modèle de projet auquel un workflow est affecté, les actions définies dans le workflow sont déclenchées.

Les workflows sont activés et configurés pour Adobe Experience Manager dans son ensemble. Ces workflows peuvent ensuite être appliqués aux modèles de projet et ajustés ou personnalisés au niveau du modèle ou du projet.

Les workflows suivants sont disponibles dans l’intégration Adobe Experience Manager :

* [Création de dossiers liés à Adobe Experience Manager](#create-adobe-experience-manager-linked-folders)
* [Publication de ressources envoyées à Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Création de dossiers liés à Adobe Experience Manager

1. Activez/désactivez la variable **[!UICONTROL Créer un dossier lié]** sur .
1. Saisissez le nom du dossier lié que vous créez.
1. (Conditionnel) Activez l’option **Arborescence de dossiers par défaut** si vous souhaitez que ce dossier lié soit le dossier par défaut des projets créés avec des modèles qui utilisent cette intégration. Vous pouvez sélectionner un ou plusieurs dossiers par défaut.
1. Sélectionnez un chemin d’accès au dossier pour indiquer où vous souhaitez tous les dossiers liés associés à cette intégration.
1. (Conditionnel) Pour ajouter une arborescence de dossiers (dossiers imbriqués) à cette intégration, procédez comme suit :

   1. Cliquez sur le bouton **Ajouter un dossier** icon ![Ajouter un dossier](assets/add-folder-aem.png).
   1. Dans le **Type de nom** , sélectionnez le nom du dossier :

      * **Nom**: saisissez un nom pour le dossier.
      * **Données d’objet**: sélectionnez la source du nom du dossier, par exemple Nom du projet.

      >[!NOTE]
      >
      >* Les noms de dossier doivent comporter moins de 100 caractères.
      >* Les caractères suivants seront supprimés des noms des dossiers :
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Pour ajouter un dossier imbriqué à l’arborescence de dossiers, cliquez sur le menu à trois points en regard du dossier dans lequel vous souhaitez créer un dossier imbriqué, puis sélectionnez **Ajouter un dossier**. Renseignez les champs comme décrit à l’étape précédente.
   1. Pour lier un dossier à Workfront, sélectionnez-le et cliquez sur le bouton **Rendre le dossier lié**   icon ![Lier le dossier](assets/link-folder.png).
   1. (Facultatif) Pour modifier un dossier, sélectionnez-le, puis cliquez sur le bouton **Modifier le dossier** icon ![Icône Modifier](assets/edit-icon.png).
   1. (Facultatif) Pour supprimer un dossier, sélectionnez-le et cliquez sur le bouton **Supprimer le dossier** icon ![Supprimer le dossier](assets/delete-folder.png).
1. (Conditionnel) Pour ajouter une autre arborescence de dossiers, cliquez sur **+ Ajouter une arborescence de dossiers** et suivez les étapes de l’étape 5.

1. Cliquez sur **[!UICONTROL Enregistrer]** ou passez à la [Publication de ressources envoyées à Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) dans cet article.

>[!NOTE]
>
>* Cette intégration ne créera pas plus de 100 dossiers, quel que soit le nombre d’arborescences de dossiers créées. Par exemple, une intégration avec 4 arborescences de dossiers peut créer jusqu’à 100 dossiers, et non pas 400 dossiers.
>* Le premier dossier de l’arborescence de dossiers est automatiquement marqué comme lié à Workfront. Si vous ne souhaitez pas que ce dossier soit lié, vous pouvez le dissocier.
>* Si aucune arborescence de dossiers n’est fournie, le dossier racine devient le dossier lié.


### Publication de ressources envoyées à Adobe Experience Manager Assets

1. Activation **[!UICONTROL Publier automatiquement les ressources]**.
1. Cochez la case en regard de l’emplacement où vous souhaitez publier les ressources envoyées aux ressources Adobe Experience Manager. Vous pouvez activer l’une des options ou les deux.
1. (Conditionnel) Si vous avez activé l’option Brand Portal, sélectionnez le Brand Portal dans lequel vous souhaitez publier des ressources.
1. Cliquez sur **[!UICONTROL Enregistrer]** ou passez à la [Configuration des dossiers liés (facultatif)](#set-up-linked-folders-optional) dans cet article.

## Configuration des dossiers liés (facultatif)

Vous pouvez permettre aux utilisateurs de créer des dossiers liés à [!DNL Experience Manager] pendant un événement [!DNL Workfront] projet. Lorsqu’un dossier est lié, toute ressource ajoutée au dossier apparaît automatiquement dans les deux [!DNL Workfront] et [!DNL Experience Manager]. Lorsqu’une ressource est ajoutée au dossier lié dans [!DNL Workfront] pour la première fois, les métadonnées de la ressource sont transmises à [!DNL Experience Manager Assets].

Dans les étapes ci-dessous, vous indiquez où vous souhaitez créer les dossiers liés. Chaque intégration ne peut avoir qu’un seul emplacement pour tous les dossiers liés.

Pour configurer les dossiers liés :

1. Activez/désactivez la variable **[!UICONTROL Activer le dossier lié]** sur .
1. Sélectionnez un chemin d’accès au dossier pour indiquer où vous souhaitez tous les dossiers liés associés à cette intégration.

   >[!NOTE]
   >
   >Les utilisateurs doivent avoir un accès en écriture dans [!DNL Adobe Experience Manager Assets] au dossier spécifié pour créer un dossier lié.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
