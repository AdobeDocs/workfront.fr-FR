---
title: Envoi de requêtes Adobe Workfront Planning
description: Une fois qu'une personne a partagé avec vous un lien vers un formulaire de demande à partir d'une page de type d'enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une demande afin de créer des enregistrements pour le type d'enregistrement associé au formulaire de demande.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 46c86c1a5e4bb5379409c46669a348ddb53e260b
workflow-type: tm+mt
source-wordcount: '975'
ht-degree: 10%

---

# Envoi de requêtes Adobe Workfront Planning pour créer des enregistrements

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Une fois qu&#39;une personne a partagé avec vous un lien vers un formulaire de demande à partir d&#39;une page de type d&#39;enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une demande afin de créer des enregistrements pour le type d&#39;enregistrement associé au formulaire de demande.

Les utilisateurs de Workfront et les utilisateurs externes peuvent envoyer des demandes aux types d&#39;enregistrements Planning et créer des enregistrements. <!--double check on the external users-->

Cet article décrit comment soumettre une demande d&#39;ajout de nouveaux enregistrements à un type d&#39;enregistrement.

Pour plus d’informations sur la manière dont un gestionnaire d’espace de travail peut créer un formulaire de demande et l’associer à un type d’enregistrement, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

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
<p>L’un des plans Workfront suivants :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p>
   </td>
<tr>
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>
<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Licence externe, contributeur, light ou standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p>
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
   <p>Autorisations d’affichage ou supérieures pour un espace de travail, si vous êtes un utilisateur de Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Pour accéder à la zone Planning dans Workfront, vous devez disposer d'un modèle de mise en page qui inclut la zone Planning dans le menu principal. </p>
   <p> Cependant, il n’est pas nécessaire d’accéder à la zone Planning pour envoyer des requêtes à Workfront Planning. </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Les éléments suivants doivent être en place avant de pouvoir soumettre une demande à un formulaire de demande Workfront Planning :

* Les éléments suivants doivent exister dans Workfront Planning :

   * Un espace de travail
   * Type d’enregistrement associé à un formulaire de demande. Pour plus d’informations, voir [Création d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Le formulaire de demande doit être partagé avec un lien de manière à pouvoir y accéder. Les scénarios suivants sont possibles :

   * Si vous disposez d’un compte Workfront, le lien a été partagé uniquement avec des personnes internes et vous disposez d’un accès de niveau Contribution ou supérieur à l’espace de travail. Les personnes extérieures à Workfront ne peuvent pas accéder à un lien partagé en interne.
   * Si vous ne disposez pas d’un compte Workfront, le lien a été partagé avec des personnes externes. Les utilisateurs de Workfront peuvent également accéder à un lien partagé avec des personnes externes.

* Le lien vers le formulaire ne doit pas expirer.

## Considérations relatives à l’envoi de requêtes à Workfront Planning

* Vous pouvez accéder à un formulaire de demande pour les demandes Workfront Planning uniquement à partir d’un lien spécifique vers le formulaire.
* Vous ne pouvez pas modifier une demande après l’avoir envoyée à Workfront Planning.
* Chaque demande envoyée crée un enregistrement pour le type d’enregistrement associé au formulaire que vous utilisez <span class="preview">si le formulaire n’est pas associé à une approbation ou si l’approbation a été accordée par tous les approbateurs.</span>
* Les enregistrements créés en soumettant des formulaires de demande ne peuvent pas être différenciés des enregistrements ajoutés par une autre méthode. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* <span class="preview">Les demandes envoyées s’affichent dans l’onglet Planification de la section Envoyées de la zone Demandes de la </span> Workfront.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Envoi d’une demande à Workfront Planning

1. Accédez au lien partagé avec vous à partir d’un type d’enregistrement Workfront Planning .

1. Mettez à jour les champs disponibles dans le formulaire. Les champs avec un astérisque sont obligatoires.

   >[!TIP]
   >
   >   Si le champ **Objet** est disponible, il ne sera pas visible dans Workfront Planning, une fois la demande soumise.
   >
   >Nous vous recommandons de mettre à jour autant de champs que possible dans votre demande afin de rendre le nouvel enregistrement identifiable lorsqu&#39;il est ajouté au type d&#39;enregistrement dans Workfront Planning.

1. Cliquez sur **Soumettre**.

   Votre formulaire est envoyé et les événements suivants se produisent :

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à l’onglet <span class="preview">Planification) de la section Envoyés de la zone des Demandes Workfront </span> et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

   * Si le formulaire de demande a été associé à une approbation, la demande de <span class="preview"> est ajoutée à l’onglet Planification de la section Soumis de la zone Demandes Workfront . Un nouvel enregistrement n&#39;est ajouté à la page de type d&#39;enregistrement qu&#39;une fois que tous les approbateurs l&#39;ont approuvé.</span>
     <span class="preview">Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md).</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview">Tous les utilisateurs ayant accès à au moins un espace de travail peuvent afficher l&#39;onglet Planification dans la zone Demandes. Vous pouvez afficher uniquement les requêtes que vous ou une autre personne avez envoyées aux espaces de travail que vous êtes au moins autorisé à afficher. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système. </span> <!--ensure this is correct; asking team in slack-->

   * <span class="preview">Vous recevez une notification in-app et par e-mail indiquant que la demande a été soumise avec succès ou a été envoyée pour révision.</span>
   * <span class="preview">Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.</span>

     >[!NOTE]
     >
     ><span class="preview">Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée d’Adobe.</span>




