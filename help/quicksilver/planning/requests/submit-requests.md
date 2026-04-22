---
title: Envoi de requêtes Adobe Workfront Planning
description: Une fois qu'une personne a partagé avec vous un lien vers un formulaire de demande à partir d'une page de type d'enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une demande afin de créer des enregistrements pour le type d'enregistrement associé au formulaire de demande.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 3%

---

# Envoyer des demandes Adobe Workfront Planning pour créer des enregistrements

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Une fois qu’un gestionnaire d’espace de travail a créé un formulaire de demande pour un type d’enregistrement dans Adobe Workfront Planning, vous pouvez utiliser le formulaire pour envoyer des demandes qui créeront des enregistrements pour le type d’enregistrement associé au formulaire.

Vous pouvez envoyer une demande Workfront Planning à partir des zones suivantes :

* Dans la zone des Requêtes de Workfront ou dans le widget Mes requêtes de l’Accueil.
* D’un lien direct vers le formulaire de demande qui a été partagé.
* À partir de la page Type d’enregistrement , lorsque vous ajoutez un nouvel enregistrement en soumettant une demande. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

Cet article décrit comment envoyer une demande d’ajout de nouveaux enregistrements à un type d’enregistrement à partir de la zone des Demandes de Workfront ou d’un lien partagé.

Les responsables Workspace peuvent créer des formulaires de demande que vous pouvez utiliser, en tant qu&#39;utilisateur ou personne externe, pour envoyer des demandes aux types d&#39;enregistrements Planning. Les demandes créent des enregistrements pour le type d’enregistrement associé au formulaire de demande.

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
<p>Tout package de Workfront ou de workflow</p>
<p>Tout package Workfront Planning</p>
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
   * Zone des requêtes dans Workfront.
   * Dans un champ connecté d’une page de type d’enregistrement dans Workfront Planning, lorsque vous ajoutez la requête en tant qu’enregistrement connecté.
   * Dans un champ connecté de la zone Détails d’un enregistrement dans Workfront Planning lorsque vous ajoutez la requête en tant qu’enregistrement connecté.

  >[!TIP]
  >
  >Vous pouvez afficher le nom de la demande dans le champ Objet de la zone Demandes de Workfront ou dans le champ Connexion à la demande d’origine de Workfront Planning.

* Les demandes Planning envoyées sont visibles uniquement dans la nouvelle expérience de demande. Les requêtes Planning ne s’affichent pas dans l’expérience des requêtes héritées.

  Pour plus d’informations, voir [Création et envoi de demandes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Il existe des limitations dans l’affichage de certains types de champs dans un formulaire de demande ou dans la page des détails de la demande après l’envoi d’un formulaire.

  Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--
Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.
-->


## Envoyez une demande à Workfront Planning dans la zone des Demandes de Workfront.

{{step1-to-requests}}

1. Activez le paramètre **Utiliser une nouvelle expérience** dans le coin supérieur droit de l’écran.
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

1. Cliquez dans le champ **Quelle requête souhaitez-vous soumettre ?** la barre pour ouvrir une liste de formulaires de demande.
1. Sélectionnez un formulaire de demande dans la liste ou commencez à saisir son nom, puis sélectionnez-le lorsqu’il apparaît dans la liste.

   Une fenêtre s’ouvre avec le nom du formulaire de demande en haut.

   >[!TIP]
   >
   >Les files d’attente des demandes Workfront contiennent le nom de la file d’attente et le nom du formulaire dans la liste des demandes. Les formulaires de demandes Planning affichent uniquement le nom du formulaire dans la liste des demandes.

1. Mettez à jour le champ **Objet**. Il s’agit du nom de la requête. Champ obligatoire.
1. Mettez à jour le champ **Nom**. Il s’agit du nom du futur enregistrement.

   >[!TIP]
   >
   >Le champ **Nom** est propre à votre organisation et peut afficher un libellé différent dans votre instance Workfront. Le champ est le champ principal de l’enregistrement.

1. Mettez à jour les champs restants dans le formulaire de demande. Les champs avec un astérisque rouge sont obligatoires.
1. (Conditionnel) Si votre entreprise autorise le **remplissage de formulaire** optimisé par l’IA, vous pouvez charger des documents sous forme d’invites. L’IA utilise ces documents pour remplir le formulaire. Vous pouvez accepter ou refuser les suggestions de l’IA avant d’envoyer la requête.


   Pour obtenir des instructions, consultez [Utilisation du remplissage de formulaire optimisé par l’IA pour remplir une requête à l’aide d’invites ou de documents](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).
1. Cliquez sur **Soumettre**.

   Le formulaire se ferme et vous revenez à la zone **Demandes**.

   Votre formulaire est envoyé et les événements suivants se produisent :

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et du widget Mes demandes dans l’Accueil, et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

     Les champs suivants affichent les informations de demande et d’enregistrement dans la zone des Demandes et le widget Mes demandes dans l’Accueil :

      * **Objet** : nom de la demande d’origine tel qu’il a été ajouté dans la zone des Demandes. Vous ne pouvez pas masquer ni supprimer le champ **Objet** de la liste des demandes. Le nom comporte un lien qui ouvre la page de requête dans Planning.
      * **Objet créé** : nom de l&#39;enregistrement créé à partir de la demande tel qu&#39;il s&#39;affiche dans Planning. Le nom de l’objet Créé comporte un lien qui ouvre l’enregistrement créé à partir de la requête.
      * **Type d&#39;objet** : nom de l&#39;espace de travail et type d&#39;enregistrement dans lequel des enregistrements ont été créés à partir de la demande dans Planning.
      * **Statut** : statut de l’objet de la requête.
      * **Formulaire de demande** : nom du formulaire de demande associé au type d&#39;enregistrement dans Planning.
      * **Statut de l’objet créé** : le statut de l’enregistrement créé.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et au widget Mes Demandes avec le statut **En attente de révision**. Un nouvel enregistrement n&#39;est ajouté à la page de type d&#39;enregistrement qu&#39;une fois que les approbateurs l&#39;ont approuvé.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * Vous pouvez ajouter le champ de connexion **Demande d&#39;origine** à un type d&#39;enregistrement dans Planning afin d&#39;afficher le nom de la demande d&#39;origine qui a créé un enregistrement. Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).
   * La demande est visible uniquement par le propriétaire, l&#39;approbateur et les personnes qui disposent au moins des autorisations d&#39;affichage de l&#39;espace de travail. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système.
   * Vous recevez une notification in-app et un e-mail vous informant que la demande a été soumise avec succès ou envoyée pour révision.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.
     >
     >La demande est associée à un lien dans l’e-mail de confirmation ou de validation.

1. (Facultatif) Cliquez sur **Afficher votre demande** dans le message de confirmation, pour ouvrir la demande, ou cliquez sur l’icône **X** pour fermer la confirmation.
1. (Facultatif) Pour gérer l’affichage des informations dans la liste des demandes, mettez à jour les éléments d’affichage suivants pour la liste :

   * Afficher
   * Filtre
   * Colonnes
   * Regroupement
   * Formater les cellules
   * Hauteur de ligne

   Pour plus d’informations, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   <!-- 
   Removing this as this is covered at a higher level in the Use enhanced lists article: 
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

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
   >* Si le formulaire de demande est associé à une approbation, l&#39;approbation doit être accordée avant que vous puissiez accéder à l&#39;enregistrement à partir de la page de demande. L&#39;enregistrement n&#39;est pas créé tant que l&#39;approbation n&#39;a pas été accordée.

1. (Facultatif) Cliquez sur le nom du **Type d’enregistrement**.

   La page de type d’enregistrement s’ouvre dans Workfront Planning.

## Envoyez une demande à Workfront Planning à partir d’un lien partagé vers un formulaire de demande

Les informations de cette section s’appliquent uniquement aux personnes qui envoient une demande à partir d’un lien partagé et qui peuvent ne pas disposer d’un compte Workfront.

Les personnes externes ne peuvent pas accéder aux zones internes de Workfront, comme **Demandes** ou **Accueil**.

1. Accédez au lien partagé avec vous à partir d’un type d’enregistrement Workfront Planning .

1. Mettez à jour les champs disponibles dans le formulaire. Les champs avec un astérisque sont obligatoires.

   >[!TIP]
   >
   >   Si le champ **Objet** est disponible, il ne sera pas visible dans Workfront Planning, une fois la demande soumise.
   >
   >Nous vous recommandons de mettre à jour autant de champs que possible dans votre demande afin de rendre le nouvel enregistrement identifiable lorsqu&#39;il est ajouté au type d&#39;enregistrement dans Workfront Planning.

1. Cliquez sur **Soumettre**.

   Votre formulaire est envoyé et vous obtenez une confirmation.

   Si le formulaire est associé à une approbation, il doit être approuvé avant de créer un enregistrement.

1. (Facultatif) Cliquez sur **Soumettre une autre demande** pour ajouter une autre demande utilisant le même lien partagé.

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et du widget Mes demandes dans l’Accueil, et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire. Cette option est disponible uniquement lorsque vous vous connectez à Workfront.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à la liste des Demandes dans la zone des Demandes Workfront et au widget Mes demandes a le statut En attente de révision. Un nouvel enregistrement n&#39;est ajouté à la page de type d&#39;enregistrement qu&#39;une fois que tous les approbateurs l&#39;ont approuvé. Cette option est disponible uniquement lorsque vous vous connectez à Workfront.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     >[!IMPORTANT]
     >
     >Vous pouvez afficher uniquement les requêtes que vous ou une autre personne avez envoyées aux espaces de travail que vous êtes au moins autorisé à afficher. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système.

   * Vous recevez une notification in-app et un e-mail vous informant que la demande a été soumise avec succès ou envoyée pour révision.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.

     Une fois la demande approuvée et l&#39;enregistrement créé, les champs Date d&#39;approbation par et Date d&#39;approbation affichent des informations sur l&#39;approbation dans l&#39;enregistrement.

1. (Facultatif) Cliquez sur **Afficher votre demande** pour ouvrir la demande dans Workfront.

Ou

Cliquez sur [Soumettre une autre demande](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) pour ouvrir le formulaire de demande et ajouter une nouvelle demande.

La page des détails de la requête s’ouvre.

![Demander une page avec des commentaires](assets/new-request-page-with-comment.png)

1. (Facultatif) Saisissez un commentaire dans la zone **Commentaires**.
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

La copie d’une demande Planning existante et son envoi en tant que nouvelle sont similaires à la copie d’une demande Workfront existante.

Pour plus d’informations, voir [Copier et soumettre des demandes](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Créer des brouillons et des demandes à partir de brouillons existants

Vous pouvez créer un brouillon d’une demande, puis revenir au brouillon et l’envoyer ultérieurement en tant que demande.

Cette option est disponible uniquement dans la nouvelle expérience de demande. La création de brouillons et de demandes à partir de brouillons existants dans Workfront Planning est identique à leur création à partir d’Adobe Workfront.

Pour plus d’informations, consultez la section [Créer des demandes à partir de brouillons](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

## Supprimer les brouillons ou les demandes envoyées

Vous pouvez supprimer des demandes envoyées ou leurs brouillons lorsque vous utilisez la nouvelle expérience de demandes.

Lorsque vous supprimez une demande Planning, les événements suivants se produisent :

* La requête ne peut pas être récupérée.
* L’enregistrement créé à partir de la demande n’est pas supprimé.
* Les brouillons supprimés ne peuvent pas être récupérés. Aucun enregistrement n&#39;est associé aux brouillons.

La suppression des demandes Planning est similaire à la suppression des demandes Workfront.

Pour plus d’informations, voir [Supprimer une demande envoyée ou un brouillon de demande](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md).







