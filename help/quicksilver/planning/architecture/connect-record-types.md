---
title: Connexion à des types d’enregistrement
description: Une façon d’indiquer comment les types d’enregistrements individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrements Adobe Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et utilisatrices et de garder leur attention sur une seule application.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '2196'
ht-degree: 44%

---


# Connecter des types d’enregistrements

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Vous pouvez connecter des types d’enregistrement les uns aux autres ou connecter des types d’enregistrement à des types d’objets provenant d’autres applications.

Cet article décrit comment vous pouvez connecter deux types d’enregistrement Workfront Planning ou un type d’enregistrement Workfront Planning à un objet provenant d’une autre application.

Après avoir établi la connexion entre les enregistrements ou les types d’objets, vous pouvez connecter des enregistrements individuels les uns aux autres et afficher les champs de l’enregistrement ou des types d’objets liés sur un enregistrement Workfront Planning.

Pour des informations générales sur les types de connexions, voir [Présentation des types d’enregistrements connectés](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Pour plus d&#39;informations sur la connexion d&#39;enregistrements ou d&#39;enregistrements avec des objets provenant d&#39;autres applications, voir [Connexion d&#39;enregistrements](/help/quicksilver/planning/records/connect-records.md).

Pour un exemple de connexion de types d&#39;enregistrements et d&#39;enregistrements, voir [Exemple de connexion de types d&#39;enregistrements et d&#39;enregistrements](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Pour pouvoir accéder à Workfront Planning, vous devez disposer des éléments suivants :

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
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
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
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td> 
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
   <td> <p>Standard</p> 
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
   <td>   <p>Autorisations de gestion pour un espace de travail</a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Tous les utilisateurs, y compris les administrateurs Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planification dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Connecter les types d’enregistrements

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dont vous souhaitez vous connecter aux types d&#39;enregistrements,

   Ou

   Dans un espace de travail, développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.
1. Cliquez sur la vignette d’un type d’enregistrement pour ouvrir la page du type d’enregistrement.
1. Cliquez sur l’icône **+** dans le coin supérieur droit de la vue tableau, puis cliquez sur l’onglet **Nouvelle connexion**.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Dans le champ **Type d’enregistrement**, recherchez un type d’enregistrement ou sélectionnez l’un des éléments suivants :

   * Autre type d’enregistrement de l’espace de travail actuel

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>
     >[!TIP]
     >
     > 
     >Si vous n’avez pas d’autres types d’enregistrements dans l’espace de travail sélectionné, la section de l’espace de travail ne s’affiche pas.


   * Type d’enregistrement d’un autre espace de travail configuré pour se connecter à partir d’autres espaces de travail. Pour plus d’informations, voir [Modification des types d’enregistrement](/help/quicksilver/planning/architecture/edit-record-types.md).

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

     >[!TIP]
     >
     >Si aucun type d’enregistrement n’est configuré pour se connecter à partir d’autres espaces de travail, la section espace de travail ne s’affiche pas.


   * Un **projet, un portfolio, un programme, une entreprise** ou un **groupe** depuis la section **Types d’objets Workfront**.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** depuis la section **Adobe Applications**.

     <span class="preview">![](assets/aem-assets-connection-selection.png)</span>

1. Mettez à jour les informations suivantes :

   * **Nom** : nom du champ connecté, tel qu’il apparaît dans la vue Tableau ou la page de l’enregistrement original. Cela crée la colonne des enregistrements liés dans la vue table du type d&#39;enregistrement d&#39;origine ou du champ d&#39;enregistrement lié pour les enregistrements d&#39;origine. Par défaut, le nom du champ correspond au nom de l’enregistrement ou de l’objet auquel vous vous connectez.

   >[!TIP]
   >
   >Vous pouvez avoir plusieurs connexions au même type d’enregistrement ou d’objet. Si vous ne modifiez pas le nom du champ connecté, Workfront ajoute un nombre après le nom de l’enregistrement connecté, afin d’indiquer le nombre de types d’enregistrements connectés par le même nom.

   * **Description** : informations supplémentaires sur le champ de l’enregistrement connecté. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Autoriser plusieurs enregistrements** : sélectionnez cette option pour indiquer que vous autorisez les utilisateurs à ajouter plusieurs enregistrements lorsque le champ de type d’enregistrement associé s’affiche sur les enregistrements d’origine. Cette option est sélectionnée par défaut.

     Cette option est disponible uniquement lors de la connexion d’enregistrements provenant de deux espaces de travail différents ou d’un enregistrement et d’un objet de ressource Adobe Experience Manager.

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

   * **Type de connexion** : sélectionnez l’une des options suivantes pour indiquer le nombre d’enregistrements auxquels ils peuvent se connecter et à partir de :

      * Multiple-à-multiple
      * Un-à-multiple
      * Multiple-à-un
      * Un-à-un

     Cette option est disponible uniquement lors de la connexion d’enregistrements du même espace de travail ou d’un enregistrement et d’un type d’objet Workfront.

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>

     Pour plus d’informations sur les types de connexions, voir [Présentation des types d’enregistrements connectés](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Sélectionner les champs de recherche** : sélectionnez cette option pour ajouter les champs du type d’enregistrement sélectionné. Les champs de recherche sont des champs associés au type d’enregistrement ou d’objet vers lequel vous établissez un lien. Leur liaison affiche des informations sur l’enregistrement ou l’objet auquel vous créez un lien dans l’enregistrement à partir duquel vous créez un lien. Cette option est sélectionnée par défaut.

     >[!TIP]
     >
     > Vous ne pouvez pas ajouter les types de champ suivants comme champs de recherche :
     >
     >    * Personnes
     >    * Créé par
     >    * Dernière modification par
     >    * Champs de saisie anticipée Workfront (y compris les champs tels que Propriétaire du projet ou Parrain du projet)

1. (Le cas échéant et facultatif) Si vous avez choisi de connecter un objet Workfront, sélectionnez un **Formulaire personnalisé** dans la section **Lier uniquement les objets correspondant à ces critères**. Seuls les objets auxquels sont attachés les formulaires personnalisés sélectionnés peuvent être liés au type d’enregistrement sélectionné. Vous pouvez sélectionner plusieurs formulaires.

   >[!NOTE]
   >
   > Vous devez créer des formulaires personnalisés dans Workfront pour les objets sélectionnés avant qu’ils ne s’affichent dans cette liste.

1. (Le cas échéant) Si vous avez choisi de vous connecter à Experience Manager Assets, sélectionnez un référentiel dans le menu déroulant **Référentiel Experience Manager** dans la section **Lier des ressources à partir du référentiel suivant**. Champ obligatoire. Seuls les référentiels auxquels vous avez accès dans Experience Manager Assets s’affichent dans ce champ.

   >[!NOTE]
   >
   >Votre administrateur Workfront peut mapper les champs de planification Workfront aux champs Experience Manager Assets par le biais du mappage des métadonnées dans Workfront. Pour plus d’informations, voir [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=fr).

1. (Conditionnel) Si vous avez choisi de vous connecter à Experience Manager Assets ou à un type d’enregistrement Workfront Planning, sélectionnez l’une des options suivantes dans la zone **Apparence d’enregistrement** :

   * <span class="preview">**Nom et image** : le nom et la miniature ou l’icône des enregistrements connectés s’affichent dans le champ d’enregistrement connecté. Il s’agit de l’option par défaut. </span>
   * <span class="preview">**Nom** : seul le nom des enregistrements connectés s’affichera dans le champ d’enregistrement connecté.</span>
   * <span class="preview">**Image** : seule la miniature ou l’icône des enregistrements connectés s’affichera dans le champ d’enregistrement connecté.</span>

   Les enregistrements sans miniature affichent à la place l’icône de type d’enregistrement . Un exemple d’affichage des enregistrements connectés s’affiche dans la zone **Apparence des enregistrements**.

   >[!TIP]
   >
   >    Lorsque vous autorisez le lien de plusieurs enregistrements, l’affichage de la miniature peut économiser de l’espace dans des zones plus petites, comme les vues d’enregistrement.
   >
   >Le nom d’un enregistrement est le champ principal de l’enregistrement. Pour plus d’informations, voir [Présentation des champs de Principal](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >La sélection d’un aspect d’enregistrement n’est pas disponible lors de la sélection de types d’objets Workfront.

1. Cliquez sur **Créer**.

1. (Le cas échéant) Si vous avez sélectionné le paramètre **Sélectionner des champs de recherche**, la boîte de dialogue **Ajouter des champs de recherche** s’ouvre.

   Cliquez sur l’icône **+** pour ajouter des champs à partir de la zone **Champs non sélectionnés**.

   Ou

   Cliquez sur l’icône **-** pour supprimer des champs de la zone **Champs sélectionnés**.

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Les valeurs des champs connectés se remplissent automatiquement lorsque vous liez des enregistrements ou des objets.

   >[!IMPORTANT]
   >
   >    Toute personne disposant d’autorisations Afficher ou d’autorisations supérieures dans l’espace de travail peut consulter les informations contenues dans les champs liés, quels que soient ses autorisations ou son niveau d’accès dans l’application des types d’objets liés.


1. (Facultatif) Cliquez sur **Ignorer** pour ignorer l’ajout de champs à partir de l’enregistrement ou du type d’objet lié. Le champ nom ou Principal de l&#39;enregistrement lié est le seul champ visible dans la vue table du type d&#39;enregistrement à partir duquel vous vous connectez.

1. (Facultatif et conditionnel) Si vous choisissez de lier un champ de type nombre, devise, pourcentage ou date, sélectionnez également une valeur d’agrégateur pour résumer plusieurs valeurs. Les valeurs des champs liés s&#39;affichent soit séparés par des virgules, soit sous la forme d&#39;une valeur résumée selon l&#39;agrégateur que vous choisissez, lorsque les utilisateurs sélectionnent plusieurs enregistrements liés dans le champ d&#39;enregistrement lié.

   Si le champ de recherche contient plusieurs valeurs qui ne sont pas résumées, tenez compte des points suivants lorsque vous utilisez le champ pour trier ou regrouper dans une vue :

   * Le tri est effectué par la première valeur

   * Les enregistrements sont regroupés selon chaque combinaison unique de valeurs de champ.

   * La vue de la chronologie est basée sur la première valeur de date.

   >[!IMPORTANT]
   >
   >    Vous devez sélectionner une valeur d’agrégateur lors de l’ajout de champs de date de recherche si vous souhaitez que les champs soient disponibles à ajouter en tant que dates de début et de fin pour les vues de chronologie et de calendrier. Par exemple, vous pouvez sélectionner le MAX ou l’agrégateur MIN pour un champ de date de recherche.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Les agrégateurs ne sont pas disponibles lors de la connexion des types d’enregistrements à Experience Manager Assets.

   Sélectionnez l’une des options suivantes :

   * **Aucun** : affiche les valeurs provenant de plusieurs enregistrements séparés par des virgules. Il s’agit de la sélection par défaut.
   * **MAX** : affiche la valeur la plus élevée de toutes les valeurs provenant de plusieurs enregistrements sélectionnés dans le champ de l’enregistrement lié.
   * **MIN** : affiche la valeur la plus basse de toutes les valeurs provenant de plusieurs enregistrements sélectionnés dans le champ de l’enregistrement lié.
   * **SOMME** : affiche le total de toutes les valeurs provenant de plusieurs enregistrements sélectionnés dans le champ de l’enregistrement lié.
   * **MOY** : affiche la moyenne de toutes les valeurs provenant de plusieurs enregistrements sélectionnés dans le champ de l’enregistrement lié.
   * **UNIQUE** : supprime les doublons des valeurs de champ de recherche et n’affiche que les valeurs uniques. Cette option n’est pas disponible pour les types de champ suivants :
      * Paragraphe
      * Case à cocher
      * Personnes

   >[!NOTE]
   >
   >Par exemple, vous pouvez lier l’enregistrement de produit (enregistrement lié) à partir de l’enregistrement de campagne (enregistrement d’origine) et le nommer &quot;champ de produit&quot;. Vous pouvez également choisir de lier le champ Budget de l’enregistrement de produit à partir de l’enregistrement de campagne et de l’appeler &quot;Budget du produit&quot;. Si vous avez autorisé la sélection de plusieurs enregistrements dans le &quot;champ Produit&quot;, vous pouvez sélectionner le Produit 1 dont le budget est de 100 000 € et le Produit 2 dont le budget est de 110 000 €, et le Produit 3 dont le budget est de 100 000 €. Selon l’agrégateur que vous avez choisi, vous pouvez consulter les informations suivantes sur le budget dans le champ lié de l’enregistrement original :
   >
   >* **Aucun** : 100 000 $, 110 000 $, 100 000 $
   >* **MAX** : 110 000 $
   >* **MIN** : 100 000 $
   >* **SUM** : 310 000 $
   >* **AVG** : 103 000,33 $
   >* **UNIQUE** : 100 000 $
   >

1. (Facultatif) Utilisez l’icône **Rechercher** ![](assets/search-icon.png) pour rechercher un champ.

1. Cliquez sur **Ajouter des champs** pour enregistrer vos modifications.

   Les éléments suivants sont ajoutés :

   * Un champ de l’enregistrement lié sur le type d’enregistrement à partir duquel vous créez un lien. Le champ d’enregistrement lié affichera les enregistrements individuels du type d’enregistrement lié, après les avoir ajoutés manuellement. Pour plus d’informations sur l’ajout d’enregistrements, voir [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md). Le nom du champ de l’enregistrement lié est celui que vous avez sélectionné à l’étape 6.<!--accurate-->

   * Champ (ou champ) lié(e) qui affiche des informations sur l’enregistrement ou les types d’objet liés après avoir ajouté manuellement les enregistrements ou les objets dans le champ d’enregistrement lié. Les champs de recherche ne sont créés que lorsque le paramètre **Sélectionner les champs de recherche** est sélectionné lors de la création de la connexion. Les champs de recherche sont automatiquement nommés selon ce modèle :

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Par exemple, si vous avez lié un type d’enregistrement Campaign à un type d’enregistrement Program et que vous nommez le champ d’enregistrement associé au programme &quot;Informations sur le programme&quot;, puis que vous sélectionnez ce champ pour afficher également le champ Budget du programme dans la vue de table de la campagne, le champ lié est automatiquement nommé `Budget (from Program information)` dans la vue de table de la campagne.

   * Lorsque vous liez des types d’enregistrement les uns aux autres, un champ d’enregistrement lié est également ajouté au type d’enregistrement auquel vous liez l’enregistrement. Le nom du champ d’enregistrement lié sur le type d’enregistrement lié correspond au nom du type d’enregistrement à partir duquel vous créez un lien.

     Par exemple, si vous associez le type d’enregistrement &quot;Produit&quot; du type d’enregistrement &quot;Campagne&quot; et que vous avez nommé le champ connecté de la campagne &quot;Produit lié&quot;, un champ d’enregistrement lié &quot;Campagne&quot; est créé pour le type d’enregistrement Produit .

     >[!TIP]
     >
     > Un champ d’enregistrement lié n’est pas créé pour les objets d’une autre application vers le type d’enregistrement que vous liez dans Workfront Planning.

1. (Facultatif et le cas échéant) À partir de la vue de tableau du type d’enregistrement d’origine ou d’enregistrement lié, cliquez sur la flèche du bas dans l’en-tête des champs d’enregistrement liés, puis sélectionnez l’une des options suivantes :

   * **Modifier le champ** : mettez à jour le **nom** et les informations **Description** du champ.
   * **Modifier les champs de recherche** : ajoutez ou supprimez un ou plusieurs champs de l’enregistrement lié.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Pour ajouter ou supprimer des champs de recherche, suivez les instructions des étapes 16 à 17 ci-dessus. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Vous ne pouvez pas ajouter de champ de recherche appartenant à des types d’enregistrement que vous liez à des types d’objets provenant d’une autre application.
   >
   > Par exemple, vous ne pouvez pas ajouter le champ de recherche « Statut de la campagne » à un projet Workfront à partir duquel vous créez un lien vers les campagnes.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas dans l’en-tête d’un champ d’enregistrement lié ou dans l’en-tête d’un champ de recherche du type d’enregistrement à partir duquel vous créez un lien, puis cliquez sur **Supprimer**.

   Le champ d’enregistrement ou le champ de recherche est supprimé. Si vous supprimez un champ d’enregistrement, tous les champs de recherche associés à l’enregistrement lié sont également supprimés.
