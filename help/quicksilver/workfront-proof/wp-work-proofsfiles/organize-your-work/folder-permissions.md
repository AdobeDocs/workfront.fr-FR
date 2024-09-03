---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Comprendre les autorisations de dossier dans  [!DNL Workfront Proof]
description: Si une personne est autorisée à voir un élément dans un dossier, elle peut également voir le dossier lui-même. Cependant, elle ne peut voir que les éléments du dossier qui ont été explicitement partagés avec elle.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 100%

---

# Comprendre les autorisations de dossier dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Si une personne est autorisée à voir un élément dans un dossier, elle peut également voir le dossier lui-même. Cependant, elle ne peut voir que les éléments du dossier qui ont été explicitement partagés avec elle.

## Dossiers publics

Si un dossier est public, les utilisateurs et les utilisatrices du compte (à l’exclusion des personnes qui observent ou qui ont une licence Light) peuvent voir le nom du dossier dans la barre latérale gauche.

Votre profil d’autorisation affecte également les droits que vous avez sur les dossiers publics :

| **Profil / Action** | **Afficher tous les éléments du dossier** | **Afficher les éléments partagés explicitement avec les personnes** | **Ajouter des éléments** | **Supprimer des éléments** | **Ajouter des sous-dossiers** | **Supprimer des sous-dossiers** | **Modifier les détails du dossier** |
|---|---|---|---|---|---|---|---|
| **Personne chargée de la création** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de l’administration de la facturation** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de l’administration** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de la supervision** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de la gestion** | Non | Oui | Oui | Non | Oui | Non | Oui |
| **Observateur ou observatrice** | Non | Oui | Non | Non | Non | Non | Non |

{style="table-layout:auto"}

Si le dossier public est détenu par un ou une responsable, il ou elle peut supprimer le dossier racine et tous les sous-dossiers.

Pour plus d’informations, voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Dossiers privés

Si un dossier est privé, les autres personnes du même compte ne pourront pas voir le nom du dossier dans la barre latérale gauche, sauf si le dossier ou les éléments du dossier ont été explicitement partagés avec elles ou si elles disposent d’un profil de responsable, d’administrateur ou d’administratrice ou d’administrateur ou administratrice de facturation :

| **Profile/Action** | **Afficher tous les éléments du dossier** | **Afficher les éléments partagés explicitement avec les personnes** | **Ajouter des éléments** | **Supprimer des éléments** | **Ajouter des sous-dossiers** | **Supprimer des sous-dossiers** | **Modifier les détails du dossier** |
|---|---|---|---|---|---|---|---|
| **Personne chargée de la création** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de l’administration de la facturation** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de l’administration** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de la supervision** | Oui | Oui | Oui | Oui | Oui | Oui | Oui |
| **Personne chargée de la gestion** | Non | Oui | Non | Non | Non | Non | Non |
| **Personne chargée de l’observation** | Non | Oui | Non | Non | Non | Non | Non |

{style="table-layout:auto"}

Si, par exemple, vous souhaitez que la personne chargée de la gestion de vos projets et ses équipes puissent uniquement afficher des dossiers spécifiques, elle peut configurer un dossier privé, puis le partager avec des utilisateurs et utilisatrices spécifiques.

Lorsque vous partagez un dossier privé, vous pouvez décider si vous souhaitez que les personnes gestionnaires puissent créer, modifier et supprimer des éléments de dossier.

Vous pouvez définir cette option pour chaque personne individuellement sur la page Nouveau dossier et la modifier dans la section [!UICONTROL Partagé avec] de la page Détails du dossier. Pour plus d’informations, consultez [Création de dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) et [Gestion des dossiers et de leur contenu dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Si un dossier privé est partagé avec un observateur ou une observatrice, cette personne aura accès en lecture seule à tous les éléments du dossier. Pour plus d’informations, consultez [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) et [Partage de dossiers dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Si un dossier parent est privé, tous les sous-dossiers seront également privés. Vous ne pouvez pas avoir de sous-dossier public sous un dossier parent privé. Vous pouvez toutefois disposer d’un sous-dossier privé sous un dossier parent public.
>* La personne qui a créé le dossier et celle qui en est propriétaire y auront toujours accès et il ne pourra pas être supprimé.
>* Seules la personne qui a créé le dossier privé et celle qui en est propriétaire peuvent supprimer le dossier.

