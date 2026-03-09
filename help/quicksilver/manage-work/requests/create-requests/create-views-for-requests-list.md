---
product-area: requests
navigation-topic: create-requests
title: Créer et gérer des vues dans la zone Requêtes
description: Si vous utilisez la nouvelle expérience de demande, vous pouvez créer et enregistrer des vues pour la zone des Demandes.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 9%

---


# Créer et gérer des vues dans la zone Requêtes

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>





Si vous utilisez la nouvelle expérience de demande dans Adobe Workfront, vous pouvez créer et enregistrer des vues pour la zone des Demandes . Ces vues incluent des filtres et des dispositions de colonnes.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Cette fonctionnalité n’est disponible que dans la nouvelle expérience de demande de la zone des Demandes .
>* Les paramètres d’affichage sont également disponibles dans le widget Mes requêtes de l’Accueil. Toutefois, les vues de la zone des Demandes sont distinctes de celles du widget Mes demandes .
>* La liste des demandes de la zone des Demandes utilise la liste améliorée de Workfront. Pour plus d’informations, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

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
   <td> <p>Contributeur ou supérieur</p>
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

## Création d’une vue pour les requêtes

Vous pouvez créer une vue dans la zone des Demandes de Workfront lorsque vous utilisez la nouvelle expérience de demandes.

1. Pour accéder à la liste Demandes :

   {{step1-to-requests}}

1. Assurez-vous que le paramètre **Utiliser une nouvelle expérience** est activé.

1. Dans la liste **Demandes**, cliquez sur le menu déroulant **Vues** ![Vues](assets/view-icon-requests.png) et cliquez sur **Nouvelle vue**.

   ![Nouvel affichage](assets/create-new-view.png)

1. Saisissez le nom de la nouvelle vue, puis cliquez sur **Créer**.
1. Passez à [Modifier une vue dans la zone des Demandes](#edit-a-view-in-the-requests-area).

## Modification d’une vue pour les requêtes

Vous pouvez modifier des vues existantes, y compris les vues que vous venez de créer dans la zone des Demandes de Workfront.

En modifiant une vue dans la zone Demandes , vous pouvez modifier les éléments suivants de la vue :

* Nom
* Filtres
* Colonnes

Les modifications que vous apportez à une vue sont visibles pour toutes les personnes avec lesquelles vous partagez cette vue.

1. Pour accéder à une liste de demandes dans les demandes, procédez comme suit :

   {{step1-to-requests}}

1. Assurez-vous que le paramètre **Utiliser une nouvelle expérience** est activé.
1. Dans la liste **Demandes**, recherchez la vue à modifier dans le menu déroulant **Vues** ![Vues](assets/view-icon-requests.png).

1. Cliquez sur la liste déroulante **Vues** ![Liste déroulante Vues](assets/view-icon-requests.png) et cliquez sur le menu à trois points en regard de la vue, sélectionnez **Renommer**, puis saisissez le nouveau nom de la vue.
1. Appuyez sur Entrée pour enregistrer le nouveau nom.
1. Cliquez sur la liste déroulante **Vues** ![Vues déroulantes](assets/view-icon-requests.png) et sélectionnez la vue à modifier.
1. Pour ajouter un champ sous forme d’une colonne, cliquez sur l’icône **Ajouter une colonne** ![Ajouter une colonne](assets/add-column.png) dans le coin supérieur droit de la liste.

   Le **Gestionnaire de colonnes** s’ouvre.
1. Cliquez sur l’icône plus en regard du champ que vous souhaitez ajouter en tant que colonne à l’affichage, puis cliquez sur **Enregistrer**.

   Les champs associés aux objets de la liste peuvent être ajoutés en tant que colonnes. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Les champs que vous ajoutez aux colonnes doivent exister avant d’être disponibles dans le **Gestionnaire de colonnes**.


1. (Facultatif) Cliquez sur **Colonnes** pour ouvrir la zone Visibilité et ordre **champs**.
1. Activez le paramètre pour chaque champ que vous souhaitez afficher dans la liste, désactivez-le pour le masquer ou faites glisser et déposez les champs dans un ordre différent.

1. (Facultatif) Cliquez sur **Filtres** et commencez à ajouter des conditions pour les requêtes que vous souhaitez afficher.

   Vous pouvez filtrer selon les champs de requête suivants :

   * **Workspace** : espace de travail auquel le formulaire de demande est associé.
   * **Type d’objet** : type d’enregistrement auquel le formulaire de demande est associé.
   * **Date d’entrée** : date à laquelle la demande a été soumise.
   * **Formulaire de demande** : nom du formulaire de demande utilisé pour soumettre la demande.
   * **Statut** : statut de la demande.
   * **Saisi par** : nom de l’utilisateur qui a ajouté la demande. Si la demande a été ajoutée par une personne extérieure à Workfront, le champ **Saisi par** affiche `N/A`.

   Vous pouvez également filtrer selon les champs qui ont été ajoutés à la vue pour tout objet visible dans la vue.

   Plusieurs filtres peuvent être joints par **Et** ou **Ou**.
La liste des demandes est automatiquement filtrée à mesure que vous ajoutez les conditions de filtrage.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Les modifications apportées aux vues sont enregistrées automatiquement.
> * Toute personne qui utilise la vue peut voir les modifications apportées aux vues.
> * Utilisez le caractère générique de filtre **Moi (utilisateur connecté)** dans tout champ ayant des utilisateurs comme valeur.

## Ajoutez la vue Demandes à un modèle de mise en page.

Un administrateur Workfront peut ajouter la nouvelle vue aux modèles de mise en page.

Pour obtenir des instructions, voir [Personnaliser des filtres, des vues et des regroupements à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Partager une vue

Vous pouvez partager les vues que vous créez avec d&#39;autres utilisateurs, équipes ou groupes.

1. Pour accéder à une liste de demandes dans les demandes, procédez comme suit :

   {{step1-to-requests}}

1. Assurez-vous que le paramètre **Utiliser une nouvelle expérience** est activé.
1. Dans la liste **Demandes**, recherchez la vue que vous souhaitez partager.
1. Pointez sur la vue à partager, puis cliquez sur le menu à trois points situé à droite du nom de la vue, puis cliquez sur **Partager**.
1. Dans la zone **Partager**, saisissez les personnes, équipes, rôles, groupes ou sociétés avec lesquels vous souhaitez partager la vue, puis sélectionnez-les dans la liste lorsqu&#39;elles apparaissent.
1. Cliquez sur **Enregistrer**.

   La vue est partagée avec les entités que vous indiquez. Ils peuvent afficher les éléments de vue mis à jour que vous avez modifiés pour la vue avant de la partager. <span class="preview">S&#39;ils mettent à jour la vue, leurs modifications ne seront pas visibles par les autres utilisateurs, à moins qu&#39;ils ne fassent une copie de la même vue et conservent leurs modifications avant de partager la copie. Pour plus d&#39;informations, voir [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
