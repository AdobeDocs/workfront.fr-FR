---
title: Partage d’un document
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Votre administrateur Adobe Workfront permet aux utilisateurs d’afficher ou de modifier des documents lorsqu’ils leur attribuent des niveaux d’accès, comme expliqué dans Accorder l’accès aux documents.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# Partage d’un document

Votre administrateur Adobe Workfront permet aux utilisateurs d’afficher ou de modifier des documents lorsqu’ils attribuent des niveaux d’accès, comme expliqué dans la section [Accorder l’accès aux documents](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Le niveau d’accès accordé par l’administrateur Workfront aux utilisateurs leur permet d’afficher ou de modifier des documents. En outre, d’autres utilisateurs peuvent également accorder à d’autres utilisateurs l’autorisation d’afficher ou de gérer des documents spécifiques qu’ils ont téléchargés eux-mêmes ou qu’ils ont accès au partage.

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément. Pour plus d’informations sur les autorisations d’objet, voir [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Par défaut, l’utilisateur qui télécharge un document vers Workfront dispose des autorisations de gestion .

Pour plus d’informations sur le partage d’un dossier de document entier, voir [Partage d’un dossier de document](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Observations relatives au partage de documents

Outre les considérations ci-dessous, reportez-vous également à la section [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un administrateur Workfront peut ajouter ou supprimer des autorisations à n’importe quel élément du système, pour tous les utilisateurs, sans en être le propriétaire.

* Le partage d’un document est similaire au partage d’un autre objet dans Workfront. Pour plus d’informations sur le partage de documents dans Workfront, voir [Partage d’un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Vous pouvez accorder les autorisations suivantes aux documents :

   * Afficher
   * Gérer

* Vous pouvez également partager un document publiquement ou à l’échelle du système.

   >[!CAUTION]
   >
   >Nous vous recommandons d’être prudent lors du partage d’un objet contenant des informations confidentielles avec des utilisateurs externes. Cela leur permet d’afficher des informations sans être un utilisateur Workfront ou un membre de votre entreprise.

* Vous pouvez partager un document avec une personne qui ne dispose pas d’un compte Workfront en ajoutant son adresse électronique dans le champ Accorder l’accès au document .
* Lorsque vous partagez un document, les utilisateurs ont le même accès à toutes les versions de document et à tous les BAT de document.\
   Pour plus d’informations sur la vérification dans Workfront, voir [Vérification](../../review-and-approve-work/proofing/proofing.md) .

* Vous pouvez hériter des autorisations de documents des objets auxquels ils sont associés. Votre administrateur Workfront peut restreindre l’héritage des autorisations pour les documents de votre niveau d’accès.

   Pour plus d’informations sur la restriction des autorisations héritées sur les documents, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   Vous pouvez supprimer manuellement les autorisations héritées sur les documents. Pour plus d’informations, voir [Suppression des autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Un document joint hérite uniquement des autorisations de l’objet auquel il a été joint. Si vous créez un dossier sur l’objet et que vous déplacez le document dans le dossier, il hérite des autorisations du dossier. Cependant, si vous créez un dossier sur un objet parent ou grand-parent et que vous déplacez le document dans ce dossier, il n’hérite pas des autorisations de ce dossier.

## Autorisations de document

Le tableau suivant indique les autorisations que vous pouvez accorder aux utilisateurs lorsqu’ils peuvent afficher ou gérer des documents :

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
   <td scope="row">Télécharger</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Passage en caisse</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ajouter des approbateurs</td> 
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
   <td scope="row">Mises à jour/commentaires</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Chargement d’une nouvelle version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Supprimer la version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Afficher le ou les documents</td> 
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
   <td scope="row">Créer une épreuve**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Supprimer l'épreuve**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Partager*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Partager sur le système*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Partager les documents publiquement*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Partager avec une adresse électronique externe</td> 
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
   <td scope="row">Lien (avec intégration)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Dissocier (avec intégration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; L’action est partagée par les documents et les dossiers de document.

&#42;&#42; Pour pouvoir BAT de documents, une licence de vérification distincte doit être associée à votre compte Workfront. Contactez votre gestionnaire de compte au sujet de l’acquisition d’une licence de vérification. Pour plus d’informations sur la vérification dans Workfront, voir [Vérification](../../review-and-approve-work/proofing/proofing.md).
