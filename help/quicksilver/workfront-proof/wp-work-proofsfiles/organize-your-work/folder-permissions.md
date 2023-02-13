---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Présentation des autorisations de dossier dans [!DNL Workfront Proof]
description: Si une personne est autorisée à voir un élément dans un dossier, elle peut également voir le dossier lui-même. Cependant, ils ne peuvent voir que les éléments du dossier qui ont été explicitement partagés avec eux.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 17%

---

# Présentation des autorisations de dossier dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Si une personne est autorisée à voir un élément dans un dossier, elle peut également voir le dossier lui-même. Cependant, ils ne peuvent voir que les éléments du dossier qui ont été explicitement partagés avec eux.

## Dossiers publics

Si un dossier est public, les utilisateurs du compte (à l’exclusion des observateurs et des utilisateurs légers) peuvent voir le nom du dossier dans la barre latérale gauche.

Votre profil d’autorisation affecte également les droits que vous avez sur les dossiers publics :

| **Profile/Action** | **Afficher tous les éléments du dossier** | **Voir les éléments partagés explicitement avec eux** | **Ajout d’éléments** | **Suppression d’éléments** | **Ajouter des sous-dossiers** | **Suppression de sous-dossiers** | **Modifier les détails du dossier** |
|---|---|---|---|---|---|---|---|
| **Créateur** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Administrateur de facturation** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Administrateur** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Superviseur** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Gestionnaire** | Non | Oui | Oui | Non | Oui | Non | Oui |
| **Observateur** | Non | Oui | Non | Non | Non | Non | Non |

{style=&quot;table-layout:auto&quot;}

Si le dossier public est détenu par un responsable, il peut supprimer le dossier racine et tous les sous-dossiers.

Pour plus d’informations, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Dossiers privés

Si un dossier est privé, les autres utilisateurs du même compte ne pourront pas voir le nom du dossier dans la barre latérale gauche, sauf si le ou les éléments du dossier ont été explicitement partagés avec eux ou s’ils disposent d’un profil de responsable, d’administrateur ou d’administrateur de facturation :

| **Profile/Action** | **Afficher tous les éléments du dossier** | **Voir les éléments partagés explicitement avec eux** | **Ajout d’éléments** | **Suppression d’éléments** | **Ajouter des sous-dossiers** | **Suppression de sous-dossiers** | **Modifier les détails du dossier** |
|---|---|---|---|---|---|---|---|
| **Créateur** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Administrateur de facturation** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Administrateur** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Superviseur** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Gestionnaire** | Non | Oui | Non | Non | Non | Non | Non |
| **Observateur** | Non | Oui | Non | Non | Non | Non | Non |

{style=&quot;table-layout:auto&quot;}

Si, par exemple, vous souhaitez que votre chef de projet et ses équipes affichent uniquement des dossiers spécifiques, le chef de projet peut configurer un dossier privé, puis le partager avec des utilisateurs spécifiques.

Lorsque vous partagez un dossier privé, vous pouvez décider si vous souhaitez que les gestionnaires puissent créer, modifier et supprimer des éléments de dossier.

Vous pouvez définir cette option pour chaque personne individuellement sur la page Nouveau dossier et la modifier dans la variable [!UICONTROL Partagé avec] de la page Détails du dossier. Pour plus d’informations, voir [Création de dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) et [Gestion des dossiers et de leur contenu dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Si un dossier privé est partagé avec un observateur ou , il aura accès en lecture seule à tous les éléments du dossier. Pour plus d’informations, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) et [Partage de dossiers dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Si un dossier parent est privé, tous les sous-dossiers seront également privés. Vous ne pouvez pas avoir de sous-dossier public sous un dossier parent privé. Vous pouvez toutefois disposer d’un sous-dossier privé sous un dossier parent public.
>* Le créateur et le propriétaire du dossier y aura toujours accès et ne pourra pas être supprimé.
>* Seul le créateur et le propriétaire du dossier privé peut supprimer le dossier.


