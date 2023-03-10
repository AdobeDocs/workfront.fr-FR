---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Intégrations Adobe Experience Manager Assets
description: Vous pouvez connecter votre travail avec les intégrations Adobe Experience Manager Assets suivantes.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 0%

---

# Configurez la variable [!UICONTROL Experience Manager Assets as a Cloud Service] integration

Vous pouvez connecter votre travail à votre contenu dans [!DNL Experience Manager Assets]&#x200B; :

* Push sur les ressources et les métadonnées à partir de [!DNL Adobe Workfront] to [!DNL Experience Manager Assets]&#x200B;
* Lier des ressources depuis [!DNL Experience Manager Assets] à vos projets et tâches dans [!DNL Workfront&#x200B;]
* Faciliter les cas d’utilisation de contrôle de version
* Création de dossiers liés à [!DNL Experience Manager Assets]
* Suivi des métadonnées pour les ressources et les dossiers
* Synchronisation des métadonnées de projet entre [!DNL Workfront] et [!DNL Experience Manager Assets]


## Exigences d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan*</strong>
   </td>
   <td>Tous
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licences*</strong>
   </td>
   <td>[!UICONTROL Plan]
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
   <td>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <strong>Octroi d’un accès administratif complet à un utilisateur</strong>.
   </td>
  </tr>
</table>


*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.


## Conditions préalables

Avant de commencer,

* Vous devez avoir [!DNL Workfront] et [!DNL Adobe Experience Manager Assets] associé à un ID d’organisation dans la variable [!DNL Adobe Admin Consol]e. Pour plus d’informations, voir [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configuration des informations d’intégration

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Configuration]** .
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
>Vous ne pouvez mapper les métadonnées que dans une seule direction : de [!DNL Workfront] to [!DNL Experience Manager]. Métadonnées pour les documents liés à [!DNL Workfront] de [!DNL Experience Manager] ne peut pas être transféré vers [!DNL Workfront].



### Configuration des champs de métadonnées

1. Configuration d’un schéma de métadonnées dans [!DNL Experience Manager Assets] comme expliqué dans [Configuration du mappage des métadonnées de ressource entre les Adobes [!DNL Workfront] et [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. Configurez les champs de formulaire personnalisés dans Workfront. [!DNL Workfront] comporte de nombreux champs personnalisés intégrés que vous pouvez utiliser. Cependant, vous pouvez également créer vos propres champs personnalisés, comme expliqué dans la section [Création ou modification d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Ressources

Mappages des métadonnées lorsqu’une ressource est transférée à partir de [!DNL Workfront] pour la première fois. Les documents contenant des champs intégrés ou personnalisés sont automatiquement associés aux champs spécifiés lors de la première envoi d’une ressource à [!DNL Experience Manager Assets].

>[!NOTE]
>
>Cette intégration ne prend pas en charge les métadonnées personnalisées de [!DNL Adobe Experience Manager].

Pour mapper les métadonnées des ressources :

1. Sélectionner **[!UICONTROL Ressources]** au-dessus du tableau de métadonnées.
1. Dans le **[!UICONTROL [!DNL Workfront]field]** , choisissez un champ Workfront intégré ou personnalisé.

   >[!NOTE]
   >
   >Vous pouvez mapper une seule [!DNL Workfront] champ à plusieurs [!UICONTROL Experience Manager Assets] champs. Vous ne pouvez pas mapper plusieurs [!DNL Workfront] à un seul champ [!DNL Experience Manager Assets] champ .

1. Dans le [!DNL Experience Manager Assets] , recherchez dans les catégories prérenseignées ou saisissez au moins deux lettres dans le champ de recherche pour accéder à d’autres catégories.
1. Répétez les étapes 2 et 3 si nécessaire.
   ![Champs de métadonnées](assets/asset-metadata.png)
1. Cliquez sur [!UICONTROL Enregistrer] ou passez à la [Dossiers](#folders) dans cet article.

### Dossiers

Lorsque les utilisateurs créent un dossier lié sur un projet, les données de projet, de portfolio et de programme associées sont mappées aux champs de métadonnées de dossier dans [!DNL Experience Manager Assets].

>[!NOTE]
>
>Cette intégration ne prend pas en charge les métadonnées personnalisées de [!DNL Adobe Experience Manager].

Pour mapper les métadonnées des dossiers :

1. Sélectionner **[!UICONTROL Dossiers]** au-dessus du tableau de métadonnées.
1. Dans le **[!UICONTROL [!DNL Workfront]field]** , choisissez un champ Workfront intégré ou personnalisé.

   >[!NOTE]
   >
   >Vous pouvez mapper un champ Workfront unique à plusieurs champs Experience Manager Assets. Vous ne pouvez pas mapper plusieurs [!DNL Workfront] à un seul champ [!DNL Experience Manager Assets] champ .

1. Dans le **[!DNL Experience Manager Assets]** , recherchez dans les catégories prérenseignées ou saisissez au moins deux lettres dans le champ de recherche pour accéder à d’autres catégories.
1. Répétez les étapes 2 et 3 si nécessaire.
   ![métadonnées de dossier](assets/folder-metadata.png)
1. Cliquez sur **[!UICONTROL Enregistrer]** ou passez à la [Synchronisation des métadonnées du projet](#project-metadata-sync) dans cet article.


### Synchronisation des métadonnées d’objet

Un [!DNL Experience Manager] champs mappés à [!DNL Workfront] les champs de portefeuille, de programme, de projet, de tâche, d’émission et de document sont automatiquement mis à jour lorsque le champ est modifié dans [!DNL Workfront].

>[!IMPORTANT]
>
>Les utilisateurs doivent disposer d’un accès en écriture dans [!DNL Experience Manager] pour les ressources vivant dans l’objet afin que les métadonnées soient synchronisées lors de leur mise à jour.

1. Activez la variable **[!UICONTROL Métadonnées d’objet de synchronisation]** champ .
1. Cliquez sur Enregistrer ou passez à la [Configuration des dossiers liés (facultatif)](#set-up-linked-folders-optional) dans cet article.

## Configuration des dossiers liés (facultatif)

Vous pouvez permettre aux utilisateurs de créer des dossiers liés à [!DNL Experience Manager] pendant un événement [!DNL Workfront] projet. Lorsqu’un dossier est lié, toute ressource ajoutée au dossier s’affiche automatiquement dans les deux [!DNL Workfront] et [!DNL Experience Manager]. Lorsqu’une ressource est ajoutée au dossier lié dans [!DNL Workfront] pour la première fois, les métadonnées de la ressource sont transmises à [!DNL Experience Manager Assets].

Dans les étapes ci-dessous, vous indiquez où vous souhaitez créer les dossiers liés. Chaque intégration ne peut avoir qu’un seul emplacement pour tous les dossiers liés.

Pour configurer les dossiers liés :

1. Activez/désactivez la variable **[!UICONTROL Activer le dossier lié]** sur .
1. Sélectionnez un chemin d’accès au dossier pour indiquer où vous souhaitez tous les dossiers liés associés à cette intégration.

   >[!NOTE]
   >
   >Les utilisateurs doivent disposer d’un accès en écriture dans [!DNL Adobe Experience Manager Assets] au dossier spécifié pour créer un dossier lié.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
