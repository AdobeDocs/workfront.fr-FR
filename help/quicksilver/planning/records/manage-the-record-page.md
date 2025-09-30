---
title: Gestion de la mise en page des enregistrements
description: Vous pouvez modifier la disposition de la page et de l’aperçu de l’enregistrement dans Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 03c1f17504846fc4b8c4114ddc32df687281bc07
workflow-type: tm+mt
source-wordcount: '2308'
ht-degree: 7%

---


# Gérer la mise en page de la page d’enregistrement

<span class="preview">Les informations mises en évidence sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles pour tous. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez modifier la disposition de la page et de l’aperçu de l’enregistrement dans Adobe Workfront Planning.

La prévisualisation d’enregistrement est une vue plus petite de la page d’enregistrement qui s’affiche dans la vue d’un type d’enregistrement.

Lorsque vous modifiez la disposition d&#39;un aperçu d&#39;enregistrement et d&#39;une page, les modifications affectent les zones d&#39;aperçu et les pages de détails de tous les enregistrements du même type.

Cet article décrit comment modifier la disposition et l&#39;aspect d&#39;une zone d&#39;aperçu d&#39;enregistrement ou d&#39;une page d&#39;enregistrement. Pour plus d’informations sur la modification des enregistrements, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

Vous devez créer des types d&#39;enregistrements et des enregistrements avant de pouvoir commencer à modifier les pages d&#39;enregistrement.

Pour plus d’informations, voir les articles suivants :

* [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md)

* [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès. 

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
<p>L’un des plans Workfront suivants :</p>
<ul><li>Sélectionner</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p>
   </td>

<tr>
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td>
   <td>
<p>Tous</p>
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <p>Autorisations de niveau Contribution ou supérieur à un espace de travail et type d’enregistrement </a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> 
  </td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considérations relatives à la modification des pages d’enregistrement

* Par défaut, les détails et les pages de prévisualisation d&#39;un enregistrement affichent tous les champs associés à l&#39;enregistrement.

* Vous ne pouvez pas ajouter de nouveaux champs pour un enregistrement dans la page de prévisualisation ou de détails. Vous devez ajouter de nouveaux champs en mode Tableau pour les afficher dans les pages de prévisualisation et de détails.

* Vous pouvez ajouter des sections à une page d’aperçu d’enregistrement ou de détails, afin d’organiser les informations selon des critères communs et de les retrouver plus facilement.

* Les modifications suivantes affectent tous les enregistrements du même type et sont visibles par tous les utilisateurs qui accèdent à ces enregistrements :

   * Réorganisation des champs
   * Ajout ou suppression de sections

* Les modifications d’affichage effectuées dans la prévisualisation de l’enregistrement sont immédiatement visibles dans la page des détails de l’enregistrement. Les modifications apportées à la page d’enregistrement sont également visibles dans la zone d’aperçu de l’enregistrement.

* L’ajout d’une image de couverture ou d’une miniature à un enregistrement ne fait pas partie de la mise en page globale de l’aperçu de l’enregistrement ou de la page. Vous pouvez ajouter des images de couverture ou des miniatures uniques à chaque enregistrement. Pour plus d’informations, voir [Ajouter une image de couverture à un enregistrement](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) et [Ajouter une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Ajouter des sections à un aperçu d’enregistrement ou à une page

Tenez compte des points suivants lors de l’ajout de sections à une page d’enregistrement :

* Le nombre de sections que vous pouvez avoir sur une page n’est pas limité.
* Une section ne peut pas être vide. Vous devez avoir au moins un champ dans une section.
* Vous pouvez faire glisser des champs d’une section à une autre. Pour plus d’informations, consultez la section [Réorganiser les champs dans la page de prévisualisation des enregistrements ou de détails](#rearrange-fields-in-the-record-preview-or-details-page) dans cet article.
* Lorsque vous supprimez tous les champs d’une section, celle-ci est automatiquement supprimée et ne peut pas être récupérée.

Pour ajouter une section à une prévisualisation d’enregistrement ou à une page :

{{step1-to-planning}}

1. Cliquez sur la vignette d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page du type d’enregistrement s’ouvre.

1. Dans une vue de tout type, cliquez sur le nom d’un enregistrement.

   Ou

   Dans la vue du tableau, cliquez sur l’icône **Ouvrir les détails** ![Icône Ouvrir les détails dans le champ du nom du tableau](assets/open-details-icon-in-table-name-field.png) dans la première colonne.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![Zone Détails](assets/details-box.png)

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![Ouvrir les détails dans une nouvelle icône d’onglet](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page d’enregistrement s’ouvre. L’onglet Détails s’ouvre par défaut.

   ![Page de détails](assets/details-page.png)

1. Dans l’onglet **Détails** de l’aperçu de l’enregistrement ou de la page, passez le curseur sur l’espace blanc à gauche des champs, puis cliquez sur l’icône **Ajouter une section** ![Icône Ajouter une section](assets/add-section-icon.png) pour ajouter une section.
1. Cliquez dans le nom de la section et remplacez **Section sans titre** par un nom, puis cliquez sur Entrée. Les champs affichés sous la section font automatiquement partie de la nouvelle section.
1. Commencez à faire glisser et à déposer des champs dans la nouvelle section, comme décrit dans la section [Réorganiser les champs dans la page d’aperçu d’enregistrement ou de détails](#rearrange-fields-in-the-record-preview-or-details-page) dans cet article.

1. (Facultatif) Passez la souris sur le nom d’une section et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png).

   ![Autres options de menu pour la section sur la page d’enregistrement](assets/more-menu-options-for-section-on-record-page.png)
1. (Facultatif) Effectuez l’une des opérations suivantes pour modifier la section :

   * Cliquez sur **Renommer** pour renommer la section

     >[!TIP]
     >
     > Vous pouvez renommer une section en ligne en cliquant sur son nom.

   * Cliquez sur **Déplacer vers le haut** pour déplacer la section d&#39;une position vers le haut

     Ou

     Cliquez sur **Déplacer vers le bas** pour déplacer la section d’une position vers le bas.
Tous les champs de la section se déplacent avec la section.

   * Cliquez sur **Supprimer** pour supprimer la section. La section est supprimée et ne peut pas être récupérée. Tous les utilisateurs accédant aux enregistrements de ce type ne verront plus la section supprimée.

1. Cliquez sur la flèche pointant vers le bas à gauche d&#39;un nom de section pour le réduire ou sur la flèche pointant vers la droite pour le développer.
Toutes les sections sont développées par défaut.

1. (Facultatif) Cliquez sur l’icône **saisir** ![saisir](assets/grab-icon.png) à gauche d’un nom de section, puis faites-la glisser et déposez-la à l’endroit souhaité.

   La nouvelle position de la section est mise à jour dans l’aperçu et la page de tous les enregistrements du même type pour tous les utilisateurs qui consultent les enregistrements.

   Toutes les modifications apportées aux sections et à l’ordre des champs sont enregistrées automatiquement.

1. (Facultatif) Cliquez sur le menu **Exporter** ![icône Exporter dans la page des détails de l’enregistrement](assets/export-icon-in-record-details-page.png) pour exporter l’onglet Détails vers un fichier Word ou PDF. Pour plus d’informations, voir [Exporter les détails d’un enregistrement](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Facultatif) Cliquez sur l’onglet **Connexions** en regard de l’onglet **Détails**. Vous devrez peut-être cliquer sur **Plus** avant de cliquer sur l’onglet **Connexions**.

   Tous les enregistrements ou objets connectés à l’enregistrement sélectionné s’affichent sous les noms du type d’enregistrement ou de l’application à laquelle ils appartiennent.

   ![Onglet Connexions enregistré dans Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Facultatif) Sélectionnez le paramètre **Afficher tous les enregistrements** dans le coin supérieur droit de l’onglet Connexions. Tous les types d’enregistrements connectés s’affichent, y compris ceux qui n’ont pas encore d’enregistrements connectés. Par défaut, le bouton (bascule) est désélectionné et les types d’enregistrements sans enregistrements connectés sont masqués.

1. (Facultatif) Cliquez sur **Connexion** pour ajouter d’autres enregistrements aux types d’enregistrements connectés. Pour plus d’informations, consultez [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).

1. (Facultatif) Pointez sur une carte d’enregistrement, puis cliquez sur l’icône Déconnecter l’enregistrement **-**, puis sur **Déconnecter**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Voici ce qui se produit :
   * L’enregistrement n’est plus connecté à l’objet Workfront.
   * L’objet Workfront est également supprimé du champ connecté de l’enregistrement dans Workfront Planning.
   * Les valeurs des champs de recherche Workfront liés à l&#39;enregistrement Planning sont également supprimées.

## Réorganiser les champs dans l’onglet Détails de l’enregistrement

{{step1-to-planning}}

1. Cliquez sur la vignette d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page du type d’enregistrement s’ouvre.

1. Dans une vue de tout type, cliquez sur le nom d’un enregistrement.

   Ou

   Dans la vue du tableau, cliquez sur l’icône **Ouvrir les détails** ![Icône Ouvrir les détails dans le champ du nom du tableau](assets/open-details-icon-in-table-name-field.png) dans la première colonne.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![Zone Détails](assets/details-box.png)

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![Ouvrir la zone des détails dans une icône d’un nouvel onglet](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   L’onglet **Détails** de l’enregistrement s’ouvre par défaut.

   ![Page de détails](assets/details-page.png)

1. Dans l’onglet Enregistrement **Détails**, cliquez sur l’icône **saisir** ![Icône saisir](assets/grab-icon.png) à gauche d’un nom de champ, puis faites-le glisser et déposez-le à l’endroit souhaité.

   >[!TIP]
   >
   >Vous pouvez faire glisser des champs vers une autre section.
   >Vous devez avoir au moins un champ dans une section.
   >

   La nouvelle position du champ est mise à jour dans l’aperçu et la page de tous les enregistrements du même type pour tous les utilisateurs qui consultent les enregistrements.

   Toutes les modifications apportées à la disposition de l’aperçu d’enregistrement ou de la page sont enregistrées automatiquement.

## Ajouter une page Enregistrements connectés à un enregistrement

Vous pouvez afficher les informations des enregistrements ou objets connectés en ajoutant un onglet pour une page Enregistrements connectés à un enregistrement.

Les informations des enregistrements connectés peuvent être modifiées dans la vue Tableau. Les informations des objets connectés à partir d’une autre application ne sont pas modifiables en mode Tableau.

Tenez compte des points suivants lors de l’ajout d’une page Enregistrements connectés à un enregistrement :

* Vous pouvez ajouter une page Enregistrements connectés à un enregistrement après avoir connecté des enregistrements ou des types d&#39;objet au type d&#39;enregistrement à partir de la vue Tableau d&#39;un type d&#39;enregistrement.

* Dans l’environnement de production, vous ne pouvez pas ajouter une page Enregistrements connectés à partir de l’aperçu d’un enregistrement.

  <span class="preview">Vous pouvez ajouter une page Enregistrements connectés à partir de l’aperçu d’un enregistrement dans l’environnement Aperçu.</span>

* Les pages Enregistrements connectés affichent uniquement les objets connectés ou les enregistrements d&#39;un type d&#39;objet ou d&#39;enregistrement dans une vue Tableau. La page n’affiche pas tous les enregistrements de ce type en mode Tableau.

* Selon l’environnement utilisé, vous remarquerez peut-être les éléments suivants :

   * Dans l’environnement de production, après avoir ajouté une page Enregistrements connectés à un enregistrement, l’onglet de page est visible à partir de la zone d’aperçu de l’enregistrement, mais il est vide. Vous devez accéder à la page complète pour afficher la vue du tableau pour l’enregistrement connecté.
   * <span class="preview">Dans l’environnement de Prévisualisation, la page Enregistrements connectés est visible à partir de la zone de prévisualisation de l’enregistrement et de l’onglet du navigateur.</span>

* Vous pouvez ajouter des pages Enregistrements connectés pour les types d’objet ou d’enregistrement connectés suivants :

   * Types d’enregistrements Workfront Planning
   * Projets, programmes, portfolios, groupes ou sociétés Workfront. Vous pouvez afficher les objets Workfront connectés même si vous ne disposez pas des autorisations nécessaires pour y accéder dans Workfront.

  >[!NOTE]
  >
  >   Vous ne pouvez pas ajouter de page Enregistrements connectés pour les enregistrements AEM Assets connectés.

Pour ajouter une page Enregistrements connectés :

1. Cliquez sur le nom de l’enregistrement pour l’ouvrir.
1. Cliquez sur **Ajouter une page** dans l’une des zones suivantes :

   * <span class="preview">Fenêtre d&#39;aperçu de l&#39;enregistrement</span>
   * la page de détails de l’enregistrement, après avoir cliqué sur l’icône **Ouvrir dans un nouvel onglet** ![Ouvrir les détails dans une nouvelle icône d’onglet](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de la page d’aperçu.

   La boîte de dialogue **Créer une page** s’ouvre.

   ![Boîte de dialogue modale Ajouter la page Enregistrements connectés](assets/add-connection-view-page-modal.png)

1. Ajoutez le **Nom de la page**, cliquez sur **Page des enregistrements connectés**, puis sur **Créer**.

   Un nouvel onglet est ajouté à la page de l’enregistrement.
1. Recherchez ou cliquez sur le nom d’un enregistrement ou d’un type d’objet connecté dans la liste.
La vue Tableau du type d’enregistrement que vous avez sélectionné s’affiche dans la nouvelle page et les enregistrements connectés s’affichent dans la vue Tableau.
Tous les champs de l&#39;enregistrement connecté s&#39;affichent dans la vue Tableau de l&#39;onglet de l&#39;enregistrement connecté.

   Les cinq premiers champs de la table des enregistrements connectés s’affichent par défaut. Aucun champ de recherche n’est affiché par défaut.

   ![Vue du tableau connecté à l’audience sous les détails de la campagne](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Facultatif) Dans la vue Tableau des enregistrements connectés, effectuez l’une des opérations suivantes :

   * Cliquez sur le nom d’un enregistrement. La page de l&#39;enregistrement s&#39;ouvre alors dans un nouvel onglet.

     Cette action ouvre la page d&#39;aperçu de l&#39;enregistrement. Cliquez sur l&#39;icône **Ouvrir dans un nouvel onglet** ![Ouvrir dans une nouvelle icône d&#39;onglet](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit pour ouvrir la page de l&#39;enregistrement connecté.

   * Cliquez sur **Connexion** pour connecter d&#39;autres enregistrements, puis cliquez en dehors de la zone de connexion pour la fermer. Les nouveaux enregistrements sont automatiquement ajoutés à la table.
   * Modifiez toutes les informations des enregistrements connectés dans la vue Tableau.

   * Pointez sur le nom d’un enregistrement connecté, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur l’une des options suivantes :
      * Afficher
      * Copier le lien
      * Modifier la miniature
      * Dupliquer
      * Insérer un enregistrement au-dessus ou en dessous
      * Supprimer
   * Sélectionnez l&#39;un des enregistrements puis cliquez sur l&#39;une des options suivantes dans la barre bleue située en bas de l&#39;écran :
      * Afficher
      * Copier le lien
      * Modifier la miniature
      * Dupliquer
      * Supprimer. La suppression est la seule option disponible lorsque vous sélectionnez plusieurs enregistrements.

     Pour plus d&#39;informations sur la modification des enregistrements en mode Tableau, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

   * Modifiez sur la ligne l’un des enregistrements de la table de la page Enregistrements connectés . Dans l’environnement de production, tous les objets Workfront s’affichent dans une vue de tableau en lecture seule et vous ne pouvez pas les modifier. <span class="preview">Vous pouvez modifier les projets Workfront sur la ligne dans l’environnement de prévisualisation.</span>

1. (Facultatif) Double-cliquez sur le nom de l’onglet Page Enregistrements connectés

   Ou

   Pointez sur le nom de l’onglet, puis cliquez sur **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Renommer** pour renommer en nouvel onglet Vue connectée.
1. (Facultatif) Utilisez l’un des éléments d’affichage suivants dans la barre d’outils pour gérer la vue du tableau :

   * Filtres
   * Trier
   * Regroupement 
   * Champs, pour afficher, masquer ou réorganiser les champs

   Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >   Vous ne pouvez pas créer, modifier ou supprimer des champs dans la vue Tableau de l&#39;onglet d&#39;un enregistrement connecté.
   >

1. (Conditionnel) Pour connecter d’autres enregistrements ou objets, effectuez l’une des opérations suivantes :

   * Cliquez sur **Connexion** au bas du tableau, pour ajouter ou supprimer des enregistrements ou tout objet Workfront <span class="preview">à l’exception des projets</span>.
   * <span class="preview">Dans l’environnement Aperçu, cliquez sur **Connecter des enregistrements** dans le coin supérieur droit de la page des enregistrements connectés, ou **Nouvelle ligne** au bas du tableau pour ajouter ou supprimer des projets.</span>

   Pour plus d’informations, consultez la section [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).
1. (Facultatif) Pointez sur le nom de l’onglet Page Enregistrements connectés , cliquez sur **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Supprimer** pour supprimer de l’onglet.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



