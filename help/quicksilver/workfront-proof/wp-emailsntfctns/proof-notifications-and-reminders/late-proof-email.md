---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: E-mail d’épreuve tardif
description: L'email Bon à tirer est envoyé aux destinataires lorsqu'un BAT se rapproche de la date limite d'envoi ou atteint la date limite d'envoi. Ces types d’emails ne peuvent pas être désactivés au niveau du BAT, mais peuvent être configurés au niveau du compte et des paramètres personnels de l’utilisateur.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL  Email de retard ]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

L&#39;email [!UICONTROL BAT tardif] est envoyé aux destinataires lorsqu&#39;un BAT se rapproche de l&#39;échéance ou atteint l&#39;échéance. Ces types d’emails ne peuvent pas être désactivés au niveau du BAT, mais peuvent être configurés au niveau du compte et des paramètres personnels de l’utilisateur.

* [!UICONTROL Les emails de retard de BAT] sont automatiquement envoyés aux réviseurs lorsqu’un BAT atteint son délai d’expiration et que toutes les révisions ou décisions n’ont pas été prises.

  Ces emails sont activés par défaut et ne peuvent pas être ajustés pour l’ensemble des comptes, mais les utilisateurs peuvent les désactiver dans leurs paramètres de Bon à tirer par défaut.

* Les emails à risque sont envoyés aux opérateurs validants lorsqu&#39;un BAT est proche de la date limite d&#39;envoi. Ils sont désactivés par défaut et peuvent être activés dans les [!UICONTROL Paramètres du compte]. Une fois activés, ils peuvent également être ajustés dans les [!UICONTROL valeurs par défaut du correctif].

Ces notifications ne peuvent pas être personnalisées.

Les personnes qui seront averties sont les suivantes :

* Le propriétaire, uniquement lorsque l’alerte [!UICONTROL Email] lorsque les bons à tirer sont en retard, est activé dans les [!UICONTROL  valeurs par défaut de vérification du propriétaire].
* Tout approbateur qui n’a pas encore pris sa décision sur le BAT. Pour plus d’informations sur les décisions, voir [Prise d’une décision sur un BAT dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Si les notifications par e-mail sont désactivées par défaut dans les [!UICONTROL Paramètres du compte], aucun [!UICONTROL  e-mail de retard de BAT] ne sera envoyé même si les réviseurs et les approbateurs n&#39;ont pas encore soumis leurs commentaires et décisions. Vous pouvez également désactiver les [!UICONTROL BAT tardif] dans les valeurs par défaut de la vérification.

Tenez compte des points suivants concernant les notifications de BAT :

* Votre administrateur [!DNL Workfront] ou [!DNL Workfront Proof] peut inclure le logo de votre entreprise dans vos notifications par e-mail, comme expliqué dans la section [Marque du  [!DNL Workfront Proof] site](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Si vous devez partager plusieurs BAT avec les mêmes réviseurs et que vous ne souhaitez pas qu’ils reçoivent plusieurs emails, vous pouvez les télécharger simultanément. Tous les validants reçoivent un email détaillant tous les BAT et une URL personnelle pour chaque BAT.

  >[!NOTE]
  >
  >Le créateur des BAT reçoit un email [!UICONTROL BAT fait] distinct pour chacun des BAT créés. Pour plus d’informations, voir le [courrier électronique [!UICONTROL BAT fait]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Si vous ou vos réviseurs ne recevez pas de notification par e-mail attendue, consultez la section [Configuration [!DNL Workfront Proof] des emails pour éviter les filtres de spam](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
