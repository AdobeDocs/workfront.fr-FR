---
title: Partager un document
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Votre équipe d’administration Adobe Workfront accorde aux utilisateurs et utilisatrices l’accès en affichage ou en modification des documents lorsqu’elle attribue des niveaux d’accès, comme expliqué dans la section Accorder l’accès aux documents.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 7f8c9b9f63770d6364f0eb1b9c23e4648dacaf93
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 45%

---

# Partager un document

L’administrateur Workfront contrôle qui peut afficher ou modifier des documents dans la zone Niveaux d’accès du programme d’installation. Pour plus d’informations, voir [Accorder l’accès aux documents](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Les utilisateurs peuvent également partager des documents qu’ils ont téléchargés ou auxquels ils ont accès, en donnant à d’autres l’autorisation de les afficher ou de les gérer.

* Les autorisations s’appliquent à des éléments individuels et définissent les actions qu’une personne peut entreprendre.
* La personne qui télécharge un document obtient automatiquement le contrôle total (autorisations de gestion).
* Pour partager un dossier entier, voir [Partager un dossier](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md) de documents.

>[!NOTE]
>
>Si votre instance Workfront utilise Adobe stockage d’entreprise, vous ne pouvez pas partager de documents individuels. Au lieu de cela, vous accordez l’accès au niveau du projet. Gardez à l’esprit que le partage du projet peut donner accès à des informations sensibles sur le projet, telles que des données financières, en fonction du niveau d’autorisation choisi.



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
   <td> <p>Standard</p> 
   <p>Travail ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou supérieur aux objets que vous souhaitez partager.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour les objets que vous souhaitez partager.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Partager un document

L’utilisateur ou utilisatrice qui charge un document dans Workfront dispose par défaut d’autorisations de gestion.

{{step1-to-documents}}

1. Dans la **page Documents**, passez la souris sur le document que vous souhaitez partager, puis cliquez sur le lien Détails **du document qui s’affiche**. La **page Détails du** document s’ouvre.

   ![Lien Détails du document](assets/document-details-link.png)

1. Cliquez sur l’icône Plus Plus **à droite du nom du document, puis cliquez sur** Partager![.](assets/more-icon.png) **&#x200B;**&#x200B;La **boîte de dialogue Partager [le nom]** du document s’ouvre.

   ![Partager un document](assets/share-a-document-350x160.png)

1. Dans le champ Accorder l’accès **au** document, commencez à taper le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société avec lequel vous souhaitez partager le document, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   >
   >Vous ne pouvez partager un document qu’avec des utilisateurs, des équipes, des rôles ou des sociétés actifs.


1. (Facultatif) Sélectionnez la **liste déroulante Qui a accès** et sélectionnez le niveau d’accès du document :

   * **Seules les personnes invitées peuvent y accéder :** seuls les utilisateurs invités au document peuvent y accéder (par défaut).
   * **Tout le monde peut afficher le document** : tous les utilisateurs du système peuvent afficher le document sans invitation.

1. (Facultatif) Pour rendre le document public, cliquez sur l’icône d’engrenage ![sélectionnez l’icône d’engrenage](assets/gear-icon.png), puis cliquez sur la zone en ligne avec **Rendez ceci public pour les utilisateurs externes**. Le bouton **Copier le lien public** s’affiche au bas de la boîte de dialogue.

1. Cliquez sur la liste déroulante située à droite du nom de l’utilisateur et sélectionnez son niveau d’autorisation pour ce document :

   * **Afficher** : l’utilisateur peut réviser et partager le document.
   * **Gérer** : l’utilisateur dispose d’un accès complet au document sans droits d’administration, qui sont accordés au niveau d’accès (inclut également toutes les autorisations d’affichage).

1. (Facultatif) Cliquez sur l’icône des options avancées en regard du niveau d’autorisation que vous avez accordé pour configurer des autorisations spécifiques sur le document.

   ![Options d’autorisation avancées configurées](assets/advanced-options-icon.png)

1. (Facultatif) Pour désactiver les autorisations héritées pour les objets enfants du document, cliquez sur **Désactiver** en ligne avec **Autorisations héritées**.

1. (Conditionnel) Pour copier le lien public qui permet de partager le document avec des utilisateurs externes, cliquez sur **Copier le lien public**.

   >[!CAUTION]
   >
   >Nous vous recommandons de faire preuve de prudence lorsque vous partagez un document contenant des informations confidentielles avec des utilisateurs externes. Cette fonction leur permet d’afficher des informations sans être un utilisateur ou une utilisatrice Workfront ou une personne membre de votre organisation.

1. Cliquer sur **Enregistrer**.

## Partage de documents en masse

{{step1-to-documents}}

1. Dans l’onglet **Tous les documents** de la **page Documents**, maintenez la touche Commande **(Mac) ou** Ctrl **(Windows) enfoncée** sur votre clavier, puis cliquez sur chaque document que vous souhaitez partager.

1. En haut de la page, cliquez sur l’icône **Partager** ![Icône Partager](assets/share-icon.png). La boîte de dialogue modale de partage s’ouvre.

   ![icône Partager](assets/share-documents-in-bulk.png)

1. Dans le champ **Accorder l’accès au document à**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société avec lequel vous souhaitez partager les documents, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   >
   >Vous pouvez uniquement partager des documents avec des utilisateurs actifs, des équipes, des rôles ou des entreprises.


1. (Facultatif) Sélectionnez le menu déroulant **Qui a accès** et sélectionnez le niveau d’accès aux documents :

   * **Seuls les utilisateurs invités peuvent y accéder :** seuls les utilisateurs invités aux documents peuvent y accéder (par défaut).
   * **Tous les utilisateurs du système peuvent afficher** : tous les utilisateurs du système peuvent afficher les documents sans invitation.

1. Cliquez sur la liste déroulante située à droite du nom de l’utilisateur et sélectionnez son niveau d’autorisation pour les documents :

   * **Afficher** : l’utilisateur peut consulter et partager les documents.
   * **Gérer** : l’utilisateur dispose d’un accès complet aux documents sans droits d’administration, qui sont accordés au niveau d’accès (inclut également toutes les autorisations d’affichage).

1. (Facultatif) Cliquez sur l’icône des options avancées en regard du niveau d’autorisation que vous avez accordé pour configurer des autorisations spécifiques sur les documents.

   ![Options d’autorisation avancées configurées](assets/advanced-options-icon.png)

1. Cliquer sur **Enregistrer**.

## Partage de documents avec Adobe stockage d’entreprise

Workfront est en transition vers la solution de stockage d’entreprise Adobe afin de fournir une meilleure connectivité avec Adobe Creative Cloud produits. Les clients existants seront migrés vers le nouveau modèle par étapes. Pour plus d’informations sur les avantages du stockage d’entreprise Adobe, consultez [Adobe vue d’ensemble](/help/quicksilver/review-and-approve-work/esm-overview.md) du stockage d’entreprise.

Si votre instance Workfront utilise le stockage d’entreprise Adobe, vous ne pouvez pas partager directement des documents individuels. Au lieu de cela, vous devez accorder l’accès au niveau du projet.

>[!IMPORTANT]
>
>Le partage d’un projet peut également donner aux utilisateurs l’accès à des informations sensibles sur le projet, telles que les données financières, en fonction du niveau d’autorisation que vous choisissez.
>
>Veillez à bien lire les paramètres d’autorisation avant de partager.

## Autorisations de documents

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément. Pour plus d’informations sur les autorisations relatives aux objets, voir [Vue d’ensemble du partage des autorisations sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Le tableau suivant indique les autorisations que vous pouvez accorder lorsque les personnes sont autorisées à consulter ou à gérer des documents :

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Action</strong> </p> </th> 
   <th> <p><strong>Gérer</strong> </p> </th> 
   <th> <p><strong>Afficher</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Créer</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier les détails du document</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Supprimer*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Téléchargement</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Passage en caisse</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter des approbateurs et approbatrices</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Approuver le document</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Joindre un formulaire personnalisé</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifier les champs personnalisés</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Déplacer vers (objet)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Envoyer à (intégration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Mises à jour / commentaires</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Charger une nouvelle version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Supprimer la version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Afficher un ou plusieurs documents</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aperçu</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Épreuve**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Générer une épreuve**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Supprimer une épreuve**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Partager*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Partager à l’échelle du système*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Partager les documents publiquement*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Partager avec une adresse e-mail externe</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter/Supprimer</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Renommer</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Lier (avec intégration)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Annuler le lien (avec intégration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; L’action est partagée par les documents et les dossiers de documents.

&#42;&#42; Vous devez disposer d’une licence de relecture distincte associée à votre compte Workfront pour pouvoir relire des documents. Contactez votre personne gestionnaire de compte pour obtenir une licence de relecture. Pour plus d’informations sur la relecture dans Workfront, voir [Relecture](../../review-and-approve-work/proofing/proofing.md).

## Remarques sur le partage de documents

Outre les considérations ci-dessous, voir également [Vue d’ensemble du partage des autorisations sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Une équipe d’administration Workfront peut ajouter ou supprimer des autorisations à tous les éléments du système, pour toutes les personnes, sans être la personne propriétaire de ces éléments.

* Le partage d’un document est similaire au partage de tout autre objet dans Workfront. Pour plus d’informations sur le partage de documents dans Workfront, voir [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Vous pouvez accorder les autorisations suivantes aux documents :

   * Afficher
   * Gérer

* Vous pouvez également partager un document publiquement ou à l’échelle du système.

  >[!CAUTION]
  >
  >Nous avisons la prudence lors du partage d’un objet contenant des informations confidentielles avec des utilisateurs et utilisatrices externes. Cette fonction leur permet d’afficher des informations sans être un utilisateur ou une utilisatrice Workfront ou une personne membre de votre organisation.

* Vous pouvez partager un document avec une personne qui n’a pas de compte Workfront, en ajoutant son adresse e-mail dans le champ Accorder l’accès au document à.
* Lorsque vous partagez un document, les utilisateurs et utilisatrices ont le même accès à toutes les versions et toutes les épreuves du document.\
  Pour plus d’informations sur la relecture dans Workfront, voir la section [Relecture](../../review-and-approve-work/proofing/proofing.md).

* Vous pouvez hériter des autorisations sur les documents à partir des objets auxquels ils sont associés. Votre équipe d’administration Workfront peut limiter l’héritage des autorisations pour les documents de votre niveau d’accès.

  Pour plus d’informations sur la limitation des autorisations héritées sur les documents, voir [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Vous pouvez supprimer manuellement les autorisations héritées sur les documents. Pour plus d’informations, voir [Supprimer les autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Un document joint n’hérite des autorisations que de l’objet auquel il a été joint. Si vous créez un dossier sur l’objet et que vous déplacez le document dans le dossier, il hérite des autorisations du dossier. En revanche, si vous créez un dossier sur un objet parent ou grand-parent et que vous déplacez le document dans ce dossier, il n’hérite pas des autorisations de ce dossier.