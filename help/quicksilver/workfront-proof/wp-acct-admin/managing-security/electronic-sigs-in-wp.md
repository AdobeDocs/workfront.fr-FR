---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Comprendre les signatures électroniques dans  [!DNL Workfront Proof]
description: L’emploi de signatures électroniques permet de sécuriser vos documents et de répondre aux exigences de normes industrielles comme la norme ISO.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 100%

---

# Comprendre les signatures électroniques dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

L’emploi de signatures électroniques permet de sécuriser vos documents et de répondre aux exigences de normes industrielles comme la norme ISO.

Ce paramètre peut être rendu obligatoire ou non au niveau du compte. S’il est obligatoire par défaut, il est activé pour toutes les épreuves créées dans votre compte et ne peut pas être désactivé au niveau de l’épreuve. Si ce paramètre n’est pas obligatoire par défaut, vous pourrez l’activer/le désactiver au niveau de l’épreuve.

Pour plus d’informations, voir :

Avec l’activation de la signature électronique sur un document, une zone de signature électronique invite toute personne qui prend une décision sur l’épreuve à entrer son e-mail et son mot de passe.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## Signatures électroniques sur la page [!UICONTROL Détails de l’épreuve]

Si une personne chargée de la révision prend une décision en la sélectionnant sur la page [!UICONTROL Détails de l’épreuve] (1), une fenêtre contextuelle [!UICONTROL Signature électronique] apparaît, lui demandant de saisir ses coordonnées (2) et de confirmer sa décision (3).

La fenêtre pop-up affiche le jeu de messages par défaut (le cas échéant) et la personne chargée de la révision doit saisir son e-mail et son mot de passe.

La [!UICONTROL signature électronique] de la personne chargée de la révision s’affiche dans la visionneuse de relecture et sur la page [!UICONTROL Détails de l’épreuve] à condition que la décision soit prise à ce niveau.

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

Si l’option [!UICONTROL Authentification unique] est activée sur l’épreuve, les détails de son e-mail et de son mot de passe ne seront pas affichés dans la fenêtre pop-up [!UICONTROL Signature électronique] lors de la prise de décision.

Après avoir cliqué sur le bouton [!UICONTROL Confirmer] (4) dans cette fenêtre pop-up, la personne chargée de la révision est redirigée vers la page d’[!UICONTROL authentification unique].

Après avoir saisi ses identifiants d’authentification unique, la personne chargée de la révision sera automatiquement redirigée vers la page [!UICONTROL Détails de l’épreuve] (ou vers la [!UICONTROL visionneuse de relecture] si la décision est prise à partir de cette page).

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> Si la décision est signée électroniquement, l’**[!UICONTROL icône de signature]** (5) apparaît à côté de la décision dans la section [!UICONTROL Workflow] de la page [!UICONTROL Détails de l’épreuve]. Dans le cas où une autre personne, autorisée à modifier le document, intervient pour changer la décision sans être la personne chargée de la révision, aucune demande de signature électronique ne sera faite et l’icône de signature ne figurera pas à côté de la décision.

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Pour plus d’informations sur l’authentification unique, consultez la section [Authentification unique dans Workfront Proof](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

Pour plus d’informations sur la page des détails de l’épreuve, consultez la section [Gérer les détails de l’épreuve dans  [!DNL Workfront]  Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
