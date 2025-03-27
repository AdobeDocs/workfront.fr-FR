---
title: Envoi de requêtes Adobe Workfront Planning
description: Une fois qu'une personne a partagé avec vous un lien vers un formulaire de demande à partir d'une page de type d'enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une demande afin de créer des enregistrements pour le type d'enregistrement associé au formulaire de demande.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '1878'
ht-degree: 5%

---

# Envoi de requêtes Adobe Workfront Planning pour créer des enregistrements

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Une fois qu’un gestionnaire d’espace de travail a créé un formulaire de demande pour un type d’enregistrement dans Adobe Workfront Planning, vous pouvez utiliser le formulaire pour envoyer des demandes qui créeront des enregistrements pour le type d’enregistrement associé au formulaire.

Vous pouvez envoyer une demande Workfront Planning à partir des zones suivantes :

* Dans la zone Demandes de Workfront.
* D’un lien direct vers le formulaire de demande qui a été partagé.

  Cet article décrit comment envoyer une demande d’ajout de nouveaux enregistrements à un type d’enregistrement à partir de la zone des Demandes de Workfront ou d’un lien partagé.
* <span class="preview">À partir de la page Type d’enregistrement, lorsque vous ajoutez ou demandez un nouvel enregistrement. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).</span>

Les utilisateurs de Workfront et les utilisateurs externes peuvent envoyer des demandes aux types d&#39;enregistrements Planning et créer des enregistrements. <!--double check on the external users-->

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
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p>
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
   <p>Autorisations d’affichage ou supérieures à un <!--<span class="preview">and record type</span>--> d’espace de travail, si vous êtes un utilisateur de Workfront</p> 
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
   * Un type d’enregistrement.
   * Formulaire de demande associé à un type d’enregistrement.

     Pour plus d’informations, voir [Création d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Le formulaire de demande doit être partagé d&#39;une manière accessible. Les scénarios suivants sont possibles :

   * En interne, le formulaire doit être partagé avec les utilisateurs qui disposent d’autorisations d’affichage ou supérieures dans l’espace de travail.

     Les utilisateurs de Workfront peuvent accéder au formulaire à partir d’un lien <span class="preview">ou le trouver dans la zone des Demandes de Workfront.</span>

   * Si vous ne disposez pas d’un compte Workfront, un lien vers le formulaire a été partagé avec des personnes externes.

     Les utilisateurs de Workfront peuvent également accéder à un lien partagé avec des personnes externes.

* Le lien vers le formulaire ne doit pas expirer.

## Considérations relatives à l’envoi de requêtes à Workfront Planning

* Vous ne pouvez pas modifier une demande dans Workfront après l’avoir envoyée.
* Chaque demande envoyée crée un enregistrement pour le type d’enregistrement associé au formulaire que vous utilisez, si le formulaire n’est pas associé à une approbation ou si l’approbation a été accordée par tous les approbateurs.
* Les enregistrements créés en soumettant des formulaires de demande ne peuvent pas être différenciés des enregistrements ajoutés par une autre méthode dans Workfront Planning.

  Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* Les demandes envoyées s’affichent dans l’onglet Planification de la section Envoyées dans la zone des Demandes de Workfront.
* Il existe des limitations dans l’affichage de certains types de champs dans un formulaire de demande ou dans la page des détails de la demande après l’envoi d’un formulaire.

  Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


<div class="preview">

## Envoyez une demande à Workfront Planning dans la zone des Demandes de Workfront.

>[!NOTE]
>
>Après les versions mensuelles de la production, les fonctionnalités décrites dans cette section sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides.

{{step1-to-requests}}

1. Activez le paramètre **Basculer vers une nouvelle expérience** dans le coin supérieur droit de l’écran.
L’activation de ce paramètre rend les formulaires de demande Workfront Planning disponibles dans la zone **Demandes** de Workfront.

   >[!TIP]
   >
   >Ce paramètre est disponible uniquement lorsque les éléments suivants sont en place :
   >
   >* Votre société a acheté un package Workfront Planning.
   >* Votre instance Workfront est intégrée à l’expérience unifiée Adobe.
   >* Vous avez accès à l’affichage d’au moins un espace de travail.
   >

1. Cliquez sur **Nouvelle demande**.

   ![Nouvelle boîte de requête avec des cartes Workfront et Planning unifiées](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   La boîte de dialogue **Nouvelle demande** s’ouvre avec les informations suivantes :

   * Les 6 dernières files d’attente de demandes Workfront consultées et les formulaires de demandes Planning s’affichent dans la section Récent .
   * 50 files d’attente de demandes Workfront supplémentaires et les formulaires de demandes Planning s’affichent par ordre alphabétique dans la section **Tous les formulaires de demandes**. Vous pouvez rechercher une file d’attente de demandes qui ne s’affiche pas par défaut.

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur la carte de l&#39;un des formulaires de demande Planning dans les sections Formulaires de demande récents ou Tous les formulaires de demande
   * Commencez à saisir le nom d&#39;un formulaire de demande Planning dans la zone de recherche, puis cliquez sur la carte lorsqu&#39;elle s&#39;affiche dans la liste.

   Le formulaire de demande s’ouvre.

1. Mettez à jour les champs disponibles dans le formulaire de demande. Les champs avec un astérisque rouge sont obligatoires.
1. Cliquez sur **Soumettre**.

   Le formulaire se ferme et vous revenez à la zone **Demandes**.

   Votre formulaire est envoyé et les événements suivants se produisent :

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Envoyés de la zone Demandes Workfront et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Soumis de la zone Demandes Workfront . Un nouvel enregistrement n&#39;est ajouté à la page de type d&#39;enregistrement qu&#39;une fois que tous les approbateurs l&#39;ont approuvé.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Zone des requêtes avec bouton (bascule) pour l’onglet Planification de workflow unifiée](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >Tous les utilisateurs ayant accès à au moins un espace de travail peuvent afficher l&#39;onglet Planification dans la zone Demandes. Vous pouvez afficher uniquement les requêtes que vous ou une autre personne avez envoyées aux espaces de travail que vous êtes au moins autorisé à afficher. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système.

   * Vous recevez une notification in-app et un e-mail vous informant que la demande a été soumise avec succès ou envoyée pour révision.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.

   1. (Facultatif) Cliquez sur **Afficher votre demande** dans le message de confirmation, pour ouvrir la demande, ou cliquez sur l’icône **X** pour fermer la confirmation.

1. (Facultatif) Cliquez sur l’onglet **Planification** dans la zone Demandes pour afficher votre demande, puis cliquez sur son nom.

   La page des détails de la requête s’ouvre.

   ![Page de détails de la demande](assets/request-details-page.png)

1. (Conditionnel) Si le formulaire de demande n&#39;est pas associé à une approbation, ou si la demande a été approuvée, cliquez sur le nom de la demande, puis cliquez sur le nom de l&#39;enregistrement dans le champ **Enregistrement**.

   La page de l’enregistrement s’ouvre dans Workfront Planning.

   >[!TIP]
   >
   >* Si le champ principal de l’enregistrement n’a pas été mis à jour dans le formulaire de demande, le nom de l’enregistrement dans le champ Enregistrement de la demande s’affiche comme **Sans titre**.
   >
   >* Si le formulaire de demande est associé à une approbation, l&#39;approbation doit être accordée avant que vous puissiez accéder à l&#39;enregistrement à partir de la page de demande.

1. (Facultatif) Cliquez sur le nom du **Type d’enregistrement**.

   La page de type d’enregistrement s’ouvre dans Workfront Planning.

</div>

## Envoyez une demande à Workfront Planning à partir d’un lien partagé vers un formulaire de demande

1. Accédez au lien partagé avec vous à partir d’un type d’enregistrement Workfront Planning .

1. Mettez à jour les champs disponibles dans le formulaire. Les champs avec un astérisque sont obligatoires.

   >[!TIP]
   >
   >   Si le champ **Objet** est disponible, il ne sera pas visible dans Workfront Planning, une fois la demande soumise.
   >
   >Nous vous recommandons de mettre à jour autant de champs que possible dans votre demande afin de rendre le nouvel enregistrement identifiable lorsqu&#39;il est ajouté au type d&#39;enregistrement dans Workfront Planning.

1. Cliquez sur **Soumettre**.

   Votre formulaire est envoyé et les événements suivants se produisent :

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Envoyés de la zone Demandes Workfront et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Soumis de la zone Demandes Workfront . Un nouvel enregistrement n&#39;est ajouté à la page de type d&#39;enregistrement qu&#39;une fois que tous les approbateurs l&#39;ont approuvé.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Onglet Planification dans les demandes](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Tous les utilisateurs ayant accès à au moins un espace de travail peuvent afficher l&#39;onglet Planification dans la zone Demandes. Vous pouvez afficher uniquement les requêtes que vous ou une autre personne avez envoyées aux espaces de travail que vous êtes au moins autorisé à afficher. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système. <!--ensure this is correct; asking team in slack-->

   * Vous recevez une notification in-app et un e-mail vous informant que la demande a été soumise avec succès ou envoyée pour révision.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.

1. <span class="preview">(facultatif) Cliquez sur **Afficher votre demande** pour ouvrir la demande dans Workfront.</span>

   Ou

   <span class="preview">Cliquez sur [Soumettre une autre demande](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) pour ouvrir le formulaire de demande et ajouter une nouvelle demande. </span>

1. (Facultatif) Cliquez sur **Menu principal** > **Demandes** > l’onglet **Planification** pour afficher votre demande, puis cliquez sur son nom.

   La page des détails de la requête s’ouvre.

   ![Page de détails de la demande](assets/request-details-page.png)

1. (Conditionnel) Si le formulaire de demande n&#39;est pas associé à une approbation, ou si la demande a été approuvée, cliquez sur le nom de la demande, puis cliquez sur le nom de l&#39;enregistrement dans le champ **Enregistrement**.

   La page de l’enregistrement s’ouvre dans Workfront Planning.

   >[!TIP]
   >
   >* Si le nom d’enregistrement n’a pas été ajouté au formulaire de demande, le nom de l’enregistrement dans le champ Enregistrement de la demande s’affiche comme **Sans titre**.
   >
   >* Si le formulaire de demande est associé à une approbation, l&#39;approbation doit être accordée avant que vous puissiez accéder à l&#39;enregistrement à partir de la page de demande.

1. (Facultatif) Cliquez sur le nom du **Type d’enregistrement**.

   La page de type d’enregistrement s’ouvre dans Workfront Planning.




