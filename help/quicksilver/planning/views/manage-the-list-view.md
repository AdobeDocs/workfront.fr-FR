---
title: Gestion de la vue Liste dans Adobe Workfront Planning
description: Vous pouvez afficher les objets et leurs champs dans une vue Liste, lorsque vous y accédez dans la page Enregistrements connectés d’un enregistrement, dans Adobe Workfront Planning. Cet article décrit comment créer ou modifier une vue Liste dans la page Enregistrements connectés d’un enregistrement.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 2%

---


# Gestion de la vue Liste dans Adobe Workfront Planning

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez afficher les objets et leurs champs dans une vue Liste, lorsque vous y accédez dans la page Enregistrements connectés d’un enregistrement, dans Adobe Workfront Planning.

Cet article décrit comment créer ou modifier une vue Liste dans la page Enregistrements connectés d&#39;un enregistrement et comment modifier les objets dans la vue.

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

* Vous ne pouvez pas afficher les enregistrements dans les pages de type d’enregistrement dans une vue Liste. Vous ne pouvez afficher les objets suivants dans une vue Liste que lorsque vous les visualisez dans la page Enregistrements connectés d&#39;un enregistrement :

   * Projets Workfront

  Pour plus d&#39;informations sur la création d&#39;une page d&#39;enregistrements connectés, voir [Ajouter une page d&#39;enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Avant de pouvoir afficher une vue Liste dans une page Enregistrements connectés d’un enregistrement, vous devez connecter les projets Workfront aux types d’enregistrements Planning. Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).
* Les vues Liste sont similaires aux listes améliorées. Pour plus d’informations, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Gestion d’une vue de liste {#manage-a-list-view}

Pour plus d’informations sur la gestion des vues de liste dans Workfront, voir [ Utilisation de listes améliorées ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Cliquez sur une carte d’espace de travail, puis sur une carte de type enregistrement.
1. Depuis n’importe quel affichage, cliquez sur le nom d’un enregistrement pour ouvrir la page d’aperçu ou de détails de l’enregistrement.
1. Ajoutez une **page Enregistrements connectés** pour les projets connectés, comme décrit dans l’article [Ajouter une page Enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

   La page Enregistrements connectés affiche les projets connectés à l’enregistrement dans la vue Liste.

   ![Projets sur la page des enregistrements connectés dans la vue Liste](assets/projects-on-connected-records-page-list-view.png)

1. (Facultatif) Effectuez l’une des opérations suivantes pour modifier la vue Liste :

   1. Développez le menu des vues déroulantes dans le coin supérieur droit de la liste pour sélectionner une autre vue, ou cliquez sur **Nouvelle vue** et créez-en une autre.

      Les vues sont partagées dans l’ensemble du système. Si vous créez une vue Projets pour un type d’enregistrement, vous pouvez l’afficher sur d’autres types d’enregistrement qui affichent les projets connectés.

   1. Passez la souris sur le nom d&#39;une vue existante et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur l&#39;une des options suivantes :
      * **Renommer**, pour donner un nouveau nom à la vue
      * **Partager**, pour partager la vue avec d&#39;autres personnes
      * **Supprimer**, pour supprimer la vue.

      >[!NOTE]
      >
      >Vous devez disposer d’autorisations de niveau Gérer sur une vue pour pouvoir la modifier, la partager ou la supprimer.
      >
      >Vous ne pouvez pas modifier les vues système.
      >
   1. Cliquez sur l’icône **Filtre** ![Icône Filtre](assets/filter-icon.png) pour ajouter un filtre à la vue. Les résultats sont immédiatement filtrés dans la liste. Vous ne pouvez pas enregistrer ni nommer les filtres. Les filtres sont mémorisés lorsque vous accéderez à la page ultérieurement et ils font partie des vues partagées.
   1. Cliquez sur l’icône **Colonnes** ![Icône Colonnes](assets/columns-icon.png) pour sélectionner les colonnes à afficher ou à masquer dans la vue.
   1. Pointez sur le nom d’une colonne, puis cliquez sur la flèche vers le bas située à gauche du nom de la colonne, puis cliquez sur l’une des options suivantes :
      * **Renommer**, pour ajouter un **libellé personnalisé** pour la colonne. Le nom du champ d’origine dans Workfront ne change pas.
      * **Trier**, pour trier la liste en fonction du champ sélectionné. Une icône de tri indiquant le sens du tri est ajoutée à l’en-tête de colonne.
   1. Cliquez sur l’icône **+** dans le coin supérieur droit de la liste pour ajouter ou supprimer des colonnes dans la liste, puis cliquez sur **Enregistrer**.

      Le **Gestionnaire de colonnes** s’ouvre.

      Vous ne pouvez ajouter que des champs existants à la vue Liste.
Vous ne pouvez pas supprimer le champ principal dans la vue Liste qui s’affiche dans la première colonne.
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

   Sélectionnez un ou plusieurs éléments, remarquez la barre d&#39;actions située en bas de la liste, puis cliquez sur l&#39;un des éléments suivants :

   * **Supprimer** pour supprimer le projet. La suppression d’un projet le déconnecte de l’enregistrement et le déplace vers la Corbeille de Workfront. Les administrateurs et administratrices de Workfront peuvent récupérer les projets supprimés jusqu’à 30 jours après leur suppression.
   * **Déconnecter** pour déconnecter le projet de l’enregistrement. La déconnexion d’un projet supprime cet enregistrement et toutes les valeurs de ses champs de recherche de l’enregistrement actif.

   ![Barre d’actions dans la vue Liste des pages Enregistrements connectés](assets/actions-bar-connected-records-page-list-view.png)

