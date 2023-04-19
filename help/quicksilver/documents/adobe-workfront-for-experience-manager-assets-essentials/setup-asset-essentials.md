---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configuration de l’intégration de Experience Manager Assets Essentials
description: Connectez votre travail à votre contenu dans Experience Manager Assets Essentials - EDIT ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: b874cb1a99840db11d6d55c86b7f779aa3e6ef35
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configuration de l’intégration de Experience Manager Assets Essentials

Connectez votre travail à votre contenu dans Experience Manager Assets Essentials &#x200B; :

* Push assets and metadata from Adobe Workfront to Experience Manager Assets Essentials &#x200B;
* Lier des ressources de Experience Manager Assets Essentials à vos projets et tâches dans Workfront &#x200B;
* Faciliter les workflows de contrôle de version pour les ressources transférées vers Experience Manager Assets Essentials

Vous pouvez également connecter plusieurs référentiels Experience Manager Assets à un environnement Workfront ou plusieurs environnements Workfront à un référentiel Experience Manager Assets à l’échelle des ID d’organisation. Suivez les instructions de configuration de cet article pour chaque intégration que vous souhaitez configurer.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>Formule Adobe Workfront*</strong>
   </td>
   <td>Tous
   </td>
  </tr>
  <tr>
   <td><strong>Licences Adobe Workfront*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>licence Experience Manager</strong>
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td>Vous devez disposer de Experience Manager Assets Essentials et vous devez être ajouté au produit en tant qu’utilisateur dans le Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Paramétrages du niveau d'accès</strong>
   </td>
   <td>Vous devez être un administrateur Workfront. Pour plus d’informations sur les administrateurs Workfront, voir <strong>Octroi d’un accès administratif complet à un utilisateur</strong>.
   </td>
  </tr>
</table>


*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.


## Configuration de l’intégration

1. Cliquez sur le bouton **Menu Principal** dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration**.
1. Sélectionner  **Documents** ![icône de documents](assets/document-icon.png) dans le panneau de gauche, puis sélectionnez **Intégration de Experience Manager**.
1. Sélectionner **Ajout d’une intégration de Experience Manager**.
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
      <td>Le système renseigne automatiquement l’URL de navigation. Cette URL est utilisée pour créer un lien vers l’instance Assets Essentials de votre entreprise à partir du menu principal pour un accès rapide.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Référentiel Experience Manager Assets</strong>
      </td>
      <td>
      Le système renseigne automatiquement le référentiel de Experience Manager associé à votre ID d’organisation.
      </td>
   </tr>
   </table>

1. Cliquez sur **Enregistrer** ou passez à la [Configuration des métadonnées (facultatif)](#set-up-metadata-optional) dans cet article.


## Configuration des métadonnées (facultatif)

Mappez les données d’objet Workfront sur les champs des médias de ressources dans Experience Manager Assets. Les métadonnées sont mappées lorsqu’une ressource est poussée depuis Workfront pour la première fois.


### Conditions préalables

Avant de commencer, vous devez

* Configurez un schéma de métadonnées dans Experience Manager Assets Essentials, en suivant la procédure décrite à la section [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Facultatif) Configurez les champs de formulaire personnalisés dans Workfront. Workfront comporte de nombreux champs personnalisés intégrés que vous pouvez utiliser. Cependant, vous pouvez également créer vos propres champs personnalisés. Pour plus d’informations, voir [Création ou modification d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Ressources

Les métadonnées sont mises en correspondance lorsqu’une ressource est envoyée de Workfront pour la première fois. Les documents contenant des champs intégrés ou personnalisés sont automatiquement associés aux champs spécifiés lors de la première envoi d’une ressource à Experience Manager Assets Essentials.

1. Dans le **Champ Workfront** , choisissez un champ Workfront intégré ou personnalisé.
   >[!NOTE]
   >
   >Vous pouvez mapper un champ Workfront unique à plusieurs champs Experience Manager Assets. Vous ne pouvez pas mapper plusieurs champs Workfront à un seul champ Experience Manager Assets.
1. Dans le **Experience Manager** , choisissez un champ Experience Manager Assets .
1. Répétez les étapes 1 et 2 si nécessaire.
   ![activation des métadonnées](assets/metadata-assets-essentials.png)
1. Cliquez sur **Enregistrer** ou passez à la [Configuration des dossiers liés (facultatif)](#set-up-linked-folders-optional) dans cet article.


## Configuration des dossiers liés (facultatif)

{{setup-linked-folder}}
