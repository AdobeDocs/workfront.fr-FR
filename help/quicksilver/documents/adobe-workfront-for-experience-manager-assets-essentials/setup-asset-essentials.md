---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configuration de l’intégration de Experience Manager Assets Essentials
description: Connectez votre travail à votre contenu dans Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 96%

---

# Configurer l’intégration d’Experience Manager Assets Essentials

Connectez votre travail à votre contenu dans Experience Manager Assets Essentials :

* Transmettre des ressources et des métadonnées d’Adobe Workfront vers Experience Manager Assets Essentials
* Lier les ressources d’Experience Manager Assets Essentials à vos projets et tâches dans Workfront
* Faciliter les workflows de contrôle de version pour les ressources transférées vers Experience Manager Assets Essentials

>[!NOTE]
>
>Vous pouvez également relier plusieurs référentiels Experience Manager Assets à un environnement Workfront, ou plusieurs environnements Workfront à un référentiel Experience Manager Assets à travers des ID d’organisation. Suivez les instructions de configuration de cet article pour chaque intégration que vous souhaitez configurer.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table>
  <tr>
   <td><strong>Package Adobe Workfront</strong>
   </td>
   <td>Tous
   </td>
  </tr>
  <tr>
   <td><strong>Licences Adobe Workfront</strong>
   </td>
   <td>
   <p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
  <tr>
   <td><strong>Produits supplémentaires</strong>
   </td>
   <td>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials et faire l’objet d’un ajout au produit en tant qu’utilisateur ou utilisatrice.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations pour Experience Manager</strong>
   </td>
   <td>Vous devez disposer d’un accès en écriture au dossier de destination dans l’intégration d’Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configurations du niveau d’accès</strong>
   </td>
   <td>Pour configurer une intégration d’Experience Manager, vous devez être un administrateur ou une administratrice de Workfront. Une fois la configuration effectuée, les utilisateurs et utilisatrices disposant d’une licence de plan peuvent configurer des dossiers liés sur des projets individuels.
   </td>
  </tr>
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer l’intégration

{{step-1-to-setup}}

1. Sélectionnez **Documents** ![Icône Documents](assets/document-icon.png) dans le panneau de gauche, puis **Intégration Experience Manager**.
1. Sélectionnez **Ajouter l’intégration Experience Manager**.
1. Indiquez les informations suivantes :

   <table>
   <tr>
      <td><strong>Nom</strong>
      </td>
      <td>Saisissez le nom que vous souhaitez que les utilisateurs et utilisatrices voient dans le bouton Ajouter nouveau dans la zone Documents.
      </td>
   </tr>
   <tr>
      <td><strong>URL de navigation</strong>
      </td>
      <td>Le système renseigne automatiquement l’URL de navigation. Cette URL est utilisée pour créer un lien vers l’instance Assets Essentials de votre organisation à partir du menu principal pour un accès rapide.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Référentiel Experience Manager Assets</strong>
      </td>
      <td>
      Le système remplit automatiquement le référentiel Experience Manager associé à votre ID d’organisation.
      </td>
   </tr>
   </table>

1. Cliquez sur **Enregistrer** ou passez à la section [Configurer les métadonnées (facultatif)](#set-up-metadata-optional) de cet article.


## Configurer les métadonnées (facultatif)

Mappez les données de l’objet Workfront aux champs de média de la ressource dans Experience Manager Assets. Les métadonnées sont mappées lorsqu’une ressource est transmise depuis Workfront pour la première fois.


### Conditions préalables

Avant de commencer, vous devez

* Configurez un schéma de métadonnées dans Experience Manager Assets Essentials comme expliqué dans [Configurer le mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
* (Facultatif) Configurer les champs de formulaire personnalisés dans Workfront. Workfront dispose de nombreux champs personnalisés intégrés que vous pouvez utiliser. Vous pouvez également créer vos propres champs personnalisés. Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Champs Workfront et Experience Manager Assets pris en charge

### Mot-clé AEM

Vous pouvez mapper n’importe quel champ pris en charge par Workfront à un mot-clé dans Experience Manager Assets Essentials.

Pour lier un champ à un mot-clé, sélectionnez `xcm:keywords` dans le menu déroulant du champ Experience Manager Assets de la zone de mappage des métadonnées.

Pour mapper plusieurs champs de texte d’une seule ligne à des mots-clés, saisissez une liste de valeurs de mots-clés séparées par des virgules dans la partie Workfront du mappage des métadonnées, et `xcm:keywords` dans la partie Experience Manager Assets. Chaque valeur de champ correspond à un mot-clé distinct. Vous pouvez utiliser un champ calculé pour combiner plusieurs champs Workfront en un seul champ de texte séparé par des virgules.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### Ressources

Les métadonnées sont mappées lorsqu’une ressource est transmise depuis Workfront pour la première fois. Les documents comportant des champs intégrés ou personnalisés sont automatiquement mis en correspondance avec les champs spécifiés la première fois qu’une ressource est envoyée à Experience Manager Assets Essentials.

1. Dans la colonne **Champ Workfront**, choisissez un champ Workfront intégré ou personnalisé.

   >[!NOTE]
   >
   >Vous pouvez mapper un champ Workfront unique à plusieurs champs Experience Manager Assets. Vous ne pouvez pas mapper plusieurs champs Workfront à un seul champ Experience Manager Assets.

1. Dans le champ **Experience Manager**, choisissez un champ Experience Manager Assets.

   Pour associer un champ Workfront à une balise Experience Manager Assets, sélectionnez `xcm:keywords`.

1. Répétez les étapes 1 et 2 si nécessaire.
   ![Activation des métadonnées](assets/metadata-assets-essentials.png)
1. Cliquez sur **Enregistrer** ou passez à la section [Configurer les dossiers liés (facultatif)](#set-up-linked-folders-optional) de cet article.


## Configurer des dossiers liés (facultatif)

{{setup-linked-folder}}
