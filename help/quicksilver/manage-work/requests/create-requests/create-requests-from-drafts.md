---
product-area: requests
navigation-topic: create-requests
title: Créer des demandes à partir de brouillons
description: En plus d’utiliser les brouillons disponibles, suggérés par Workfront, lorsque vous saisissez une nouvelle demande, vous pouvez accéder à un brouillon de demande à partir de la section Brouillons et finir de l’envoyer à partir de là.
author: Becky
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 319c45bc6617269f358af1e7b5f6132a8694710b
workflow-type: tm+mt
source-wordcount: '836'
ht-degree: 72%

---

# Créer des demandes à partir de brouillons

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

En plus d’utiliser les brouillons disponibles, suggérés par Workfront, lorsque vous saisissez une nouvelle demande, vous pouvez accéder à un brouillon de demande à partir de la section Brouillons et finir de l’envoyer à partir de là.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>Modifier l’accès aux problèmes</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produit</td> 
   <td> <ul><li>Adobe Workfront</li><li>Vous devez disposer d’Adobe Workfront Planning pour afficher les demandes Planning ou les formulaires de demande</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables à la création de demandes à partir de brouillons

Vous devez effectuer les opérations suivantes avant de pouvoir créer une demande à partir d’un brouillon :

* Commencez à créer une demande. Cette opération enregistre automatiquement la demande sous forme de brouillon dans la section Brouillons.

  Pour plus d’informations sur la création de demandes, voir la section [Créer et envoyer des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Créer des demandes à partir de brouillons

La procédure de création de requêtes à partir de brouillons diffère entre la nouvelle expérience de requête et l’expérience héritée.

* <span class="preview">[Créer des requêtes à partir de brouillons dans la nouvelle expérience de requête](#create-requests-from-drafts-in-the-new-requesting-experience)</span>
* [Créer des requêtes à partir de brouillons dans l’expérience de requête héritée](#create-requests-from-drafts-in-the-legacy-requesting-experience)

<div class="preview">

### Créer des requêtes à partir de brouillons dans la nouvelle expérience de requête




1. Ouvrez le brouillon.

   Les brouillons se trouvent aux emplacements suivants :

   * Dans la liste des demandes de la zone des Demandes
   * Dans la liste des requêtes du widget Mes requêtes de l’Accueil
   * Dans la boîte de dialogue Nouvelle demande (inclut uniquement les brouillons de demandes créées avec le formulaire sélectionné)

   >[!NOTE]
   >
   >Les brouillons créés dans l’expérience de demande héritée ne sont pas disponibles dans la nouvelle expérience de demande.

1. Mettez à jour les informations relatives à la demande, tel que décrit dans la section [Créer et envoyer des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Facultatif et le cas échéant) À tout moment au cours de la saisie de la demande, cliquez sur **Ignorer** le brouillon si vous souhaitez supprimer le brouillon. Le brouillon est supprimé.

   Si vous avez ignoré votre brouillon par erreur, vous pouvez immédiatement cliquer sur **Annuler** dans le message en bas de l’écran. Cette option n’est disponible que pendant quelques secondes.

   Pour plus d’informations sur la suppression des brouillons, voir [Supprimer une demande envoyée ou demander un brouillon](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Facultatif) Pour enregistrer les modifications apportées au brouillon sans l’envoyer, quittez la page Nouvelle demande . Les modifications sont enregistrées automatiquement.

1. Une fois les informations de la demande renseignées, cliquez sur **Soumettre**.

   Lorsque vous envoyez la demande, le brouillon est supprimé et ne peut pas être restauré.

</div>

### Créer des requêtes à partir de brouillons dans l’expérience de requête héritée

{{step1-to-requests}}

1. Sélectionnez **Brouillons** dans le panneau de gauche.

   Un brouillon pour chaque rubrique de file d’attente de chaque file d’attente des demandes s’affiche dans cette liste.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Facultatif) Cliquez sur l’en-tête d’une colonne pour trier la liste en fonction de cette colonne.

1. Examinez les informations relatives à chaque brouillon dans les colonnes suivantes de la liste Brouillons :

   | Objet | Il s’agit du nom que vous avez donné à votre demande lorsque vous avez commencé à la créer. |
   | --- | --- |
   | Chemin d’accès | Nom de la file d’attente des demandes, des groupes de rubriques et des rubriques de file d’attente où vous aviez l’intention d’envoyer la demande à l’origine. |
   | Date d’entrée | Date à laquelle vous avez initié la création de la demande. |
   | Date de dernière mise à jour | Votre dernière mise à jour. Si vous n’avez pas effectué de mise à jour depuis le début de la création de la demande, la date d’entrée en vigueur et la date de la dernière mise à jour doivent être identiques. |

   {style="table-layout:auto"}

1. (Facultatif) À l’aide du filtre rapide situé en haut à droite de la liste Brouillons, commencez à saisir le nom d’une demande, d’une file d’attente des demandes, d’une rubrique de file d’attente ou d’un groupe de rubriques à l’état de brouillon, puis cliquez sur le nom d’un brouillon pour l’ouvrir.

   >[!TIP]
   >
   >Vous ne pouvez pas appliquer de filtres permanents dans la section Brouillons de la zone Demandes. En outre, il n’existe aucune option permettant de modifier ou de changer l’affichage de la liste des brouillons.

1. Mettez à jour les informations relatives à la demande, tel que décrit dans la section [Créer et envoyer des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Facultatif et le cas échéant) À tout moment au cours de la saisie de la demande, cliquez sur **Ignorer** le brouillon si vous souhaitez supprimer le brouillon. Cette opération supprime le brouillon, qui ne pourra plus être récupéré. Pour plus d’informations sur la suppression des brouillons, voir la section [Supprimer un brouillon de demande](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Facultatif) Cliquez sur **Annuler** en bas à gauche de la page si vous souhaitez annuler votre action et conserver le brouillon.

1. Après avoir complété les informations relatives à la demande, effectuez l’une des opérations suivantes :

   * Cliquez sur **Envoyer** si la demande est prête à être envoyée. La demande est enregistrée dans la section Envoyé. En fonction de la règle de transmission de la file d’attente des demandes, cette demande peut être transmise vers un projet différent de celui désigné comme file d’attente des demandes. Pour plus d’informations sur les règles de transmission, voir la section [Créer des règles de transmission](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Ou

     Cliquez sur **Fermer** si l’envoi n’est pas encore prêt. Vous pourrez ainsi y revenir pour terminer plus tard. Votre demande est enregistrée dans la section Brouillons et sera disponible la prochaine fois que vous enverrez une demande pour cette file d’attente des demandes.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Lorsque vous envoyez la demande, le brouillon est supprimé et ne peut pas être restauré.

