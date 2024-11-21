---
title: Connexion d’enregistrements
description: Après avoir créé des connexions entre les types d’enregistrement, vous pouvez connecter des enregistrements individuels les uns aux autres. Vous pouvez afficher les informations d’un enregistrement sur un autre enregistrement lorsque vous les connectez.
recommendations: noDisplay, noCatalog
feature: Workfront Planning
role: User, Admin
author: Alina
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '2988'
ht-degree: 45%

---


# Connect records

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez connecter des enregistrements de planification Adobe Workfront les uns aux autres ou aux objets d’autres applications. Vous pouvez afficher les informations d’un enregistrement sur un autre enregistrement lorsque vous les connectez.

Cet article décrit comment connecter des enregistrements. Pour plus d’informations sur la connexion des enregistrements, voir [Présentation des enregistrements connectés](/help/quicksilver/planning/records/connected-records-overview.md).

Vous devez d’abord connecter deux types d’enregistrement l’un à l’autre, ou un type d’enregistrement à un type d’objet à partir d’une autre application. Cela crée des champs d’enregistrement liés. Vous pouvez ensuite connecter des enregistrements les uns aux autres ou des enregistrements à d’autres objets à partir d’autres applications à l’aide des champs d’enregistrement liés.

La connexion d’enregistrements est similaire à la connexion d’enregistrements à des objets à partir d’une autre application.

Pour plus d’informations sur la connexion des types d’enregistrement les uns aux autres ou à des types d’objets d’autres applications, voir [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

Pour obtenir un exemple de connexion de types d’enregistrement, voir [Exemple de connexion de types d’enregistrements et d’enregistrements](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

Vous pouvez connecter les éléments suivants :

* Enregistrements d’Adobe Workfront Planning
* Enregistrements d’Adobe Workfront Planning avec des objets provenant d’autres applications

  Vous pouvez connecter des enregistrements à des objets des types répertoriés ci-dessous à partir des applications suivantes :

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

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

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
   <li><p>Adobe Experience Manager Assets, si vous souhaitez connecter AEM ressources à des enregistrements de planification<p>
   <p>Vous devez disposer d’une licence Adobe Experience Manager Assets et d’une intégration entre AEM Assets et Workfront.
    Pour plus d’informations, voir <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials : article index</a>. </p>
   </li>  
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package de planification Adobe Workfront*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td> Standard
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations sur un espace de travail pour connecter des enregistrements </p>  
   <p>Afficher ou des autorisations supérieures à un espace de travail pour afficher toutes les connexions aux objets et aux champs d’autres applications, quel que soit votre accès dans l’autre application. </p>
   <p>Afficher ou des autorisations supérieures aux objets que vous souhaitez lier à partir de Workfront ou Experience Manager Assets. </p>
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Tous les utilisateurs, y compris les administrateurs Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planification dans le menu principal. </p> </td> 
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

* Vous pouvez connecter un ou plusieurs enregistrements ou objets les uns par rapport aux autres. Cela dépend du type de connexion que vous avez sélectionné lors de la connexion des types d’enregistrement ou d’objet. Pour plus d’informations, reportez-vous à la section [Présentation des types d’enregistrement Connect](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Connexion d’enregistrements à partir de Workfront Planning

Vous pouvez connecter des enregistrements à partir de Workfront Planning dans les zones suivantes d’un enregistrement Planning :

* Champs d’enregistrement connectés dans la vue de tableau.
* Prévisualisation ou page de l’enregistrement dans les champs d’enregistrement connectés dans l’onglet Détails .
* Aperçu ou page de l’enregistrement dans l’onglet Connexions .

### Connexion des enregistrements de planification Adobe Workfront depuis la vue Tableau ou la zone Détails

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dont vous souhaitez vous connecter.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.
1. Cliquez sur la vignette d’un type d’enregistrement pour ouvrir la page du type d’enregistrement.
1. Cliquez sur le nom d’une vue de tableau pour l’ouvrir.
1. (Facultatif) Ajoutez des enregistrements au type d’enregistrement que vous avez sélectionné en ajoutant une nouvelle ligne au tableau. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
1. (Conditionnel) Une fois que vous avez connecté le type d’enregistrement sélectionné à un autre type d’enregistrement, accédez à la colonne des enregistrements liés et double-cliquez sur la cellule correspondant à l’enregistrement que vous souhaitez lier à d’autres enregistrements.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur le nom d’un enregistrement connecté dans la liste pour l’ajouter à l’enregistrement sélectionné. L’enregistrement est ajouté automatiquement.
   * Commencez à saisir le nom d’un enregistrement et cliquez dessus lorsqu’il s’affiche dans la liste. L’enregistrement est ajouté automatiquement.

   >[!TIP]
   >
   >Si seule l’image de l’enregistrement a été sélectionnée pour s’afficher lorsque les types d’enregistrement ont été connectés, seule la miniature ou l’icône de l’enregistrement s’affiche dans le champ connecté. Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
   >

1. <span class="preview"> (Conditionnel) Si vous avez sélectionné Un à plusieurs ou Un à un pour le type Connexion lorsque vous avez connecté les types d’enregistrement et que vous essayez de connecter un enregistrement ou un objet déjà connecté ailleurs, vous recevrez un avertissement indiquant que le reconnecter le supprimera de la connexion d’origine. Cliquez sur **Se connecter** pour autoriser la suppression et connecter l&#39;enregistrement, ou sur **Annuler** pour revenir au champ et sélectionner un autre enregistrement.</span>
1. (Facultatif) Si vous ne trouvez pas d’enregistrement ou d’objet à connecter et que vous souhaitez l’ajouter, cliquez sur **+ Ajouter** pour ajouter un nouvel enregistrement. Pour plus d’informations, reportez-vous à la section &quot;Créer des enregistrements lors de leur connexion&quot; dans l’article [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

   >[!TIP]
   >
   >    Vous pouvez ouvrir la page d’un enregistrement et connecter d’autres enregistrements en procédant comme suit dans la vue de tableau :
   >1. Cliquez sur le nom de l’enregistrement dans la vue.
   >1. Recherchez le champ d&#39;enregistrement lié et double-cliquez sur le champ (si des enregistrements sont déjà connectés).
   >Ou
   >Cliquez sur **Connecter des enregistrements** (si le champ est vide) pour ajouter des enregistrements de l’enregistrement ou du type d’objet connecté.
   >
   >![](assets/connect-records-from-record-page-field.png)

1. (Facultatif) Cliquez sur **Afficher tout** pour afficher tous les enregistrements.

1. (Le cas échéant) Si vous avez cliqué sur **Afficher tout** à l’étape précédente, la zone **Connecter des objets** s’affiche.

   ![](assets/connected-objects-table-for-records.png)

1. Commencez à saisir le nom d’un enregistrement dans la zone de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Ou

   Sélectionnez le nom d&#39;un ou plusieurs enregistrements dans la zone, puis cliquez sur **Connecter des objets**.

   Les éléments suivants sont ajoutés :

   * Les enregistrements liés s&#39;affichent dans le champ enregistrement lié de l&#39;enregistrement que vous avez sélectionné à l&#39;étape précédente.
   * Les champs liés sont renseignés avec les informations des enregistrements liés, si vous avez ajouté des champs de recherche liés lorsque vous avez connecté les types d’enregistrement.

   La mise à jour des enregistrements liés met à jour automatiquement les champs liés pour les enregistrements à partir desquels vous effectuez la liaison. Vous ne pouvez pas modifier manuellement les champs liés.

   >[!TIP]
   >
   >* Nous utilisons de manière interchangeable « champs liés » et « champs de recherche ».
   >
   >* Lorsque vous choisissez de connecter plusieurs enregistrements lorsque vous connectez les types d&#39;enregistrements, les valeurs des champs de plusieurs objets sont affichées séparées par des virgules ou sont agrégées selon l&#39;agrégateur choisi lors de la connexion des types d&#39;enregistrements.

1. (Facultatif) Fermez la page du type enregistrement et accédez à l’espace de travail que vous avez sélectionné.
1. Cliquez sur la carte correspondant au type d’enregistrement que vous avez lié.

   Par exemple, si vous avez connecté l’enregistrement **Campagne** avec l’enregistrement Produit, cliquez sur la carte **Produit**.

   La carte de type d’enregistrement doit s’ouvrir dans la vue de tableau. Dans le cas contraire, sélectionnez une vue Tableau.

   Notez que le champ d’enregistrements liés **Campagne** affiche les noms des campagnes que vous avez liées à des produits dans la page type d’enregistrement du Produit. La mise à jour des informations de Campagne met automatiquement à jour le champ d’enregistrement lié Campagne pour le type d’enregistrement Produit.

### Connecter des enregistrements de planification Adobe Workfront à des objets Workfront depuis la vue de tableau ou l’onglet Détails de la page d’enregistrement

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

Après avoir créé une connexion entre un type d’enregistrement et un type d’objet Workfront, vous pouvez connecter des enregistrements individuels à des objets dans Workfront. Les champs Workfront que vous avez connectés sont automatiquement renseignés sur les enregistrements à partir desquels vous liez les objets.

>[!NOTE]
>
>Vous ne pouvez pas connecter les types d’objets Workfront aux types d’enregistrement Workfront Planning de Workfront.


{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dont vous souhaitez vous connecter.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.
1. Cliquez sur la vignette d’un type d’enregistrement pour ouvrir la page du type d’enregistrement.
1. Sélectionnez une vue en **Tableau** dans le menu déroulant **Affichage**.

1. Cliquez sur **Nouvel enregistrement** pour ajouter des enregistrements individuels au type d’enregistrement que vous avez sélectionné. Pour plus d’informations, consultez la section [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

1. (Conditionnel) Une fois que vous avez connecté le type d’enregistrement sélectionné à un type d’objet Workfront, accédez à la colonne d’objet lié et double-cliquez sur la cellule correspondant à l’enregistrement que vous souhaitez lier aux objets de Workfront.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur un objet de la liste pour l’ajouter à l’enregistrement sélectionné. Les objets sont répertoriés par ordre alphabétique. L’objet est ajouté automatiquement.
   * Commencez à saisir le nom d’un objet et cliquez dessus lorsqu’il s’affiche dans la liste. L’objet est ajouté automatiquement.

   >[!TIP]
   >
   >Vous pouvez ouvrir la page d’un enregistrement à partir de la vue, double-cliquer sur le champ d’enregistrement lié ou cliquer sur **Se connecter** dans le champ pour ajouter des objets du type d’objet connecté.

1. (Facultatif) Si vous ne trouvez pas d’objet à connecter et que vous souhaitez l’ajouter, cliquez sur **+ Ajouter** pour créer et ajouter un nouveau projet ou portfolio.

   Vous ne pouvez ajouter que des projets sans modèle ni portfolios lors de leur connexion aux enregistrements de planification. Vous ne pouvez pas ajouter de nouveaux programmes, groupes ou entreprises.

1. (Facultatif) Cliquez sur **Afficher tout** pour afficher tous les objets que vous avez au moins les autorisations d’afficher.

   Si vous avez cliqué sur **Afficher tout** à l’étape précédente, la zone **Se connecter aux objets** s’affiche.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Commencez à saisir le nom d’un objet Workfront dans la zone de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Ou

   Sélectionnez le nom d&#39;un ou plusieurs objets dans la zone, puis cliquez sur **Connecter des objets**.

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
   >* Lorsque vous choisissez de connecter plusieurs enregistrements lors de la connexion des types d&#39;enregistrements, les valeurs des champs de recherche sont affichées séparées par des virgules ou sont agrégées en fonction de l&#39;agrégateur que vous avez choisi.
   >
   >* Un champ d’enregistrement lié n’est pas créé pour les objets Workfront liés dans Workfront.

1. (Facultatif) Dans la vue de tableau du type d’enregistrement, pointez sur l’en-tête de colonne de l’objet Workfront lié, cliquez sur le menu déroulant, puis sur **Modifier les champs de recherche**.

1. Ajoutez des champs d’objet Workfront à partir de la zone **Champs non sélectionnés**

   Ou

   Supprimez des champs d’objet Workfront à partir de la zone **Champs sélectionnés**.

   Cela permet d’ajouter ou de supprimer des champs liés dans les enregistrements Workfront Planning. Les informations associées aux champs supprimés restent dans Workfront.


### Connecter des enregistrements de planification Workfront à des objets Adobe Experience Manager depuis la vue de tableau ou l’onglet Détails de la page d’enregistrement

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console pour pouvoir connecter des enregistrements Workfront Planning à Adobe Experience Manager Assets.
>
>Si vous avez des questions relatives à l’intégration à Adobe Admin Console, voir les [Questions fréquentes sur Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Après avoir créé une connexion entre un type d’enregistrement et Adobe Experience Manager Assets, vous pouvez connecter des enregistrements individuels à des ressources Experience Manager. Les champs de ressource que vous avez connectés à partir d’Experience Manager Assets lors de la création de la connexion sont automatiquement renseignés sur le type d’enregistrement à partir duquel vous avez créé un lien.

>[!NOTE]
>
>La planification des enregistrements et de leurs champs est accessible à partir de Experience Manager Assets lorsque votre administrateur Workfront configure le mappage des métadonnées par le biais de l’intégration entre Workfront et Adobe Experience Manager Assets. Pour plus d’informations, voir [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=fr).

Pour connecter des enregistrements à des ressources Experience Manager :

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dont vous souhaitez vous connecter.

   L’espace de travail et les types d’enregistrement s’affichent.
1. Cliquez sur la vignette d’un type d’enregistrement pour ouvrir la page du type d’enregistrement.
1. Sélectionnez une vue en **Tableau** à partir du menu déroulant **Affichage** dans le coin supérieur droit de la page du type enregistrement.

1. (Facultatif) Cliquez sur **Nouvel enregistrement** pour ajouter de nouveaux enregistrements au type d’enregistrement que vous avez sélectionné. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
1. (Conditionnel) Après avoir connecté le type d’enregistrement sélectionné à Experience Manager Assets, accédez à la colonne d’objet lié et survolez la cellule correspondant à l’enregistrement que vous souhaitez lier à d’autres objets d’Experience Manager, puis cliquez sur l’icône **+** .

   >[!TIP]
   >
   >  Vous pouvez ajouter l’icône **+** dans le champ d’objet lié de la page d’enregistrement pour connecter les ressources à l’enregistrement.

   La zone **Sélectionner les ressources** s’affiche. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

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
     >* Lorsque vous choisissez de connecter plusieurs enregistrements lors de la connexion des types d&#39;enregistrements, les valeurs de plusieurs objets s&#39;affichent séparés par des virgules ou agrégés selon l&#39;agrégateur que vous choisissez.
     >
     >* Un champ d’enregistrement lié aux enregistrements liés de Workfront Planning n’est pas créé pour les ressources de Experience Manager liées dans l’application Experience Manager Assets.

1. (Facultatif) Accédez au type d’enregistrement à partir duquel vous avez créer un lien ver Experience Manager Assets et cliquez sur le nom d’une ressource dans le champ d’enregistrement lié. Les détails Experience Manager de la ressource s’affichent dans une fenêtre contextuelle.

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

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

1. (Facultatif) Pour ouvrir la page d’enregistrement des ressources Experience Manager dans Experience Manager, accédez à la page de type d’enregistrement de l’enregistrement à partir duquel vous liez, cliquez sur le nom d’une ressource dans le champ d’enregistrement lié pour ouvrir la fenêtre contextuelle, puis cliquez sur l’icône **Ouvrir dans AEM** ![](assets/open-asset-icon.png) pour ouvrir la ressource.

   Cette opération ouvre la ressource Experience Manager dans Adobe Experience Manager Assets.

1. (Facultatif) Dans la vue Tableau du type d’enregistrement, pointez sur l’en-tête de colonne de la ressource Experience Manager liée, cliquez sur le menu déroulant, puis sur **Modifier les champs de recherche**.

1. Ajoutez des champs d’objet Experience Manager Assets à partir de la zone **Champs non sélectionnés**

   Ou

   Supprimez des champs d’objet Workfront de la zone **Champs sélectionnés**.

   Cela permet d’ajouter ou de supprimer des champs liés des enregistrements. Les informations associées aux champs supprimés restent dans Adobe Experience Assets.

### Connecter Workfront Planning des enregistrements à d’autres enregistrements ou objets depuis l’onglet Connexions de la page d’enregistrement

1. Accédez à n’importe quelle vue d’un type d’enregistrement qui a été connecté à d’autres types d’enregistrements ou d’objets Planning depuis d’autres applications.
1. Suivez les étapes décrites dans les sous-sections précédentes pour trouver un enregistrement dans la vue que vous souhaitez connecter à d’autres enregistrements ou objets.
1. Cliquez sur le nom d’un enregistrement.

   La page d’aperçu s’ouvre.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) pour ouvrir la page de l’enregistrement.
1. Cliquez sur l’onglet **Connexions** dans l’aperçu ou la page de l’enregistrement.

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

   Tous les types d’enregistrement ou d’objet liés au type d’enregistrement sélectionné s’affichent sous forme de sections. Les enregistrements ou objets connectés s’affichent sous leurs noms d’enregistrement ou de type d’objet sur les cartes.

   >[!TIP]
   >
   >    Seuls les enregistrements connectés qui possèdent des enregistrements individuels sont affichés par défaut.

1. (Facultatif) Cliquez sur **Afficher toutes les connexions** pour afficher tous les types d’enregistrements connectés, y compris ceux sans enregistrements connectés.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à gauche d’une section pour la réduire.

1. (Conditionnel) Cliquez sur **Se connecter** pour ajouter d’autres enregistrements ou objets du même type.
1. Suivez les étapes décrites dans les sections précédentes pour connecter des enregistrements de Workfront Planning ou des objets de Workfront ou Experience Manager Assets.
Les enregistrements et les objets sont ajoutés immédiatement.
1. (Facultatif) Pointez sur la carte connectée d’un enregistrement ou d’un objet, puis cliquez sur l’icône **Déconnecter l’enregistrement** ![](assets/disconnect-icon-with-tooltip.png) pour le déconnecter de l’enregistrement sélectionné.

   ![](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   L’enregistrement est immédiatement déconnecté de toutes les zones de Workfront Planning ou d’autres applications où il peut s’afficher comme connecté. Toutes les valeurs de champ de recherche sont également supprimées.

## Connexion d’enregistrements à partir d’objets Workfront

Vous devez disposer des éléments suivants pour connecter les enregistrements Workfront Planning des objets Workfront :

* Connexions entre les types d’enregistrements et les types d’objets Workfront qui sont établis dans Workfront Planning.
* L’administrateur de Workfront ou de groupe doit ajouter la section Planification aux projets, portefeuilles et programmes Workfront de votre modèle de mise en page.

Pour plus d’informations, voir [Gestion des enregistrements dans la section Planification des objets Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
