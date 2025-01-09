---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer des groupes de sujets
description: Les groupes de sujets sont associés aux files d’attente des demandes. Ils vous permettent de classer vos files d’attente des demandes en plusieurs catégories, en fonction de la nature des demandes.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: 46c86c1a5e4bb5379409c46669a348ddb53e260b
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 91%

---

# Créer des groupes de sujets

<!-- Audited: 2/2024 -->

Les groupes de sujets sont associés aux files d’attente des demandes. Vous pouvez regrouper vos files d’attente de demandes en plusieurs catégories, selon la nature des demandes à l’aide de groupes de rubriques.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licence Adobe Workfront</p> </td> 
   <td>   
      <p>Nouveau : Standard</p>
      <p>Ou</p> 
      <p>Actuel : formule</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensembe des groupes de rubriques

Si, par exemple, vous disposez d’une file d’attente des demandes pour des requêtes marketing, vous pouvez avoir un groupe de sujets « Campagne Fête des mères », avec deux groupes de sujets de second niveau : l’un intitulé « Médias numériques » et l’autre « Médias imprimés ». Vous pouvez ensuite avoir plusieurs rubriques de file d’attente dans chaque groupe de sujets. Par exemple, « Bannière publicitaire » et « Blog » peuvent être des rubriques de file d’attente pour le groupe de sujets « Médias numériques ».

Pour plus d’informations sur la création de files d’attente des demandes, consultez la section [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Tenez compte des points suivants lorsque vous utilisez des groupes de sujets :

* Vous pouvez créer jusqu’à 10 niveaux de groupes de sujets dans une file d’attente des demandes.
* Le nombre de rubriques de file d’attente pouvant être associées à un groupe de sujets n’est pas limité.
* Les groupes de sujets sont un objet sur lequel un rapport peut être créé.
* Vous ne pouvez pas déplacer des groupes de sujets d&#39;un projet à un autre.

## Créer des groupes de sujets

Nous vous recommandons de créer des groupes de sujets avant de créer une rubrique de file d’attente. Cependant, un groupe de sujets peut être créé dans le créateur de rubriques de file d’attente. Pour plus d’informations sur la création de rubriques de file d’attente, consultez la section [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Pour créer un groupe de sujets :

1. Accédez au projet que vous avez publié en tant que file d’attente des requêtes d’aide.\
   Pour plus d’informations sur la publication d’un projet en tant que file d’attente des requêtes d’aide, consultez la section [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Cliquez sur **Groupes de sujets** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Groupes de sujets**.
1. Cliquez sur **Nouveau groupe de sujets**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Indiquez les informations suivantes :

   * **Nom** : le nom est visible pour les utilisateurs et les utilisatrices qui soumettent des demandes vers cette file d’attente des demandes.
   * **Description** : la description s’affiche lorsque les utilisateurs et les utilisatrices sélectionnent le groupe de sujets dans le processus d’envoi d’une nouvelle requête.
   * **Ajouter au groupe de sujets** : le nouveau groupe de sujets peut être soit ajouté à un groupe de sujets existant, soit ajouté directement au projet publié en tant que file d’attente des requêtes d’aide.

1. Cliquer sur **Enregistrer**.\
   Un nouveau groupe de sujets est ainsi créé dans la file d’attente des demandes. Vous pouvez désormais sélectionner des catégories supplémentaires dans le premier menu déroulant sous une file d’attente des demandes.\
   Pour plus d’informations sur l’envoi de requêtes, consultez la section [Créer et envoyer des requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
