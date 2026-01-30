---
title: Envoi de requêtes Adobe Workfront Planning
description: Une fois qu'une personne a partagé avec vous un lien vers un formulaire de demande à partir d'une page de type d'enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une demande afin de créer des enregistrements pour le type d'enregistrement associé au formulaire de demande.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '2200'
ht-degree: 2%

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
* Sur la page Type d’enregistrement , lorsque vous ajoutez ou demandez un nouvel enregistrement. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

Cet article décrit comment envoyer une demande d’ajout de nouveaux enregistrements à un type d’enregistrement à partir de la zone des Demandes de Workfront ou d’un lien partagé.

Les utilisateurs de Workfront et les utilisateurs externes peuvent envoyer des demandes aux types d’enregistrements Planning. Les demandes créent des enregistrements pour le type d’enregistrement associé au formulaire de demande. <!--double check on the external users-->

Pour plus d’informations sur la manière dont un gestionnaire d’espace de travail peut créer un formulaire de demande et l’associer à un type d’enregistrement, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Packages Adobe Workfront</p></td> 
   <td> 
<p>Tout package Workfront et tout package Planning</p>
Ou
<p>Tout package de workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Tous</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations d’affichage ou supérieures pour un espace de travail et un type d’enregistrement, si vous êtes un utilisateur Workfront</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Les éléments suivants doivent être en place avant de pouvoir soumettre une demande à un formulaire de demande Workfront Planning :

* Les éléments suivants doivent exister dans Workfront Planning :

   * Un espace de travail
   * Un type d’enregistrement
   * Formulaire de demande associé à un type d’enregistrement.

     Pour plus d’informations, voir [Création d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Le formulaire de demande doit être partagé d&#39;une manière accessible. Les scénarios suivants sont possibles :

   * En interne, le formulaire doit être partagé avec les utilisateurs qui disposent d’autorisations d’affichage ou supérieures dans l’espace de travail.

     Les utilisateurs de Workfront peuvent accéder au formulaire à partir d’un lien ou le trouver dans la zone des Demandes de Workfront.

   * En externe, en partageant un lien vers le formulaire d’enregistrement avec des personnes externes qui ne disposent pas d’un compte Workfront.

     Les utilisateurs de Workfront peuvent également accéder au lien partagé avec des personnes externes.

* S’il est partagé avec un lien, le lien vers le formulaire ne doit pas expirer.

## Considérations relatives à l’envoi de requêtes à Workfront Planning

* Vous ne pouvez pas modifier une demande dans Workfront après l’avoir envoyée.
* Chaque demande envoyée crée un enregistrement pour le type d’enregistrement associé au formulaire que vous utilisez, si le formulaire n’est pas associé à une approbation ou si l’approbation a été accordée par tous les approbateurs.
* Les enregistrements créés par l&#39;envoi de formulaires de demande sont identiques aux enregistrements ajoutés par le biais de toute autre méthode dans Workfront Planning.

  Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* Les enregistrements créés par l’envoi de formulaires de demande sont connectés à la demande d’origine. Impossible de supprimer cette connexion.
* Vous pouvez afficher à la fois les enregistrements créés et les requêtes utilisées pour les créer dans les zones suivantes :
   * Zone des requêtes dans Workfront

  <div class="preview">

   * Pages de type d’enregistrement dans Workfront Planning
   * Zone Détails d’un enregistrement dans Workfront Planning

  </div>

  >[!TIP]
  >
  ><span class="preview">Vous pouvez afficher le nom de la demande dans le champ Objet de la zone Demandes de Workfront ou dans le champ Connexion à la demande d’origine de Workfront Planning. </span>



* Les demandes envoyées s’affichent dans la zone des Demandes de Workfront.
* Les demandes Planning envoyées sont visibles uniquement dans la nouvelle expérience de demande. Les requêtes Planning ne s’affichent pas dans l’expérience des requêtes héritées.
Pour plus d’informations, voir [Création et envoi de demandes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Il existe des limitations dans l’affichage de certains types de champs dans un formulaire de demande ou dans la page des détails de la demande après l’envoi d’un formulaire.

  Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Envoyez une demande à Workfront Planning dans la zone des Demandes de Workfront.

{{step1-to-requests}}

1. Activez le paramètre **Basculer vers une nouvelle expérience** dans le coin supérieur droit de l’écran.
L’activation de ce paramètre rend les formulaires de demande Workfront Planning disponibles dans la zone **Demandes** de Workfront.

   >[!TIP]
   >
   >Ce paramètre est disponible uniquement lorsque votre instance Workfront est intégrée à l’expérience unifiée Adobe.
   >
   >Pour pouvoir envoyer des demandes Workfront Planning dans cette zone, vous devez remplir les conditions suivantes :
   >
   >* Votre société a acheté une licence Workfront Planning.
   >
   >* Vous avez accès à l’affichage d’au moins un espace de travail.

1. Cliquez dans la barre **Quelle requête souhaitez-vous envoyer** pour ouvrir une liste de formulaires de demande.
1. Sélectionnez un formulaire de demande dans la liste ou commencez à saisir son nom, puis sélectionnez-le lorsqu’il apparaît dans la liste.

   Une fenêtre s’ouvre avec le nom du formulaire de demande en haut.
1. Mettez à jour les champs disponibles dans le formulaire de demande. Les champs avec un astérisque rouge sont obligatoires.
1. Cliquez sur **Soumettre**.

   Le formulaire se ferme et vous revenez à la zone **Demandes**.

   Votre formulaire est envoyé et les événements suivants se produisent :

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et du widget Mes demandes dans l’Accueil, et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

     Les champs suivants affichent les informations de demande et d’enregistrement dans la zone des Demandes et le widget Mes demandes dans l’Accueil :

      * **Objet** : nom de la demande d’origine tel qu’il a été ajouté dans la zone des Demandes. Vous ne pouvez pas masquer ni supprimer le champ **Objet** de la liste des demandes.
      * **Objet créé** : nom de l&#39;enregistrement créé à partir de la demande tel qu&#39;il s&#39;affiche dans Planning.
      * **Type d&#39;objet** : nom de l&#39;espace de travail et type d&#39;enregistrement dans lequel des enregistrements ont été créés à partir de la demande dans Planning.
      * **Statut** : statut de l’objet de la requête.
      * **Formulaire de demande** : nom du formulaire de demande associé au type d&#39;enregistrement dans Planning.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et au widget Mes Demandes avec le statut En attente de révision . Un nouvel enregistrement n&#39;est ajouté à la page de type d&#39;enregistrement qu&#39;une fois que les approbateurs l&#39;ont approuvé.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * <span class="preview">Vous pouvez ajouter le champ Connexion de la demande d&#39;origine à un type d&#39;enregistrement dans Planning pour afficher le nom de la demande d&#39;origine qui a créé un enregistrement. Pour plus d’informations, voir [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * La demande est visible uniquement par le propriétaire, l&#39;approbateur et les personnes qui disposent au moins des autorisations d&#39;affichage de l&#39;espace de travail. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système.

   * Vous recevez une notification in-app et un e-mail vous informant que la demande a été soumise avec succès ou envoyée pour révision.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.
     >
     >La demande est associée à un lien dans l’e-mail de confirmation ou de validation.

1. (Facultatif) Cliquez sur **Afficher votre demande** dans le message de confirmation, pour ouvrir la demande, ou cliquez sur l’icône **X** pour fermer la confirmation.
1. (Facultatif) Dans la liste des requêtes, effectuez l’une des opérations suivantes :

   * Cliquez sur **Filtres** et commencez à ajouter des conditions pour les requêtes que vous souhaitez afficher dans la liste des Requêtes.

     ![Modification des filtres dans la zone des Demandes](assets/filters-editing-box-in-requests-planning-tab.png)

     Vous pouvez filtrer selon les champs suivants :

      * **Workspace** : espace de travail auquel le formulaire de demande est associé.
      * **Type d’enregistrement** : type d’enregistrement auquel le formulaire de demande est associé.
      * **Date d’entrée** : date à laquelle la demande a été soumise.
      * **Formulaire de demande** : nom du formulaire de demande utilisé pour soumettre la demande.
      * **Statut** : statut de la demande.
      * **Saisi par** : nom de l’utilisateur qui a ajouté la demande. Si la demande a été ajoutée par une personne extérieure à Workfront, le champ **Saisi par** affiche `N/A`.
      * **Statut de l’objet créé** : le statut de l’enregistrement créé.

     Plusieurs filtres peuvent être joints par **Et** ou **Ou**.
La liste des demandes est automatiquement filtrée à mesure que vous ajoutez les conditions de filtrage.

   * Cliquez sur **Colonnes** pour ouvrir la zone **Visibilité et ordre des champs**, puis masquez, affichez ou réorganisez les colonnes de la liste des demandes.

     >[!TIP]
     >
     >Vous ne pouvez plus ajouter de colonnes.

     ![Zone d&#39;édition Colonnes de la zone Demandes](assets/columns-editing-box-in-requests-planning-tab.png)
   * Cliquez sur l’icône **+** dans le coin supérieur droit de la liste des requêtes pour ouvrir le **Gestionnaire de colonnes** et ajouter ou supprimer des colonnes de la liste des requêtes.

1. Cliquez sur le nom d’une requête dans la liste.

   La page des détails de la requête s’ouvre.

   ![Demander une page avec des commentaires](assets/new-request-page-with-comment.png)

1. (Facultatif) Saisissez un commentaire dans la zone **Commentaires**.
1. (Conditionnel) Si le formulaire de demande n&#39;est pas associé à une approbation, ou si la demande a été approuvée, cliquez sur le nom de la demande, puis cliquez sur le nom de l&#39;enregistrement dans le champ **Objet créé**.

   La page de l’enregistrement s’ouvre dans Workfront Planning.

   >[!TIP]
   >
   >* Si le champ principal de l’enregistrement n’a pas été mis à jour dans le formulaire de demande, le nom de l’enregistrement dans le champ Enregistrement de la demande s’affiche comme **Sans titre**.
   >
   >* Si le formulaire de demande est associé à une approbation, l&#39;approbation doit être accordée avant que vous puissiez accéder à l&#39;enregistrement à partir de la page de demande.

1. (Facultatif) Cliquez sur le nom du **Type d’enregistrement**.

   La page de type d’enregistrement s’ouvre dans Workfront Planning.

## Envoyez une demande à Workfront Planning à partir d’un lien partagé vers un formulaire de demande

Les informations de cette section s’appliquent uniquement aux utilisateurs de Workfront qui envoient une demande à partir d’un lien partagé. Les personnes externes ne peuvent pas accéder aux zones internes de Workfront, comme Requêtes ou Accueil.

1. Accédez au lien partagé avec vous à partir d’un type d’enregistrement Workfront Planning .

1. Mettez à jour les champs disponibles dans le formulaire. Les champs avec un astérisque sont obligatoires.

   >[!TIP]
   >
   >   Si le champ **Objet** est disponible, il ne sera pas visible dans Workfront Planning, une fois la demande soumise.
   >
   >Nous vous recommandons de mettre à jour autant de champs que possible dans votre demande afin de rendre le nouvel enregistrement identifiable lorsqu&#39;il est ajouté au type d&#39;enregistrement dans Workfront Planning.

1. Cliquez sur **Soumettre**.

   Votre formulaire est envoyé et les événements suivants se produisent :

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et du widget Mes demandes dans l’Accueil, et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et du widget Mes Demandes . Un nouvel enregistrement n&#39;est ajouté à la page de type d&#39;enregistrement qu&#39;une fois que tous les approbateurs l&#39;ont approuvé.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     >[!IMPORTANT]
     >
     >Vous pouvez afficher uniquement les requêtes que vous ou une autre personne avez envoyées aux espaces de travail que vous êtes au moins autorisé à afficher. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système. <!--ensure this is correct; asking team in slack-->

   * Vous recevez une notification in-app et un e-mail vous informant que la demande a été soumise avec succès ou envoyée pour révision.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.

   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. (Facultatif) Cliquez sur **Afficher votre demande** pour ouvrir la demande dans Workfront.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Facultatif) Cliquez sur **Menu principal** > **Demandes** pour afficher votre demande, puis cliquez sur son nom.

   La page des détails de la requête s’ouvre.

   ![Demander une page avec des commentaires](assets/new-request-page-with-comment.png)

1. (Facultatif) Saisissez un commentaire dans la zone Commentaires.
1. (Conditionnel) Si le formulaire de demande n&#39;est pas associé à une approbation, ou si la demande a été approuvée, cliquez sur le nom de la demande, puis cliquez sur le nom de l&#39;enregistrement dans le champ **Objet créé**.

   La page de l’enregistrement s’ouvre dans Workfront Planning.

   >[!TIP]
   >
   >* Si le nom d’enregistrement n’a pas été ajouté au formulaire de demande, le nom de l’enregistrement dans le champ Enregistrement de la demande s’affiche comme **Sans titre**.
   >
   >* Si le formulaire de demande est associé à une approbation, l&#39;approbation doit être accordée avant que vous puissiez accéder à l&#39;enregistrement à partir de la page de demande.

1. (Facultatif) Cliquez sur le nom du **Type d’objet**.

   La page de type d’enregistrement s’ouvre dans Workfront Planning.

## Création d’une demande en copiant une demande existante

Vous pouvez copier une demande dans la liste des demandes de Workfront, puis modifier les détails et l’envoyer en tant que nouvelle demande.

Cette option est disponible uniquement dans la nouvelle expérience de demande.

Pour obtenir des instructions, voir [ Copier et envoyer des demandes ](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Créer des brouillons et des demandes à partir de brouillons existants

Vous pouvez créer un brouillon d’une demande, puis revenir au brouillon et l’envoyer ultérieurement en tant que demande.

Cette option est disponible uniquement dans la nouvelle expérience de demande.

Pour obtenir des instructions, voir [Création de requêtes à partir de brouillons](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).



