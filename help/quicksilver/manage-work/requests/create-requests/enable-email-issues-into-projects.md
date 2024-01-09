---
product-area: requests
navigation-topic: create-requests
title: Autorisation des utilisateurs à envoyer par courrier électronique un problème dans un projet de file d’attente des demandes
description: Autorisation des utilisateurs à envoyer par courrier électronique un problème dans un projet de file d’attente des demandes
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: dad055b0901cfa8114f7f6b13b6f689d70b31205
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Autorisation des utilisateurs à envoyer par courrier électronique un problème dans un projet de file d’attente des demandes

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Vous pouvez configurer un projet pour permettre aux utilisateurs d’ajouter des problèmes au projet par courrier électronique. Vous pouvez autoriser l’envoi de problèmes par courrier électronique dans un projet uniquement si le projet est désigné comme une file d’attente de requêtes. Pour plus d’informations sur la création d’un projet de file d’attente des demandes, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Les conditions préalables suivantes sont requises pour configurer un projet afin de permettre aux utilisateurs d’ajouter des problèmes au projet par courrier électronique.

Ces conditions doivent être remplies avant d’activer cette fonctionnalité :

* Les utilisateurs qui envoient des problèmes par courrier électronique à ce compte doivent disposer d’une licence pour Workfront.
* Les utilisateurs qui envoient des problèmes par courrier électronique à ce compte doivent disposer des autorisations Ajouter un problème sur le projet.
* Les utilisateurs externes ne peuvent pas envoyer de messages électroniques concernant des problèmes à une file d’attente de requêtes, car ils n’ont pas accès à la création de problèmes.
* Seuls les messages électroniques provenant d’une adresse électronique associée à un utilisateur Workfront actif sont autorisés à envoyer des problèmes au projet. Les courriers électroniques transférés vers un courrier électronique utilisateur Workfront actif à partir d’un courrier électronique non associé à un compte Workfront ne peuvent pas créer de problèmes sous le projet, car l’adresse électronique de l’expéditeur d’origine doit être associée à un compte Workfront actif.
* Le projet est configuré en tant que file d’attente des demandes.
* Le compte de messagerie associé au projet n’est pas lié à un compte utilisateur Workfront.

## Configuration du projet dans Workfront

>[!NOTE]
>
>Gardez les éléments suivants à l’esprit lors de l’activation des paramètres de la file d’attente des emails :
>
>* Workfront autorise un email unique par file d’attente de requêtes dans toutes les grappes. Si vous choisissez de désactiver la file d’attente des demandes, vous conserverez l’adresse électronique que vous avez créée tant qu’elle se trouve toujours dans la zone Intake Email Address (Adresse électronique d’entrée). Si vous choisissez d’arrêter l’utilisation de l’email d’ingestion, vous devez le supprimer du champ Réception d’email afin qu’il puisse être utilisé ultérieurement.
>
>* Si la file d’attente des demandes comporte plusieurs rubriques ou groupes de rubriques de file d’attente, Workfront sélectionne de manière aléatoire la rubrique de file d’attente vers laquelle les demandes envoyées par courrier électronique seront envoyées, rendant ainsi les requêtes envoyées difficilement gérables.
>Nous recommandons que le projet que vous configurez pour recevoir des requêtes par courrier électronique ne comporte pas plus d’une rubrique de file d’attente. Si les demandes envoyées sont destinées à différents projets ou ressources, vous devez les acheminer ou les déplacer manuellement, après leur envoi.

1. Accédez au projet que vous souhaitez activer pour recevoir les problèmes par email.
1. Cliquez sur **Détails de la file** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus** en premier.
1. Dans le **Type de file d’attente** zone, sélectionnez **Publier en tant que file d’attente de demande d’aide**.

1. Faites défiler l’écran vers le bas jusqu’à **Paramètres de la file d’attente des emails** puis sélectionnez **Activer l’entrée de demande par courrier électronique**.

1. Saisissez le début de l’adresse électronique dans la zone **Adresse électronique de réception** de la boîte.

   Vous devez créer une adresse électronique unique. Nous vous recommandons d’utiliser le nom de votre société dans votre adresse électronique de prise en charge.

   >[!CAUTION]
   >
   >* Cette adresse électronique ne peut pas être récupérée dans la corbeille si le projet contenant la file d’attente des demandes est supprimé.
   >
   >* Comme cette adresse électronique doit être unique, elle risque de ne plus être disponible à l’avenir si elle est supprimée.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Facultatif) Sélectionnez le **Transférer tous les problèmes qui ne peuvent pas être envoyés par courrier électronique**, puis saisissez une adresse électronique de transfert dans la zone ci-dessous.

   Cette adresse électronique reçoit des informations sur les courriers électroniques qui n’ont pas pu être envoyés au projet.

1. Cliquez sur **Enregistrer**. Désormais, lorsque les utilisateurs disposant d’un compte Workfront actif envoient un courrier électronique à cette adresse électronique, un problème est créé dans le projet Workfront.

   >[!NOTE]
   >
   >Les utilisateurs doivent avoir accès à la création de problèmes dans le projet pour pouvoir l’envoyer par courrier électronique. Vous pouvez accorder cet accès dans la boîte de dialogue Partage sous Paramètres avancés.
   >
   >Les utilisateurs externes ne peuvent pas envoyer de messages électroniques concernant des problèmes à une file d’attente de requêtes, car ils n’ont pas accès à la création de problèmes.

## Réception du problème dans Workfront

Lorsqu’un utilisateur Workfront envoie un courrier électronique à Workfront, les événements suivants se produisent :

* La ligne Objet de l’email devient le Nom du problème.
* Le corps de l’email devient la Description du problème.
* S&#39;il existe des documents joints à l&#39;email, ces documents sont joints au problème dans Workfront.
* L’utilisateur qui envoie le courrier électronique devient le contact par Principal du nouveau problème dans Workfront.
* Le corps du texte de l&#39;email ne peut pas dépasser 4000 caractères.
* Les pièces jointes aux emails ne doivent pas dépasser 7 Mo au total.
