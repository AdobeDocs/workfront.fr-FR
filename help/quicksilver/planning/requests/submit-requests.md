---
title: Soumettre Adobe des demandes de planification de front
description: Une fois qu’une personne partage avec vous un lien vers un formulaire de demande à partir d’une page de type d’enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une demande pour créer des enregistrements pour le type d’enregistrement associé au formulaire de demande.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '2019'
ht-degree: 4%

---

# Soumettre des requêtes de planification Adobe Workfront pour créer des enregistrements

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement d’aperçu pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activer ou désactiver les versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Une fois qu’un gestionnaire d’espace de travail a créé un formulaire de demande pour un type d’enregistrement dans Adobe Workfront Planning, vous pouvez utiliser le formulaire pour soumettre des demandes qui créeront des enregistrements pour le type d’enregistrement associé au formulaire.

Vous pouvez soumettre une demande de Workfront Planning à partir des zones suivantes :

* Dans la zone Requêtes de Workfront.
* À partir d’un lien direct vers le formulaire de demande qui a été partagé.

  Cet article décrit comment envoyer une demande d’ajout de nouveaux enregistrements à un type d’enregistrement à partir de la zone des Demandes de Workfront ou d’un lien partagé.
* Sur la page Type d’enregistrement , lorsque vous ajoutez ou demandez un nouvel enregistrement. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

Les utilisateurs de Workfront et les utilisateurs externes peuvent envoyer des demandes aux types d&#39;enregistrements Planning et créer des enregistrements. <!--double check on the external users-->

Pour plus d’informations sur la manière dont un gestionnaire d’espace de travail peut créer un formulaire de demande et l’associer à un type d’enregistrement, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
<p>La planification de front de travail n’est pas disponible pour les plans de front hérités</p>
   </td>
<tr>
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur ce qui est inclus dans chaque plan Workfront Planning, contactez votre responsable de compte Workfront. </td>
<tr>
   <td role="rowheader"><p>Adobe Plateforme Workfront</p></td>
   <td>
<p>L’instance Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Licence externe, Contributeur, Light ou Standard</p>
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
   <p>Afficher ou des autorisations supérieures pour un espace de travail et un type d’enregistrement, si vous êtes un utilisateur Workfront</p> 
  </td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Conditions préalables

Les éléments suivants doivent être en place pour que vous puissiez soumettre une demande à un formulaire de demande Workfront Planning :

* Les éléments suivants doivent exister dans Workfront Planning :

   * Un espace de travail
   * Type d’enregistrement.
   * Formulaire de demande associé à un type d’enregistrement.

     Pour plus d’informations, voir [Créer un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Le formulaire de demande doit être partagé d&#39;une manière accessible. Les scénarios suivants sont possibles :

   * En interne, le formulaire doit être partagé avec les utilisateurs qui disposent d’autorisations d’affichage ou supérieures dans l’espace de travail.

     Les utilisateurs de Workfront peuvent accéder au formulaire à partir d’un lien ou trouver le formulaire de demande dans la zone Requêtes de Workfront.

   * Si vous n’avez pas de compte Workfront, un lien vers le formulaire a été partagé avec des personnes externes.

     Les utilisateurs de Workfront peuvent également accéder à un lien partagé avec des personnes externes.

* Le lien vers le formulaire ne doit pas expirer.

## Considérations sur l’envoi de demandes à Workfront Planning

* Vous ne pouvez pas modifier une requête dans Workfront après l’avoir envoyée.
* Chaque demande envoyée crée un enregistrement pour le type d’enregistrement associé au formulaire que vous utilisez, si le formulaire n’est pas associé à une approbation ou si l’approbation a été accordée par tous les approbateurs.
* Les enregistrements créés en soumettant des formulaires de demande ne peuvent pas être différenciés des enregistrements ajoutés via toute autre méthode dans Workfront Planning.

  Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* Les demandes envoyées s’affichent dans l’onglet Planification de la section Envoyées de la zone Demandes de Workfront.
* Il existe des limitations dans la façon dont certains types de champs s’affichent dans un formulaire de demande ou dans la page des détails de la demande après l’envoi d’un formulaire.

  Pour plus d’informations, voir [Créer et gérer un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Envoyez une demande à Workfront Planning dans la zone Requêtes de Workfront

{{step1-to-requests}}

1. Activez le **paramètre Basculer vers une nouvelle expérience** , dans le coin supérieur droit de l’écran.
L’activation de ce paramètre rend les formulaires de demande Workfront Planning disponibles dans la **zone Requêtes** de Workfront.

   >[!TIP]
   >
   >Ce paramètre n’est disponible que lorsque les éléments suivants sont en place :
   >
   >* Votre société a acheté un package Workfront Planning.
   >* Votre instance Workfront est intégrée à l’Adobe Unified Experience.
   >* Vous avez accès à l’affichage d’au moins un espace de travail.
   >

1. Cliquez sur **Nouvelle requête**.

   ![Nouvelle boîte de demande avec cartes Workfront et Planning unifiées](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   La **boîte de dialogue Nouvelle demande** s’ouvre avec les informations suivantes :

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

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Envoyé de la zone Demandes frontales et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Envoyé de la zone Demandes frontales. Un nouvel enregistrement n’est ajouté à la page de type d’enregistrement qu’après que tous les approbateurs l’ont approuvé.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire](/help/quicksilver/planning/requests/add-approval-to-request-form.md) de demande.

     ![Zone Demandes avec bascule pour l’onglet Planification unifiée des workflows](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >Tous les utilisateurs qui ont accès à au moins un espace de travail peuvent afficher l’onglet Planification dans la zone Demandes. Vous pouvez afficher uniquement les demandes soumises par vous ou toute autre personne aux espaces de travail que vous avez au moins l’autorisation d’afficher. Les administrateurs de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système.

   * La demande n’est visible que par le propriétaire, l’approbateur et les personnes disposant au moins d’autorisations d’affichage sur l’espace de travail.

   * Vous recevez une notification dans l’application et un e-mail indiquant que la demande a été soumise avec succès ou a été envoyée pour examen.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification dans l’application et un e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >L’e-mail et les notifications dans l’application ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.
     >
     >Il existe un lien vers la demande dans l’e-mail de confirmation ou de notification d’approbation.

1. (Facultatif) Cliquez sur **Afficher votre demande** dans le message de confirmation, pour ouvrir la demande, ou cliquez sur l’icône **X** pour fermer la confirmation.

1. (Facultatif) Cliquez sur l’onglet **Planification** dans la **zone Demandes** pour afficher vos demandes.
Toutes les demandes auxquelles vous avez accès et qui ont été soumises à un formulaire de demande de planification s’affichent dans une liste.
1. (Facultatif) Effectuez l’une des opérations suivantes :

   * Cliquez sur **Filtres** et commencez à ajouter des conditions pour les demandes que vous souhaitez afficher dans l’onglet Planification.

     ![Modification des filtres de l’onglet Demandes de planification](assets/filters-editing-box-in-requests-planning-tab.png)

     Vous pouvez filtrer le contenu selon les champs suivants :

      * **Workspace** : l’espace de travail auquel le formulaire de demande est associé.
      * **Type d’enregistrement** : type d’enregistrement auquel le formulaire de demande est associé.
      * **Date d’entrée** : La date à laquelle la demande a été soumise.
      * **Formulaire** de demande : nom du formulaire de demande utilisé pour soumettre la demande.
      * **État** : état de la demande.
      * **Entré par** : nom de l’utilisateur qui a ajouté la demande. Si la demande a été ajoutée par une personne extérieure à Workfront, le **champ Saisi par** affiche `N/A`.

        Plusieurs filtres peuvent être unis par **And** ou Or ****.
La liste des requêtes est filtrée automatiquement, à mesure que vous ajoutez les conditions de filtrage.

   * Cliquez sur **Colonnes** et masquez, affichez ou réorganisez les colonnes de la liste de requêtes.

     >[!TIP]
     >
     >Vous ne pouvez pas ajouter d’autres colonnes.
     >
     >Vous ne pouvez pas afficher le **champ Objet** .

     ![](assets/columns-editing-box-in-requests-planning-tab.png)


1. Cliquez sur le nom d’une requête dans la liste.

   La page Détails de la demande s’ouvre.

   ![Page de détails de la demande](assets/request-details-page.png)


1. (Conditionnel) Si le formulaire de demande n’est pas associé à une approbation, ou si la demande a été approuvée, cliquez sur le nom de la demande, puis cliquez sur le nom de l’enregistrement dans le **champ Enregistrement** .

   La page de l’enregistrement s’ouvre dans Workfront Planning.

   >[!TIP]
   >
   >* Si le champ principal de l’enregistrement n’a pas été mis à jour dans le formulaire de demande, le nom de l’enregistrement dans le champ Enregistrement de la demande s’affiche comme **Sans titre**.
   >
   >* Si le formulaire de demande est associé à une approbation, l’approbation doit être accordée avant que vous puissiez accéder à l’enregistrement à partir de la page de demande.

1. (Facultatif) Cliquez sur le nom du type **d’enregistrement**.

   La page Type d’enregistrement s’ouvre dans Workfront Planning.

## Envoi d’une demande à Workfront Planning à partir d’un lien partagé vers un formulaire de demande

1. Accédez au lien partagé avec vous à partir d’un type d’enregistrement Workfront Planning.

1. Mettez à jour les champs disponibles dans le formulaire. Les champs marqués d’un astérisque sont obligatoires.

   >[!TIP]
   >
   >   Si le **champ Objet** est disponible, il ne sera pas visible dans Workfront Planning, une fois la demande envoyée.
   >
   >Nous vous recommandons de mettre à jour autant de champs de votre requête que possible pour rendre le nouvel enregistrement identifiable lorsqu’il est ajouté au type d’enregistrement dans Workfront Planning.

1. Cliquez sur **Soumettre**.

   Votre formulaire est envoyé et les choses suivantes se produisent :

   * Si le formulaire de demande n’a pas été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Envoyé de la zone Demandes frontales et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.

   * Si le formulaire de demande a été associé à une approbation, la demande est ajoutée à l’onglet Planification de la section Envoyé de la zone Demandes frontales. Un nouvel enregistrement n’est ajouté à la page de type d’enregistrement qu’après que tous les approbateurs l’ont approuvé.

     Pour plus d’informations, voir [Ajouter une approbation à un formulaire](/help/quicksilver/planning/requests/add-approval-to-request-form.md) de demande.

     ![Onglet Planification des requêtes](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Tous les utilisateurs ayant accès à au moins un espace de travail peuvent afficher l&#39;onglet Planification dans la zone Demandes. Vous pouvez afficher uniquement les requêtes que vous ou une autre personne avez envoyées aux espaces de travail que vous êtes au moins autorisé à afficher. Les administrateurs et administratrices de Workfront peuvent afficher toutes les demandes envoyées à n’importe quel espace de travail du système. <!--ensure this is correct; asking team in slack-->

   * Vous recevez une notification in-app et un e-mail vous informant que la demande a été soumise avec succès ou envoyée pour révision.
   * Si le formulaire de demande a été associé à une approbation, les approbateurs reçoivent une notification in-app et par e-mail pour examiner et approuver la demande.

     >[!NOTE]
     >
     >Les notifications par e-mail et in-app ne sont visibles que lorsque l’instance de Workfront de votre organisation est intégrée à l’expérience unifiée Adobe.

   * <span class="preview"> Une fois la demande approuvée et l&#39;enregistrement créé, les champs Date d&#39;approbation par et Date d&#39;approbation affichent des informations sur l&#39;approbation dans l&#39;enregistrement.</span>

1. (Facultatif) Cliquez sur **Afficher votre demande** pour ouvrir la demande dans Workfront.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Facultatif) Cliquez sur **Menu principal** > **Demandes** > l’onglet **Planification** pour afficher votre demande, puis cliquez sur son nom.

   La page des détails de la requête s’ouvre.

   ![Page de détails de la demande](assets/request-details-page.png)

1. (Conditionnel) Si le formulaire de demande n&#39;est pas associé à une approbation, ou si la demande a été approuvée, cliquez sur le nom de la demande, puis cliquez sur le nom de l&#39;enregistrement dans le champ **Enregistrement**.

   La page de l’enregistrement s’ouvre dans Workfront Planning.

   >[!TIP]
   >
   >* Si le nom de l’enregistrement n’a pas été ajouté au formulaire de demande, le nom de l’enregistrement dans le champ Enregistrement de la demande s’affiche comme **Sans titre**.
   >
   >* Si le formulaire de demande est associé à une approbation, l’approbation doit être accordée avant que vous puissiez accéder à l’enregistrement à partir de la page de demande.

1. (Facultatif) Cliquez sur le nom du type **d’enregistrement**.

   La page Type d’enregistrement s’ouvre dans Workfront Planning.




