---
product-area: requests
navigation-topic: create-requests
title: Création de requêtes à partir de brouillons
description: Outre l’utilisation des brouillons disponibles que Workfront vous suggère lorsque vous entrez une nouvelle requête, vous pouvez également accéder à une demande de brouillon à partir de la section Brouillons et terminer son envoi à partir de là.
author: Lisa
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 28%

---

# Créer des demandes à partir de brouillons

Outre l’utilisation des brouillons disponibles que Workfront vous suggère lorsque vous entrez une nouvelle requête, vous pouvez également accéder à une demande de brouillon à partir de la section Brouillons et terminer son envoi à partir de là.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure</p>
   Ou
   <p>Actuelle : demande ou supérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables pour la création de requêtes à partir de brouillons

Vous devez effectuer les opérations suivantes avant de pouvoir créer une requête à partir d’un brouillon : 

* Commencez à créer une requête. Cette opération enregistre automatiquement la demande en tant que brouillon dans la section Brouillons .

  Pour plus d’informations sur la création de demandes, consultez la section [Créer et envoyer des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Créer des demandes à partir de brouillons

{{step1-to-requests}}

1. Sélectionnez **Brouillons** dans le panneau de gauche.

   Un brouillon pour chaque rubrique de file d’attente de chaque file d’attente de demande s’affiche dans cette liste.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Facultatif) Cliquez sur un en-tête de colonne pour trier la liste en fonction de cette colonne.

1. Consultez les informations sur chaque brouillon dans les colonnes suivantes de la liste Brouillons :

   | Objet | Il s’agit du nom que vous avez donné à votre requête au moment où vous avez commencé à la créer. |
   |---|---|
   | Chemin d’accès | Nom de la file d’attente des demandes, des groupes de rubriques et des rubriques de la file d’attente dans laquelle vous aviez l’intention initiale d’envoyer la demande. |
   | Date d’entrée | Date à laquelle vous avez commencé la création de la requête. |
   | Date de dernière mise à jour | Dernière de votre dernière mise à jour. Si vous ne l’avez pas mise à jour depuis le premier démarrage de la requête, la Date d’entrée et la Date de dernière mise à jour doivent être identiques. |

   {style="table-layout:auto"}

1. (Facultatif) À l’aide du filtre rapide dans le coin supérieur droit de la liste Brouillons, commencez à saisir le nom d’une requête, d’une file d’attente de requêtes, d’une rubrique de file d’attente ou d’un groupe de rubriques, puis cliquez sur le nom d’un brouillon pour l’ouvrir.

   >[!TIP]
   >
   >Vous ne pouvez pas appliquer de filtres permanents dans la section Brouillons de la zone Demandes . En outre, il n’existe aucune option pour modifier l’affichage de la liste des brouillons.

1. Mettez à jour les informations de la requête comme décrit dans [Créer et envoyer des requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Facultatif et conditionnel) À tout moment lors de la saisie de la requête, cliquez sur **Ignorer** si vous souhaitez supprimer le brouillon. Cette opération supprime le brouillon, qui ne pourra plus être récupéré. Pour plus d’informations sur la suppression de brouillons, voir [Suppression d’un brouillon de demande](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Facultatif) Cliquez sur **Annuler** dans le coin inférieur gauche de la page si vous souhaitez annuler votre action et conserver le brouillon.

1. Après avoir renseigné les informations de la requête, effectuez l’une des opérations suivantes :

   * Cliquez sur Soumettre si vous voulez soumettre la demande. **** La demande est enregistrée dans la section Envoyé . En fonction de la règle de transmission de la file d’attente des demandes, cette demande peut être transmise vers un projet différent de celui désigné comme file d’attente des demandes. Pour plus d’informations sur les règles de transmission, consultez [Créer des règles de transmission](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Ou

     Cliquez sur Fermer si vous ne souhaitez pas soumettre immédiatement la demande. Vous pouvez revenir la terminer plus tard. **** Votre demande est enregistrée dans la section Brouillons et vous sera disponible la prochaine fois que vous soumettrez une demande pour cette file d’attente de demandes.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Lorsque vous soumettez la demande, le brouillon est supprimé et ne peut pas être restauré.
