---
title: Approbation d’une requête
description: Lorsqu’un utilisateur envoie une requête à un formulaire de demande associé à une validation dans Adobe Workfront Planning, les approbateurs reçoivent une notification et un e-mail sur la validation en attente. Il doit approuver la requête avant que Workfront Planning ne crée un objet.
hide: true
hidefromTOC: true
source-git-commit: a999b805016361bdd101a6cd9c61967284a71014
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 20%

---


<!--

---
title: Approve a Request
description: When a user submits a request to a request form associated with an approval in Adobe Workfront Planning, approvers receive a notification and an email about the pending approval. They must approve the request before Workfront Planning creates an object. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->


# Approbation d’une requête

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Lorsqu’un utilisateur envoie une requête à un formulaire de demande associé à une validation dans Adobe Workfront Planning, les approbateurs reçoivent une notification et un e-mail sur la validation en attente. Il doit approuver la requête avant que Workfront Planning ne crée un objet.

Cet article décrit comment un gestionnaire d’espace de travail peut approuver une requête envoyée à Workfront Planning pour créer un enregistrement.

Nous vous recommandons de consulter également les articles suivants :

* [Création et gestion d’un formulaire de requête dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Soumettre des demandes de planification Adobe Workfront pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md)
* [Ajouter une validation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Observations relatives à l’approbation des requêtes et états des requêtes

Les requêtes envoyées s’affichent dans l’onglet Planification de la section Envoyées de la zone Demandes de Workfront avec l’un des états de requête suivants :

* **En attente d’examen** : cet état s’affiche lorsqu’aucun approbateur n’a ouvert l’objet de requête.
* **In review** : l’état devient **In review** lorsque au moins un approbateur ouvre l’objet de requête.
* **Approuvé** : lorsqu’un approbateur approuve l’objet de demande, son état individuel devient
* **Approuvé**, mais l’état global de l’objet de requête reste **En révision** jusqu’à ce que tous les approbateurs aient pris leurs décisions.
* **Completed** : si tous les approbateurs approuvent l’objet de demande, son état passe à **Completed**, ou si la demande n’a pas besoin d’une approbation.
* **Refusé** : si un approbateur rejette l’objet de requête, l’état devient **Refusé**.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produits</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planification d’Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td>
   <td>
<p>L’un des projets Workfront suivants est prévu :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p>
   </td>

<tr>
   <td role="rowheader"><p>Package de planification Adobe Workfront*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <ul>
   <li><p>Gérer les autorisations d’un espace de travail</p></li>
    <li><p>L’administration système peut gérer les espaces de travail qu’elle n’a pas créés. </p></li>
    </ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Approuver une requête pour créer un enregistrement

Une fois que les utilisateurs ont ajouté des requêtes à un formulaire de demande de type enregistrement associé à une validation, la demande est envoyée aux approbateurs.

Les approbateurs reçoivent les notifications suivantes concernant une demande en attente de leur approbation :

* Une notification in-app
* Notification par e-mail

Pour approuver une requête :

1. Utilisez l’une des méthodes suivantes :

   * Dans le **menu principal** ![](assets/dots-menu.png) de Workfront situé dans le coin supérieur droit de l’écran, ou dans le **menu principal** ![](assets/lines-menu.png) dans le coin supérieur gauche, si disponible, cliquez sur **Demandes** > **Envoyées** > **Planification** et cliquez sur la demande avec le statut **Dans la révision**}}. 4}<!--did they change this to Pending approval; logged  a bug-->
   * Accédez à la zone **Notifications** dans le coin supérieur droit de l’écran et cliquez sur la notification à propos d’une demande en attente de votre approbation pour ouvrir la demande.
   * Accédez à la notification électronique dans votre email vous informant d’une demande en attente de votre approbation, puis cliquez pour ouvrir la demande. <!--add the name of the button here, from the email-->

   La page de demande s’ouvre en mode lecture seule.

   ![](assets/read-only-reqeust-page-in-review-status.png)
1. (Facultatif) Cliquez sur l’icône **Validations** ![](assets/approvals-icon.png) dans le coin supérieur droit de la requête pour afficher les approbateurs.
1. Cliquez sur **Réviser et approuver**, puis sélectionnez l’une des options suivantes : <!--did they fix the button and removed the &??-->

   * **Approve** : pour approuver la demande. Un enregistrement est immédiatement créé pour le type d’enregistrement associé au formulaire de demande.
   * **Rejeter** : pour rejeter la demande. Aucun enregistrement n’est créé pour le type d’enregistrement associé au formulaire de demande. <!--check to see if there is a notification sent to the requestor about it being rejected OR approved??-->
