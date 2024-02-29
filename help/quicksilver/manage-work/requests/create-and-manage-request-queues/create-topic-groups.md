---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Création de groupes de rubriques
description: Les groupes de rubriques sont associés aux files d’attente de demandes. Ils vous permettent de regrouper vos files d’attente de requêtes en plusieurs catégories, selon la nature des requêtes.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: 246750d2a7a053d74df2ceb150f14fdb50f32ade
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Création de groupes de rubriques

<!-- Audited: 2/2024 -->

Les groupes de rubriques sont associés aux files d’attente de demandes. Ils vous permettent de regrouper vos files d’attente de requêtes en plusieurs catégories, selon la nature des requêtes.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licence Adobe Workfront</p> </td> 
   <td>   
      <p>Nouveau : Standard</p>
      <p>Ou</p> 
      <p>Actuel : formule</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Gestion des autorisations pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Présentation des groupes de rubriques

Si, par exemple, vous disposez d’une file d’attente de demandes pour les demandes marketing, vous pouvez avoir un groupe de rubriques de &quot;campagne de la fête des mères&quot;, avec un groupe de rubriques de second niveau de &quot;médias numériques&quot; et un autre groupe de rubriques de second niveau de &quot;médias d’impression&quot;. Vous pouvez ensuite avoir plusieurs rubriques de file d’attente dans chaque groupe de rubriques. Par exemple, &quot;Bannière publicitaire&quot; et &quot;Blog&quot; peuvent être des rubriques de file d’attente pour le groupe de rubriques &quot;Média numérique&quot;.

Pour plus d’informations sur la création de files d’attente de requête, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* Vous pouvez créer jusqu’à 10 niveaux de groupes de rubriques dans une file d’attente de requêtes.
>* Le nombre de rubriques de file d’attente pouvant être associées à un groupe de rubriques n’est pas limité.
>* Les groupes de rubriques sont un objet à reporter.
>

## Création de groupes de rubriques

Nous vous recommandons de créer des groupes de rubriques avant de créer une rubrique de file d’attente. Cependant, un groupe de rubriques peut être créé dans le créateur de rubriques de file d’attente. Pour plus d’informations sur la création de rubriques de file d’attente, voir [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Pour créer un groupe de rubriques :

1. Accédez au projet que vous avez publié en tant que file d’attente des demandes d’aide.\
   Pour plus d’informations sur la publication d’un projet en tant que file d’attente des demandes d’aide, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Cliquez sur **Groupes de rubriques** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis **Groupes de rubriques**.
1. Cliquez sur **Nouveau groupe de rubriques**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Indiquez les informations suivantes :

   * **Nom**: le nom est visible pour les utilisateurs qui envoient des requêtes vers cette file d’attente de requêtes.
   * **Description**: la description s’affiche lorsque les utilisateurs sélectionnent le groupe de rubriques dans le processus d’envoi d’une nouvelle demande.
   * **Ajouter au groupe de rubriques**: vous pouvez ajouter le nouveau groupe de rubriques à un groupe de rubriques existant, ou vous pouvez l’ajouter directement au projet publié en tant que file d’attente de demande d’aide.

1. Cliquer sur **Enregistrer**.\
   Un nouveau groupe de rubriques est ainsi créé dans la file d’attente des demandes. Vous pouvez désormais sélectionner d’autres catégories dans le premier menu déroulant sous une file d’attente de requêtes.\
   Pour plus d’informations sur l’envoi de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
