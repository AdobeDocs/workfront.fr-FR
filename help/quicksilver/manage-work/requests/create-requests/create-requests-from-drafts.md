---
product-area: requests
navigation-topic: create-requests
title: Créer des demandes à partir de brouillons
description: Outre l’utilisation des brouillons disponibles que Workfront vous suggère lorsque vous entrez une nouvelle requête, vous pouvez également accéder à une demande de brouillon à partir de la section Brouillons et terminer son envoi à partir de là.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 0f30ff23ef828d32c406cc2d9733c23b095014c9
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 16%

---

# Créer des demandes à partir de brouillons

Outre l’utilisation des brouillons disponibles que Workfront vous suggère lorsque vous entrez une nouvelle requête, vous pouvez également accéder à une demande de brouillon à partir de la section Brouillons et terminer son envoi à partir de là.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables pour la création de requêtes à partir de brouillons

Vous devez effectuer les opérations suivantes avant de pouvoir créer une requête à partir d’un brouillon : 

* Commencez à créer une requête. Cette opération enregistre automatiquement la demande en tant que brouillon dans la section Brouillons .

  Pour plus d’informations sur la création de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Créer des demandes à partir de brouillons

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront.
1. Cliquez sur **Requêtes** > **Brouillons**.

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
1. (Facultatif et conditionnel) À tout moment lors de la saisie de la requête, cliquez sur **Ignorer** si vous souhaitez supprimer le brouillon. Cette opération supprime le brouillon qui ne peut pas être récupéré. Pour plus d’informations sur la suppression de brouillons, voir [Suppression d’un brouillon de demande](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Facultatif) Cliquez sur **Annuler** dans le coin inférieur gauche de la page si vous souhaitez annuler votre action et conserver le brouillon.

1. Après avoir renseigné les informations de la requête, effectuez l’une des opérations suivantes :

   * Cliquez sur **Submit** si vous êtes prêt à envoyer la demande. La demande est enregistrée dans la section Envoyé . Selon la règle de routage de la file d’attente des requêtes, cette requête peut être acheminée vers un projet différent de celui désigné comme file d’attente des requêtes. Pour plus d’informations sur les règles de routage, voir [Création de règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Ou

     Cliquez sur **Fermer** si vous n’êtes pas tout à fait prêt à l’envoyer et que vous pouvez y revenir et le terminer ultérieurement. Votre demande est enregistrée dans la section Brouillons et vous sera disponible la prochaine fois que vous soumettrez une demande pour cette file d’attente de demandes.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Lorsque vous soumettez la demande, le brouillon est supprimé et ne peut pas être restauré.
