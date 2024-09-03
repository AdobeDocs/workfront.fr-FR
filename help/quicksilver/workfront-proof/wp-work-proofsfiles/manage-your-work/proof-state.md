---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Comprendre le statut d’une épreuve dans Workfront Proof
description: Dans  [!DNL Workfront Proof], les épreuves existent dans différents états. Ces états déterminent les actions que vous pouvez entreprendre sur l’épreuve, comme des commentaires ou des décisions.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 100%

---

# Comprendre le statut d’une épreuve dans Workfront Proof

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Dans [!DNL Workfront Proof], les épreuves existent dans différents états. Ces états déterminent les actions que vous pouvez entreprendre sur l’épreuve, comme des commentaires ou des décisions.

## Comprendre l’état des épreuves

Les quatre états sont les suivants :

* [Actif](#active)
* [Verrouillé](#locked)
* [Brouillon (zone de dépôt uniquement)](#draft-dropzone-only)
* [Soumis (zone de dépôt uniquement)](#submitted-dropzone-only)

### Actif {#active}

Les épreuves qui sont chargées vers [!DNL Workfront Proof] via la page Nouvelle épreuve ou la zone de dépôt apparaissent avec le statut Actif après leur traitement. Lorsqu’une épreuve est active, les personnes peuvent examiner, faire des commentaires et prendre des décisions sur l’épreuve.

>[!NOTE]
>
>Les épreuves chargées via la zone de dépôt apparaissent comme actives uniquement si l’option Activer l’épreuve lors de la soumission est activée. Si l’option n’est pas activée, vous devez activer manuellement l’épreuve.

Pour plus d’informations sur les paramètres de zone de dépôt, voir [Configurer la zone de dépôt dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Verrouillé {#locked}

Vous pouvez verrouiller une épreuve une fois que vous avez fini de la réviser. Verrouiller une épreuve signifie qu’il n’est plus possible de faire des commentaires ni de prendre des décisions sur l’épreuve, mais que l’épreuve peut toujours être ouverte.

Toute personne disposant de droits de modificaion sur l’épreuve peut la déverrouiller.

Pour plus d’informations sur les droits, voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>Les notifications par e-mail ne sont plus envoyées lorsqu’une épreuve est verrouillée. Par exemple, si une épreuve est verrouillée avant sa date d’échéance, aucun e-mail de notification n’est envoyé à la date d’échéance.

### Brouillon (zone de dépôt uniquement) {#draft-dropzone-only}

Lorsque vous envoyez une épreuve via la zone de dépôt, elle passe à l’état Brouillon avant que l’administrateur ou l’administratrice ne l’active. Lorsqu’elle se trouve dans la zone Brouillon, vous ne pouvez pas agir sur l’épreuve.

### Soumis (zone de dépôt uniquement) {#submitted-dropzone-only}

Une fois qu’un brouillon est activé par l’administrateur ou l’administratrice, votre épreuve apparaît comme Soumise dans la zone de dépôt. Une fois l’épreuve soumise, vous pouvez agir dessus.

## Afficher et modifier l’état de l’épreuve

Pour plus d’informations sur l’affichage d’une liste de toutes les épreuves dans un état spécifique, comme l’affichage de toutes les épreuves actives ou verrouillées, voir [Gérer des éléments sur la page Vues dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) dans l’article [Gérer des éléments sur la page Vues dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Accédez à votre tableau de bord [!DNL Workfront Proof].

   Pour plus d’informations, voir [Accéder à  [!DNL Workfront Proof]  à partir d’Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. Sur le **[!UICONTROL Tableau de bord]**, cliquez sur la flèche **[!UICONTROL Développer]** en regard de l’épreuve dont vous souhaitez afficher ou modifier l’état.

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   La section **[!UICONTROL Processus de workflow]** s’affiche.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Affichez l’**[!UICONTROL état]** dans le **[!UICONTROL Processus de workflow]**.

1. (Facultatif) Pour modifier l’état, placez pointez sur l’**[!UICONTROL état]** actuel puis cliquez sur le menu déroulant et sélectionnez un nouvel état.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
