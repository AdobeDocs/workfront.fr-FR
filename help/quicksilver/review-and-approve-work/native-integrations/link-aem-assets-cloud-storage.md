---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: Lier du contenu et des dossiers de Experience Manager Assets à l’espace de stockage dans le cloud Adobe
description: Si votre entreprise utilise l’espace de stockage Adobe, vous pouvez lier du contenu et des dossiers de Experience Manager Assets à n’importe quel objet Adobe Workfront prenant en charge les documents.
author: Courtney
source-git-commit: 66635b2edc78833ec2d08cef382b39b89238b565
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 12%

---

# Lier du contenu et des dossiers de Experience Manager Assets à l’espace de stockage dans le cloud Adobe

Si votre entreprise utilise l’espace de stockage Adobe, vous pouvez lier du contenu et des dossiers de Experience Manager Assets à Workfront. Une fois lié, vous pouvez afficher et gérer le contenu dans Workfront. Toute modification apportée au contenu dans Experience Manager Assets sera répercutée dans Workfront.

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
   <td>Vous devez disposer d’Experience Manager as a Cloud Service et être ajouté au produit en tant qu’utilisateur dans Admin Console.</td> 
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

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer :

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, voir [Utilisation d’Adobe Experience Manager avec l’intégration Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Pour utiliser la fonctionnalité de suggestions intelligentes ou de résumés de campagne, vous devez signer un Cavalier GenAI. Pour plus d’informations, voir [Utilisation de la fonction de conseil sur l’accès au contenu AEM dans les applications Adobe](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).

## Lier du contenu depuis Experience Manager Assets

Pour lier du contenu :

1. Accédez à l’objet Workfront auquel vous souhaitez lier du contenu.
1. Cliquez sur la section **Documents** dans le panneau de gauche.
1. Cliquez sur **Nouveau** dans la partie droite de la page, puis sur **Fichiers AEM** pour lier une ressource individuelle.
   ![Ajouter des fichiers AEM à la zone des documents](assets/aem-files.png)

1. Grâce au gestionnaire d’accès, vous pouvez :

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Recherche de ressources à l’aide de Recherche optimisée par l'IA.</strong> Utilisez une recherche optimisée par l’IA qui comprend le sens et l’intention derrière les requêtes, en prenant en charge plusieurs langues, fautes de frappe et synonymes.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Recherche optimisée par l'IA pour une découverte de ressources plus intelligente</a>.</td>
      </tr>
      <tr>
         <td><strong>Afficher des suggestions intelligentes en fonction du contexte et de l’intention.</strong> Découvrez les ressources qui correspondent à vos besoins en matière de contenu à l’aide de recommandations contextuelles issues de l’application Adobe hôte.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Suggestions intelligentes basées sur le contexte et l’intention</a>.</td>
      </tr>
      <tr>
         <td><strong>Chargez un résumé de campagne pour découvrir les ressources pertinentes.</strong> Téléchargez un document de résumé de campagne PDF, DOCX ou TXT afin que le conseiller d’accès puisse l’analyser et recommander des ressources appropriées.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Briefs de campagne pour découvrir les ressources pertinentes</a>.</td>
      </tr>
      <tr>
         <td><strong>Affichage et sélection des rendus de ressources Dynamic Media.</strong> Parcourez les rendus optimisés pour les canaux, y compris les paramètres d’image prédéfinis, les recadrages intelligents et les types de format, et appliquez les modificateurs Dynamic Media pour prévisualiser les réglages en temps réel.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendus de ressources Dynamic Media disponibles</a>.</td>
      </tr>
      <tr>
         <td><strong>Application de modificateurs Dynamic Media aux rendus.</strong> Ajoutez des modificateurs pour transformer les rendus de ressources en temps réel et prévisualisez les résultats avant de sélectionner un rendu pour votre application hôte.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Rendus de ressources Dynamic Media disponibles</a>.</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>Accès aux métadonnées des ressources.</strong> Consultez les propriétés de la ressource telles que le titre, la description, le format, la taille et d’autres onglets de métadonnées (Produit, Campagne, Balises) cohérents avec la vue Assets.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Accès aux métadonnées des ressources cohérentes avec la vue Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtrage des ressources à l’aide de filtres prédéfinis.</strong> Affinez les résultats des ressources à l’aide de filtres tels que le type de fichier, le format de fichier, le statut de la ressource, la taille de fichier, la largeur d’image, la hauteur d’image, la date de modification et la date de création.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Accès aux filtres cohérents avec la vue Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Enregistrer et réutiliser des recherches.</strong> Créez des recherches enregistrées en spécifiant un terme de recherche et des options de filtre, puis réutilisez-les dans Experience Manager Assets et d’autres applications Adobe.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Accéder aux recherches récentes et enregistrées et les réutiliser</a>.</td>
      </tr>
      <tr>
         <td><strong>Rechercher des ressources dans et entre les collections.</strong> Recherchez des ressources ou des collections dans toutes les collections ou limitez votre recherche à une collection spécifique.</td>
         <td>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Recherche de ressources dans et entre des collections</a>.</td>
      </tr>
   </tbody>
   </table>

   >[!NOTE]
   >
   >Le contenu recommandé dans le gestionnaire d’accès utilise les données suivantes pour déterminer le contenu suggéré dans Workfront :
   >
   >* Champs de nom et de description de l’objet Workfront
   >* Champs de formulaire personnalisés marqués comme obligatoires
   >* Données des documents joints

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## Considérations

* Les workflows de révision et d’approbation ne sont pas pris en charge pour les ressources AEM liées.
* Les champs de métadonnées sont d’abord mappés lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets. Si votre équipe d’administration Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.
