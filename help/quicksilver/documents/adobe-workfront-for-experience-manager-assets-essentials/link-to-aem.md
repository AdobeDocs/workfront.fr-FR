---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Lier du contenu et des dossiers avec le gestionnaire de contenu optimisé par Experience Manager Assets
description: Vous pouvez utiliser le gestionnaire d’accès pour lier du contenu ou des dossiers de Experience Manager Assets à tout objet Adobe Workfront prenant en charge les documents. Le gestionnaire de contenu permet une découverte intelligente et contextuelle directement dans Workfront, ce qui vous aide à trouver rapidement du contenu pertinent et approuvé.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 22%

---

# Lier du contenu et des dossiers au gestionnaire de contenu de Experience Manager Assets

Le gestionnaire de contenu permet une découverte intelligente et contextuelle directement dans Workfront, ce qui vous permet de trouver rapidement du contenu pertinent et approuvé en fonction du contexte. Grâce à des fonctionnalités telles que les suggestions intelligentes, les rendus Dynamic Media et les métadonnées de ressources détaillées, il vous permet d’évaluer et de réutiliser efficacement le contenu sans quitter Workfront, ce qui accélère la création de contenu tout en préservant la cohérence de la marque.

Vous pouvez utiliser le gestionnaire de contenu pour lier du contenu et des dossiers de Experience Manager Assets vers Workfront. Une fois lié, vous pouvez afficher et gérer le contenu dans Workfront. Toute modification apportée au contenu dans Experience Manager Assets sera répercutée dans Workfront.

>[!IMPORTANT]
>
>Si votre entreprise refuse de signer l’accord GenAI Rider, vous pouvez toujours utiliser le gestionnaire de contenu pour choisir les ressources et les dossiers dans Experience Manager Assets, mais vous n’aurez pas accès aux fonctionnalités optimisées par l’IA telles que Recherche optimisée par l&#39;IA, les suggestions intelligentes ou l’analyse des résumés de campagne.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou supérieur</p> 
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td>Vous devez disposer d’Experience Manager as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans l’Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorisations Experience Manager</td> 
    <td>Vous devez disposer d’un accès en écriture au dossier.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher accès ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer :

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, voir [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

* Pour utiliser la fonctionnalité de suggestions intelligentes ou de résumés de campagne, vous devez signer un Cavalier GenAI. Pour plus d’informations, voir [Utilisation de la fonction de conseil sur l’accès au contenu AEM dans les applications Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).



## Lier du contenu de Experience Manager Assets avec le gestionnaire de contenu

Vous pouvez désormais utiliser le gestionnaire de contenu pour lier le contenu de Experience Manager Assets directement dans Workfront. Le gestionnaire de contenu n’est pas disponible pour Assets Essentials.

Pour lier du contenu :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur Workfront peut choisir n’importe quel nom pour cette intégration et ne pas mentionner spécifiquement Experience Manager Assets.

1. Grâce au gestionnaire d’accès, vous pouvez :


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Rechercher des ressources à l’aide de Recherche optimisée par l'IA.</strong> Utilisez une recherche optimisée par l’IA qui comprend le sens et l’intention derrière les requêtes, en prenant en charge plusieurs langues, fautes de frappe et synonymes.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Recherche optimisée par l'IA pour une découverte de ressources plus intelligente</a>.</td>
      </tr>
      <tr>
         <td><strong>Afficher des suggestions intelligentes en fonction du contexte et de l’intention.</strong> Découvrez les ressources qui correspondent à vos besoins en matière de contenu à l’aide de recommandations contextuelles issues de l’application Adobe hôte.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Suggestions intelligentes basées sur le contexte et l’intention</a>.</td>
      </tr>
      <tr>
         <td><strong>Chargez un résumé de campagne pour découvrir les ressources pertinentes.</strong> Téléchargez un document de résumé de campagne PDF, DOCX ou TXT afin que le conseiller d’accès puisse l’analyser et recommander des ressources appropriées.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Briefs de campagne pour découvrir les ressources pertinentes</a>.</td>
      </tr>
      <tr>
         <td><strong>Affichage et sélection des rendus de ressources Dynamic Media.</strong> Parcourez les rendus optimisés pour les canaux, y compris les paramètres d’image prédéfinis, les recadrages intelligents et les types de format, et appliquez des modificateurs Dynamic Media pour prévisualiser les réglages en temps réel.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendus de ressources Dynamic Media disponibles</a>.</td>
      </tr>
      <tr>
         <td><strong>Application de modificateurs Dynamic Media aux rendus.</strong> Ajouter des modificateurs pour transformer les rendus de ressources en temps réel et prévisualiser les résultats avant de sélectionner un rendu pour votre application hôte.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendus de ressources Dynamic Media disponibles</a>.</td>
      </tr>
      <tr>
         <td><strong>Découvrir et parcourir les fragments de contenu.</strong> Effectuer une recherche dans les fragments de contenu, afficher des aperçus de miniatures en direct, vérifier le statut (Brouillon, Modifié ou Publié) et inspecter les propriétés, références et variations détaillées.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor"> Découverte de fragments de contenu </a>.</td>
      </tr>
      <tr>
         <td><strong>Accès aux métadonnées des ressources.</strong> Consultez les propriétés de la ressource telles que le titre, la description, le format, la taille et d’autres onglets de métadonnées (Produit, Campagne, Balises) cohérents avec la vue Assets.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Accès aux métadonnées des ressources cohérentes avec la vue Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtrage des ressources à l’aide de filtres prédéfinis.</strong> affiner les résultats des ressources à l’aide de filtres tels que le type de fichier, le format de fichier, le statut de la ressource, la taille de fichier, la largeur d’image, la hauteur d’image, la date de modification et la date de création.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Accès aux filtres cohérents avec la vue Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Enregistrer et réutiliser les recherches.</strong> Créez des recherches enregistrées en spécifiant un terme de recherche et des options de filtre, puis réutilisez-les dans Experience Manager Assets et d’autres applications Adobe.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Accéder aux recherches récentes et enregistrées et les réutiliser</a>.</td>
      </tr>
      <tr>
         <td><strong>Rechercher des ressources dans et entre les collections.</strong> Recherchez des ressources ou des collections dans toutes les collections ou limitez votre recherche à une collection spécifique.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Recherche de ressources dans et entre des collections</a>.</td>
      </tr>
   </tbody>
   </table>


### Liaison d’une nouvelle version de Experience Manager Assets à la fonction de conseil

Vous pouvez extraire du nouveau contenu de Experience Manager Assets ou d’Assets Essentials et l’ajouter à une ressource existante en tant que nouvelle version. Si le document est déjà lié et qu’une nouvelle version est ajoutée dans Experience Manager Assets ou Assets Essentials, la nouvelle version s’affiche automatiquement dans Workfront.

Pour lier une nouvelle version :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez la ressource à remplacer par une nouvelle version. Vous ne pouvez pas créer de version d’une ressource dans un dossier lié.
1. Sélectionnez **Ajouter** > **Version**, puis sélectionnez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur Workfront peut choisir n’importe quel nom pour cette intégration et il se peut donc qu’il ne mentionne pas spécifiquement Experience Manager Assets.

1. Sélectionnez le contenu que vous souhaitez lier :

   * Sélectionnez l’onglet Assets pour parcourir les ressources, les dossiers ou les collections dans Experience Manager Assets ou Assets Essentials.

     ![Conseiller en contenu](assets/content-advisor-full.png)

   * Les fragments de contenu ne prennent pas en charge les versions . Si vous sélectionnez un fragment de contenu, la nouvelle version remplacera le fragment de contenu existant au lieu de créer une nouvelle version.

1. Cliquez sur **Sélectionner**.

## Liaison d’un dossier de Experience Manager Assets au gestionnaire de contenu

Les autorisations d’affichage de ressources individuelles dans un dossier dépendent des autorisations Experience Manager Assets.

Pour lier un dossier :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez placer le dossier.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur Workfront peut choisir n’importe quel nom pour cette intégration et il se peut donc qu’il ne mentionne pas spécifiquement Experience Manager Assets.

1. Cliquez sur **** > **Fichiers et dossiers**.

1. Cliquez sur l’icône **Filtre** puis, dans la section **Type de ressource**, choisissez **Dossiers**.

1. Sélectionnez le dossier à lier.

1. Cliquez sur **Sélectionner**.

## Considérations

* La fonctionnalité de gestionnaire d’accès n’est pas disponible pour les objets utilisant Adobe Enterprise Storage. Si votre organisation utilise le stockage d’entreprise Adobe, vous pouvez toujours lier des ressources et des dossiers à partir de Experience Manager Assets ou d’Assets Essentials, mais vous n’aurez pas accès aux fonctionnalités du gestionnaire de contenu telles que Recherche optimisée par l&#39;IA, les suggestions intelligentes ou les rendus Dynamic Media. Pour plus d’informations, voir [Utilisation d’Adobe Experience Manager avec l’intégration Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* La fonctionnalité de gestionnaire d’accès n’est pas disponible pour Assets Essentials. Pour lier des ressources et des dossiers à partir d’Assets Essentials, voir [Lier des ressources et des dossiers à partir de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md).

* Les champs de métadonnées sont d’abord mappés lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets. Si votre équipe d’administration Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.
