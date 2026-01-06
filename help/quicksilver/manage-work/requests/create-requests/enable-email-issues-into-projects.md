---
product-area: requests
navigation-topic: create-requests
title: Autoriser les utilisateurs à envoyer par e-mail un événement dans un projet de file d'attente des demandes
description: Vous pouvez configurer un projet pour permettre aux utilisateurs d’ajouter des problèmes au projet par e-mail.
author: Becky
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 82%

---

# Permettre aux utilisateurs et utilisatrices d’envoyer par e-mail un problème dans un projet de la file d’attente des demandes

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Vous pouvez configurer un projet pour permettre aux utilisateurs et utilisatrices d’ajouter des problèmes au projet par e-mail. Vous ne pouvez autoriser l&#39;envoi d&#39;e-mails pour des problèmes dans un projet que si le projet est désigné comme une file d&#39;attente des demandes. Pour plus d’informations sur la création d’un projet de file d’attente des demandes, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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

## Conditions préalables

Les conditions suivantes sont requises pour configurer un projet afin de permettre aux utilisateurs d’ajouter des problèmes au projet par e-mail :

* Les personnes qui envoient des problèmes par e-mail à ce compte doivent être des utilisateurs ou utilisatrices actifs disposant d’une licence pour Workfront.
* Les personnes qui envoient des problèmes par e-mail à ce compte doivent disposer des autorisations Ajouter un problème sur le projet.
* Les personnes externes ne peuvent pas envoyer des problèmes par e-mail à une file d’attente des demandes, car elles n’ont pas accès à la création de problèmes.
* Seuls les e-mails provenant d’une adresse associée à un utilisateur ou une utilisatrice Workfront actif sont autorisés à envoyer des problèmes au projet. Les e-mails transférés vers l’adresse de messagerie d’un utilisateur ou d’une utilisatrice Workfront actif à partir d’une adresse e-mail non associée à un compte Workfront ne peuvent pas créer de problèmes sous le projet, car l’adresse e-mail de l’expéditeur ou expéditrice d’origine doit être associée à un compte Workfront actif.
* Le projet est configuré en tant que file d’attente des demandes.
* Le compte de messagerie associé au projet n’est pas lié à un compte d’utilisateur ou d’utilisatrice Workfront.

## Configurer le projet dans Workfront

>[!NOTE]
>
>Gardez les éléments suivants à l’esprit lors de l’activation des paramètres de la file d’attente des e-mails :
>
>* Workfront autorise un e-mail unique par file d’attente des demandes dans tous les clusters. Si vous choisissez de désactiver la file d’attente des demandes, vous conserverez l’adresse e-mail que vous avez créée tant qu’elle se trouve toujours dans la zone Adresse e-mail de réception. Si vous choisissez d’arrêter l’utilisation de l’adresse e-mail de réception, vous devez la supprimer du champ Adresse e-mail de réception afin qu’elle puisse être utilisée ultérieurement.
>
>* Si la file d’attente des demandes comporte plusieurs rubriques ou groupes de rubriques de file d’attente, Workfront sélectionne aléatoirement la rubrique de file d’attente à laquelle les demandes envoyées par e-mail seront envoyées, ce qui rend les demandes envoyées par e-mail difficiles à gérer.
>Nous recommandons que le projet que vous configurez pour recevoir des demandes par e-mail ne comporte pas plus d’une rubrique de file d’attente. Si les demandes envoyées sont destinées à différents projets ou ressources, vous devez les acheminer ou les déplacer manuellement, après leur envoi.

1. Accédez au projet sur lequel vous souhaitez activer la réception des problèmes par e-mail.
1. Cliquez sur **Détails de la file d’attente** dans le panneau de gauche.
1. Dans la zone **Type de file d’attente**, sélectionnez **Publier en tant que file d’attente des demandes d’aide**.

1. Faites défiler l’écran vers le bas jusqu’à **Paramètres de la file d’attente de messagerie**, puis sélectionnez **Activer la réception de demandes par e-mail**.

1. Saisissez le début de l’adresse e-mail dans la zone **Adresse e-mail de réception**.

   Vous devez créer une adresse e-mail unique. Nous vous recommandons d’utiliser le nom de votre société dans votre adresse e-mail de réception.

   >[!CAUTION]
   >
   >* Cette adresse e-mail ne peut pas être récupérée dans la corbeille si le projet contenant la file d’attente des demandes est supprimé.
   >
   >* Comme cette adresse e-mail doit être unique, elle risque de ne plus être disponible à l’avenir si elle est supprimée.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in Workfront. Only emails created from this email address are added as issues.
   -->

1. (Facultatif) Sélectionnez **Transférer tous les problèmes qui ne peuvent pas être envoyés par e-mail**, puis saisissez une adresse e-mail de transfert dans la zone ci-dessous.

   Cette adresse e-mail reçoit des informations sur les e-mails qui n’ont pas pu être envoyés au projet.

1. Cliquer sur **Enregistrer**. Désormais, lorsque les utilisateurs et utilisatrices disposant d’un compte Workfront actif envoient un e-mail à cette adresse de messagerie, un problème est créé dans le projet Workfront.

   >[!NOTE]
   >
   >Les utilisateurs et utilisatrices doivent avoir accès à la création de problèmes dans le projet pour pouvoir envoyer des problèmes par e-mail. Vous pouvez accorder cet accès dans la boîte de dialogue Partage sous Paramètres avancés.
   >
   >Les personnes externes ne peuvent pas envoyer des problèmes par e-mail à une file d’attente des demandes, car elles n’ont pas accès à la création de problèmes.

## Recevoir le problème dans Workfront

Lorsqu’un utilisateur ou une utilisatrice Workfront envoie un e-mail à Workfront, les événements suivants se produisent :

* La ligne Objet de l’e-mail devient le Nom du problème.
* Le corps de l’e-mail devient la Description du problème.
* Si l’e-mail contient des documents en pièces jointes, ces documents sont joints au problème dans Workfront.

  >[!NOTE]
  >
  > Les fichiers MSG ne sont pas pris en charge et ne seront pas joints au problème dans Workfront.

* La personne qui envoie l’e-mail devient le contact principal du nouveau problème dans Workfront.
* Le corps du texte de l’e-mail ne peut pas dépasser 4 000 caractères.
* Les pièces jointes aux e-mails ne doivent pas dépasser 7 Mo au total.
