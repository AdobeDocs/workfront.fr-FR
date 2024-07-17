---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: La page de facturation du BAT [!DNL Workfront]
description: Pour accéder à la page [!UICONTROL Facturation] , ouvrez le menu Paramètres en haut à droite de l’écran et choisissez Facturation dans le menu déroulant.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# La page de facturation [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## Page de facturation

Pour accéder à la page [!UICONTROL Facturation], ouvrez le menu **[!UICONTROL Paramètres]** en haut à droite de l’écran et sélectionnez **[!UICONTROL Facturation]** dans le menu déroulant.

La page [!UICONTROL Facturation] contient les éléments suivants :

* Nom du compte (1)
* Liste des comptes (par exemple, si vous disposez de comptes satellites)(2)
* Changement de plan (3)
* Modifier les détails du paiement (4)
* Nouveau compte satellite (5)
* Fermer le compte (6)
* Informations sur le plan actuel (7)
* Contact et adresse de facturation (8)
* Statistiques d’utilisation (9)
* Historique de facturation (10)
* Activité Facturation (11)

  ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Plan actuel]

Cette section (7) présente les détails de votre plan actuel, notamment :

* Nom du plan
* Mode de paiement actuel
* Dates de début et de fin du plan actuel
* Type de plan suivant
* Méthode de paiement du prochain plan

  Pour plus d’informations, voir [Choix de votre mode de paiement dans [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Contact et adresse de facturation]

Cette section (8) présente les coordonnées principales de contact et d’adresse de facturation de votre compte.

Le contact de facturation ne peut être sélectionné que parmi les utilisateurs configurés en tant qu’administrateurs de facturation sur votre compte. Sur les comptes satellites, seuls les administrateurs de facturation du compte principal peuvent être définis dans ce champ.

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> Vous pouvez avoir plusieurs administrateurs de facturation sur votre compte, mais un seul d’entre eux, sélectionné dans le champ [!UICONTROL Contact de facturation], recevra toutes les notifications de facturation et les alertes d’utilisation du compte.

Cela inclut les emails de notification suivants :

* Utilisation des BAT
* Facturations
* Rétrogradation
* Alerte de suspension de paiement en retard/compte
* Échec de la carte de crédit

  ![Billin_CC.png](assets/billin-cc-350x103.png)

Le champ [!UICONTROL Facturation CC] vous permet également d’ajouter une adresse électronique à copier sur tous les emails liés à la facturation. Cliquez sur le champ pour activer l’édition d’inclusion et saisissez l’adresse électronique de votre choix (il peut également s’agir de l’adresse électronique d’un utilisateur existant).

## [!UICONTROL Adresse de facturation]

Cette section utilise les modifications intégrées. Il suffit donc de cliquer sur les champs pour saisir/modifier le texte.

>[!NOTE]
>
> Nous incluons cette adresse dans vos factures d&#39;abonnement afin de vous assurer que ces données sont toujours à jour.

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL Statistiques d’utilisation]

Cette section présente les statistiques d’utilisation de votre compte au cours de la période de facturation actuelle, notamment :

* Stockage utilisé
* Bons à tirer utilisés
* Limite d’utilisateurs utilisée

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Avertissements d’utilisation]

Les [[!UICONTROL profils d’autorisations de BAT] dans [!DNL Workfront] BAT](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) définis comme contact de facturation (1) sur votre compte seront avertis par e-mail lorsque votre compte arrivera à :

* 75 %, puis 98 % de votre capacité de stockage
* 75 % puis 100 % de votre limite de BAT

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

Une fois les BAT ou les limites de stockage atteintes, les alertes s’affichent également en haut de la page [!UICONTROL Facturation] :

* Pour la limite de BAT atteinte

  ![Proofs_limit_reach.png](assets/proofs-limit-reached-350x65.png)

* Pour la limite de stockage atteinte

![Storage_limit_reach.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>Le nombre de BAT est utilisé lorsque des BAT sont créés dans votre compte et ne peuvent pas être restaurés en supprimant les BAT.

L’espace de stockage peut être libéré en supprimant les bons à tirer et les fichiers et en vidant la [!UICONTROL corbeille] par la suite.

N’oubliez pas que si vous avez besoin d’autres BAT, stockage ou utilisateurs, vous pouvez mettre à niveau votre compte à tout moment et cela prend effet immédiatement.

## [!UICONTROL Historique de facturation]

Cette section présente l&#39;activité pour toutes les périodes de facturation récentes. Vous pouvez également télécharger vos factures à partir de cette section.

Pour plus d’informations, voir &quot; [Téléchargement de votre [!DNL Workfront Proof] facture](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md)&quot;.

## [!UICONTROL Activité de facturation]

Cette section présente les modifications récentes apportées à la configuration de la facturation, par exemple les abonnements, les mises à niveau, les mises à niveau, les mises à niveau et les renouvellements de votre formule [!DNL Workfront Proof].

Si vous définissez votre formule d’abonnement sur une limite d’utilisateurs inférieure (1), les utilisateurs qui dépassent la nouvelle limite seront automatiquement désactivés au début du nouveau forfait. Cette activité sera également capturée dans vos logs de compte (2).

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![ Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
