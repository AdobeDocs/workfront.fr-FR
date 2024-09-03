---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Gérer les rôles d’épreuve dans  [!DNL Workfront Proof]
description: Les rôles d’épreuve vous permettent d’accorder des autorisations aux utilisateurs et utilisatrices limités par le profil d’autorisation configuré sur leur profil d’utilisateur ou d’utilisatrice.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 100%

---

# Gérer les rôles d’épreuve dans [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Les rôles d’épreuve vous permettent d’accorder des autorisations aux utilisateurs et utilisatrices limités par le profil d’autorisation configuré sur leur profil d’utilisateur ou d’utilisatrice. (Pour plus d’informations sur les profils d’autorisation, voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Les rôles d’épreuve sont différents des profils de compte. Le profil de votre compte correspond au niveau d’autorisation global dont vous disposez dans votre compte et aura une incidence sur les droits dont vous disposez sur toutes les épreuves de votre compte, même celles qui n’ont pas été explicitement partagées avec vous.

Pour plus d’informations, voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## À propos des rôles d’épreuve

Les rôles d‘épreuve suivants sont attribués aux utilisateurs et utilisatrices pour une épreuve individuelle au moment où la personne est invitée à réviser l’épreuve :

* [Lecture seule](#read-only)
* [Réviseur](#reviewer)
* [Approbateur](#approver)
* [Réviseur et approbateur](#reviewer-approver)
* [Auteur](#author)
* [Modérateur](#moderator)

Le rôle d’épreuve définit les actions qu’un réviseur ou une réviseuse peut effectuer sur cette épreuve.

Par exemple, si vous êtes un réviseur ou une réviseuse, on vous invite à réviser l’épreuve en ajoutant des annotations et des commentaires. Si vous êtes une personne chargée de la révision et de l’approbation, on vous demande de réviser l’épreuve et de prendre une décision à son sujet.

Certains rôles d’épreuve donnent aux réviseurs et réviseuses des droits de modification sur l’épreuve (même si leur profil de compte ne le leur permet pas) et leur permet d’utiliser des fonctionnalités supplémentaires telles que l’ajout d’actions sur les commentaires, la création de nouvelles versions et l’ajout d’autres réviseurs et réviseuse à l’épreuve.

Pour plus d’informations, consultez les articles suivants :

* [Utiliser des actions sur les commentaires d’une épreuve](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Partager une épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Lecture seule

{#read-only}

![cleaner.png](assets/cleaner.png) Peut afficher une épreuve.

![no.png](assets/no.png) Ne peut pas ajouter d’annotations.

![no.png](assets/no.png) Ne peut pas ajouter de commentaires.

![no.png](assets/no.png) Ne peut pas prendre de décision.

![no.png](assets/no.png) Ne peut pas supprimer les commentaires des autres.

![no.png](assets/no.png) Ne dispose pas de droits de modification sur l’épreuve.

>[!NOTE]
>
>Si un dossier est partagé avec des utilisateurs et des utilisatrices de [!DNL Workfront Proof], ils se verront attribuer automatiquement des droits en lecture seule sur tous les éléments existants et ajoutés par la suite dans le dossier.

Pour plus d’informations, voir [Partager des dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Réviseur {#reviewer}

![cleaner.png](assets/cleaner.png) Peut afficher une épreuve.

![cleaner.png](assets/cleaner.png) Peut ajouter des annotations.

![cleaner.png](assets/cleaner.png) Peut ajouter des commentaires.

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse.

![no.png](assets/no.png) Ne peut pas prendre de décision.

![no.png](assets/no.png) Ne peut pas modifier ou supprimer les commentaires effectués par d’autres personnes.

![no.png](assets/no.png) Ne dispose pas de droits de modification sur l’épreuve.

### Approbateur {#approver}

![cleaner.png](assets/cleaner.png) Peut afficher une épreuve.

![cleaner.png](assets/cleaner.png) Peut prendre une décision.

![no.png](assets/no.png) Ne peut pas ajouter des annotations.

![no.png](assets/no.png) Ne peut pas ajouter de commentaires.

![no.png](assets/no.png) Ne peut pas modifier ou supprimer les commentaires effectués par d’autres personnes.

![no.png](assets/no.png) Ne dispose pas de droits de modification sur l’épreuve.

### Réviseur et approbateur {#reviewer-approver}

![cleaner.png](assets/cleaner.png) Peut afficher une épreuve.

![cleaner.png](assets/cleaner.png) Peut ajouter des annotations.

![cleaner.png](assets/cleaner.png) Peut ajouter des commentaires.

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse.

![cleaner.png](assets/cleaner.png) Peut prendre une décision.

![no.png](assets/no.png) Ne peut pas modifier ou supprimer les commentaires effectués par d’autres personnes.

![no.png](assets/no.png) Ne dispose pas de droits de modification sur l’épreuve.

### Auteur {#author}

![cleaner.png](assets/cleaner.png) Peut ajouter des annotations.

![cleaner.png](assets/cleaner.png) Peut ajouter des commentaires.

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse.

![cleaner.png](assets/cleaner.png) Peut prendre une décision.

![cleaner.png](assets/cleaner.png) Peut soumettre de nouvelles versions.

![cleaner.png](assets/cleaner.png) Peut créer une copie de l’épreuve.

![cleaner.png](assets/cleaner.png) Peut partager l’épreuve avec d‘’autres personnes.

![cleaner.png](assets/cleaner.png) Peut appliquer des actions aux commentaires.

![cleaner.png](assets/cleaner.png) Peut résoudre des commentaires.

![no.png](assets/no.png) Ne peut pas modifier ou supprimer les commentaires effectués par d’autres personnes.

>[!NOTE]
>
>Ce rôle ne peut être affecté qu’aux utilisateurs et utilisatrices de [!DNL Workfront Proof].

### Modérateur {#moderator}

![cleaner.png](assets/cleaner.png) Peut ajouter des annotations.

![cleaner.png](assets/cleaner.png) Peut ajouter des commentaires.

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse.

![cleaner.png](assets/cleaner.png) Peut prendre une décision.

![cleaner.png](assets/cleaner.png) Peut soumettre de nouvelles versions.

![cleaner.png](assets/cleaner.png) Peut ajouter de nouveaux réviseurs et réviseuses.

![cleaner.png](assets/cleaner.png) Peut appliquer des actions aux commentaires.

![cleaner.png](assets/cleaner.png) Peut résoudre des commentaires.

![cleaner.png](assets/cleaner.png) Peut supprimer les commentaires et réponses sur l’épreuve (effectués par cette personne ou par d’autres).

* La suppression du premier commentaire dans un thread de commentaires supprime l’ensemble du thread.
* La suppression d’une réponse dans le thread de commentaires supprime uniquement cette réponse.

![no.png](assets/no.png) Ne peut pas modifier les commentaires effectués par d’autres personnes.

Ce rôle permet à la personne de gérer et de modérer les commentaires de l’épreuve, ce qui lui donne l‘opportunité de ne conserver que les commentaires pertinents sur l’épreuve et de supprimer les commentaires non pertinents.

>[!NOTE]
>
>Ce rôle ne peut être affecté qu’aux utilisateurs et utilisatrices de [!DNL Workfront Proof].

## Affecter des rôles d’épreuve

Vous pouvez affecter des rôles d’épreuve lors de la création d’épreuves ou de nouvelles versions d’épreuves existantes, ou sur des épreuves existantes.

### Nouvelles épreuves {#new-proofs}

Les rôles d’épreuve peuvent être attribués aux réviseurs et réviseuses sur la page [!UICONTROL Nouvelle épreuve] pendant le processus de création d’épreuve (1).

![Proof_fields_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Nouvelles versions {#new-versions}

Lors de la création d’une nouvelle version d’une épreuve, les personnes chargées de la révision de la version précédente seront automatiquement affichées (avec le même rôle que pour la version précédente).

Vous pouvez modifier les rôles d’épreuve appliqués aux personnes chargées de la révision lors de la création de la nouvelle version (1).

![Proof_tasks_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Épreuves existantes {#existing-proofs}

Si vous souhaitez modifier le rôle d’une personne sur une épreuve existante, vous pouvez le faire sur la page [!UICONTROL Détails de l’épreuve] en modifiant en ligne son rôle dans la section de workflow (1).

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Vérifier les rôles dans la visionneuse d’épreuve

Vous pouvez vérifier le rôle d’une personne chargée de la révision directement à partir de la visionneuse d’épreuve (1) et le modifier (2) si nécessaire.

![Proof_tasks_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Rôles d’épreuve par défaut

Vous pouvez définir votre rôle d’épreuve par défaut sur la page [!DNL Proofing Defaults] dans vos paramètres personnels. Cela signifie que lors de votre ajout à une épreuve, votre rôle d’épreuve par défaut est renseigné automatiquement. Notez que ce rôle peut être modifié au niveau de l’épreuve par un utilisateur ou une utilisatrice disposant de droits de modification sur une épreuve.

>[!NOTE]
>
>Seuls les utilisateurs et utilisatrices disposant de profils de personnes chargées de l’administration ou de l’administration de facturation peuvent modifier les paramètres de relecture par défaut des autres utilisateurs et utilisatrices dans leur compte.

Pour plus d’informations, voir [Paramètres personnels dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Créateurs et créatrices et personnes propriétaires

Les créateurs et créatrices et les personnes propriétaires disposent de droits de modification intégraux sur l’épreuve.

### Créateurs et créatrices {#creators}

Le créateur ou la créatrice d’épreuve est la personne qui charge l’épreuve en première instance. Le créateur ou la créatrice d’épreuve s’affichera automatiquement dans la liste de personnes pour l’épreuve (dans son rôle par défaut).

Sur la page [!UICONTROL Nouvelle épreuve], vous pouvez attribuer un rôle d’épreuve différent au créateur ou à la créatrice d’épreuve (autre que son rôle par défaut).

La personne qui a créé l’épreuve ne peut pas être modifiée ni supprimée d’une épreuve.

### Propriétaires {#owners}

Par défaut, le créateur ou la créatrice est également la personne propriétaire de l’épreuve ; toutefois, le créateur ou la créatrice peut nommer une autre personne comme propriétaire de l’épreuve lors de la création initiale de l’épreuve (sur la page [!UICONTROL Nouvelle épreuve]).

Pour modifier la personne propriétaire sur la page Nouvelle épreuve, procédez comme suit :

1. Cliquez sur le lien de modification affiché en regard du nom du créateur ou de la créatrice.
1. Sélectionnez la nouvelle personne propriétaire dans le menu déroulant. (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Une fois l’épreuve créée, il est toujours possible de modifier la personne propriétaire. Toute personne disposant de droits de modification sur l’épreuve pourra transférer la propriété de cette dernière à une autre personne via la page [!UICONTROL Détails de l’épreuve] (voir ci-dessous).

La possibilité de modifier la personne propriétaire d’une épreuve est particulièrement utile du point de vue de la gestion des workflow. Cela permet à la personne responsable du projet d’assumer la propriété des épreuves, ce qui lui donne les droits de modification sur les épreuves et la possibilité de les afficher dans la vue [!UICONTROL Mes épreuves].

Pour modifier la personne propriétaire de l’épreuve via la page [!UICONTROL Détails de l’épreuve], procédez comme suit :

* Cliquez sur le menu Actions en regard du nom de la personne que vous souhaitez désigner comme propriétaire.
* Sélectionnez [!UICONTROL **Rendre propriétaire**] dans le menu déroulant.
* Vous pouvez également cliquer sur le champ [!UICONTROL **Personne propriétaire**] en regard de l’image de l‘épreuve et sélectionner la nouvelle personne propriétaire dans la liste déroulante affichée.

Une fois cette opération effectuée, le mot « Propriétaire » s’affiche en regard du nom de cette personne.

>[!NOTE]
>
>Seul un profil utilisateur du même compte ou d’un compte partenaire peut devenir propriétaire d’une épreuve. Un utilisateur ou une utilisatrice disposant d’un compte partenaire ne peut devenir propriétaire d’une épreuve que dans les cas suivants :
>
>* Une relation de partenaire existante est définie entre les comptes. Pour plus d’informations, voir [Comptes partenaires dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* Il n’existe aucun champ personnalisé sur la page [!UICONTROL Nouvelle épreuve].
>* L’épreuve n’a pas été affectée à un dossier.
>* Aucune balise n’a été appliquée à l’épreuve.

Pour déléguer temporairement la propriété de l’épreuve dans [!DNL Workfront Proof], voir [Désignation de personnes propriétaires temporaires d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
