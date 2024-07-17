---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Profils d’autorisations d’épreuve dans l’épreuve Workfront
description: En tant qu’administrateur Workfront ou administrateur Workfront Proof, vous pouvez affecter un profil d’autorisations de BAT à un utilisateur afin de spécifier les fonctionnalités de vérification que l’utilisateur aura pour tous les bons à tirer du système. Pour plus d’informations sur la configuration du profil d’autorisation de BAT d’un utilisateur, voir Configuration du profil d’autorisation de BAT d’un utilisateur dans Workfront Proof .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1764'
ht-degree: 1%

---

# Profils d’autorisations de BAT dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

En tant qu’administrateur [!DNL Workfront] ou [!DNL Workfront Proof], vous pouvez affecter un profil d’autorisations de BAT à un utilisateur afin de spécifier les fonctionnalités de vérification que l’utilisateur aura pour tous les bons à tirer du système. Pour plus d’informations sur la configuration du profil d’autorisation de BAT d’un utilisateur, voir [Configuration du profil d’autorisation de BAT d’un utilisateur dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>Vous pouvez également effectuer les opérations suivantes :
>
>* Octroi aux utilisateurs de rôles spécifiques sur des bons à tirer individuels. Pour plus d’informations sur les rôles de BAT, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Créez des profils personnalisés pour les utilisateurs de votre entreprise. Pour plus d’informations, voir [Configuration de profils personnalisés dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>

Le tableau suivant affiche les autorisations disponibles pour chaque profil d’autorisations de BAT.

| **Éléments propres** |  |  |  |  | **Autres éléments d’utilisateurs** |  |  | **Admin** | **Facturation** |
|---|---|---|---|---|---|---|---|---|---|
|   | **Ajouter** | **Afficher** | **Modifier** | **Supprimer** | **Afficher** | **Modifier** | **Supprimer** | **Modifier et supprimer** | **Modifier** |
| Administrateur de facturation | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Administration | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Superviseur | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Gestionnaire | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Observateur |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Visiteur |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

Tenez compte des points suivants concernant les rôles et les autorisations :

* Les autorisations de profil attribuées concernent uniquement les utilisateurs et les éléments de votre propre compte. L’exception concerne les comptes satellites, où l’administrateur et l’administrateur de facturation des comptes principaux (hub) peuvent accéder aux paramètres du compte et les gérer, ainsi que leur facturation, à partir du niveau du compte central.
* Les administrateurs et administrateurs de facturation peuvent supprimer des utilisateurs. Cette opération ne peut être effectuée que dans les paramètres du compte.
* Lorsque les administrateurs et les administrateurs de facturation affichent les bons à tirer qui sont possédés par d’autres utilisateurs dans leur compte, ils les voient avec le rôle de réviseur.
* En utilisant le rôle Lecture seule, les administrateurs de facturation et les administrateurs peuvent accéder aux BAT dans des dossiers partagés avec eux ou dans des dossiers créés par eux.

Les sections suivantes décrivent chaque profil et les autorisations associées au profil dans une configuration [!DNL Workfront Proof] standard :

* [Administrateur de facturation](#billing-administrator)
* [Administrateur](#administrator)
* [Superviseur](#supervisor)
* [Manager](#manager)
* [Observateur](#observer)
* [Visitor](#visitor)
* [Invité](#guest)

## Administrateur de facturation {#billing-administrator}

Les administrateurs de facturation ont accès aux [paramètres du compte dans la  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et disposent des autorisations suivantes :

![](assets/cleaner2.png) Peut générer des bons à tirer, télécharger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Télécharger des fichiers et du contenu web dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) et [Créer des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Peut afficher, modifier et supprimer ses propres BAT et fichiers qu’ils créent.

![](assets/cleaner2.png)Peut afficher, modifier et supprimer les bons à tirer et les fichiers créés par tous les utilisateurs de l’entreprise.

![](assets/cleaner2.png)Peut supprimer les dossiers publics des autres utilisateurs. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispose de droits d’édition sur tous les BAT créés dans le compte.

![](assets/cleaner2.png)Peut être défini comme propriétaire de zone de dépôt. Pour plus d’informations, voir [Configuration de la zone de dépôt dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Peut accéder à la page de facturation et modifier les détails de facturation. Pour plus d’informations, voir [La  [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Peut accéder à la page Paramètres du compte et modifier les détails du compte. Pour plus d’informations, voir [Paramètres du compte dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Peut vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Peut ajouter, modifier et supprimer des utilisateurs.

![](assets/cleaner2.png)Peut créer des groupes et ajouter de nouveaux contacts.

![](assets/cleaner2.png)Peut supprimer des contacts.

![](assets/cleaner2.png) Peut modifier les bons à tirer s’ils ne contiennent aucune réponse.

![](assets/no2.png)Impossible de modifier les réponses du BAT.

![](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Pour plus d’informations sur les paramètres du compte, voir [Paramètres du compte dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Pour plus d’informations sur la facturation, voir [La  [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administrateur {#administrator}

Les administrateurs ont accès aux [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) et disposent des autorisations suivantes :

![](assets/cleaner2.png) Peut créer des BAT, télécharger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Télécharger des fichiers et du contenu web dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) et [Créer des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png) Peut afficher, modifier et supprimer les bons à tirer et les fichiers qu’ils ont créés.

![](assets/cleaner2.png)Peut afficher, modifier et supprimer les bons à tirer et les fichiers créés par tous les utilisateurs de l’entreprise.

![](assets/cleaner2.png)Peut supprimer les dossiers publics des autres utilisateurs. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispose de droits d’édition sur tous les BAT créés dans le compte.

![](assets/cleaner2.png)Peut être défini comme propriétaire de zone de dépôt. Pour plus d’informations, voir [Configuration de la zone de dépôt dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Peut accéder à la page Paramètres du compte et modifier les détails du compte. Pour plus d’informations, voir [Paramètres du compte dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Peut vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Peut ajouter, modifier et supprimer des utilisateurs.

![](assets/cleaner2.png)Peut créer des groupes et ajouter de nouveaux contacts.

![](assets/cleaner2.png)Peut supprimer des contacts.

![](assets/cleaner2.png) Peut modifier les bons à tirer s’ils ne contiennent aucune réponse.

![](assets/no2.png)Impossible de modifier les réponses du BAT.

![](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossible d&#39;accéder à la page Facturation ou de modifier les détails de facturation. Pour plus d’informations, voir [La  [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Superviseur {#supervisor}

Les superviseurs disposent des autorisations suivantes :

![](assets/cleaner2.png) Peut créer des BAT, télécharger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Télécharger des fichiers et du contenu web dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) et [Créer des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Peut afficher, modifier et supprimer ses propres BAT et fichiers qu’ils ont créés.

![](assets/cleaner2.png)Peut afficher, modifier et supprimer les bons à tirer et les fichiers créés par tous les utilisateurs de l’entreprise.

![](assets/cleaner2.png)Peut supprimer les dossiers publics des autres utilisateurs. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispose de droits d’édition sur tous les BAT créés dans le compte.

![](assets/cleaner2.png)Peut être défini comme propriétaire de zone de dépôt. Pour plus d’informations, voir [Configuration de la zone de dépôt dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Peut créer des groupes et ajouter de nouveaux contacts.

![](assets/cleaner2.png)Peut supprimer des contacts.

![](assets/cleaner2.png) Peut modifier les bons à tirer s’ils ne contiennent aucune réponse.

![](assets/no2.png)Impossible de modifier les réponses du BAT.

![](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, voir [Dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png) Impossible d&#39;accéder à la page de facturation ou aux paramètres du compte. Pour plus d’informations, voir [La  [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et les [paramètres du compte dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Gestionnaire {#manager}

Les gestionnaires disposent des autorisations suivantes :

![](assets/cleaner2.png) Peut créer des BAT, télécharger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Télécharger des fichiers et du contenu web dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) et [Créer des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Peut afficher, modifier et supprimer les propres BAT et fichiers qu’ils créent ou qu’ils détiennent.

![](assets/cleaner2.png)Peut afficher, réviser et approuver les BAT d’autres utilisateurs qui sont explicitement partagés avec eux (droits en lecture seule sur tout ce qui se trouve dans un dossier partagé). Pour plus d’informations, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Peut créer des groupes et ajouter un nouveau contact.

![](assets/no2.png)Impossible d’afficher, de modifier ou de supprimer les bons à tirer et les fichiers créés par d’autres utilisateurs de l’organisation.

![](assets/no2.png)Impossible de modifier les BAT ou les réponses.

![](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossible de supprimer les dossiers publics des autres utilisateurs. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png) Impossible d&#39;accéder à la page de facturation ou aux paramètres du compte. Pour plus d’informations, voir [La  [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et les [paramètres du compte dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Ne peut pas être défini comme propriétaire de la zone de dépôt. Pour plus d’informations, voir [Configuration de la zone de dépôt dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![](assets/no2.png)Impossible de supprimer les contacts.

### Observateur {#observer}

Les observateurs disposent des autorisations suivantes :

![](assets/cleaner2.png)Peut afficher, réviser et approuver les BAT d’autres utilisateurs qui sont explicitement partagés avec eux (droits en lecture seule sur tout ce qui se trouve dans un dossier partagé). Pour plus d’informations, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Peut afficher les fichiers qui sont explicitement partagés avec eux.

![](assets/cleaner2.png) Peut afficher les contacts et les groupes

![](assets/no2.png)Impossible de créer des bons à tirer, de charger des fichiers et de créer des dossiers. Pour plus d’informations, voir [Téléchargement de fichiers et de contenu web vers [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Impossible d’afficher, de modifier ou de supprimer les bons à tirer et les fichiers créés par d’autres utilisateurs de l’organisation.

![](assets/no2.png)Impossible de modifier les BAT ou les réponses.

![](assets/no2.png)Impossible de supprimer les éléments créés dans l’organisation.

![](assets/no2.png) Impossible d&#39;accéder à la page de facturation ou aux paramètres du compte. Pour plus d’informations, voir [La  [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et les [paramètres du compte dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Ne peut pas être défini comme propriétaire de la zone de dépôt. Pour plus d’informations, voir [Configuration de la zone de dépôt dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![](assets/no2.png)Impossible de créer des groupes ou d’ajouter de nouveaux contacts.

![](assets/no2.png)Impossible de supprimer les contacts.

>[!NOTE]
>
>Les menus et fonctions disponibles pour les observateurs sont limités.
>
>* Les observateurs ne voient pas le menu En-tête ou Nouveau vert dans leur tableau de bord.
>* Les observateurs ne voient pas les liens suivants dans leurs paramètres : Paramètres du compte, Facturation
>

### Visiteur {#visitor}

Les visiteurs disposent des autorisations suivantes :

![](assets/cleaner2.png)Peut afficher, réviser et approuver les BAT d’autres utilisateurs qui sont explicitement partagés avec eux (droits en lecture seule sur tout ce qui se trouve dans un dossier partagé). Pour plus d’informations, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Peut afficher les fichiers qui sont explicitement partagés avec eux.

![](assets/no2.png) Impossible d’afficher les contacts et les groupes

![](assets/no2.png)Impossible de créer des bons à tirer, de charger des fichiers et de créer des dossiers. Pour plus d’informations, voir [Téléchargement de fichiers et de contenu web vers [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Impossible d’afficher, de modifier ou de supprimer les bons à tirer et les fichiers créés par d’autres utilisateurs de l’organisation.

![](assets/no2.png)Impossible de modifier les BAT ou les réponses.

![](assets/no2.png)Impossible de supprimer les éléments créés dans l’organisation.

![](assets/no2.png) Impossible d&#39;accéder à la page de facturation ou aux paramètres du compte. Pour plus d’informations, voir [La  [!DNL Workfront Proof] page de facturation](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et les [paramètres du compte dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Ne peut pas être défini comme propriétaire de la zone de dépôt. Pour plus d’informations, voir [Configuration de la zone de dépôt dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![](assets/no2.png)Impossible de créer des groupes ou d’ajouter de nouveaux contacts.

![](assets/no2.png)Impossible de supprimer les contacts.

>[!NOTE]
>
>Les menus et fonctions disponibles pour les visiteurs sont limités.
>
>* Le menu En-tête ou Nouveau vert n’apparaît pas dans le tableau de bord des visiteurs.
>* Les liens suivants ne s’affichent pas dans les paramètres des visiteurs : Paramètres du compte, Facturation
>

### Invité {#guest}

Le profil d’invité permet d’accéder aux bons à tirer pour les réviseurs qui n’ont pas leur propre compte Workfront Proof. Les invités peuvent accéder aux BAT partagés avec eux directement via leur email de notification.

![](assets/cleaner2.png) Peut afficher, réviser et approuver les bons à tirer qui sont explicitement partagés avec eux.

![](assets/cleaner2.png)Peut afficher les fichiers qui sont explicitement partagés avec eux.

![](assets/no2.png)Impossible d’accéder au tableau de bord.

![](assets/no2.png)Les dossiers ne peuvent pas être partagés avec eux. Pour plus d’informations, voir [Gestion des dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Ne peut pas être ajouté en tant qu’auteurs ou modérateurs aux bons à tirer. Pour plus d’informations, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Les clients ne sont pas des utilisateurs de Workfront Proof, ils ne peuvent donc pas voir tous les bons à tirer partagés avec eux dans leur propre tableau de bord.

## Modification du profil d’autorisation de BAT d’un utilisateur

Les administrateurs et les administrateurs de facturation peuvent modifier les profils d’autorisation de tous les utilisateurs du compte.

1. Pour trouver l’utilisateur à modifier, effectuez l’une des opérations suivantes :

   * Accédez à **[!UICONTROL Paramètres du compte]**, puis cliquez sur l’onglet **[!UICONTROL Utilisateurs]**.

   * Accédez à la page **[!UICONTROL Contacts]** .

1. Cliquez sur le nom de l’utilisateur dont vous souhaitez modifier les autorisations. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Profil d’autorisations]** et sélectionnez un nouveau profil d’autorisation. :

   ![Capture d’écran_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   Les profils d’autorisation sont Administrateur, Superviseur, Gestionnaire et Observateur.

1. Cliquez n’importe où en dehors du menu pour enregistrer.

>[!NOTE]
>
>Les administrateurs ne peuvent pas affecter le profil Administrateur de facturation. Vous trouverez une liste des modifications de profil dans les journaux suivants :
>
>* Logs de l’activité Compte
>* Journal du profil de l’utilisateur (accessible uniquement à cet utilisateur)
>

Pour plus d’informations sur les journaux d’activité, voir [Présentation du  [!DNL Workfront Proof] journal d’audit d’activité](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
