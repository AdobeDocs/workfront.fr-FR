---
title: Connecter les enregistrements
description: Après avoir créé des connexions entre les types d’enregistrements, vous pouvez connecter des enregistrements individuels les uns aux autres. Vous pouvez afficher les informations d'un enregistrement sur un autre lorsque vous les connectez.
recommendations: noDisplay, noCatalog
feature: Workfront Planning
role: User, Admin
author: Alina
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '3355'
ht-degree: 38%

---


# Connect records

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez connecter des enregistrements Adobe Workfront Planning entre eux ou à des objets provenant d&#39;autres applications. Vous pouvez afficher les informations d&#39;un enregistrement sur un autre lorsque vous les connectez.

Cet article décrit comment connecter des enregistrements. Pour plus d&#39;informations générales sur la connexion des enregistrements, voir [Présentation des enregistrements connectés](/help/quicksilver/planning/records/connected-records-overview.md).

Vous devez d’abord connecter deux types d’enregistrement l’un à l’autre, ou un type d’enregistrement à un type d’objet à partir d’une autre application. Cela crée des champs d’enregistrement connectés. Vous pouvez ensuite connecter des enregistrements entre eux ou des enregistrements à d&#39;autres objets à partir d&#39;autres applications dans les champs d&#39;enregistrement connectés.

La connexion d’enregistrements est similaire à la connexion d’enregistrements à des objets à partir d’une autre application.

Pour plus d’informations sur la connexion des types d’enregistrement les uns aux autres ou à des types d’objets d’autres applications, voir [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

Pour obtenir un exemple de connexion de types d’enregistrement, voir [Exemple de connexion de types d’enregistrements et d’enregistrements](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

Vous pouvez connecter les éléments suivants :

* Enregistrements Adobe Workfront Planning entre eux
* Enregistrements d’Adobe Workfront Planning avec des objets provenant d’autres applications

  Vous pouvez connecter des enregistrements avec des objets des types répertoriés ci-dessous à partir des applications suivantes :

   * Adobe Workfront

      * Projets
      * Portefeuilles
      * Programmes
      * Entreprises
      * Groupes

   * Adobe Experience Manager Assets

      * Fichiers d’images
      * Dossiers

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li>
   <li><p>Adobe Experience Manager Assets, pour connecter des ressources AEM à des enregistrements Planning<p>
   <p>Vous devez disposer d’une licence Adobe Experience Manager Assets et d’une intégration entre AEM Assets et Workfront.
    Pour plus d’informations, voir <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront pour Experience Manager Assets et Assets Essentials : index d’article</a>. </p>
   </li>  
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td> Standard
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n'existe aucun contrôle de niveau d'accès pour les objets Adobe Workfront Planning</p> 
   <p>Autorisations d’affichage ou supérieures aux types d’objets que vous souhaitez lier à partir de Workfront.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations de niveau Contribution ou supérieur à un espace de travail <span class="preview">et type d’enregistrement</span> pour connecter des enregistrements </p>  
   <p>Autorisations d’affichage ou supérieures à un espace de travail <span class="preview">et type d’enregistrement</span> pour afficher toutes les connexions aux objets et champs d’autres applications, quel que soit votre accès dans l’autre application. </p>
   <p>Autorisations d’affichage ou supérieures aux objets que vous souhaitez lier à partir de Workfront ou Experience Manager Assets. </p>
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à la connexion des enregistrements

* Pour connecter des enregistrements à d&#39;autres enregistrements ou objets, vous devez disposer des éléments suivants :

   * Au moins un espace de travail, un type d’enregistrement et un enregistrement

     Pour plus d’informations, consultez les articles suivants :

      * [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md)
      * [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md)
      * [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md)

   * Connexions entre types d’enregistrement ou entre types d’enregistrement et objets d’autres applications. Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

* Vous pouvez connecter un ou plusieurs enregistrements ou objets les uns aux autres. Cela dépend du type de connexion que vous avez sélectionné lors de la connexion des types d&#39;enregistrement ou d&#39;objet. Pour plus d’informations, voir [Présentation des types d’enregistrements Connect](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Connecter des enregistrements à partir de Workfront Planning

Vous pouvez connecter des enregistrements de Workfront Planning dans les zones suivantes d&#39;un enregistrement Planning :

* Champs d’enregistrement connectés en mode Tableau.
* la zone ou la page d’aperçu de l’enregistrement dans les champs d’enregistrement connectés sur l’onglet Détails ;
* La zone ou la page d&#39;aperçu de l&#39;enregistrement dans l&#39;onglet Connexions.
* La page de l’enregistrement dans un onglet <span class="preview">Page des enregistrements connectés</span>.

### Connecter des enregistrements Workfront Planning à partir de la vue Tableau ou de la zone Détails d&#39;un enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez connecter les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.
1. Cliquez sur la vignette d’un type d’enregistrement pour ouvrir la page du type d’enregistrement.
1. Cliquez sur le nom d’une vue de tableau pour l’ouvrir.
1. (Facultatif) Ajoutez des enregistrements au type d’enregistrement que vous avez sélectionné en ajoutant une nouvelle ligne au tableau. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
1. (Conditionnel) Après avoir connecté le type d’enregistrement sélectionné à un autre type d’enregistrement, accédez au champ connecté d’un enregistrement et cliquez dans le champ ou cliquez sur **Connecter** pour ajouter un enregistrement.

   ![Connecter d&#39;autres enregistrements en mode Tableau](assets/connect-other-records-smaller-box-in-table-view.png)

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur le nom d’un enregistrement connecté dans la liste pour l’ajouter à l’enregistrement sélectionné. L’enregistrement est ajouté automatiquement.
   * Commencez à saisir le nom d’un enregistrement et cliquez dessus lorsqu’il s’affiche dans la liste. L’enregistrement est ajouté automatiquement.

   >[!TIP]
   >
   >Si seule l’image de l’enregistrement a été sélectionnée pour s’afficher lorsque les types d’enregistrement étaient connectés, seule la miniature ou l’icône de l’enregistrement s’affiche dans le champ connecté. Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
   >

1. (Conditionnel) Si vous avez sélectionné Un à plusieurs ou Un à un pour le type de connexion lorsque vous avez connecté les types d&#39;enregistrements, et que vous essayez de connecter un enregistrement ou un objet déjà connecté ailleurs, vous recevrez un avertissement indiquant que le connecter à nouveau le supprimera de la connexion d&#39;origine. Cliquez sur **Connecter** pour autoriser la suppression et connecter l’enregistrement, ou **Annuler** pour revenir au champ et sélectionner un autre enregistrement.
1. (Facultatif) Si vous ne trouvez pas un objet à connecter et que vous souhaitez l’ajouter, cliquez sur **+ Ajouter**

   Ou

   Commencez à saisir un nom pour l’objet, puis cliquez sur **+ Ajouter** pour le créer et l’ajouter.

   Pour plus d&#39;informations, reportez-vous à la section « Créer des enregistrements en les connectant à partir d&#39;autres enregistrements » de l&#39;article [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

   >[!TIP]
   >
   >    Vous pouvez ouvrir la page d&#39;un enregistrement et connecter d&#39;autres enregistrements en procédant comme suit en mode Tableau :
   >1. Cliquez sur le nom de l’enregistrement dans la vue.
   >1. Recherchez le champ d&#39;enregistrement lié et double-cliquez sur le champ (si des enregistrements sont déjà connectés)
   >Ou
   >Cliquez sur **Connecter des enregistrements** (si le champ est vide) pour ajouter des enregistrements du type d&#39;objet ou d&#39;enregistrement connecté.
   >
   >![Connecter des enregistrements à partir du champ de page d’enregistrement](assets/connect-records-from-record-page-field.png)

1. (Facultatif) Cliquez sur **Voir tout** pour afficher tous les enregistrements.

1. (Le cas échéant) Si vous avez cliqué sur **Afficher tout** à l’étape précédente, la zone **Connecter des objets** s’affiche.

   ![Table des objets connectés pour les enregistrements](assets/connected-objects-table-for-records.png)

1. Commencez à saisir le nom d’un enregistrement dans la zone de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Ou

   Sélectionnez le nom d&#39;un ou de plusieurs enregistrements dans la zone, puis cliquez sur **Connecter des objets**.

   Les éléments suivants sont ajoutés :

   * Les enregistrements liés s&#39;affichent dans le champ d&#39;enregistrement lié de l&#39;enregistrement que vous avez sélectionné à l&#39;étape précédente.
   * Les champs liés sont renseignés avec les informations des enregistrements liés, si vous avez ajouté des champs de recherche liés lorsque vous avez connecté les types d’enregistrement.

   La mise à jour des enregistrements liés met à jour automatiquement les champs liés pour les enregistrements à partir desquels vous effectuez la liaison. Vous ne pouvez pas modifier manuellement les champs liés.

   >[!TIP]
   >
   >* Nous utilisons de manière interchangeable « champs liés » et « champs de recherche ».
   >
   >* Lorsque vous choisissez de connecter plusieurs enregistrements lors de la connexion des types d’enregistrements, les valeurs des champs des différents objets sont affichées séparées par des virgules ou sont agrégées en fonction de l’agrégateur que vous avez choisi lors de la connexion des types d’enregistrements.

1. (Facultatif) Fermez la page du type enregistrement et accédez à l’espace de travail que vous avez sélectionné.
1. Cliquez sur la carte correspondant au type d’enregistrement que vous avez lié.

   Par exemple, si vous avez connecté l’enregistrement **Campagne** avec l’enregistrement Produit, cliquez sur la carte **Produit**.

   La carte de type d’enregistrement doit s’ouvrir en mode Tableau. Dans le cas contraire, sélectionnez une vue Tableau.

   Notez que le champ d’enregistrements liés **Campagne** affiche les noms des campagnes que vous avez liées à des produits dans la page type d’enregistrement du Produit. La mise à jour des informations de Campagne met automatiquement à jour le champ d’enregistrement lié Campagne pour le type d’enregistrement Produit.

### Connectez les enregistrements Workfront Planning aux objets Workfront à partir de la vue Tableau ou de la zone Détails d&#39;un enregistrement

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

Après avoir établi une connexion entre un type d’enregistrement et un type d’objet Workfront, vous pouvez connecter des enregistrements individuels à des objets dans Workfront. Les champs Workfront que vous avez connectés sont automatiquement renseignés sur les enregistrements à partir desquels vous liez les objets.

>[!NOTE]
>
>Vous ne pouvez pas connecter des types d’objet Workfront à des types d’enregistrement Workfront Planning à partir de Workfront.


{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez connecter les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.
1. Cliquez sur la vignette d’un type d’enregistrement pour ouvrir la page du type d’enregistrement.
1. Sélectionnez une vue en **Tableau** dans le menu déroulant **Affichage**.

1. Cliquez sur **Nouvel enregistrement** pour ajouter des enregistrements individuels au type d’enregistrement que vous avez sélectionné. Pour plus d’informations, consultez la section [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

1. (Conditionnel) Après avoir connecté le type d’enregistrement sélectionné à un type d’objet Workfront, accédez au champ connecté d’un enregistrement et cliquez sur le champ ou cliquez sur **Connexion** pour ajouter des objets Workfront.

   ![Connecter des projets en mode Tableau](assets/connect-projects-smaller-box-in-table-view.png)

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur un objet de la liste pour l’ajouter à l’enregistrement sélectionné. Les objets sont répertoriés par ordre alphabétique. L’objet est ajouté automatiquement.
   * Commencez à saisir le nom d’un objet et cliquez dessus lorsqu’il s’affiche dans la liste. L’objet est ajouté automatiquement.

   >[!TIP]
   >
   >Vous pouvez ouvrir la page d&#39;un enregistrement à partir de la vue, double-cliquer sur le champ d&#39;enregistrement lié ou cliquer sur **Connecter** dans le champ pour ajouter des objets à partir du type d&#39;objet connecté.

1. (Facultatif) Si vous ne trouvez pas un objet à connecter et que vous souhaitez l’ajouter, cliquez sur **+ Ajouter**

   Ou

   Commencez à saisir un nom pour l’objet, puis cliquez sur **+ Ajouter** pour créer et ajouter un nouveau projet, portfolio ou programme.

   Pour plus d’informations, voir [Création d’objets Workfront à partir de Workfront Planning](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

1. (Facultatif) Cliquez sur **Voir tout** pour afficher tous les objets que vous êtes au moins autorisé à consulter.

   Si vous avez cliqué sur **Voir tout** à l’étape précédente, la zone **Connecter des objets** s’affiche.

   ![Zone Connecter des objets pour sélectionner des projets](assets/connect-objects-box-to-select-projects.png)

1. Commencez à saisir le nom d’un objet Workfront dans la zone de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Ou

   Sélectionnez le nom d&#39;un ou de plusieurs objets dans la zone, puis cliquez sur **Connecter des objets**.

   >[!IMPORTANT]
   >
   >* Vous ne pouvez ajouter que des objets Workfront pour lesquels vous disposez d’une autorisation d’affichage.
   >
   >* Une fois que vous avez ajouté des objets Workfront, toutes les personnes disposant d’autorisations d’affichage ou supérieures de l’espace de travail peuvent afficher les objets Workfront et leurs informations de champ, indépendamment de leurs autorisations ou de leur accès dans Workfront.

   Les éléments suivants sont ajoutés :

   * Les objets Workfront sélectionnés sont ajoutés au champ d’enregistrement lié.
   * Si vous les avez ajoutés lorsque vous avez connecté le type d’enregistrement à Workfront, les champs liés (ou les champs de recherche) des objets Workfront sont automatiquement renseignés avec les informations de Workfront.

   Pour plus d’informations sur la connexion des types d’enregistrement à des objets à partir d’une autre application, voir [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

1. (Facultatif) Cliquez sur le nom d’un objet Workfront connecté à un enregistrement Workfront Planning dans le champ lié d’une vue de tableau ou du champ lié dans la page d’enregistrement.

   L’objet Workfront s’ouvre alors dans Workfront, si vous disposez au moins des autorisations d’affichage sur l’objet.

   >[!TIP]
   >
   >* Lorsque vous choisissez de connecter plusieurs enregistrements lors de la connexion des types d’enregistrements, les valeurs des champs de recherche sont affichées séparées par des virgules ou sont agrégées en fonction de l’agrégateur que vous avez choisi.
   >
   >* Un champ d’enregistrement lié n’est pas créé pour les objets Workfront liés dans Workfront.

1. (Facultatif) Dans la vue de tableau du type d’enregistrement, pointez sur l’en-tête de colonne de l’objet Workfront lié, cliquez sur le menu déroulant, puis sur **Modifier les champs de recherche**.

1. Ajoutez des champs d’objet Workfront à partir de la zone **Champs non sélectionnés**

   Ou

   Supprimez des champs d’objet Workfront à partir de la zone **Champs sélectionnés**.

   Cela permet d’ajouter ou de supprimer des champs liés dans les enregistrements Workfront Planning. Les informations associées aux champs supprimés restent dans Workfront.


### Connectez les enregistrements Workfront Planning aux objets Adobe Experience Manager à partir de la vue Tableau ou de la zone Détails d&#39;un enregistrement

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console pour pouvoir connecter des enregistrements Workfront Planning à Adobe Experience Manager Assets.
>
>Si vous avez des questions relatives à l’intégration à Adobe Admin Console, voir les [Questions fréquentes sur Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Après avoir créé une connexion entre un type d’enregistrement et Adobe Experience Manager Assets, vous pouvez connecter des enregistrements individuels à des ressources Experience Manager. Les champs de ressource que vous avez connectés à partir d’Experience Manager Assets lors de la création de la connexion sont automatiquement renseignés sur le type d’enregistrement à partir duquel vous avez créé un lien.

>[!NOTE]
>
>Les enregistrements Planning et leurs champs sont accessibles depuis Experience Manager Assets lorsque votre administrateur Workfront configure le mappage des métadonnées par le biais de l’intégration entre Workfront et Adobe Experience Manager Assets. Pour plus d’informations, consultez [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).

Pour connecter des enregistrements à des ressources Experience Manager :

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez connecter les enregistrements.

   L’espace de travail et les types d’enregistrement s’affichent.
1. Cliquez sur la vignette d’un type d’enregistrement pour ouvrir la page du type d’enregistrement.
1. Sélectionnez une vue en **Tableau** à partir du menu déroulant **Affichage** dans le coin supérieur droit de la page du type enregistrement.

1. (Facultatif) Cliquez sur **Nouvel enregistrement** pour ajouter de nouveaux enregistrements au type d’enregistrement que vous avez sélectionné. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
1. (Conditionnel) Après avoir connecté le type d’enregistrement sélectionné à Experience Manager Assets, accédez au champ connecté d’un enregistrement et cliquez sur le champ ou cliquez sur **Connexion** pour ajouter des ressources Experience Manager à l’enregistrement, puis cliquez sur l’icône **+**.

   >[!TIP]
   >
   >  Vous pouvez ajouter l’icône **+** dans le champ d’objet lié de la page d’enregistrement pour connecter les ressources à l’enregistrement.

   La zone **Sélectionner les ressources** s’affiche. <!--we might change this to Connect assets-->

   ![Zone Sélectionner les ressources pour les connexions d’enregistrement AEM](assets/select-assets-box-for-aem-record-connections.png)

1. Cliquez pour sélectionner certains des types de ressource suivants :

   * Images
   * Dossiers

   Vous pouvez sélectionner plusieurs ressources.

   >[!IMPORTANT]
   >
   > Vous pouvez connecter uniquement les ressources que vous pouvez afficher dans Experience Manager. Une fois connectées, toutes les personnes de Workfront Planning peuvent afficher les ressources dans Workfront Planning, quel que soit leur accès dans Experience Manager Assets.

1. Cliquez sur **Sélectionner**. <!-- we might change this to Connect-->

   Les éléments suivants sont ajoutés :

   * Les ressources d’Experience Manager sélectionnées sont ajoutées au champ d’enregistrement lié.
   * Les champs liés (ou champs de recherche) sont renseignés avec les informations des ressources connectées d’Experience Manager.

     Toutes les informations existantes provenant des champs des ressources d’Experience Manager s’affichent automatiquement dans les champs liés ou de recherche.

     >[!TIP]
     >
     >* Lorsque vous choisissez de connecter plusieurs enregistrements lors de la connexion des types d’enregistrements, les valeurs des différents objets s’affichent séparées par des virgules ou agrégées en fonction de l’agrégateur de votre choix.
     >
     >* Un champ d’enregistrement lié aux enregistrements liés de Workfront Planning n’est pas créé pour les ressources de Experience Manager liées dans l’application Experience Manager Assets.

1. (Facultatif) Accédez au type d’enregistrement à partir duquel vous avez créer un lien ver Experience Manager Assets et cliquez sur le nom d’une ressource dans le champ d’enregistrement lié. Les détails Experience Manager de la ressource s’affichent dans une fenêtre pop-up.

   ![Fenêtre pop-up de ressource avec des détails et une miniature AEM](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Les champs suivants s’affichent pour un fichier image :

   * Une miniature de l’image
   * Le nom du fichier image
   * Dimensions
   * Taille
   * Description
   * Le chemin d’accès au fichier dans Experience Manager
   * Le type de ressource
   * Date de création
   * Date de modification

1. (Facultatif) Pour ouvrir la page d’enregistrement des ressources Experience Manager dans Experience Manager, accédez à la page de type d’enregistrement de l’enregistrement à partir duquel vous effectuez le lien, cliquez sur le nom d’une ressource dans le champ Enregistrement lié pour ouvrir la fenêtre pop-up, puis cliquez sur l’icône **Ouvrir dans AEM** ![Icône Ouvrir une ressource dans AEM](assets/open-asset-icon.png) pour ouvrir la ressource.

   Cette opération ouvre la ressource Experience Manager dans Adobe Experience Manager Assets.

1. (Facultatif) Dans la vue Tableau du type d’enregistrement, pointez sur l’en-tête de colonne de la ressource Experience Manager liée, cliquez sur le menu déroulant, puis sur **Modifier les champs de recherche**.

1. Ajoutez des champs d’objet Experience Manager Assets à partir de la zone **Champs non sélectionnés**

   Ou

   Supprimez des champs d’objet Workfront de la zone **Champs sélectionnés**.

   Cela permet d’ajouter ou de supprimer des champs liés des enregistrements. Les informations associées aux champs supprimés restent dans Adobe Experience Assets.

### Connectez les enregistrements Workfront Planning à d’autres enregistrements ou objets à partir de l’onglet Connexions de la page d’enregistrement

1. Accédez à n&#39;importe quelle vue d&#39;un type d&#39;enregistrement qui a été connecté à d&#39;autres types d&#39;enregistrement Planning ou à d&#39;autres types d&#39;objet d&#39;autres applications.
1. Suivez les étapes décrites dans les sous-sections précédentes pour trouver un enregistrement dans la vue que vous souhaitez connecter à d&#39;autres enregistrements ou objets.
1. Cliquez sur le nom d’un enregistrement.

   La page d’aperçu s’ouvre.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![Ouvrir les détails dans une nouvelle icône d’onglet](assets/open-details-in-a-new-tab-icon.png) pour ouvrir la page de l’enregistrement.
1. Cliquez sur l&#39;onglet **Connexions** dans la page ou l&#39;aperçu de l&#39;enregistrement.

   ![Onglet Connexions enregistré dans Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

   Tous les types d&#39;enregistrement ou d&#39;objet liés au type d&#39;enregistrement sélectionné s&#39;affichent sous forme de sections. Les enregistrements ou objets connectés s’affichent sous leur nom d’enregistrement ou de type d’objet sur les cartes.

   >[!TIP]
   >
   >    Seuls les enregistrements connectés ayant des enregistrements individuels connectés s’affichent par défaut.

1. (Facultatif) Cliquez sur **Afficher toutes les connexions** pour afficher tous les types d’enregistrements connectés, y compris ceux sans enregistrements connectés.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas à gauche d’une section pour la réduire.

1. (Conditionnel) Cliquez sur **Connexion** pour ajouter d’autres enregistrements ou objets du même type.
1. (Facultatif) Si vous ne parvenez pas à trouver un enregistrement ou un objet à connecter et que vous souhaitez l’ajouter, cliquez sur **+ Ajouter**

   Ou

   Commencez à saisir un nom pour l’objet, puis cliquez sur **+ Ajouter** pour le créer et l’ajouter à l’enregistrement.

   Pour plus d&#39;informations, reportez-vous à la section « Créer des enregistrements en les connectant à partir d&#39;autres enregistrements » de l&#39;article [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
1. Suivez les étapes décrites dans les sections précédentes pour connecter des enregistrements de Workfront Planning ou des objets de Workfront ou Experience Manager Assets.
Les enregistrements et les objets sont immédiatement ajoutés.
1. (Facultatif) Pointez sur la carte connectée d’un enregistrement ou d’un objet, puis cliquez sur l’icône **Déconnecter l’enregistrement** ![Déconnecter l’enregistrement](assets/disconnect-icon-with-tooltip.png) pour le déconnecter de l’enregistrement sélectionné.

   ![ Icône Déconnecter l’enregistrement avec une info-bulle sur l’onglet Connexions ](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   L&#39;enregistrement est immédiatement déconnecté de toutes les zones de Workfront Planning ou d&#39;autres applications où il peut apparaître comme connecté. Toutes les valeurs de champ de recherche sont également supprimées.

### Connecter des enregistrements à partir de la <span class="preview">page Enregistrements connectés</span> d’un enregistrement


1. Accédez à n&#39;importe quelle vue d&#39;un type d&#39;enregistrement qui a été connecté à d&#39;autres types d&#39;enregistrement Planning ou à d&#39;autres types d&#39;objet d&#39;autres applications.
1. Suivez les étapes décrites dans les sous-sections précédentes pour trouver un enregistrement dans la vue que vous souhaitez connecter à d&#39;autres enregistrements ou objets.
1. Cliquez sur le nom d’un enregistrement.

   La page d’aperçu s’ouvre.
1. Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![Ouvrir les détails dans une nouvelle icône d’onglet](assets/open-details-in-a-new-tab-icon.png) pour ouvrir la page de l’enregistrement.
1. Cliquez sur un onglet existant <span class="preview">Page des enregistrements connectés</span> dans la page de l’enregistrement. Vous devez d’abord créer une <span class="preview">page Enregistrements connectés</span>. Pour plus d’informations, voir [Gérer la mise en page des enregistrements](/help/quicksilver/planning/records/manage-the-record-page.md).

   Une page de type d’enregistrement connectée s’affiche en mode Tableau.

   Tous les enregistrements connectés d’un type s’affichent dans le tableau.
1. Cliquez sur **Connexion** pour ajouter ou supprimer des enregistrements.

   ![Bouton Connexion mis en surbrillance dans l’onglet Détails de l’enregistrement connecté](assets/connect-button-highlighted-in-connected-record-details-tab.png)
1. (Facultatif) Si vous ne trouvez pas d’enregistrement connecté, cliquez sur **+ Ajouter** pour les créer et les connecter.

## Connecter des enregistrements à partir d’objets Workfront

Vous devez disposer des éléments suivants pour connecter les enregistrements Workfront Planning à partir d’objets Workfront :

* Connexions entre les types d&#39;enregistrements et les types d&#39;objets Workfront établis dans Workfront Planning.
* Votre administrateur Workfront ou de groupe doit ajouter l’un des éléments suivants à un type d’objet Workfront :

   * La section Planification des projets, portfolios et programmes Workfront dans votre modèle de mise en page.

   * Le champ personnalisé Planification se connecte à un formulaire personnalisé pour l&#39;un des objets suivants :

      * Projet
      * Portfolio
      * Programme
      * Groupe
      * Entreprise

  Pour plus d’informations, voir [Gérer les connexions d’enregistrement à partir d’objets Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
