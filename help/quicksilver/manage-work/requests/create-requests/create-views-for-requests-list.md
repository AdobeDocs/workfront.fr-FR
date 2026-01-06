---
product-area: requests
navigation-topic: create-requests
title: Créer et gérer des vues dans la zone des Demandes
description: Si vous utilisez la nouvelle expérience de demande, vous pouvez créer et enregistrer des vues pour la zone des Demandes.
author: Becky
feature: Work Management
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 9%

---

# Créer et gérer des vues dans la zone des Demandes

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

Si vous utilisez la nouvelle expérience de demande, vous pouvez créer et enregistrer des vues pour la zone des Demandes. Ces vues incluent des filtres et des dispositions de colonnes.

Les vues peuvent être créées et gérées dans la zone des Demandes de Workfront et dans le widget Mes demandes de l’Accueil. Les paramètres d’affichage sont conservés entre la zone des Requêtes et le widget.

>[!IMPORTANT]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle expérience de demande.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p>  <p>Vous devez être un administrateur Workfront pour ajouter des vues aux modèles de disposition</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produit</td> 
   <td> <ul><li>Adobe Workfront</li><li>Vous devez disposer d’Adobe Workfront Planning pour afficher les demandes Planning ou les formulaires de demande</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une vue dans la zone des Demandes

Vous pouvez créer une vue dans la zone des Demandes de Workfront ou dans le widget Mes demandes de l’Accueil.

1. Pour accéder à la liste Demandes :

   {{step1-to-requests}}

1. Pour accéder au widget Mes requêtes dans l’Accueil :

   {{step1-to-home}}

   1. Recherchez le widget Mes requêtes .

      Pour plus d’informations sur le widget Mes requêtes, voir [Utiliser le widget Mes requêtes](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Dans la liste des Demandes ou dans le widget Mes demandes, cliquez sur la liste déroulante **Vues** ![Liste déroulante Vues](assets/view-icon-requests.png) et sélectionnez **Nouvelle vue**.

   ![Nouvel affichage](assets/create-new-view.png)

1. Saisissez le nom de la nouvelle vue, puis cliquez sur **Créer**.
1. Passez à [Modifier une vue dans la zone des Demandes](#edit-a-view-in-the-requests-area).

## Modifier une vue dans la zone des Demandes

Vous pouvez modifier les vues existantes, y compris les vues que vous venez de créer.

1. Pour accéder à la liste Demandes :

   {{step1-to-requests}}

1. Pour accéder au widget Mes requêtes dans l’Accueil :

   {{step1-to-home}}

   1. Recherchez le widget Mes requêtes .

      Pour plus d’informations sur le widget Mes requêtes, voir [Utiliser le widget Mes requêtes](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Dans la liste des Demandes ou dans le widget Mes demandes, recherchez la vue à modifier.

1. (Facultatif) Pour renommer une vue, cliquez sur la liste déroulante **Vues** ![Liste déroulante des vues](assets/view-icon-requests.png), puis cliquez sur le menu à trois points en regard de la vue, sélectionnez **Renommer**, puis saisissez le nouveau nom de la vue.
1. Cliquez sur la liste déroulante **Vues** ![Vues déroulantes](assets/view-icon-requests.png) et sélectionnez la vue à modifier.
1. <span class="preview">Pour ajouter un champ personnalisé sous forme d’une colonne, cliquez sur l’icône **Ajouter une colonne** ![Ajouter une colonne](assets/add-column.png) à droite de l’écran, puis cliquez sur l’icône plus en regard du champ de formulaire personnalisé que vous souhaitez ajouter en tant que colonne à l’affichage.</span>

   <span class="preview">Vous pouvez ajouter des champs personnalisés sur les formulaires joints à l’objet dans la liste sous forme de colonnes.</span>

   >[!TIP]
   >
   >Vous ne pouvez actuellement pas ajouter de colonnes dans l’environnement de production.
1. (Facultatif) Cliquez sur **Colonnes** et masquez, affichez ou réorganisez les colonnes de la liste des demandes.

   ![Zone Colonnes](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >Actuellement, vous ne pouvez plus ajouter de colonne dans l’environnement de production.

1. (Facultatif) Cliquez sur **Filtres** et commencez à ajouter des conditions pour les requêtes que vous souhaitez afficher dans l’onglet Planification.

   ![Modification de filtres dans l&#39;onglet Demandes Planning](assets/filters-editing-box-in-requests-planning-tab.png)

   Vous pouvez filtrer selon les champs suivants :

   * **Workspace** : espace de travail auquel le formulaire de demande est associé.
   * **Type d’enregistrement** : type d’enregistrement auquel le formulaire de demande est associé.
   * **Date d’entrée** : date à laquelle la demande a été soumise.
   * **Formulaire de demande** : nom du formulaire de demande utilisé pour soumettre la demande.
   * **Statut** : statut de la demande.
   * **Saisi par** : nom de l’utilisateur qui a ajouté la demande. Si la demande a été ajoutée par une personne extérieure à Workfront, le champ **Saisi par** affiche `N/A`.

   <span class="preview">Dans l’environnement Aperçu , vous pouvez également filtrer selon les champs personnalisés qui ont été ajoutés à l’affichage.</span>

   Plusieurs filtres peuvent être joints par **Et** ou **Ou**.
La liste des demandes est automatiquement filtrée à mesure que vous ajoutez les conditions de filtrage.



>[!IMPORTANT]
>
> * Les modifications apportées aux vues sont enregistrées automatiquement.
> * Toute personne qui utilise la vue peut voir les modifications apportées aux vues.

## Ajoutez la vue à un modèle de mise en page.

Un administrateur Workfront peut ajouter la nouvelle vue aux modèles de mise en page.

Pour obtenir des instructions, voir [Personnaliser des filtres, des vues et des regroupements à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Partager une vue

Vous pouvez partager les vues que vous créez avec d&#39;autres utilisateurs, équipes ou groupes.

1. Pour accéder à la liste Demandes :

   {{step1-to-requests}}

1. Pour accéder au widget Mes requêtes dans l’Accueil :

   {{step1-to-home}}

   1. Recherchez le widget Mes requêtes .

      Pour plus d’informations sur le widget Mes requêtes, voir [Utiliser le widget Mes requêtes](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Dans la liste des Demandes ou dans le widget Mes demandes, recherchez la vue que vous souhaitez partager.
1. Pointez sur la vue à partager, puis cliquez sur le menu à trois points lorsqu’il s’affiche.
1. Sélectionnez **Partager**.
1. Dans la boîte de dialogue qui s’ouvre, saisissez les noms des utilisateurs, des équipes ou des groupes avec lesquels vous souhaitez partager la vue, puis sélectionnez-les dans la liste lorsqu’ils apparaissent.
1. Cliquer sur **Enregistrer**.

