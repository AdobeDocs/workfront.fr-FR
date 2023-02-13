---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Gestion des versions de BAT dans [!DNL Workfront Proof]
description: Gérer les commentaires sur plusieurs versions ou révisions d’un travail peut s’avérer un énorme défi. [!DNL Workfront Proof] simplifie ce processus en vous permettant de créer et de comparer plusieurs versions d’un BAT.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Gestion des versions de BAT dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Gérer les commentaires sur plusieurs versions ou révisions d’un travail peut s’avérer un énorme défi. [!DNL Workfront Proof] simplifie ce processus en vous permettant de créer et de comparer plusieurs versions d’un BAT.

Le nombre de versions d’un BAT que vous pouvez créer n’est pas limité. Ainsi, si vous devez passer en revue de nombreuses révisions avec un client pour obtenir une approbation finale, toutes les versions créées peuvent être visualisées et facilement gérées dans [!DNL Workfront Proof].

Les autorisations sont spécifiques à une version. Vous pouvez donc accorder à une personne l’autorisation d’afficher une version, mais pas une autre. Inversement, si vous partagez une version ultérieure avec une personne, elle ne pourra pas voir les versions antérieures, sauf si vous revenez en arrière et les ajoutez explicitement à ces versions précédentes.

Pour créer une nouvelle version d’un BAT, vous devez disposer des droits d’édition sur le BAT.

Veuillez consulter [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) pour obtenir plus d’informations sur qui dispose de droits de modification sur un BAT. Voir pour en savoir plus sur la création de versions.

## Affichage des versions de BAT dans la visionneuse de vérification

Le nom complet de la version que vous affichez s’affiche en haut à gauche de la visionneuse de vérification. Toutes les autres versions du BAT s’afficheront sous forme de numéros de version uniquement.

1. Ouvrez un BAT dans la visionneuse de vérification, comme décrit dans la section [Ouverture d’un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. Dans la visionneuse de BAT, cliquez sur le numéro de version situé à droite du nom du BAT.
1. Pour afficher l’autre version, cliquez sur son nom dans le menu qui s’affiche lorsque vous cliquez sur le numéro de version.
1. Pour comparer deux versions, cliquez sur le bouton **[!UICONTROL Comparaison de BAT]** icône .\
   ![Compare_Proofs_button.png](assets/compare-proofs-button.png)\
   S’il existe plusieurs versions du BAT, vous pouvez sélectionner les deux versions que vous souhaitez comparer en cliquant sur le numéro de version approprié dans chaque côté de l’écran partagé du mode de comparaison.

Pour plus d’informations sur la révision des BAT dans une visionneuse de BAT, voir [Vérification d’un BAT](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Accès aux versions de BAT via la page Détails du BAT

Vous pouvez accéder à toutes les versions d&#39;un BAT à partir de la page Détails du BAT .

1. Ouvrez la page Détails du BAT pour un BAT, comme décrit dans la section [Gérer les détails du BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Cliquez sur l’onglet correspondant aux onglets de version en haut de la page, puis cliquez sur **[!UICONTROL Accéder au BAT]** pour ouvrir la version souhaitée dans la visionneuse de vérification.\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## Liaison de versions de BAT

Si votre BAT comporte plusieurs versions, la version précédente du BAT est généralement appelée BAT parent.

Si vous souhaitez modifier le BAT parent (version précédente) en un autre BAT dans votre compte, ou connecter un seul BAT à un autre BAT dans votre compte (en tant que nouvelle version de l’autre BAT), vous pouvez le faire facilement en procédant comme suit :

1. Ouvrez la page Détails du BAT pour un BAT, comme décrit dans la section [Gérer les détails du BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Modification de la version précédente]**.

1. Dans le **[!UICONTROL Modification de la version précédente]** s’affiche, sélectionnez le BAT que vous souhaitez définir comme BAT parent (version précédente).\
   Si vous avez besoin d’aide pour trouver le BAT dans la liste, vous pouvez trier les colonnes en cliquant sur l’en-tête de colonne.

1. Cliquez sur **[!UICONTROL Modification de la version précédente]** en bas de la boîte pour connecter les versions.

>[!NOTE]
>
>Lorsque vous connectez un BAT à un autre BAT dans votre compte (en tant que nouvelle version), [!DNL Workfront Proof] verrouille le BAT qui est désormais la version précédente.

## Suppression de liens vers des versions de BAT

Vous pouvez dissocier le BAT que vous affichez actuellement de son BAT parent (version précédente) sans le lier à un autre BAT de votre compte :

1. Ouvrez la page Détails du BAT pour un BAT, comme décrit dans la section [Gérer les détails du BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Supprimer le lien vers la version précédente]**.

   * Seule la dernière version peut être dissociée (déconnectée) de l’ensemble des versions. Cela deviendra alors une preuve unique.
   * Si vous devez insérer une version entre deux versions existantes, vous pouvez dissocier toutes les versions du même BAT et les réassocier dans l&#39;ordre approprié.

## À propos des jeux de versions et des limites de BAT

Chaque ensemble de cinq versions est compté comme un BAT par rapport à votre limite de BAT totale.

Par exemple, si vous téléchargez cinq versions d’une conception (y compris la version d’origine), cela compte comme un bon à tirer. Si vous chargez six versions d’une conception, cela compte comme deux bons à tirer. Onze versions comptent comme trois bons à tirer, etc.

Pour les fichiers audio-visuels, chaque nouvelle version est considérée comme un nouveau BAT.
