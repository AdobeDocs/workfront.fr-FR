---
title: Soumettre des demandes de planification Adobe Workfront
description: Une fois qu’une personne a partagé avec vous un lien vers un formulaire de demande à partir d’une page de type enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une requête pour créer des enregistrements pour le type d’enregistrement associé au formulaire de demande.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: d7c7b09b033705142b2c658c9d275e63299d3fd0
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 12%

---


# Soumettre des demandes de planification Adobe Workfront pour créer des enregistrements

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Une fois qu’une personne a partagé avec vous un lien vers un formulaire de demande à partir d’une page de type enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une requête pour créer des enregistrements pour le type d’enregistrement associé au formulaire de demande.

Les utilisateurs de Workfront et les utilisateurs externes peuvent envoyer des requêtes à Planification des types d’enregistrement et créer des enregistrements. <!--double check on the external users-->

Cet article décrit comment envoyer une demande d’ajout de nouveaux enregistrements à un type d’enregistrement.

Pour plus d’informations sur la façon dont un gestionnaire d’espace de travail peut créer un formulaire de requête et l’associer à un type d’enregistrement, voir [Création et gestion d’un formulaire de requête dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

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
   <p>Licence externe, contributeur, légère ou standard</p>
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
   <p>Affichage ou autorisations supérieures à un espace de travail si vous êtes un utilisateur Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Pour accéder à la zone Planning dans Workfront, vous devez disposer d’un modèle de mise en page comprenant la zone Planning dans le menu principal. </p>
   <p> Toutefois, l’accès à la zone Planification n’est pas nécessaire pour envoyer des requêtes à Workfront Planning. </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Les éléments suivants doivent être en place avant de pouvoir envoyer une requête à un formulaire de demande de planification Workfront :

* Les éléments suivants doivent exister dans la planification Workfront :

   * Un espace de travail
   * Type d’enregistrement associé à un formulaire de demande. Pour plus d’informations, voir [Création d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Le formulaire de demande doit être partagé avec un lien d’une manière accessible. Les scénarios suivants sont possibles :

   * Si vous disposez d’un compte Workfront, le lien a été partagé uniquement avec les personnes internes et vous disposez d’un accès à l’espace de travail comportant une contribution ou un accès supérieur. Les personnes en dehors de Workfront ne peuvent pas accéder à un lien partagé en interne.
   * Si vous ne disposez pas d’un compte Workfront, le lien a été partagé avec des personnes externes. Les utilisateurs de Workfront peuvent également accéder à un lien partagé avec des personnes externes.

* Le lien vers le formulaire ne doit pas avoir expiré.

## Observations relatives à l’envoi de requêtes à la planification Workfront

* Vous ne pouvez accéder à un formulaire de demande pour les demandes de planification Workfront qu’à partir d’un lien spécifique vers le formulaire.
* Vous ne pouvez pas modifier une requête une fois que vous l’avez envoyée à Workfront Planning.
* Chaque requête envoyée crée un enregistrement pour le type d’enregistrement associé au formulaire que vous utilisez <!--<span class="preview">if the form is not associated with an approval, or if the approval has been granted.</span> -->.
* Les enregistrements créés lors de l’envoi de formulaires de demande ne peuvent pas être différenciés des enregistrements ajoutés par une autre méthode. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* <span class="preview">Les demandes envoyées s’affichent dans l’onglet Planification de la section Envoyées de la zone Demandes de Workfront </span>.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some incosistency between unified-approvals-service and intake-approvals-flow.-->


## Envoi d’une requête à Workfront Planning

1. Accédez au lien partagé avec vous à partir d’un type d’enregistrement Workfront Planning .

1. Mettez à jour les champs disponibles dans le formulaire. Les champs avec un astérisque sont obligatoires.

   >[!TIP]
   >
   >   Si le champ **Objet** est disponible, il ne sera pas visible dans la planification Workfront une fois la demande envoyée.
   >
   >Nous vous recommandons de mettre à jour autant de champs que possible dans votre requête pour que le nouvel enregistrement soit identifiable lorsqu’il est ajouté au type d’enregistrement dans Workfront Planning.

1. Cliquez sur **Soumettre**.

   Votre formulaire est envoyé et les événements suivants se produisent :

   * <!--If the request form was not associated with an approval, or <span class="preview">if the approval was granted</span>, a-->Un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.


   * <!--If the request form was not associated with an approval, the--> <span class="preview"> La demande est ajoutée à la section Envoyée de la zone Requêtes Workfront et un nouvel enregistrement est ajouté à la page de type enregistrement.</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview">Tous les utilisateurs ayant accès à au moins un espace de travail peuvent afficher l’onglet Planification dans la zone Demandes . Vous pouvez afficher uniquement les requêtes que vous avez envoyées. Les administrateurs de Workfront peuvent afficher toutes les requêtes du système. </span> <!--ensure this is correct; asking team in slack-->

   <!--
   * <span class="preview">If the request form was associated with an approval, the request is temporarily saved to the Planning tab in the Submitted section of the Workfront Requests area. No record is created for the record type associated with the request form.</span>

      <span class="preview">For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).</span>  
   -->
   <!--

   * <span class="preview">You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.</span> 
   * <span class="preview">If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.</span> 
   -->



