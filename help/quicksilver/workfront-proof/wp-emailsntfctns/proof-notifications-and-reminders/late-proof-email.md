---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Email de retard
description: L'email Bon à tirer est envoyé aux destinataires lorsqu'un BAT se rapproche de la date limite d'envoi ou atteint la date limite d'envoi. Ces types d’emails ne peuvent pas être désactivés au niveau du BAT, mais peuvent être configurés au niveau du compte et des paramètres personnels de l’utilisateur.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL BAT tardif] email

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Le [!UICONTROL Preuve tardive] l&#39;email est envoyé aux destinataires lorsqu&#39;un BAT se rapproche de la date limite d&#39;envoi ou atteint la date limite d&#39;envoi. Ces types d’emails ne peuvent pas être désactivés au niveau du BAT, mais peuvent être configurés au niveau du compte et des paramètres personnels de l’utilisateur.

* [!UICONTROL BAT tardif] les emails sont automatiquement envoyés aux validants lorsqu&#39;un BAT arrive à échéance et que des révisions ou décisions n&#39;ont pas été prises.

   Ces emails sont activés par défaut et ne peuvent pas être ajustés pour l’ensemble des comptes, mais les utilisateurs peuvent les désactiver dans leurs paramètres de Bon à tirer par défaut.

* Les emails à risque sont envoyés aux opérateurs validants lorsqu&#39;un BAT est proche de la date limite d&#39;envoi. Ils sont désactivés par défaut et peuvent être activés dans la variable [!UICONTROL Paramètres du compte]. Une fois activés, ils peuvent également être ajustés dans la variable [!UICONTROL Vérification des paramètres par défaut].

Ces notifications ne peuvent pas être personnalisées.

Les personnes qui seront averties sont les suivantes :

* Le propriétaire, uniquement lorsque [!UICONTROL Email] l’alerte lorsque les bons à tirer sont en retard est activée dans la variable [!UICONTROL Paramètres par défaut de vérification du propriétaire].
* Tout approbateur qui n’a pas encore pris sa décision sur le BAT. Pour plus d’informations sur les décisions, voir [Prendre une décision sur un BAT dans la visionneuse de vérification](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Si les notifications électroniques sont désactivées par défaut dans la variable [!UICONTROL Paramètres du compte], non [!UICONTROL BAT tardif] Les emails seront envoyés même si les validants et les approbateurs n&#39;ont pas encore soumis leurs commentaires et décisions. Vous pouvez également désactiver [!UICONTROL BAT tardif] emails dans les valeurs par défaut de la vérification.

Tenez compte des points suivants concernant les notifications de BAT :

* Votre [!DNL Workfront] administrateur ou [!DNL Workfront Proof] L’administrateur peut inclure le logo de votre entreprise dans vos notifications par e-mail, comme expliqué à la section [Marque [!DNL Workfront Proof] site](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Si vous devez partager plusieurs BAT avec les mêmes réviseurs et que vous ne souhaitez pas qu’ils reçoivent plusieurs emails, vous pouvez les télécharger simultanément. Tous les validants reçoivent un email détaillant tous les BAT et une URL personnelle pour chaque BAT.

   >[!NOTE]
   >
   >Le créateur des BAT reçoit une [!UICONTROL Preuve faite] email pour chacun des BAT créés. Pour plus d’informations, voir [Le [!UICONTROL Bon à tirer] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Si vous, ou vos réviseurs, ne recevez pas de notification électronique attendue, reportez-vous à la section  [Configurer [!DNL Workfront Proof] emails pour éviter les filtres anti-spam](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
