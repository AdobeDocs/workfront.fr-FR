---
title: Gestion de la vue Liste dans Adobe Workfront Planning
description: Vous pouvez afficher les objets et leurs champs dans une vue Liste, lorsque vous y accédez dans la page Enregistrements connectés d’un enregistrement, dans Adobe Workfront Planning. Cet article décrit comment créer ou modifier une vue Liste dans la page Enregistrements connectés d’un enregistrement.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: ddf10844646a79c43accaffa1789caf24290cc8a
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 1%

---


# Gestion de la vue Liste dans Adobe Workfront Planning

<span class="preview">Les informations mises en évidence sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles pour tous. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez afficher les objets dans la vue Liste dans les zones suivantes de Workfront Planning :

* Une page d&#39;enregistrements connectée pour les projets dans la zone des détails d&#39;un enregistrement

  ![Projets sur la page des enregistrements connectés dans la vue Liste](assets/projects-on-connected-records-page-list-view.png)

* Une liste de formulaires de demande au niveau du type d’enregistrement

  ![Formulaires de demande dans la vue Liste](assets/request-forms-in-list-view.png)

Cet article décrit comment parcourir, créer ou modifier une vue de liste qui affiche des objets dans Workfront Planning. <!--change 'projects' to other objects when they become available and the location of the list view-->

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront et tout package Planning</p>
<p>Tout workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p> Standard pour créer et supprimer des vues</p>
   <p>Contributeur ou version ultérieure pour mettre à jour les éléments d’affichage</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations pour une vue</p>  
   <p>Autorisations d’affichage d’une vue pour modifier temporairement les paramètres d’affichage ou la dupliquer</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> Les utilisateurs disposant d'une licence light ou contributor doivent se voir attribuer un modèle de mise en page incluant Planning.
   <p>Les zones Planning sont activées par défaut pour les utilisateurs standard et les administrateurs système.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Considérations relatives aux vues Liste

* Tenez compte des points suivants pour la vue Liste de pages des enregistrements connectés :

   * Vous pouvez uniquement afficher les projets dans la vue Liste dans la page Enregistrements connectés d’un enregistrement. La vue Liste n&#39;est disponible pour aucun autre objet ou type d&#39;enregistrement dans une page d&#39;enregistrements connectée.

  Pour plus d&#39;informations sur la création d&#39;une page d&#39;enregistrements connectés, voir [Ajouter une page d&#39;enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
   * Avant de pouvoir afficher une vue Liste dans une page Enregistrements connectés d’un enregistrement, vous devez connecter les projets Workfront aux types d’enregistrements Planning. Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).
   * Vous pouvez créer plusieurs vues de liste pour les projets dans la page d&#39;enregistrements connectés d&#39;un enregistrement.

* Tenez compte des points suivants pour la vue Liste des formulaires de demande :

   * Vous ne pouvez pas créer ou modifier des vues de liste supplémentaires pour les formulaires de demande Planning. Workfront crée une vue Liste pour les formulaires de demande. <!--this will change-->

     Pour plus d’informations sur les formulaires de demande, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Selon l’emplacement d’affichage, toutes les vues de liste ne comportent pas les mêmes éléments décrits dans cet article.


## Gestion d’une vue de liste {#manage-a-list-view}

Les vues Liste sont similaires aux listes améliorées. La plupart des éléments des vues améliorées existent également dans les vues Liste de Workfront Planning.

Pour plus d’informations, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. Accédez à une vue Liste dans l’une des zones suivantes :

   * Page Enregistrements connectés dans la zone des détails d&#39;un enregistrement
   * Page Formulaires de demande d’un enregistrement

1. (Conditionnel) Si disponible, effectuez l’une des opérations suivantes pour modifier la vue Liste :

   1. Développez le menu des vues déroulantes dans le coin supérieur gauche de la liste pour sélectionner une autre vue, ou cliquez sur **Nouvelle vue** et créez-en une autre.

      Les vues sont partagées dans l’ensemble du système. Si vous créez une vue Projets pour un type d’enregistrement, vous pouvez l’afficher sur d’autres types d’enregistrement qui affichent les projets connectés.

   1. Passez la souris sur le nom d&#39;une vue existante et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur l&#39;une des options suivantes :
      * **Renommer**, pour donner un nouveau nom à la vue
      * **Partager**, pour partager la vue avec d&#39;autres personnes
      * **Supprimer**, pour supprimer la vue.

      >[!NOTE]
      >
      >* Vous devez disposer d’autorisations de niveau Gérer sur une vue pour pouvoir la modifier, la partager ou la supprimer.
      >
      >* Vous ne pouvez pas modifier les vues système.
      >
      >* <span class="preview">Vous pouvez réinitialiser un affichage partagé avec vous et pour lequel vous disposez uniquement d’autorisations d’affichage, après l’avoir modifié pour restaurer ses préférences d’origine, ou vous pouvez le copier avec vos modifications et partager la copie. Pour plus d&#39;informations, voir [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

      <!--
        And hide everything else below for these elements, after moving it to the Use enhanced lists article: 
        1. <span class="preview">To update one of the following view elements, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md):</span>
            <div class="preview">
            * Filter
            * Columns
            * Format cells
            * Row height
            </div>
        -->

   1. Cliquez sur l’icône **Filtre** ![Icône Filtre](assets/filter-icon.png) pour ajouter un filtre à la vue. Les résultats sont immédiatement filtrés dans la liste. Vous ne pouvez pas enregistrer ni nommer les filtres. Les filtres sont mémorisés lorsque vous accéderez à la page ultérieurement et ils font partie des vues partagées.
   1. Cliquez sur l’icône **Colonnes** ![Icône Colonnes](assets/columns-icon.png) pour sélectionner les colonnes à afficher ou à masquer dans la vue.
   1. Pointez sur le nom d’une colonne, puis cliquez sur la flèche vers le bas située à gauche du nom de la colonne, puis cliquez sur l’une des options suivantes :
      * **Renommer**, pour ajouter un **libellé personnalisé** pour la colonne. Le nom du champ d’origine dans Workfront ne change pas.
      * **Trier**, pour trier la liste en fonction du champ sélectionné. Une icône de tri indiquant le sens du tri est ajoutée à l’en-tête de colonne.
   1. Cliquez sur l’icône **+** dans le coin supérieur droit de la liste pour ajouter ou supprimer des colonnes dans la liste, puis cliquez sur **Enregistrer**.

      Le **Gestionnaire de colonnes** s’ouvre.

      Vous ne pouvez ajouter que des champs existants à la vue Liste.
Vous ne pouvez pas supprimer le champ principal dans la vue Liste qui s’affiche dans la première colonne.

   1. <span class="preview">Cliquez sur l’icône **Format de cellule** ![Format de cellule](assets/format-cells-icon.png). La boîte **Format** s’ouvre.</span> <!--change the name of the box when they update it-->
      <span class="preview">Procédez comme suit : </span>

      1. Cliquez sur **Ajouter une condition**.
      1. <span class="preview">Dans la ligne **If**, sélectionnez un champ, choisissez une valeur de champ et ajoutez un modificateur. Les modificateurs changent en fonction du type de champ choisi. </span>

         >[!TIP]
         >
         ><span class="preview">Seuls les champs visibles dans la vue Liste sont disponibles pour la mise en forme conditionnelle.</span>

      1. <span class="preview">(Facultatif) Au lieu d’ajouter une valeur de champ, cliquez sur l’icône **Comparer à un autre champ** ![Comparer à un autre champ](assets/compare-to-another-field-icon.png) et sélectionnez un champ dont vous souhaitez comparer la valeur à celle du champ sélectionné. Par exemple, vous pouvez filtrer les projets dont le propriétaire correspond au sponsor du projet. </span>

         >[!TIP]
         >
         ><span class="preview">Seuls les champs visibles dans la vue Liste sont disponibles pour la mise en forme conditionnelle.</span>

      1. <span class="preview">(Facultatif) Cliquez sur **Ajouter une condition** dans la ligne **Si** pour ajouter d’autres conditions à la même règle.</span>

         >[!TIP]
         >
         ><span class="preview">Vous pouvez ajouter jusqu’à 10 conditions dans une règle de conditionnement et vous pouvez avoir jusqu’à 20 règles pour un champ.</span>

      <div class="preview">

      1. Cliquez sur le connecteur **Ou** entre les conditions pour passer à **Et** et indiquer que plusieurs conditions doivent être remplies en même temps. **Or** est le connecteur par défaut.
      1. Sur la ligne **Format**, sélectionnez un champ pour indiquer la colonne à mettre en forme. <!--edit this area, if it changes names??-->
      1. (Facultatif) Cliquez sur l’icône **cercle de couleur** ![icône cercle de couleur](assets/color-circle.png) en regard du champ sélectionné pour le développer et choisir une autre <!--for a cell or the text of the cell that matches your criteria--> de couleur. <!--is this where the bold, italic is? I had no UI for this when I wrote it-->
      1. Activez le paramètre **Appliquer à la ligne** pour appliquer la mise en forme à l’ensemble de la ligne du champ qui répond aux conditions.
      1. (Facultatif) Cliquez sur **Ajouter une condition** dans la zone **Format** pour ajouter une autre règle pour un autre champ, puis répétez les étapes ci-dessus.
      1. (Facultatif) Cliquez sur **Effacer tout** pour supprimer toute mise en forme.
      1. Cliquez en dehors de la zone **Format** pour la fermer.

         Vous revenez alors à la vue Liste.
La mise en forme est appliquée immédiatement à la vue Liste.
Un point bleu est placé en regard de l’icône **Formater les cellules** pour indiquer qu’une mise en forme spéciale est appliquée à la vue.

      </div>

   <!--leave these here-->

1. (Facultatif) Ajoutez un mot-clé dans la zone de recherche située dans le coin supérieur droit de la liste pour rechercher un élément.

   Les éléments qui correspondent à votre terme de recherche sont mis en surbrillance dans la liste.

1. (Facultatif) Pour ajouter d’autres éléments à la liste et les connecter automatiquement à l’enregistrement sélectionné, effectuez l’une des opérations suivantes :

   * Cliquez sur **Connecter des enregistrements** dans le coin supérieur droit de la liste pour ajouter des éléments existants.
   * Cliquez sur **Nouvelle ligne** au bas de la liste pour ajouter de nouveaux éléments.
1. Cliquez sur le nom d’un élément connecté de la liste pour l’ouvrir dans un autre onglet du navigateur.
1. Double-cliquez à l&#39;intérieur d&#39;une cellule de la liste pour modifier les informations d&#39;un champ, puis appuyez sur Entrée pour enregistrer vos modifications.

   Certains champs sont en lecture seule. Par exemple, le pourcentage d’achèvement d’un projet est un champ calculé par le système et que vous ne pouvez pas modifier manuellement.

1. Pointez sur le nom d’un élément dans la liste, cliquez sur le menu **Plus** [Plus](assets/more-menu.png), puis sur **Affichage** pour ouvrir le projet dans un autre onglet

   Ou

   Sélectionnez un ou plusieurs éléments, remarquez la barre d’actions située en bas de la liste, puis cliquez sur l’un des éléments suivants, le cas échéant :

   * **Supprimer** pour supprimer l’élément. La suppression d’un projet le déconnecte de l’enregistrement et le déplace vers la Corbeille de Workfront. Les administrateurs et administratrices de Workfront peuvent récupérer les projets supprimés jusqu’à 30 jours après leur suppression. La suppression d’un formulaire ne supprime pas les demandes ou les enregistrements créés lors de l’envoi du formulaire.
   * **Déconnecter** pour déconnecter le projet de l’enregistrement. La déconnexion d’un projet supprime cet enregistrement et toutes les valeurs de ses champs de recherche de l’enregistrement actif.

   ![Barre d’actions dans la vue Liste des pages Enregistrements connectés](assets/actions-bar-connected-records-page-list-view.png)

