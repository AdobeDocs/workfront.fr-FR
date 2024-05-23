---
title: Connecter des enregistrements
description: Après avoir créé des connexions entre les types d’enregistrement, vous pouvez connecter des enregistrements individuels les uns aux autres.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: f042cd0466f65a7b1179026927b167ae6b208c86
workflow-type: tm+mt
source-wordcount: '2463'
ht-degree: 2%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connecter des enregistrements

{{maestro-important-intro}}

Vous pouvez connecter des enregistrements de planification Adobe Workfront les uns aux autres ou aux objets d’autres applications.

Vous devez d’abord connecter deux types d’enregistrement l’un à l’autre, ou un type d’enregistrement à un type d’objet à partir d’une autre application. Cela crée des champs d’enregistrement liés. Vous pouvez ensuite connecter des enregistrements les uns aux autres ou des enregistrements à d’autres objets à partir d’autres applications à l’aide des champs d’enregistrement liés.

La connexion d&#39;enregistrements est similaire à la connexion d&#39;enregistrements à des objets à partir d&#39;une autre application.

Pour plus d’informations sur la connexion des types d’enregistrement les uns aux autres ou sur les types d’objets d’autres applications, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

Pour un exemple de connexion des types d’enregistrement, voir [Exemple de connexion de types d&#39;enregistrements et d&#39;enregistrements](../architecture/example-connect-record-types-and-records.md).

Vous pouvez connecter les éléments suivants :

* Enregistrements de planification Adobe Workfront
* Enregistrements de planification Adobe Workfront avec des objets provenant d’autres applications.

  Vous pouvez connecter des enregistrements à des objets des types répertoriés ci-dessous à partir des applications suivantes :

   * Adobe Workfront

      * Projets
      * Portefeuilles
      * Programmes
      * Entreprise
      * Groupe

   * Adobe Experience Manager Assets

      * Fichiers image
      * Dossiers

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Pour connecter les enregistrements de planification Adobe Workfront à Experience Manager Assets, vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe. Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe d’une expérience unifiée pour Workfront</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé d’Adobe Workfront Planning. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>N’importe quelle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gérer les autorisations d’un espace de travail pour connecter des enregistrements </p>  
   <p>Afficher ou des autorisations supérieures à un espace de travail pour afficher toutes les connexions aux objets et aux champs d’autres applications, quel que soit votre accès dans une autre application. </p>
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considérations relatives à la connexion des enregistrements

* Une fois que vous avez connecté les types d’enregistrement, les types d’enregistrement connectés s’affichent sous forme de champs d’enregistrement liés dans la table des types d’enregistrement à partir desquels ils sont liés et sur les pages des enregistrements.
* Vous pouvez parcourir et ajouter des enregistrements et des objets de l’enregistrement et des types d’objets liés à partir des champs d’enregistrement liés.
* Vous pouvez ajouter des champs des types d’enregistrement liés à la table du type d’enregistrement à partir duquel vous effectuez la liaison.
* Vous ne pouvez pas mettre à jour manuellement les valeurs des champs liés sur les enregistrements à partir desquels vous effectuez la liaison.

  Les valeurs des champs liés des enregistrements liés renseignent l’enregistrement Workfront Planning à partir duquel vous effectuez une liaison automatique à partir de l’enregistrement ou de l’objet d’origine.

* Toute personne ayant accès à Workfront Planning et View ou à des autorisations supérieures de l&#39;espace de travail peut voir les connexions que vous effectuez entre des enregistrements ou entre des enregistrements et des objets d&#39;autres applications. Ils peuvent afficher les enregistrements et les objets connectés, quelles que soient leurs autorisations dans les applications auxquelles vous vous connectez.
* Vous pouvez afficher et modifier les connexions de tous les autres utilisateurs, si vous disposez des autorisations de gestion de l’espace de travail dans lequel se trouvent les enregistrements connectés.
* Vous pouvez connecter un enregistrement à un ou plusieurs objets à partir d’une autre application.
* Pour lier des enregistrements à d’autres enregistrements ou objets, vous devez disposer des éléments suivants :

   * Au moins un espace de travail, un type d’enregistrement et un enregistrement.

     Pour plus d’informations, voir les articles suivants :

      * [Créer des espaces de travail](../architecture/create-workspaces.md)
      * [Création de types d’enregistrement](../architecture/create-record-types.md)
      * [Créer des enregistrements](../records/create-records.md)

   * Connexions entre types d’enregistrement ou entre types d’enregistrement et objets d’autres applications. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md)
* Vous pouvez connecter des objets de Workfront à des enregistrements Workfront Planning dans les zones suivantes :
   * À partir d’un enregistrement de planification dans la planification Workfront.
   * Dans la section Planification d’un objet Workfront.

## Connexion d’enregistrements à partir de Workfront Planning

### Connexion aux enregistrements de planification Adobe Workfront

{{step1-to-maestro}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à partir duquel vous souhaitez connecter des enregistrements.
1. Cliquez sur la carte d’un type d’enregistrement pour ouvrir la page de type d’enregistrement.
1. Sélectionnez une **Tableau** de la vue **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.
1. (Facultatif) Ajoutez des enregistrements au type d’enregistrement que vous avez sélectionné en ajoutant une nouvelle ligne au tableau. Pour plus d’informations, voir [Créer des enregistrements](../../maestro/records/create-records.md).
1. (Conditionnel) Une fois que vous avez connecté le type d’enregistrement sélectionné à un autre type d’enregistrement, accédez à la colonne d’enregistrement lié et double-cliquez sur la cellule correspondant à l’enregistrement que vous souhaitez lier à d’autres enregistrements.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur le nom d’un enregistrement connecté dans la liste pour l’ajouter à l’enregistrement sélectionné. L’enregistrement est ajouté automatiquement.
   * Commencez à saisir le nom d’un enregistrement et cliquez dessus lorsqu’il s’affiche dans la liste. L’enregistrement est ajouté automatiquement.
   * Cliquez sur **Afficher tout** pour afficher tous les enregistrements.

1. (Conditionnel) Si vous avez cliqué sur **Tout sélectionner** à l’étape précédente, la variable **Connexion d’objets** s’affiche.

   ![](assets/connected-objects-table-for-records.png)

1. Commencez à saisir le nom d’un enregistrement dans la zone de recherche, puis sélectionnez-le à son affichage dans la liste.

   Ou

   Sélectionnez le nom d’un ou de plusieurs enregistrements dans la zone, puis cliquez sur **Connexion d’objets** dans le coin supérieur droit de la zone Connexion aux objets .

   >[!TIP]
   >
   >    Vous pouvez ouvrir la page d’un enregistrement, rechercher le champ d’enregistrement lié et cliquer sur **Connexion d’enregistrements** dans le champ pour ajouter des enregistrements de l’enregistrement connecté ou du type d’objet.
   >
   >![](assets/connect-records-from-record-page-field.png)

   Les éléments suivants sont ajoutés :

   * Les enregistrements liés s&#39;affichent dans le champ enregistrement lié de l&#39;enregistrement que vous avez sélectionné à l&#39;étape 6. <!--accurate?-->
   * Les champs liés sont renseignés avec les informations des enregistrements liés, si vous avez ajouté des champs de recherche liés lorsque vous avez connecté les types d&#39;enregistrements.

   La mise à jour des enregistrements liés met à jour automatiquement les champs liés pour les enregistrements à partir desquels vous effectuez la liaison. Vous ne pouvez pas modifier manuellement les champs liés.

   >[!TIP]
   >
   >* Nous utilisons de manière interchangeable les &quot;champs liés&quot; et &quot;champs de recherche&quot;.
   >
   >* Si vous avez activé la variable **Autoriser plusieurs enregistrements** lorsque vous connectez les types d&#39;enregistrements, les valeurs des champs des multiples objets sélectionnés sont affichées séparées par des virgules ou sont agrégées selon l&#39;agrégateur que vous avez choisi.

1. (Facultatif) Fermez la page de type enregistrement et accédez à l’espace de travail que vous avez sélectionné.
1. Cliquez sur la carte correspondant au type d’enregistrement auquel vous avez lié.

   Par exemple, si vous avez connecté la variable **Campagne** Enregistrez avec l’enregistrement de produit, cliquez sur le bouton **Produit** carte.

   La carte de type d’enregistrement doit s’ouvrir dans la vue Tableau. Dans le cas contraire, sélectionnez une vue de tableau.

   Notez que la variable **Campagne** le champ enregistrement lié affiche les noms des campagnes auxquelles vous avez lié des produits dans la page Type d’enregistrement de produit . La mise à jour des informations de Campaign met automatiquement à jour le champ d’enregistrement lié à Campaign pour le type d’enregistrement Produit .

### Connexion des enregistrements de planification Adobe Workfront aux objets Workfront

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

Après avoir créé une connexion entre un type d’enregistrement et un type d’objet Workfront, vous pouvez connecter des enregistrements individuels à des objets dans Workfront. Les champs Workfront que vous avez connectés sont automatiquement renseignés sur les enregistrements à partir desquels vous liez les objets.

>[!NOTE]
>
>Vous ne pouvez pas connecter les types d’objets Workfront aux types d’enregistrement Workfront Planning de Workfront.


{{step1-to-maestro}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à partir duquel vous souhaitez connecter des enregistrements.
1. Cliquez sur la carte d’un type d’enregistrement pour ouvrir la page de type d’enregistrement.
1. Sélectionnez une **Tableau** de la vue **Affichage** menu déroulant.

1. Cliquez sur **Nouvel enregistrement**  pour ajouter des enregistrements individuels au type d’enregistrement que vous avez sélectionné. Pour plus d’informations, voir [Créer des enregistrements](../../maestro/records/create-records.md).
1. (Conditionnel) Une fois que vous avez connecté le type d’enregistrement sélectionné à un type d’objet Workfront, accédez à la colonne d’objet lié et double-cliquez sur la cellule correspondant à l’enregistrement que vous souhaitez lier aux objets de Workfront.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur un objet de la liste pour l’ajouter à l’enregistrement sélectionné. Les objets sont répertoriés par ordre alphabétique. L’objet est ajouté automatiquement.
   * Commencez à saisir le nom d’un objet et cliquez dessus lorsqu’il s’affiche dans la liste. L’objet est ajouté automatiquement.
   * Cliquez sur **Afficher tout** pour afficher tous les objets que vous disposez au moins des autorisations nécessaires.

1. (Conditionnel) Si vous avez cliqué sur **Afficher tout** à l’étape précédente, la variable **Connexion d’objets** s’affiche.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Commencez à saisir le nom d’un objet Workfront dans la zone de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Ou

   Sélectionnez le nom d’un ou de plusieurs objets dans la zone, puis cliquez sur **Connexion d’objets** dans le coin supérieur droit de la zone Connexion aux objets .

   >[!IMPORTANT]
   >
   >* Vous pouvez uniquement ajouter des objets Workfront que vous avez accès à la vue.
   >
   >* Une fois que vous avez ajouté des objets Workfront, toutes les personnes disposant d’autorisations de vue ou supérieures à l’espace de travail peuvent afficher les objets Workfront et leurs informations de champ, indépendamment de leurs autorisations ou de leur accès dans Workfront.

   Les éléments suivants sont ajoutés :

   * Les objets Workfront sélectionnés sont ajoutés au champ d’enregistrement associé.
   * Si vous les avez ajoutés lorsque vous avez connecté le type d’enregistrement à Workfront, les champs liés (ou les champs de recherche) des objets Workfront sont automatiquement renseignés avec les informations de Workfront.

   >[!TIP]
   >
   >Vous pouvez ouvrir la page d’un enregistrement, rechercher le champ d’enregistrement lié et cliquer sur le bouton **+** dans le champ pour ajouter des objets du type d’objet connecté.

   Pour plus d’informations sur la connexion des types d’enregistrement aux objets d’une autre application, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

1. (Facultatif) Cliquez sur le nom d’un objet Workfront connecté à un enregistrement Workfront Planning dans le champ lié d’une vue de table ou dans le champ lié de la page d’enregistrement.

   Cela ouvre la page d’enregistrement de la planification Workfront en lecture seule pour l’objet Workfront lié. Les champs que vous avez sélectionnés comme champs de recherche lorsque vous avez connecté le type d’enregistrement à l’objet Workfront s’affichent dans la page d’enregistrement de Workfront Planning.

   >[!TIP]
   >
   >* Lorsque vous activez le paramètre Autoriser plusieurs enregistrements , les valeurs des champs de recherche sont affichées séparées par des virgules ou sont agrégées selon l&#39;agrégateur que vous avez choisi.
   >
   >* Un champ d’enregistrement lié n’est pas créé pour les objets Workfront liés dans Workfront.

1. (Facultatif) Pour ouvrir l’objet Workfront lié dans Workfront, cliquez sur **Accéder à la source** dans le coin supérieur droit de la page d’enregistrement de l’objet Workfront.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Cette opération ouvre la page d’objet Workfront, si vous disposez au moins des autorisations de vue pour afficher l’objet. Si vous êtes autorisé à le faire, vous pouvez modifier les informations relatives à l’objet Workfront.

1. (Facultatif) Dans la vue Tableau du type d’enregistrement, passez la souris sur l’en-tête de colonne de l’objet Workfront lié, cliquez sur le menu déroulant, puis cliquez sur **Modifier les champs de recherche**.

1. Ajoutez des champs d’objet Workfront à partir du **Champs non sélectionnés** area

   Ou

   Suppression des champs d’objet Workfront du **Champs sélectionnés** zone.

   Cela permet d’ajouter ou de supprimer des champs liés dans les enregistrements de planification Workfront. Les informations associées aux champs supprimés restent dans Workfront.


### Connexion des enregistrements de planification Workfront aux objets Adobe Experience Manager

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>Vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance de Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console pour pouvoir connecter les enregistrements Workfront Planning à Adobe Experience Manager Assets.
>
>Si vous avez des questions sur l’intégration à Adobe Admin Console, reportez-vous à la section [FAQ sur l’expérience unifiée Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Après avoir créé une connexion entre un type d’enregistrement et Adobe Experience Manager Assets, vous pouvez connecter des enregistrements individuels à des ressources du Experience Manager. Les champs de ressource que vous avez connectés à partir de Experience Manager Assets lors de la création de la connexion sont automatiquement renseignés sur le type d’enregistrement à partir duquel vous avez créé un lien.

{{step1-to-maestro}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à partir duquel vous souhaitez connecter des enregistrements.
1. Cliquez sur la carte d’un type d’enregistrement pour ouvrir la page de type d’enregistrement.
1. Sélectionnez une **Tableau** de la vue **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.

1. (Facultatif) Cliquez sur **Nouvel enregistrement** pour ajouter de nouveaux enregistrements au type d’enregistrement que vous avez sélectionné. Pour plus d’informations, voir [Créer des enregistrements](../../maestro/records/create-records.md).
1. (Conditionnel) Une fois que vous avez connecté le type d’enregistrement sélectionné à Experience Manager Assets, accédez à la colonne d’objet lié et survolez la cellule correspondant à l’enregistrement que vous souhaitez lier à d’autres objets de Experience Manager, puis cliquez sur le bouton **+** Icône

   >[!TIP]
   >
   >  Vous pouvez ajouter des **+** dans le champ d’objet lié de la page d’enregistrement pour connecter les ressources à l’enregistrement.

   La variable **Sélectionner les ressources** s’affiche. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. Cliquez sur pour sélectionner certains des types de ressources suivants :

   * Images
   * Dossiers

   Vous pouvez sélectionner plusieurs ressources.

   >[!IMPORTANT]
   >
   > Vous pouvez connecter uniquement les ressources que vous avez accès à afficher dans Experience Manager. Une fois connecté, tous les utilisateurs de la planification Workfront peuvent afficher les ressources dans la planification Workfront, quel que soit leur accès dans Experience Manager Assets.

1. Cliquez sur **Sélectionner**. <!-- we might change this to Connect-->

   Les éléments suivants sont ajoutés :

   * Les ressources de Experience Manager sélectionnées sont ajoutées au champ d’enregistrement lié.
   * Les champs liés (ou champs de recherche) sont renseignés avec les informations des ressources connectées au Experience Manager.

     Toutes les informations existantes provenant des champs des ressources du Experience Manager s’affichent automatiquement dans les champs liés ou de recherche.

     >[!TIP]
     >
     >* Si vous avez activé le paramètre Autoriser plusieurs enregistrements , les valeurs de plusieurs objets s’affichent soit séparées par des virgules, soit agrégées selon l’agrégateur choisi.
     >
     >* Un champ d’enregistrement lié aux enregistrements liés de la planification Workfront n’est pas créé pour les ressources de Experience Manager liées dans l’application Experience Manager Assets.

1. (Facultatif) Accédez au type d’enregistrement à partir duquel vous avez lié Experience Manager Assets et cliquez sur le nom d’une ressource dans le champ d’enregistrement lié. Les détails du Experience Manager de la ressource s’affichent dans une fenêtre contextuelle. <!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Les champs suivants s’affichent pour un fichier image :

   * Une miniature de l’image
   * Nom du fichier image
   * Dimensions
   * Taille
   * Description
   * Chemin d’accès au fichier en Experience Manager
   * Type de ressource
   * Date de création
   * Date de modification

1. (Facultatif) Pour ouvrir la page d’enregistrement des ressources du Experience Manager dans Experience Manager, accédez à la page de type d’enregistrement de l’enregistrement à partir duquel vous créez un lien, cliquez sur le nom d’une ressource dans le champ d’enregistrement lié pour ouvrir la fenêtre contextuelle, puis cliquez sur le bouton **Ouvrir** icon ![](assets/open-asset-icon.png) pour ouvrir la ressource.

   Cette opération ouvre la ressource du Experience Manager dans Adobe Experience Manager Assets.

1. (Facultatif) Dans la vue Tableau du type d’enregistrement, passez la souris sur l’en-tête de colonne de la ressource de Experience Manager liée, cliquez sur le menu déroulant, puis sur **Modifier les champs de recherche**.

1. Ajoutez des champs d’objet Experience Manager Assets à partir du **Champs non sélectionnés** area

   Ou

   Suppression des champs d’objet Workfront du **Champs sélectionnés** zone.

   Cela permet d&#39;ajouter ou de supprimer des champs liés des enregistrements. Les informations associées aux champs supprimés restent dans Adobe Experience Assets.

## Connexion d’enregistrements à partir d’objets Workfront

Vous devez disposer des éléments suivants pour connecter les enregistrements Workfront Planning des objets Workfront :

* Connexions entre les types d’enregistrement et les types d’objets Workforce.
* Au moins une connexion entre un enregistrement et un objet Workfront.
* L’administrateur de Workfront ou de groupe doit ajouter la section Planification aux types d’objets Workfront qui peuvent se connecter à des types d’enregistrements Planification .

Pour plus d’informations, voir [Gestion des enregistrements dans la section Planification des objets Adobe Workfront](/help/quicksilver/maestro/records/manage-records-in-planning-section.md).
