---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Comprendre l’état de l’épreuve dans l’épreuve Workfront
description: Dans  [!DNL Workfront Proof], les bons à tirer existent dans différents états. Ces états déterminent les actions que vous pouvez entreprendre sur le BAT, comme des commentaires ou des décisions.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 3%

---

# Comprendre l’état de l’épreuve dans l’épreuve Workfront

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Dans [!DNL Workfront Proof], les bons à tirer existent dans différents états. Ces états déterminent les actions que vous pouvez entreprendre sur le BAT, comme des commentaires ou des décisions.

## Compréhension de l’état de preuve

Les quatre états sont les suivants :

* [Actif](#active)
* [Verrouillé](#locked)
* [Version préliminaire (zone de dépôt uniquement)](#draft-dropzone-only)
* [Envoyé (zone de dépôt uniquement)](#submitted-dropzone-only)

### Actif {#active}

Les bons à tirer qui sont chargés vers [!DNL Workfront Proof] via la page Nouveau bon à tirer ou la zone de dépôt apparaissent comme actifs une fois qu’ils ont été traités. Lorsqu’un BAT est actif, les utilisateurs peuvent examiner, faire des commentaires et prendre des décisions sur le BAT.

>[!NOTE]
>
>Les bons à tirer chargés via la zone de dépôt apparaissent comme actifs uniquement si l’option Activer le BAT lors de l’envoi est activée. Si l’option n’est pas activée, vous devez activer manuellement le BAT.

Pour plus d’informations sur les paramètres de zone de dépôt, voir [Configuration de la zone de dépôt dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Verrouillé {#locked}

Vous pouvez verrouiller un bon à tirer une fois que vous avez fini de le vérifier. Verrouiller un BAT signifie qu&#39;il n&#39;y a plus de commentaires ni de décisions à prendre sur le BAT, mais le BAT peut toujours être ouvert.

Tout utilisateur disposant de droits d&#39;édition sur le BAT peut le déverrouiller.

Pour plus d’informations sur les droits, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>Les notifications électroniques ne sont plus envoyées lorsqu’un BAT est verrouillé. Par exemple, si un BAT est verrouillé avant son expiration, aucun email de notification n’est envoyé à l’expiration du délai.

### Version préliminaire (zone de dépôt uniquement) {#draft-dropzone-only}

Lorsque vous envoyez un BAT via la zone de dépôt, il passe à l’état Brouillon avant que l’administrateur ne l’active. Lorsqu&#39;il se trouve dans la zone de brouillon, vous ne pouvez pas agir sur le BAT.

### Envoyé (zone de dépôt uniquement) {#submitted-dropzone-only}

Une fois qu’un brouillon est activé par l’administrateur, votre BAT apparaît comme Envoyé dans la zone de dépôt. Une fois envoyé, vous pouvez agir sur le BAT.

## Affichage et modification de l’état du BAT

Pour plus d’informations sur l’affichage d’une liste de tous les bons à tirer dans un état spécifique, comme l’affichage de tous les bons à tirer actifs ou verrouillés, voir [Gestion des éléments sur la page des vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) de l’article [Gérer les éléments sur la page des vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Accédez à votre tableau de bord [!DNL Workfront Proof].

   Pour plus d’informations, voir [Accès [!DNL Workfront Proof]  depuis Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. Sur le **[!UICONTROL tableau de bord]**, cliquez sur la flèche **[!UICONTROL Développer]** située en regard du BAT dont vous souhaitez afficher ou modifier l’état.

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   La section **[!UICONTROL Processus de workflow]** s’affiche.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Affichez l’ **[!UICONTROL état]** dans le **[!UICONTROL processus de workflow]**.

1. (Facultatif) Pour modifier l’état, placez le pointeur de la souris sur l’état actuel **[!UICONTROL State]** et cliquez sur le menu déroulant, puis sélectionnez un nouvel état.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
