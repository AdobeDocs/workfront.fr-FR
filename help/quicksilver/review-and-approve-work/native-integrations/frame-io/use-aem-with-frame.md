---
product-area: documents
navigation-topic: approvals
title: Utilisation de Adobe Experience Manager avec Workfront et le stockage dans le cloud Adobe
description: Utilisation de Adobe Experience Manager avec Workfront et le stockage dans le cloud Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 04d0f295-5206-4c5d-8003-bdf333150903
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Riv4jrZbD1vLx6eLq9utk2TIMRJh6ekBxE5ZBVc7D9c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5ba0b1d553d67beb5924eb9255880a7ba1728ad9
workflow-type: tm+mt
source-wordcount: 2112
ht-degree: 56%

---

# Utilisation de Adobe Experience Manager avec Workfront et le stockage dans le cloud Adobe

Vous pouvez utiliser le &#x200B;&#x200B; pour gérer et stocker vos ressources numériques qui ont passé le cycle de révision et d’approbation. [!DNL Experience Manager Assets]Cette intégration permet d’exploiter les fonctionnalités d’Adobe Experience Manager, Frame.io et Workfront afin de rationaliser vos processus de gestion de contenu et de collaboration.

## Configuration de l’intégration de Experience Manager Assets

Vous pouvez connecter votre travail à votre contenu dans [!DNL Experience Manager Assets] :

* Transférer des ressources et des métadonnées à partir d’[!DNL Adobe Workfront] vers [!DNL Experience Manager Assets]
* Faciliter les cas d’utilisation de contrôle de version
* Suivi des métadonnées des ressources
* Synchroniser les métadonnées de projet entre [!DNL Workfront] et [!DNL Experience Manager Assets]

>[!NOTE]
>
>Vous pouvez également connecter plusieurs référentiels [!DNL Experience Manager Assets] à un environnement [!UICONTROL Workfront] ou plusieurs environnements [!DNL Workfront] à un référentiel [!DNL Experience Manager Assets] dans les ID d’organisation. Suivez les instructions de configuration de cet article pour chaque intégration que vous souhaitez configurer.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Licences Adobe Workfront
   </td>
   <td>
  <p>Pour configurer l’intégration :</p>
   <p>Standard</p>
   <p>Plan</p>

<p>Pour envoyer des documents à Experience Manager Assets :</p>
   <p>Contributeur ou supérieur</p>
   <p>Requête ou supérieure</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Licences Adobe Experience Manager
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td>Produits supplémentaires
   </td>
   <td>Vous devez avoir [!DNL Experience Manager Assets as a Cloud Service], et vous devez faire l’objet d’un ajout au produit en tant qu’utilisateur ou utilisatrice.
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, voir la section [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer

* Vous devez avoir [!DNL Workfront] et [!DNL Adobe Experience Manager Assets] associés à un ID d’organisation dans l’[!DNL Adobe Admin Console]. Pour plus d’informations, voir [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
* Votre instance Workfront doit utiliser l’espace de stockage Adobe dans le cloud.


## Configurer les informations d’intégration

{{step-1-to-setup}}

1. Sélectionnez **[!UICONTROL Documents]** dans le panneau de gauche, puis Intégration **[!UICONTROL [!DNL Experience Manager]]**.
1. Sélectionner **[!UICONTROL Ajouter une intégration [!DNL Experience Manager]]**.
1. Dans le champ **[!UICONTROL Nom]**, saisissez le nom que les utilisateurs et utilisatrices doivent voir lorsqu’ils interagissent avec cette intégration dans Workfront et Experience Manager Assets.
1. Dans le champ **[!UICONTROL URL de navigation]**, le système renseigne automatiquement l’URL de navigation. Cette URL en lecture seule est utilisée pour créer un lien vers l’instance [!DNL Experience Manager] de votre organisation à partir du [!UICONTROL Menu principal] pour un accès rapide.
1. Sélectionnez un référentiel dans le menu déroulant Référentiel de ressources **[!UICONTROL [!DNL Experience Manager]]**. Le système renseigne automatiquement les référentiels [!DNL Experience Manager] associés à l’ID d’organisation auquel votre profil utilisateur est affecté.
   ![Choix du référentiel Experience Manager](assets/setup-information.png)

1. Cliquez sur **[!UICONTROL Enregistrer]** ou passez à la section [Configurer les métadonnées (facultatif)](#set-up-metadata-optional) de cet article.

   >[!IMPORTANT]
   >
   >En raison de la complexité de l’intégration, vous ne pouvez pas modifier le référentiel après avoir enregistré la configuration initiale.


## Configurer les métadonnées (facultatif)

Vous pouvez mapper des données d’objet [!DNL Workfront] aux champs de média de ressources dans [!DNL Experience Manager] Assets.

>[!NOTE]
>
>Vous ne pouvez mapper les métadonnées que dans une seule direction : de [!DNL Workfront] vers [!DNL Experience Manager]. Les métadonnées des documents liés à [!DNL Workfront] à partir d’[!DNL Experience Manager] ne peuvent pas être transférées vers [!DNL Workfront].

### Configurer les champs de métadonnées

Avant de commencer à mapper les champs de métadonnées, vous devez configurer les champs de métadonnées dans Workfront et Experience Manager Assets.

Pour configurer les champs de métadonnées, procédez comme suit :

1. Configurez un schéma de métadonnées dans [!DNL Experience Manager Assets] comme expliqué dans [Configurer le mappage des métadonnées de ressource entre Adobe  [!DNL Workfront]  et  [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. Configurez les champs de formulaire personnalisés dans Workfront. [!DNL Workfront] comporte de nombreux champs personnalisés intégrés que vous pouvez utiliser. Cependant, vous pouvez également créer vos propres champs personnalisés, comme expliqué dans la section [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

+++ **Développer pour afficher plus d’informations sur les champs Workfront et Experience Manager Assets pris en charge** 

**Balises Experience Manager Assets**

Vous pouvez mapper n’importe quel champ pris en charge par Workfront à une balise dans Experience Manager Assets. Pour cela, vous devez vous assurer que les valeurs de balise dans Experience Manager Assets correspondent à Workfront.

* Les balises et les valeurs de champ Workfront doivent correspondre exactement à l’orthographe et au format.
* Les valeurs de champ Workfront mappées aux balises Experience Manager Assets doivent être toutes en minuscules, même si la balise dans Experience Manager Assets comportent des lettres majuscules.
* Les valeurs de champ Workfront ne doivent pas inclure d’espaces.
* La valeur de champ dans Workfront doit également inclure la structure de dossiers de la balise Experience Manager Assets.
* Pour mapper plusieurs champs de texte d’une seule ligne à des balises, saisissez une liste séparée par des virgules des valeurs de balise du côté Workfront du mappage de métadonnées, et `xcm:keywords` du côté Experience Manager Assets. Chaque valeur de champ correspond à une balise distincte. Vous pouvez utiliser un champ calculé pour combiner plusieurs champs Workfront en un seul champ de texte séparé par des virgules.
* Vous pouvez mapper des valeurs à partir de champs de liste déroulante, de case d’option ou de case à cocher en saisissant une liste des valeurs disponibles dans ce champ, séparées par des virgules.


>[!INFO]
>
>**Exemple** : pour correspondre à la balise affichée ici dans la structure de dossiers, la valeur de champ dans Workfront est `landscapes:trees/spruce`. Notez les minuscules dans la valeur du champ Workfront.
>
>Si vous souhaitez que la balise soit située le plus à gauche dans l’arborescence des balises, elle doit être suivie d’un signe deux-points. Dans cet exemple, pour mapper la balise de paysage, la valeur de champ dans Workfront est `landscapes:`.
>
>![Structure de dossiers dans AEM](assets/aem-folder-structure-with-red-boxes.png)


Une fois les balises créées dans Experience Manager Assets, elles s’affichent dans la liste déroulante Balises de la section Métadonnées. Pour lier un champ à une balise, sélectionnez `xcm:keywords` dans la liste déroulante du champ Experience Manager Assets de la zone de mappage des métadonnées.

Pour plus d’informations sur les balises dans Experience Manager Assets, notamment sur la création et la gestion des balises, voir [Administrer les balises](https://experienceleague.adobe.com/fr/docs/experience-manager-64/administering/contentmanagement/tags).

**Champs de schéma de métadonnées personnalisés Experience Manager Assets**

Vous pouvez mapper des champs Workfront intégrés et personnalisés à des champs de schéma de métadonnées personnalisés dans Experience Manager Assets.

Les champs de métadonnées personnalisés créés dans Experience Manager Assets sont organisés dans leur propre section dans la zone de configuration des métadonnées.

![Section de métadonnées personnalisées](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Champs Workfront**

Vous pouvez mapper des champs Workfront intégrés et personnalisés à Experience Manager Assets. Les valeurs de champ suivantes doivent correspondre au niveau des majuscules/minuscules et de l’orthographe entre Workfront et Experience Manager Assets :

* Champs de liste déroulante
* Champs à sélection multiple

>[!TIP]
>
> Pour vérifier si les valeurs de champ correspondent exactement, accédez à :
>
> * Configuration > Formulaires personnalisés dans Workfront ou le champ dans l’objet.
> * Ressources > Schémas de métadonnées dans Experience Manager Assets

+++

### Mapper les métadonnées de ressources

Les métadonnées sont mappées lorsqu’une ressource est transférée à partir de [!DNL Workfront] pour la première fois. Les documents contenant des champs intégrés ou personnalisés sont automatiquement associés aux champs spécifiés lors de la première envoi d’une ressource à [!DNL Experience Manager Assets].

Pour mapper les métadonnées des ressources :

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Dans la colonne du champ **[!UICONTROL [!DNL Workfront]]**, choisissez un champ Workfront intégré ou personnalisé.

   >[!NOTE]
   >
   >Vous pouvez mapper un seul champ [!DNL Workfront] à plusieurs champs [!UICONTROL Experience Manager Assets]. Vous ne pouvez pas mapper plusieurs champs [!DNL Workfront] à un seul champ [!DNL Experience Manager Assets].
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Dans le champ [!DNL Experience Manager Assets], recherchez dans les catégories prérenseignées ou saisissez au moins deux lettres dans le champ de recherche pour accéder à d’autres catégories.
1. Répétez les étapes 2 et 3 si nécessaire.
   ![Champs de métadonnées](assets/metadata-no-asset-toggle.png)
1. Cliquez sur [!UICONTROL **Enregistrer**] ou accédez à la section [Synchronisation des métadonnées d’objet](#object-metadata-sync) de cet article.



### Synchronisation des métadonnées d’objet

Champs [!DNL Experience Manager] qui sont mappés à [!DNL Workfront] champs de portefeuille, de programme, de projet, de tâche, de problème et de document se mettent à jour automatiquement lorsque le champ est modifié dans [!DNL Workfront].

Lorsque cette option est activée, toute ressource qui a été transmise à Adobe Experience Manager affiche une vue en temps réel des métadonnées Adobe Experience Manager du document sur la page Détails du document dans Workfront.

1. Activez le champ **[!UICONTROL Métadonnées de l’objet de synchronisation]**, puis cliquez sur **Enregistrer**.

>[!IMPORTANT]
>
>Les utilisateurs doivent disposer d’un accès en écriture dans [!DNL Experience Manager] pour les ressources résidant dans l’objet afin que les métadonnées se synchronisent lors de leur mise à jour.


## Envoyer un document vers Experience Manager Assets ou Assets Essentials

Vous pouvez envoyer des documents depuis Workfront vers Experience Manager Assets ou Assets Essentials. Les documents chargés et envoyés depuis Workfront vers Assets Essentials sont toujours pris en compte par rapport à votre stockage global de documents.

Les Assets envoyées à Experience Manager par le biais de cette intégration ont une taille maximale de **5 To**.

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

Les champs de métadonnées sont mappés pour la première fois lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets ou Assets Essentials. Toutes les métadonnées configurées pour mapper des objets parent sont également envoyées. Pour plus d’informations sur la configuration du mappage des métadonnées, voir [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration d’Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exemple** lorsque vous envoyez pour la première fois une ressource jointe à un projet, les métadonnées sont mappées à Experience Manager Assets ou Assets Essentials, ainsi qu’à toutes les métadonnées mappées à partir des objets parents tels qu’un portfolio et un programme.



### Envoyer un document depuis Workfront

Lorsqu’un utilisateur ou une utilisatrice envoie un document depuis Workfront vers Experience Manager Assets ou Assets Essentials, les métadonnées mappées sont transférées avec le document. Une fois le document envoyé, les modifications apportées aux métadonnées du document dans Workfront ne sont pas reflétées dans Assets ou Assets Essentials. Si un champ mappé dans Workfront est modifié, vous devez envoyer une nouvelle version du document avec les métadonnées mises à jour vers Assets ou Assets Essentials.

Pour envoyer un document, procédez comme suit :

1. Accédez à la zone **Documents** dans Workfront, puis sélectionnez le document à envoyer.
1. Dans la barre située en bas de l’écran, cliquez sur **Envoyer à**.

1. Sélectionnez l’intégration Experience Manager configurée par votre administrateur, puis cliquez sur **Envoyer**.

   >[!NOTE]
   >
   >L’équipe d’administration de Workfront peut choisir n’importe quel nom pour cette intégration, qui peut donc ne pas contenir spécifiquement les mentions Assets ou Assets Essentials.


1. Sélectionnez l’emplacement de la ressource, puis cliquez sur **Sélectionner un dossier**.

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

<!--
 not sure if this is in yet

### Send a new version

You can add a new version to a document you have previously uploaded to Workfront. For more information, see [Upload a new version of a document](/help/quicksilver/documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to Assets Essentials. If a mapped field in Workfront has changed, the new version updates the metadata in Assets Essentials when it sends.

>[!IMPORTANT]
>
>Before you upload a new version to Workfront, we recommend renaming the file. If you upload a new version with the exact same file name as a previous version, only the most recent version can be downloaded from Workfront. All versions can be downloaded from Experience Manager Assets or Assets Essentials regardless of the file name. - is this accuate for ESM?

To send the most recent version:

1. Go to the **Documents** area in Workfront, and locate the document.
1. In the bar at the bottom of the screen, click **Send to**. 

1. Choose the Experience Manager integration your administrator set up, then click **Send**.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Assets or Assets Essentials.

1. Click **Save**. The new version saves in the same location as the previous version.
 
 -->