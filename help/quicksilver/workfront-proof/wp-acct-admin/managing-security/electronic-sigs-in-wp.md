---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Présentation des signatures électroniques dans  [!DNL Workfront Proof]
description: Les signatures électroniques vous permettent d’améliorer la sécurité de vos BAT et de respecter les normes du secteur telles que la norme ISO.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Comprendre les signatures électroniques dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Les signatures électroniques vous permettent d’améliorer la sécurité de vos BAT et de respecter les normes du secteur telles que la norme ISO.

Ce paramètre peut être rendu obligatoire ou non au niveau du compte. Si elle est obligatoire par défaut, elle est activée sur tous les BAT créés dans votre compte et ne peut pas être désactivée au niveau du BAT. Si ce paramètre n’est pas obligatoire par défaut, vous pourrez l’activer/le désactiver au niveau du BAT.

Pour plus d’informations, poursuivez votre lecture.

Lorsque le paramètre de signature électronique est activé sur un BAT, une boîte de signature électronique invite tout réviseur qui prend la décision sur le BAT de fournir son adresse électronique et son mot de passe.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## Signatures électroniques sur la page [!UICONTROL Détails du bon à tirer]

Si un réviseur prend sa décision en la sélectionnant sur la page [!UICONTROL Détails du bon à tirer] (1), une fenêtre contextuelle [!UICONTROL Signature électronique] s’affiche, lui demandant de saisir ses détails (2) et de confirmer sa décision (3).

La fenêtre contextuelle affiche le jeu de messages par défaut (le cas échéant) et le réviseur doit saisir son email et son mot de passe.

La fenêtre contextuelle [!UICONTROL Signature électronique] s’affiche dans la visionneuse de vérification et également sur la page [!UICONTROL Détails du bon à tirer] si le réviseur décide de prendre sa décision à partir de ce niveau.

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

Si l’option [!UICONTROL Authentification unique] est activée sur le BAT, les détails de l’email et du mot de passe ne s’afficheront pas dans la fenêtre contextuelle [!UICONTROL Signature électronique] lors de la prise d’une décision.

À la place, après avoir cliqué sur le bouton [!UICONTROL Confirmer] (4) dans cette fenêtre contextuelle, le réviseur est redirigé vers la page [!UICONTROL Connexion unique].

Après avoir saisi leurs informations d’identification d’authentification unique, le réviseur est automatiquement redirigé vers la page [!UICONTROL Détails du bon à tirer] (ou vers la [!UICONTROL Visionneuse de bon à tirer] si la décision est prise à partir de là).

![Electronic_Signature_SSO_-_Proof_Details_3.png{1](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> Si la décision est signée par voie électronique, l’**[!UICONTROL icône de signature]** (5) s’affiche en regard de la décision dans la section [!UICONTROL Workflow] de la page [!UICONTROL Détails du bon à tirer]. Si la décision n&#39;est pas modifiée par le validant mais par une autre personne disposant de droits de modification sur le BAT, cette personne ne sera pas invitée à signer électroniquement la décision et il n&#39;y aura pas d&#39;icône de signature à côté de la décision (6).

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Pour plus d’informations sur l’authentification unique, reportez-vous à la section [Connexion unique dans Workfront Proof](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

Pour plus d’informations sur la page Détails du bon à tirer, voir [Gérer les détails du bon à tirer dans [!DNL Workfront] Bon à tirer](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
