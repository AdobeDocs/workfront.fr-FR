---
product-area: requests
navigation-topic: create-requests
title: Autoriser les utilisateurs à envoyer par e-mail un événement dans un projet de file d'attente des demandes
description: Vous pouvez configurer un projet pour permettre aux utilisateurs et utilisatrices d’ajouter des problèmes au projet par e-mail.
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/G-VPfyHDE9ZhcaqNGaHnZ2bP3lnAHFEwo2SN53cCw9E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 796
ht-degree: 79%

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
   <td> <p>Contributeur ou supérieur</p>
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
>Nous vous recommandons de ne pas avoir plus d’une rubrique de file d’attente pour le projet que vous configurez pour recevoir des demandes par e-mail. Si les requêtes envoyées sont destinées à différents projets ou ressources, vous devez les acheminer ou les déplacer manuellement, après les avoir envoyées.

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
  >* Les fichiers MSG ne sont pas pris en charge et ne seront pas joints au problème dans Workfront.
  >
  >* Si votre environnement a accès à l’espace de stockage Workfront et Adobe hérité pour les documents, les demandes héritent de leur type de stockage de documents à partir du projet, indépendamment de ce que l’administrateur Workfront a sélectionné pour votre préférence de stockage par défaut dans la zone Configuration . Pour plus d’informations, voir [Présentation de la gestion des documents pour les projets et les objets associés](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).

* La personne qui envoie l’e-mail devient le contact principal du nouveau problème dans Workfront.
* Le corps du texte de l’e-mail ne peut pas dépasser 4 000 caractères.
* Les pièces jointes aux e-mails ne doivent pas dépasser 7 Mo au total.
