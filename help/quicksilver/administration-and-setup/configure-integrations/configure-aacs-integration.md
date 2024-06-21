---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurer l’intégration d’[!UICONTROL Experience Manager Assets as a Cloud Service]
description: Vous pouvez connecter votre travail à votre contenu dans  [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1678'
ht-degree: 99%

---

# Configurer l’intégration d’[!UICONTROL Experience Manager Assets as a Cloud Service]

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les entreprises qui ont été intégrées à [!DNL Adobe Admin Console].

Vous pouvez connecter votre travail à votre contenu dans [!DNL Experience Manager Assets] :

* Envoyer des ressources et des métadonnées d’[!DNL Adobe Workfront] à [!DNL Experience Manager Assets]
* Lier des ressources d’[!DNL Experience Manager Assets] à vos projets et tâches dans [!DNL Workfront&#x200B;]
* Faciliter les cas d’utilisation de contrôle de version
* Créer des dossiers liés à [!DNL Experience Manager Assets]
* Suivre les métadonnées des ressources et des dossiers
* Synchroniser les métadonnées de projet entre [!DNL Workfront] et [!DNL Experience Manager Assets]

>[!NOTE]
>
>Vous pouvez également connecter plusieurs référentiels [!DNL Experience Manager Assets] entre un environnement [!UICONTROL Workfront] ou plusieurs environnements [!DNL Workfront] et un référentiel [!DNL Experience Manager Assets] dans les ID d’entreprise. Suivez les instructions de configuration de cet article pour chaque intégration que vous souhaitez configurer.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Plan <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td>N’importe quelle
   </td>
  </tr>
  <tr>
   <td>Licences <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td>Actuel : [!UICONTROL Plan] <br>
 Nouveau : [!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>Licence <strong>[!DNL Experience Manager]</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td>Vous devez avoir [!DNL Experience Manager Assets as a Cloud Service], et vous devez être ajouté au produit en tant qu’utilisateur ou utilisatrice.
   </td>
  </tr>
  <tr>
   <td>Configurations des niveau d’accès*
   </td>
   <td>Vous devez être un administrateur ou une administratrice de [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Conditions préalables

Avant de commencer

* Vous devez avoir [!DNL Workfront] et [!DNL Adobe Experience Manager Assets] associés à un ID d’entreprise dans [!DNL Adobe Admin Console]. Pour plus d’informations, voir [Différences d’administration en fonction de la plateforme ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configurer les informations d’intégration

{{step-1-to-setup}}

1. Sélectionnez **[!UICONTROL Documents]** dans le panneau de gauche, puis Intégration d’**[!UICONTROL [!DNL Experience Manager]]**.

   >[!NOTE]
   >
   >Cette zone de configuration ne s’affiche si votre environnement [!DNL Workfront] est inclus sous [!DNL Adobe Admin Console].

1. Sélectionnez **[!UICONTROL Ajouter une intégration d’[!DNL Experience Manager]]**.
1. Dans le champ **[!UICONTROL Nom]**, saisissez le nom que les utilisateurs et utilisatrices doivent voir lorsqu’ils ou elles interagissent avec cette intégration dans Workfront et Experience Manager Assets.
1. Dans le champ **[!UICONTROL URL de navigation]**, le système renseigne automatiquement l’URL de navigation. Cette URL en lecture seule est utilisée pour créer un lien vers l’instance [!DNL Experience Manager] de votre entreprise depuis le [!UICONTROL Menu principal] pour un accès rapide.
1. Choisissez un référentiel dans le menu déroulant Référentiel **[!UICONTROL [!DNL Experience Manager] Assets]**. Le système renseigne automatiquement les référentiels [!DNL Experience Manager] associés à l’ID d’entreprise auquel votre profil utilisateur ou utilisatrice est affecté.
   ![choix du référentiel experience manager](assets/setup-information.png)

1. Cliquez sur **[!UICONTROL Enregistrer]** ou passez à la section [Configurer les métadonnées (facultatif)](#set-up-metadata-optional) de cet article.

   >[!NOTE]
   >
   >En raison de la complexité de l’intégration, vous ne pouvez pas modifier le référentiel après avoir enregistré la configuration initiale.

## Configurer les métadonnées (facultatif)

Vous pouvez mapper des données d’objet [!DNL Workfront] sur les champs des médias de ressources dans [!DNL Experience Manager] Assets.

>[!IMPORTANT]
>
>Vous ne pouvez mapper les métadonnées que dans une seule direction : de [!DNL Workfront] vers [!DNL Experience Manager]. Les métadonnées de documents liés à [!DNL Workfront] à partir d’[!DNL Experience Manager] ne peuvent pas être transférées vers [!DNL Workfront].

### Configurer les champs de métadonnées

Avant de commencer à mapper des champs de métadonnées, vous devez configurer les champs de métadonnées dans Workfront et Experience Manager Assets.

Pour configurer les champs de métadonnées :

1. Configurer un schéma de métadonnées dans [!DNL Experience Manager Assets] comme expliqué dans [Configurer le mappage des métadonnées de ressource entre Adobe  [!DNL Workfront]  et  [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=fr).


1. Configurez les champs de formulaire personnalisés dans Workfront. [!DNL Workfront] comporte de nombreux champs personnalisés intégrés que vous pouvez utiliser. Cependant, vous pouvez également créer vos propres champs personnalisés, en suivant la procédure décrite à la section [Créer ou modifier un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Développer pour afficher plus d’informations sur les champs Workfront et Experience Manager Assets pris en charge**

**Balises Experience Manager Assets**

Vous pouvez mapper n’importe quel champ pris en charge par Workfront à une balise dans Experience Manager Assets. Pour ce faire, vous devez vous assurer que les valeurs de balise dans Experience Manager Assets correspondent à Workfront.

* Les balises et les valeurs de champ Workfront doivent correspondre exactement en termes d’orthographe et de format.
* Les valeurs de champ Workfront mappées aux balises Experience Manager Assets doivent être toutes en minuscules, même si la balise dans Experience Manager Assets semble comporter des lettres majuscules.
* Les valeurs de champ Workfront ne doivent pas inclure d’espaces.
* La valeur de champ dans Workfront doit également inclure la structure de dossiers de la balise Experience Manager Assets.
* Pour mapper plusieurs champs de texte d’une seule ligne à des balises, saisissez les valeurs de balise sous forme de liste séparée par des virgules dans la partie Workfront du mappage de métadonnées, et `xcm:keywords` dans la partie Experience Manager Assets. Chaque valeur de champ est mappée à une balise distincte. Vous pouvez utiliser un champ calculé pour combiner plusieurs champs Workfront en un seul champ de texte séparé par des virgules.
* Vous pouvez mapper des valeurs à partir de champs de liste déroulante, de bouton radio ou de case à cocher en saisissant une liste des valeurs disponibles séparées par des virgules dans ce champ.


>[!INFO]
>
>**Exemple** : pour correspondre à la balise affichée dans la structure de dossiers ici, la valeur de champ dans Workfront doit être `landscapes:trees/spruce`. Notez les minuscules dans la valeur du champ Workfront.
>
>Si vous souhaitez que la balise soit située le plus à gauche dans l’arborescence des balises, elle doit être suivie d’un signe deux-points. Dans cet exemple, pour mapper la balise paysages, la valeur de champ dans Workfront est `landscapes:`.
>
>![Structure de dossiers dans AEM](assets/aem-folder-structure-with-red-boxes.png)


Une fois les balises créées dans Experience Manager Assets, elles s’affichent dans la liste déroulante Balises de la section Métadonnées. Pour lier un champ à une balise, sélectionnez `xcm:keywords` dans la liste déroulante du champ Experience Manager Assets de la zone de mappage des métadonnées.

Pour plus d’informations sur les balises dans Experience Manager Assets, notamment sur la création et la gestion des balises, voir [Administration des balises](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=fr).

**Champs de schéma de métadonnées personnalisés Experience Manager Assets**

Vous pouvez mapper des champs Workfront intégrés et personnalisés à des champs de schéma de métadonnées personnalisés dans Experience Manager Assets.

Les champs de métadonnées personnalisés créés dans Experience Manager Assets sont organisés dans leur propre section dans la zone de configuration des métadonnées.

![section des métadonnées personnalisées](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Champs Workfront**

Vous pouvez mapper des champs Workfront intégrés et personnalisés à Experience Manager Assets. Les valeurs de champ suivantes doivent correspondre, tant en terme de capitalisation que d’orthographe, entre Workfront et Experience Manager Assets :

* Champs de liste déroulante
* Champs à sélection multiple

>[!TIP]
>
> Pour vérifier si les valeurs de champ correspondent exactement, accédez à
>
> * Configuration > Formulaires personnalisée dans Workfront ou le champ dans l’objet
> * Ressources > Schémas de métadonnées dans Experience Manager Assets

+++

### Mapper les métadonnées des ressources

Les métadonnées sont mappées lorsqu’une ressource est transférée à partir de [!DNL Workfront] pour la première fois. Les documents contenant des champs intégrés ou personnalisés sont automatiquement mappés aux champs spécifiés lors de la première envoi d’une ressource à [!DNL Experience Manager Assets].

Pour mapper les métadonnées des ressources :

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Dans la colonne **[!UICONTROL [!DNL Workfront]Champ]**, choisissez un champ Workfront intégré ou personnalisé.

   >[!NOTE]
   >
   >Vous pouvez mapper un seul champ [!DNL Workfront] à plusieurs champs [!UICONTROL Experience Manager Assets]. Vous ne pouvez pas mapper plusieurs champs [!DNL Workfront] à un seul champ [!DNL Experience Manager Assets].
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Dans le champ [!DNL Experience Manager Assets], recherchez dans les catégories prérenseignées ou saisissez au moins deux lettres dans le champ de recherche pour accéder à d’autres catégories.
1. Répétez les étapes 2 et 3 si nécessaire.
   ![Champs de métadonnées](assets/metadata-no-asset-toggle.png)
1. Cliquez sur [!UICONTROL Enregistrer] ou passez à la section [Configurer les workflows](#set-up-workflows-optional) dans cet article.

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

## Configurer les workflows (facultatif)

Un workflow est un ensemble d’actions qui connectent Workfront à Adobe Experience Manager as a Cloud Service. En tant qu’administrateur ou administratrice Workfront, vous pouvez configurer des workflows dans Workfront, puis les attribuer à des modèles de projet. Lorsqu’un projet est créé à l’aide d’un modèle de projet auquel un workflow est attribué, les actions définies dans le workflow sont déclenchées.

Les workflows sont activés et configurés pour Adobe Experience Manager dans son ensemble. Ces workflows peuvent ensuite être appliqués aux modèles de projet et ajustés ou personnalisés au niveau du modèle ou du projet.

Les workflows suivants sont disponibles dans l’intégration Adobe Experience Manager :

* [Créer des dossiers liés Adobe Experience Manager](#create-adobe-experience-manager-linked-folders)
* [Publier des ressources envoyées à Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Créer des dossiers liés Adobe Experience Manager

1. Activez **[!UICONTROL Créer un dossier lié]**.
1. Saisissez le nom du dossier lié que vous créez.
1. (Le cas échéant) Activez l’option **Arborescence de dossiers par défaut** si vous souhaitez que ce dossier lié soit le dossier par défaut des projets créés avec des modèles qui utilisent cette intégration. Vous pouvez sélectionner un ou plusieurs dossiers par défaut.
1. Sélectionnez un chemin d’accès au dossier pour indiquer l’emplacement de tous les dossiers liés associés à cette intégration.
1. (Le cas échéant) Pour ajouter une arborescence de dossiers (dossiers imbriqués) à cette intégration, procédez comme suit :

   1. Cliquez sur l’icône **Ajouter un dossier** ![Add folder](assets/add-folder-aem.png).
   1. Dans le champ **Type de nom**, sélectionnez le nom du dossier :

      * **Nom** : saisissez un nom pour le dossier.
      * **Données d’objet** : sélectionnez la source du nom du dossier, par exemple Nom du projet.

      >[!NOTE]
      >
      >* Les noms de dossier doivent comporter moins de 100 caractères.
      >* Les caractères suivants seront supprimés des noms des dossiers :
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Pour ajouter un dossier imbriqué à l’arborescence de dossiers, cliquez sur le menu à trois points en regard du dossier dans lequel vous souhaitez créer un dossier imbriqué, puis sélectionnez **Ajouter un dossier**. Renseignez les champs comme décrit à l’étape précédente.
   1. Pour lier un dossier à Workfront, sélectionnez-le et cliquez sur l’icône **Créer un dossier lié** ![Link folder](assets/link-folder.png).
   1. (Facultatif) Pour modifier un dossier, sélectionnez-le, puis cliquez sur l’icône **Modifier le dossier** ![Edit icon](assets/edit-icon.png).
   1. (Facultatif) Pour supprimer un dossier, sélectionnez-le et cliquez sur l’icône **Supprimer le dossier** ![Delete folder](assets/delete-folder.png).
1. (Le cas échéant) Pour ajouter une autre arborescence de dossiers, cliquez sur **+ Ajouter une arborescence de dossiers** et suivez les étapes de l’étape 5.

1. Cliquez sur **[!UICONTROL Enregistrer]**, ou passez à la section [Publier des ressources envoyées à Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) dans cet article.

>[!NOTE]
>
>* Cette intégration ne créera pas plus de 100 dossiers, quel que soit le nombre d’arborescences de dossiers créées. Par exemple, une intégration avec 4 arborescences de dossiers peut créer jusqu’à 100 dossiers, et non pas 400 dossiers.
>* Le premier dossier de l’arborescence de dossiers est automatiquement marqué comme lié à Workfront. Si vous ne souhaitez pas que ce dossier soit lié, vous pouvez le dissocier.
>* Si aucune arborescence de dossiers n’est fournie, le dossier racine devient le dossier lié.


### Publier des ressources envoyées à Adobe Experience Manager Assets

1. Activez **[!UICONTROL Publier automatiquement les ressources]**.
1. Cochez la case en regard de l’emplacement où vous souhaitez publier les ressources envoyées aux ressources Adobe Experience Manager. Vous pouvez activer l’une des options ou les deux.
1. (Le cas échéant) Si vous avez activé l’option Brand Portal, sélectionnez le Brand Portal dans lequel vous souhaitez publier des ressources.
1. Cliquez sur **[!UICONTROL Enregistrer]** ou passez à la section [Configurer des dossiers liés (facultatif)](#set-up-linked-folders-optional) dans cet article.

## Configurer des dossiers liés (facultatif)

Vous pouvez autoriser les utilisateurs et utilisatrices à créer des dossiers liés à [!DNL Experience Manager] dans un projet [!DNL Workfront]. Lorsqu’un dossier est lié, toute ressource ajoutée au dossier apparaît automatiquement dans [!DNL Workfront] et [!DNL Experience Manager]. Lorsqu’une ressource est ajoutée au dossier lié dans [!DNL Workfront] pour la première fois, les métadonnées de la ressource sont transmises à [!DNL Experience Manager Assets].

Dans les étapes ci-dessous, vous indiquez où vous souhaitez créer les dossiers liés. Chaque intégration ne peut avoir qu’un seul emplacement pour tous les dossiers liés.

Pour configurer les dossiers liés :

1. Activez **[!UICONTROL Activer le dossier lié]**.
1. Sélectionnez un chemin d’accès au dossier pour indiquer l’emplacement de tous les dossiers liés associés à cette intégration.

   >[!NOTE]
   >
   >Les utilisateurs et utilisatrices doivent avoir un accès en écriture dans [!DNL Adobe Experience Manager Assets] au dossier spécifié pour créer un dossier lié.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
