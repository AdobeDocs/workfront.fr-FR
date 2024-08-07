---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Gérer les rôles de BAT dans [!DNL Workfront Proof]
description: Les rôles de BAT vous permettent d’accorder des autorisations aux utilisateurs limités par le profil d’autorisation configuré sur leur profil utilisateur.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 6%

---

# Gérer les rôles de BAT dans [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Les rôles de BAT vous permettent d’accorder des autorisations aux utilisateurs limités par le profil d’autorisation configuré sur leur profil utilisateur. (Pour plus d’informations sur les profils d’autorisation, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Les rôles de BAT sont différents des profils de compte. Le profil de votre compte correspond au niveau d’autorisation global dont vous disposez dans votre compte et aura une incidence sur les droits dont vous disposez sur tous les bons à tirer de votre compte, même ceux qui n’ont pas été explicitement partagés avec vous.

Pour plus d’informations, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## À propos des rôles de BAT

Les rôles de BAT suivants sont attribués aux utilisateurs pour un BAT individuel au moment où l’utilisateur est invité à passer en revue le BAT :

* [Lecture seule](#read-only)
* [Réviseur](#reviewer)
* [Approbateur](#approver)
* [Réviseur et approbateur](#reviewer-approver)
* [Auteur](#author)
* [Modérateur](#moderator)

Le rôle d’épreuve définit les actions qu’une personne réviseuse peut entreprendre pour cette épreuve spécifique.

Par exemple, si vous êtes un réviseur, vous êtes invité à passer en revue le BAT en ajoutant des annotations et des commentaires. Si vous êtes un réviseur et un approbateur, vous êtes invité à passer en revue le BAT et à prendre une décision à ce sujet.

Certains rôles d’épreuve donnent aux personnes réviseuses des droits de modification sur l’épreuve (même si leur profil de compte ne comporte pas de tels droits) et leur permet d’utiliser des fonctionnalités supplémentaires telles que l’ajout d’actions sur les commentaires, la création de nouvelles versions et l’ajout d’autres personne réviseuses à l’épreuve.

Pour plus d’informations, consultez les articles suivants :

* [Utiliser des actions sur des commentaires d’épreuve](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Partage d’un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Lecture seule

{#read-only}

![clean.png](assets/cleaner.png) Peut afficher un BAT

![no.png](assets/no.png) Impossible d’ajouter des balises

![no.png](assets/no.png) Impossible d’ajouter des commentaires

![no.png](assets/no.png) Impossible de prendre une décision

![no.png](assets/no.png) Impossible de supprimer les commentaires effectués par d’autres utilisateurs

![no.png](assets/no.png) N’a pas de droits d’édition sur le BAT

>[!NOTE]
>
>Si un dossier est partagé avec un utilisateur de [!DNL Workfront Proof], il se verra automatiquement attribuer des droits en lecture seule sur tous les éléments existants et ajoutés par la suite dans le dossier.

Pour plus d’informations, voir [Partage de dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Réviseur {#reviewer}

![clean.png](assets/cleaner.png) Peut afficher un BAT

![clean.png](assets/cleaner.png) Peut ajouter des balises

![clean.png](assets/cleaner.png) Peut ajouter des commentaires

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse

![no.png](assets/no.png) Impossible de prendre une décision

![no.png](assets/no.png) Impossible de modifier ou supprimer les commentaires effectués par d’autres utilisateurs

![no.png](assets/no.png) N’a pas de droits d’édition sur le BAT

### Approbateur {#approver}

![clean.png](assets/cleaner.png) Peut afficher un BAT

![clean.png](assets/cleaner.png) Peut prendre une décision

![no.png](assets/no.png) Impossible d’ajouter des balises

![no.png](assets/no.png) Impossible d’ajouter des commentaires

![no.png](assets/no.png) Impossible de modifier ou supprimer les commentaires effectués par d’autres utilisateurs

![no.png](assets/no.png) N’a pas de droits d’édition sur le BAT

### Réviseur et approbateur {#reviewer-approver}

![clean.png](assets/cleaner.png) Peut afficher un BAT

![clean.png](assets/cleaner.png) Peut ajouter des balises

![clean.png](assets/cleaner.png) Peut ajouter des commentaires

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse

![clean.png](assets/cleaner.png) Peut prendre une décision

![no.png](assets/no.png) Impossible de modifier ou supprimer les commentaires effectués par d’autres utilisateurs

![no.png](assets/no.png) N’a pas de droits d’édition sur le BAT

### Auteur {#author}

![clean.png](assets/cleaner.png) Peut ajouter des balises

![clean.png](assets/cleaner.png) Peut ajouter des commentaires

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse

![clean.png](assets/cleaner.png) Peut prendre une décision

![clean.png](assets/cleaner.png) Peut soumettre de nouvelles versions

![clean.png](assets/cleaner.png) Peut créer une copie du BAT

![clean.png](assets/cleaner.png) Peut partager le BAT avec d’autres personnes.

![clean.png](assets/cleaner.png) Peut appliquer des actions aux commentaires

![clean.png](assets/cleaner.png) Peut résoudre les commentaires

![no.png](assets/no.png) Impossible de modifier ou supprimer les commentaires effectués par d’autres utilisateurs

>[!NOTE]
>
>Ce rôle ne peut être attribué qu’aux utilisateurs de [!DNL Workfront Proof].

### Modérateur {#moderator}

![clean.png](assets/cleaner.png) Peut ajouter des balises

![clean.png](assets/cleaner.png) Peut ajouter des commentaires

![[!DNL cleaner].png](assets/cleaner.png) Peut modifier ses propres commentaires s’il n’y a aucune réponse

![clean.png](assets/cleaner.png) Peut prendre une décision

![clean.png](assets/cleaner.png) Peut soumettre de nouvelles versions

![clean.png](assets/cleaner.png) Peut ajouter de nouveaux réviseurs

![clean.png](assets/cleaner.png) Peut appliquer des actions aux commentaires

![clean.png](assets/cleaner.png) Peut résoudre les commentaires

![clean.png](assets/cleaner.png) Peut supprimer les commentaires et les réponses sur le BAT (effectués par eux-mêmes ou par d’autres)

* La suppression du premier commentaire dans un fil de commentaire supprime l’ensemble du thread.
* La suppression des réponses dans le fil de commentaire supprime uniquement cette réponse.

![no.png](assets/no.png) Impossible de modifier les commentaires effectués par d’autres utilisateurs

Ce rôle permet à la personne de gérer et de modérer les commentaires du BAT, ce qui lui donne la possibilité de ne conserver que les commentaires pertinents sur le BAT et de supprimer les commentaires non pertinents.

>[!NOTE]
>
>Ce rôle ne peut être attribué qu’aux utilisateurs de [!DNL Workfront Proof].

## Attribution de rôles de BAT

Vous pouvez attribuer des rôles de BAT lors de la création de BAT, de la création de nouvelles versions de BAT existants ou sur les BAT existants.

### Nouveaux BAT {#new-proofs}

Les rôles de BAT peuvent être attribués aux réviseurs sur la page [!UICONTROL New BAT] pendant le processus de création du BAT (1).

![Proof_tasks_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Nouvelles versions {#new-versions}

Lors de la création d&#39;une nouvelle version d&#39;un BAT, les validants de la version précédente seront automatiquement affichés (avec le même rôle que la version précédente).

Vous pouvez modifier les rôles de BAT appliqués aux opérateurs validants lors de la création de la nouvelle version (1).

![}Proof_rôles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Bons à tirer existants {#existing-proofs}

Si vous souhaitez modifier le rôle d’une personne sur un BAT existant, vous pouvez le faire sur la page [!UICONTROL Détails du BAT] en modifiant en ligne son rôle dans la section du workflow (1).

![}Proof_Roles_-_Proof_Details_page_2.png{1](assets/proof-roles---proof-details-page-2-350x131.png)

## Vérification des rôles dans la visionneuse de BAT

Vous pouvez vérifier le rôle d’un réviseur directement à partir de la visionneuse de BAT (1) et le modifier (2) si nécessaire.

![Proof_tasks_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Rôles de BAT par défaut

Vous pouvez définir votre rôle de BAT par défaut sur la page [!DNL Proofing Defaults] de vos paramètres personnels. Cela signifie que lorsque vous êtes ajouté à un BAT, votre rôle de BAT par défaut est renseigné automatiquement. Notez que ce rôle peut être modifié au niveau du BAT par un utilisateur disposant de droits d’édition sur un BAT.

>[!NOTE]
>
>Seuls les utilisateurs disposant de profils d’administrateur ou d’administrateur de facturation peuvent modifier les paramètres de vérification par défaut des autres utilisateurs de leur compte.

Pour plus d’informations, voir [Paramètres personnels dans [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Créateurs et propriétaires

Les créateurs et les propriétaires disposent de droits de modification complets sur le BAT.

### Créateurs {#creators}

Le créateur du BAT est la personne qui télécharge le BAT en première instance. Le créateur du BAT s&#39;affichera automatiquement dans la liste des personnes pour le BAT (dans son rôle par défaut).

Sur la page [!UICONTROL New BAT] , vous pouvez affecter un rôle de BAT différent au créateur du BAT (autre que son rôle par défaut).

Le créateur du BAT ne peut pas être modifié ni supprimé d’un BAT.

### Propriétaires {#owners}

Par défaut, le créateur est également le propriétaire du BAT. Cependant, le créateur peut faire de quelqu’un d’autre le propriétaire du BAT lors de la création initiale du BAT (sur la page [!UICONTROL New BAT]).

Pour modifier le propriétaire sur la page Nouveau BAT :

1. Cliquez sur le lien de modification affiché en regard du nom du créateur.
1. Sélectionnez le nouveau propriétaire dans le menu déroulant. (2)

![Proof_rôles_-_new_proof_page_change_owner_2.png{1](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Une fois le BAT créé, il est toujours possible de changer le propriétaire. Toute personne disposant de droits de modification sur le BAT pourra modifier la propriété du BAT pour qu’elle soit affectée à un autre utilisateur via la page [!UICONTROL Détails du BAT] (voir ci-dessous).

La possibilité de changer le propriétaire d&#39;un BAT est particulièrement utile du point de vue de la gestion des workflows. Il permet à la personne responsable du projet de prendre la possession des BAT, en lui donnant les droits d’édition sur les BAT et la possibilité de les afficher dans la vue [!UICONTROL Mes BAT].

Pour modifier le propriétaire du BAT via la page [!UICONTROL Détails du BAT] :

* Cliquez sur le menu Actions en regard du nom de la personne que vous souhaitez désigner comme propriétaire.
* Sélectionnez [!UICONTROL **Make owner**] dans le menu déroulant.
* Vous pouvez également cliquer dans le champ [!UICONTROL **Propriétaire**] en regard de l’image du BAT et choisir le nouveau propriétaire dans la liste déroulante affichée.

Une fois cette opération effectuée, le mot &quot;Propriétaire&quot; s’affiche en regard du nom de cette personne.

>[!NOTE]
>
>Seul un utilisateur du même compte ou d’un compte partenaire peut devenir propriétaire d’un BAT. Un utilisateur disposant d’un compte partenaire ne peut devenir propriétaire d’un BAT que dans les cas suivants :
>
>* Une relation de partenaire existante est configurée entre les comptes. Pour plus d’informations, voir [Comptes partenaires dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* Il n’existe aucun champ personnalisé sur la page [!UICONTROL New BAT].
>* Le BAT n’a pas été affecté à un dossier.
>* Aucune balise n’a été appliquée au BAT.

Pour déléguer temporairement la propriété du BAT dans [!DNL Workfront Proof], voir [Désignation des propriétaires de BAT temporaires dans [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
