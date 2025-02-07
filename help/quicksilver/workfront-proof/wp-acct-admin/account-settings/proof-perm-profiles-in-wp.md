---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Profils des autorisations d’épreuve dans Workfront Proof
description: En tant que personne membre de l’administration Workfront ou de l’administration Workfront Proof, vous pouvez assigner un profil d’autorisation pour l’épreuve à un utilisateur ou à une utilisatrice afin de spécifier ses droits pour toutes les épreuves du système. Pour plus d’informations sur la configuration du profil d’autorisation pour l’épreuve d’un utilisateur ou d’une utilisatrice, consultez la section « Configurer le profil d’autorisation pour l’épreuve d’un utilisateur ou d’une utilisatrice dans Workfront Proof ».
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 53%

---

# Profils d’autorisation pour l’épreuve dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

En tant que personne membre de l’administration [!DNL Workfront] ou de l’administration [!DNL Workfront Proof], vous pouvez assigner un profil d’autorisation pour l’épreuve à un utilisateur ou à une utilisatrice afin de spécifier ses droits pour toutes les épreuves du système. Pour plus d’informations sur la configuration du profil d’autorisation pour l’épreuve d’un utilisateur ou d’une utilisatrice, consultez la section [Configurer le profil d’autorisation pour l’épreuve d’un utilisateur ou d’une utilisatrice dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>Vous pouvez également effectuer les opérations suivantes :
>
>* Accorder aux utilisateurs et aux utilisatrices des rôles spécifiques sur des épreuves individuelles. Pour plus d’informations sur les rôles d’épreuve, consultez la section [Gérer les rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Créez des profils personnalisés pour les utilisateurs et utilisatrices de votre organisation. Pour plus d’informations, consultez la section [Configurer des profils personnalisés dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>

Le tableau suivant présente les autorisations disponibles pour chaque profil d’autorisation pour l’épreuve.

| **Éléments propres** |  |  |  |  | **Éléments d’autres utilisateurs et utilisatrices** |  |  | **Administration** | **Facturation** |
|---|---|---|---|---|---|---|---|---|---|
|   | **Ajouter** | **Afficher** | **Modifier** | **Supprimer** | **Afficher** | **Modifier** | **Supprimer** | **Modifier et supprimer** | **Modifier** |
| Administration de la facturation | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) |
| Administration | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) |   |
| Superviseur | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) |   |   |
| Gestionnaire | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) | ![Coche](assets/cleaner2.png) |   |   |   |   |   |
| Observateur |   | ![Coche](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Visiteur ou visiteuse |   | ![Coche](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

Tenez compte de ce qui suit concernant les rôles et les autorisations :

* Les autorisations de profil attribuées ne concernent que les utilisateurs et utilisatrices et les éléments de votre propre compte. L’exception concerne les comptes satellites, pour lesquels l’équipe d’administration et la personne responsable de la facturation des comptes principaux (hub) peuvent accéder et gérer les paramètres et la facturation de ces comptes à partir du niveau du compte hub.
* Les équipes d’administration et la personne chargée de la facturation peuvent supprimer des utilisateurs et utilisatrices. Cette opération ne peut être effectuée que dans les paramètres du compte.
* Lorsque les équipes d’administration et les personnes responsables de la facturation consultent des épreuves appartenant à d’autres utilisateurs et utilisatrices de leur compte, elles les consultent avec le rôle de réviseur ou réviseuse.
* En utilisant le rôle Lecture seule, les équipes d’administration et les personnes responsables de la facturation peuvent accéder aux épreuves dans les dossiers partagés avec eux ou dans les dossiers qu’elles ont créés.

Les sections suivantes décrivent chaque profil et ses autorisations associées dans une configuration standard de [!DNL Workfront Proof] :

* [Personne responsable de la facturation](#billing-administrator)
* [Équipe d’administration](#administrator)
* [Superviseur ou superviseuse](#supervisor)
* [Personne responsable](#manager)
* [Observateur ou observatrice](#observer)
* [Visiteur ou visiteuse](#visitor)
* [Personne invitée](#guest)

## Personne responsable de la facturation {#billing-administrator}

Les personnes responsables de facturation ont accès aux [paramètres du compte sur la page de facturation  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et disposent des autorisations suivantes :

![Coche](assets/cleaner2.png)Peut générer des épreuves, charger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Charger des fichiers et du contenu web dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), et [Créer des dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Coche](assets/cleaner2.png)Peut afficher, modifier et supprimer ses propres épreuves et fichiers qu’il crée.

![Coche](assets/cleaner2.png)Peut afficher, modifier et supprimer des épreuves et des fichiers créés par tous les utilisateurs de l’entreprise.

![Coche](assets/cleaner2.png)Peut supprimer les dossiers publics d’autres utilisateurs. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Coche](assets/cleaner2.png)Dispose de droits de modification sur toutes les épreuves créées dans le compte.

![Coche](assets/cleaner2.png)Peut être défini comme propriétaire de la zone de dépôt. Pour plus d’informations, voir [Configurer la zone de dépôt dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Coche](assets/cleaner2.png)Peut accéder à la page de facturation et modifier les détails de facturation. Pour plus d’informations, voir [la page de facturation  [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![Coche](assets/cleaner2.png)Peut accéder à la page Paramètres du compte et modifier les détails du compte. Pour plus d’informations, voir [Paramètres du compte dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Coche](assets/cleaner2.png)Peut vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![Coche](assets/cleaner2.png)Permet d’ajouter, de modifier et de supprimer des utilisateurs.

![Coche](assets/cleaner2.png)Permet de créer des groupes et d’ajouter de nouveaux contacts.

![Coche](assets/cleaner2.png)Peut supprimer des contacts.

![Coche](assets/cleaner2.png)Peut modifier les épreuves en l’absence de réponse.

![Red X](assets/no2.png)Impossible de modifier les réponses de l&#39;épreuve.

![Red X](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Pour plus d’informations sur les paramètres du compte, voir [Paramètres du compte dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Pour plus d’informations sur la facturation, voir [la page de facturation  [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administrateur ou administratrice {#administrator}

Les administrateurs et les administratrices ont accès aux [paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) et disposent des autorisations suivantes :

![Coche](assets/cleaner2.png)Peut créer des épreuves, charger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Charger des fichiers et du contenu web dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), et [Créer des dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Coche](assets/cleaner2.png)Peut afficher, modifier et supprimer les épreuves et les fichiers qu’il a créés.

![Coche](assets/cleaner2.png)Peut afficher, modifier et supprimer des épreuves et des fichiers créés par tous les utilisateurs de l’entreprise.

![Coche](assets/cleaner2.png)Peut supprimer les dossiers publics d’autres utilisateurs. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Coche](assets/cleaner2.png)Dispose de droits de modification sur toutes les épreuves créées dans le compte.

![Coche](assets/cleaner2.png)Peut être défini comme propriétaire de la zone de dépôt. Pour plus d’informations, voir [Configurer la zone de dépôt dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Coche](assets/cleaner2.png)Peut accéder à la page Paramètres du compte et modifier les détails du compte. Pour plus d’informations, voir [Paramètres du compte dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Coche](assets/cleaner2.png)Peut vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![Coche](assets/cleaner2.png)Permet d’ajouter, de modifier et de supprimer des utilisateurs.

![Coche](assets/cleaner2.png)Permet de créer des groupes et d’ajouter de nouveaux contacts.

![Coche](assets/cleaner2.png)Peut supprimer des contacts.

![Coche](assets/cleaner2.png)Peut modifier les épreuves en l’absence de réponse.

![Red X](assets/no2.png)Impossible de modifier les réponses de l&#39;épreuve.

![Red X](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Rouge X](assets/no2.png)Impossible d’accéder à la page Facturation ou de modifier les détails de facturation. Pour plus d’informations, consultez [la page de facturation  [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Superviseur {#supervisor}

Les personnes responsables disposent des autorisations suivantes :

![Coche](assets/cleaner2.png)Peut créer des épreuves, charger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Charger des fichiers et du contenu web dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), et [Créer des dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Coche](assets/cleaner2.png)Peut afficher, modifier et supprimer ses propres épreuves et fichiers créés.

![Coche](assets/cleaner2.png)Peut afficher, modifier et supprimer des épreuves et des fichiers créés par tous les utilisateurs de l’entreprise.

![Coche](assets/cleaner2.png)Peut supprimer les dossiers publics d’autres utilisateurs. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Coche](assets/cleaner2.png)Dispose de droits de modification sur toutes les épreuves créées dans le compte.

![Coche](assets/cleaner2.png)Peut être défini comme propriétaire de la zone de dépôt. Pour plus d’informations, voir [Configurer la zone de dépôt dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Coche](assets/cleaner2.png)Permet de créer des groupes et d’ajouter de nouveaux contacts.

![Coche](assets/cleaner2.png)Peut supprimer des contacts.

![Coche](assets/cleaner2.png)Peut modifier les épreuves en l’absence de réponse.

![Red X](assets/no2.png)Impossible de modifier les réponses de l&#39;épreuve.

![Red X](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, consultez la section [Dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![Red X](assets/no2.png)Impossible d’accéder à la page Facturation ou aux paramètres du compte. Pour plus d’informations, consultez [la page de facturation  [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et la section [Paramètres du compte dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Red X](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![Red X](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, consultez la section [Restaurer et vider la corbeille dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Gestionnaire {#manager}

Les personnes gestionnaires disposent des autorisations suivantes :

![Coche](assets/cleaner2.png)Peut créer des épreuves, charger des fichiers et créer des dossiers. Pour plus d’informations, voir [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Charger des fichiers et du contenu web dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), et [Créer des dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Coche](assets/cleaner2.png)Peut afficher, modifier et supprimer ses propres épreuves et fichiers qu’il crée ou dont il est propriétaire.

![Coche](assets/cleaner2.png)Peut afficher, réviser et approuver les BAT d’autres utilisateurs qui sont explicitement partagés avec eux (droits en lecture seule sur tout ce qui se trouve dans un dossier partagé). Pour plus d’informations, consultez la section [Gérer les rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![Coche](assets/cleaner2.png)Peut créer des groupes et ajouter un nouveau contact.

![Red X](assets/no2.png)Impossible d’afficher, de modifier ou de supprimer des épreuves et des fichiers créés par d’autres utilisateurs de l’entreprise.

![Red X](assets/no2.png)Impossible de modifier les épreuves ou les réponses.

![Red X](assets/no2.png)Impossible de supprimer les dossiers privés des autres utilisateurs. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Red X](assets/no2.png)Impossible de supprimer les dossiers publics des autres utilisateurs. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Red X](assets/no2.png)Impossible d’accéder à la page Facturation ou aux paramètres du compte. Pour plus d’informations, consultez [la page de facturation  [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et la section [Paramètres du compte dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Red X](assets/no2.png)Cannot be set as the Dropzone owner. Pour plus d’informations, voir [Configurer la zone de dépôt dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Red X](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![Red X](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![Red X](assets/no2.png)Impossible de supprimer les contacts.

### Observateur {#observer}

Les observateurs et observatrices disposent des autorisations suivantes :

![Coche](assets/cleaner2.png)Peut afficher, réviser et approuver les BAT des autres utilisateurs qui sont explicitement partagés avec eux (Droits en lecture seule sur tout ce qui se trouve dans un dossier partagé). Pour plus d’informations, consultez la section [Gérer les rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![Coche](assets/cleaner2.png)Peut afficher les fichiers qui sont explicitement partagés avec lui.

![Coche](assets/cleaner2.png) Peut afficher des contacts et des groupes

![Red X](assets/no2.png)Impossible de créer des épreuves, de charger des fichiers et de créer des dossiers. Pour plus d’informations, voir [Charger des fichiers et du contenu web dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![Red X](assets/no2.png)Impossible d’afficher, de modifier ou de supprimer des épreuves et des fichiers créés par d’autres utilisateurs de l’entreprise.

![Red X](assets/no2.png)Impossible de modifier les épreuves ou les réponses.

![Red X](assets/no2.png)Impossible de supprimer les éléments créés dans l’organisation.

![Red X](assets/no2.png)Impossible d’accéder à la page Facturation ou aux paramètres du compte. Pour plus d’informations, consultez [la page de facturation  [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et la section [Paramètres du compte dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Red X](assets/no2.png)Cannot be set as the Dropzone owner. Pour plus d’informations, voir [Configurer la zone de dépôt dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Red X](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![Red X](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![Red X](assets/no2.png)Impossible de créer des groupes ou d’ajouter de nouveaux contacts.

![Red X](assets/no2.png)Impossible de supprimer les contacts.

>[!NOTE]
>
>Les menus et les fonctions disponibles pour les observateurs et observatrices sont limités.
>
>* Les observateurs et observatrices ne voient pas le menu d’en-tête ou le menu vert Nouveau dans leur tableau de bord.
>* Les observateurs et observatrices ne voient pas les liens suivants dans leurs paramètres : Paramètres du compte, Facturation.
>

### Visiteur ou visiteuse {#visitor}

Les visiteurs et visiteuses disposent des autorisations suivantes :

![Coche](assets/cleaner2.png)Peut afficher, réviser et approuver les BAT d’autres utilisateurs qui sont explicitement partagés avec eux (droits en lecture seule sur tout ce qui se trouve dans un dossier partagé). Pour plus d’informations, consultez la section [Gérer les rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![Coche](assets/cleaner2.png)Peut afficher les fichiers qui sont explicitement partagés avec lui.

![Red X](assets/no2.png) Impossible d’afficher les contacts et les groupes

![Red X](assets/no2.png)Impossible de créer des épreuves, de charger des fichiers et de créer des dossiers. Pour plus d’informations, voir [Charger des fichiers et du contenu web dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![Red X](assets/no2.png)Impossible d’afficher, de modifier ou de supprimer des épreuves et des fichiers créés par d’autres utilisateurs de l’entreprise.

![Red X](assets/no2.png)Impossible de modifier les épreuves ou les réponses.

![Red X](assets/no2.png)Impossible de supprimer les éléments créés dans l’organisation.

![Red X](assets/no2.png)Impossible d’accéder à la page Facturation ou aux paramètres du compte. Pour plus d’informations, consultez [la page de facturation  [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) et la section [Paramètres du compte dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Red X](assets/no2.png)Cannot be set as the Dropzone owner. Pour plus d’informations, voir [Configurer la zone de dépôt dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Red X](assets/no2.png)Impossible de vider la corbeille. Pour plus d’informations, voir [Restaurer et vider la corbeille dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![Red X](assets/no2.png)Impossible d’ajouter, de modifier ou de supprimer des utilisateurs.

![Red X](assets/no2.png)Impossible de créer des groupes ou d’ajouter de nouveaux contacts.

![Red X](assets/no2.png)Impossible de supprimer les contacts.

>[!NOTE]
>
>Les menus et les fonctions disponibles pour les visiteurs et visiteuses sont limités.
>
>* Les visiteurs et visiteuses ne voient pas le menu d’en-tête ou le menu vert Nouveau dans leur tableau de bord.
>* Les liens suivants ne s’affichent pas dans les paramètres des visiteurs et visiteuses : Paramètres du compte, Facturation
>

### Personne invitée {#guest}

Le profil Personne invitée sert à accorder l’accès aux épreuves aux personnes chargées de la révision qui ne disposent pas de compte Workfront Proof. Les personnes invitées peuvent accéder aux épreuves partagées avec elles directement via leurs notifications personnelles par e-mail.

![Coche](assets/cleaner2.png)Peut afficher, réviser et approuver les épreuves qui sont explicitement partagées avec lui.

![Coche](assets/cleaner2.png)Peut afficher les fichiers qui sont explicitement partagés avec lui.

![Red X](assets/no2.png)Impossible d&#39;accéder au tableau de bord.

![Red X](assets/no2.png)Les dossiers ne peuvent pas être partagés avec eux. Pour plus d’informations, voir [Gérer les dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Red X](assets/no2.png)ne peut pas être ajouté en tant qu’auteur ou modérateur aux épreuves. Pour plus d’informations, voir [Gérer les rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Les personnes invitées ne sont pas des utilisateurs et utilisatrices de Workfront Proof, elles ne peuvent donc pas consulter toutes les épreuves partagées avec elles dans leur propre tableau de bord.

## Modifier le profil d’autorisation pour l’épreuve d’un utilisateur ou d’une utilisatrice

Les administrateurs et administratrices de facturation peuvent modifier les profils d’autorisation de tous les utilisateurs et utilisatrices du compte.

1. Pour trouver l’utilisateur ou l’utilisatrice à modifier, effectuez l’une des opérations suivantes :

   * Naviguez vers **[!UICONTROL Paramètres du compte]**, puis cliquez sur l’onglet **[!UICONTROL Utilisateurs et utilisatrices]**.

   * Accédez à la page **[!UICONTROL Contacts]**.

1. Cliquez sur le nom de l’utilisateur dont vous souhaitez modifier les autorisations. ![Sélectionner un utilisateur](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Profil d’autorisation]** et sélectionnez un nouveau profil d’autorisation.

   ![Profil des autorisations](assets/screenshot-2018-03-30-14-18-03a.png)

   Les profils d’autorisation sont Administration, Supervision, Gestion et Observation.

1. Cliquez en dehors du menu pour enregistrer.

>[!NOTE]
>
>Les administrateurs et administratrices ne peuvent pas affecter le profil Administration de facturation. Vous trouverez une liste des modifications de profil dans les journaux suivants :
>
>* Journaux de l’activité Compte
>* Journal du profil de l’utilisateur ou de l’utilisatrice (accessible uniquement à cette personne)
>

Pour plus d’informations sur les journaux d’activité, voir [Comprendre le journal d’audit d’activité  [!DNL Workfront Proof] ](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
