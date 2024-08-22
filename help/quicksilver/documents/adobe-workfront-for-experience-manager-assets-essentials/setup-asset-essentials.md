---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configuration de l’intégration Experience Manager Assets Essentials
description: Connectez votre travail à votre contenu dans Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 17%

---

# Configurer l’intégration d’Experience Manager Assets Essentials

Connectez votre travail à votre contenu dans Experience Manager Assets Essentials &#x200B; :

* Push assets and metadata from Adobe Workfront to Experience Manager Assets Essentials &#x200B;
* Lier des ressources de Experience Manager Assets Essentials à vos projets et tâches dans Workfront &#x200B;
* Faciliter les workflows de contrôle de version pour les ressources transférées vers Experience Manager Assets Essentials

>[!NOTE]
>
>Vous pouvez également connecter plusieurs référentiels Experience Manager Assets à un environnement Workfront ou plusieurs environnements Workfront à un référentiel Experience Manager Assets à l’échelle des ID d’organisation. Suivez les instructions de configuration de cet article pour chaque intégration que vous souhaitez configurer.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plan
   </td>
   <td>N’importe quelle
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licence
   </td>
   <td><p>Actuelle : [!UICONTROL Plan]</p>
   <p>Nouvelle : [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] licence
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>Produit
   </td>
   <td>Vous devez disposer de Experience Manager Assets Essentials et vous devez être ajouté au produit en tant qu’utilisateur dans l’Admin Console.
   </td>
  </tr>
  <tr>
   <td>Configurations du niveau d’accès
   </td>
   <td>Vous devez être un administrateur ou une administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuration de l’intégration

{{step-1-to-setup}}

1. Sélectionnez **Documents** ![icône de documents](assets/document-icon.png) dans le panneau de gauche, puis sélectionnez **Intégration Experience Manager**.
1. Sélectionnez **Ajouter une intégration Experience Manager**.
1. Indiquez les informations suivantes :

   <table>
   <tr>
      <td><strong>Nom</strong>
      </td>
      <td>Saisissez le nom que vous souhaitez voir apparaître dans le bouton Ajouter un nouveau document de la zone Documents.
      </td>
   </tr>
   <tr>
      <td><strong>URL de navigation</strong>
      </td>
      <td>Le système renseigne automatiquement l’URL de navigation. Cette URL est utilisée pour créer un lien vers l’instance Assets Essentials de votre entreprise à partir du menu principal afin d’y accéder rapidement.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Référentiel Experience Manager Assets</strong>
      </td>
      <td>
      Le système renseigne automatiquement le référentiel Experience Manager associé à votre ID d’organisation.
      </td>
   </tr>
   </table>

1. Cliquez sur **Enregistrer** ou passez à la section [Configurer des métadonnées (facultatif)](#set-up-metadata-optional) de cet article.


## Configuration des métadonnées (facultatif)

Mappage des données d’objet Workfront aux champs de médias de ressources dans Experience Manager Assets. Les métadonnées sont mises en correspondance lorsqu’une ressource est envoyée de Workfront pour la première fois.


### Conditions préalables

Avant de commencer, vous devez

* Configurez un schéma de métadonnées dans Experience Manager Assets Essentials, comme expliqué dans la section [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=fr).
* (Facultatif) Configurez les champs de formulaire personnalisés dans Workfront. Workfront comporte de nombreux champs personnalisés intégrés que vous pouvez utiliser. Cependant, vous pouvez également créer vos propres champs personnalisés. Pour plus d’informations, voir [Concevoir un formulaire à l’aide du créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Champs Workfront et Experience Manager Assets pris en charge

### Mot-clé AEM

Vous pouvez mapper n’importe quel champ pris en charge par Workfront à un mot-clé dans Experience Manager Assets Essentials.

Pour lier un champ à un mot-clé, sélectionnez `xcm:keywords` dans la liste déroulante des champs Experience Manager Assets de la zone de mappage des métadonnées.

Pour mapper plusieurs champs de texte d’une seule ligne à des mots-clés, saisissez une liste séparée par des virgules des valeurs de mot-clé dans le côté Workfront du mappage de métadonnées et `xcm:keywords` du côté Experience Manager Assets. Chaque valeur de champ correspond à un mot-clé distinct. Vous pouvez utiliser un champ calculé pour combiner plusieurs champs Workfront en un seul champ de texte séparé par des virgules.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### Ressources

Les métadonnées sont mises en correspondance lorsqu’une ressource est envoyée de Workfront pour la première fois. Les documents contenant des champs intégrés ou personnalisés sont automatiquement associés aux champs spécifiés lors de la première envoi d’une ressource à Experience Manager Assets Essentials.

1. Dans la colonne **Champ Workfront** , choisissez un champ Workfront intégré ou personnalisé.

   >[!NOTE]
   >
   >Vous pouvez mapper un champ Workfront unique à plusieurs champs Experience Manager Assets. Vous ne pouvez pas mapper plusieurs champs Workfront à un seul champ Experience Manager Assets.

1. Dans le champ **Experience Manager**, choisissez un champ Experience Manager Assets.

   Pour mapper un champ Workfront à une balise Experience Manager Assets, sélectionnez `xcm:keywords`.

1. Répétez les étapes 1 et 2 si nécessaire.
   ![activer les métadonnées](assets/metadata-assets-essentials.png)
1. Cliquez sur **Enregistrer** ou passez à la section [Configurer les dossiers liés (facultatif)](#set-up-linked-folders-optional) de cet article.


## Configuration des dossiers liés (facultatif)

{{setup-linked-folder}}
