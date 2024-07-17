---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Configuration des paramètres de BAT dans [!DNL Workfront Proof]
description: Vous pouvez configurer un BAT que vous créez ou modifiez dans des BAT.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%

---

# Configuration des paramètres de BAT dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez configurer un BAT que vous créez ou modifiez de l’une des manières suivantes :

>[!NOTE]
>
>Vous pouvez configurer ces paramètres pour tous les nouveaux BAT que vous créez. Pour plus d’informations, poursuivez votre lecture.

## Verrouillage du BAT lors de la dernière décision

Vous pouvez définir un état de BAT à verrouiller lorsque l’approbateur final prend sa décision. Cela s’avère utile si vous souhaitez vous assurer que vos réviseurs ne pourront pas revenir au BAT et ajouter des commentaires supplémentaires ou modifier leurs décisions.

1. Créez un BAT, comme décrit dans la section [Générer des BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Ouvrez la page Détails du bon à tirer pour un BAT existant, comme décrit dans la section [Gérer les détails du bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Pour un nouveau BAT, sous **[!UICONTROL Paramètres du BAT]**, sélectionnez **[!UICONTROL Verrouiller le BAT lorsque toutes les décisions requises sont prises]**.\
   Ou\
   Pour un BAT existant, sous **[!UICONTROL Paramètres]**, sélectionnez **[!UICONTROL Verrouiller le BAT lorsque toutes les décisions sont prises]**.

Pour plus d’informations sur les décisions, voir [Prise d’une décision sur un BAT dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Identification requise de tous les utilisateurs qui vérifient le BAT

[!DNL Workfront Proof] est une des choses géniales que n&#39;importe qui peut passer en revue un bon à tirer, vous n&#39;avez pas besoin d&#39;avoir votre propre [!DNL Workfront Proof] pour le faire. Les destinataires reçoivent un email avec une URL personnelle qui les amène directement à la page du BAT, sans qu&#39;ils aient à se connecter à [!DNL Workfront Proof].

Cependant, si vous avez besoin de niveaux de sécurité supérieurs pour votre processus de révision et d’approbation, vous pouvez utiliser l’option de connexion requise au BAT. Cela signifie que seuls [!DNL Workfront Proof] utilisateurs peuvent être ajoutés au BAT. Et ils doivent saisir leur email et leur mot de passe avant d&#39;y accéder.

>[!NOTE]
>
>* *Pour que quelqu&#39;un se connecte au BAT (lorsque la connexion requise a été activée), il doit avoir été ajouté au BAT.*
>* *Si la connexion requise est activée, les abonnements ne peuvent pas être activés.*

Pour exiger la connexion de tous les utilisateurs qui vérifient le BAT :

1. Créez un BAT, comme décrit dans la section [Générer des BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Ouvrez la page Détails du bon à tirer pour un BAT existant, comme décrit dans la section [Gérer les détails du bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Pour un nouveau BAT, sous **[!UICONTROL Paramètres du BAT]**, sélectionnez **[!UICONTROL Require login]**.\
   Ou\
   Pour un BAT existant, sous **[!UICONTROL Settings]**, sélectionnez **[!UICONTROL Login required]**.

## Exiger une seule décision pour le BAT

Ce paramètre est utile lorsque vous avez simplement besoin d’une personne d’un groupe, d’un service ou d’une entreprise pour prendre une décision sur le BAT.

Même si vous attribuez le rôle d’approbateur ou de réviseur et d’approbateur à plusieurs personnes, une fois qu’une personne prend une décision sur un BAT, le statut du BAT est mis à jour (conformément à la décision prise). Pour plus d’informations sur l’état du BAT, voir [Affichage de l’état et de l’état d’un BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Créez un BAT, comme décrit dans la section [Générer des BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Ouvrez la page Détails du bon à tirer pour un BAT existant, comme décrit dans la section [Gérer les détails du bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Pour un nouveau BAT, sous **[!UICONTROL Workflow]**, sélectionnez **[!UICONTROL Exiger une seule décision pour cette étape]**.\
   Ou\
   Pour un BAT existant, sous **[!UICONTROL Paramètres]**, sélectionnez **[!UICONTROL Une seule décision requise]**.

Pour plus d’informations sur les décisions, voir [Prise d’une décision sur un BAT dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Exiger la signature électronique des décisions

Vous pouvez exiger une signature électronique de tout réviseur qui prend une décision sur le BAT pour fournir son email et son mot de passe. Lorsqu’un réviseur affiche une invite de décision lui demandant de saisir son adresse électronique et son mot de passe et de confirmer sa décision. Pour plus d’informations, voir [Comprendre les signatures électroniques dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Créez un BAT, comme décrit dans la section [Générer des BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Ouvrez la page Détails du bon à tirer pour un BAT existant, comme décrit dans la section [Gérer les détails du bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Pour un nouveau BAT, sous **[!UICONTROL Paramètres du BAT]**, sélectionnez **[!UICONTROL Exiger la signature électronique des décisions]**.\
   Ou\
   Pour un BAT existant, sous **[!UICONTROL Paramètres]**, sélectionnez **[!UICONTROL Exiger que les décisions soient signées électroniquement]**.

Pour plus d&#39;informations sur les décisions, voir [Configuration des options de décision d&#39;approbation dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Interdire aux utilisateurs de télécharger le fichier original

Vous pouvez empêcher les validants sur un BAT de télécharger le fichier d&#39;origine à partir duquel un BAT a été créé.

1. Créez un BAT, comme décrit dans la section [Générer des BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Ouvrez la page Détails du bon à tirer pour un BAT existant, comme décrit dans la section [Gérer les détails du bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Pour un nouveau BAT, sous **[!UICONTROL Paramètres du BAT]**, désélectionnez **[!UICONTROL Télécharger le fichier d’origine]**.\
   Ou\
   Pour un BAT existant, sous **[!UICONTROL Settings]**, sélectionnez **[!UICONTROL Download of original file]**.

## Autoriser d’autres utilisateurs à s’abonner au BAT

L’abonnement est un paramètre avancé qui fonctionne avec l’URL du bon à tirer et le BAT.

Par défaut, les personnes qui n&#39;ont pas été spécifiquement ajoutées au BAT et qui utilisent l&#39;URL du BAT ou le BAT pour y accéder ne peuvent afficher que le BAT en mode Lecture seule. Les personnes qui sont déjà réviseurs sur le BAT peuvent se connecter à l’aide de leur adresse électronique. Pour plus d’informations, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

L&#39;inscription au BAT permet aux personnes qui n&#39;ont pas été explicitement ajoutées au BAT de s&#39;inscrire au BAT (c&#39;est-à-dire de s&#39;ajouter au BAT). Le rôle et l’alerte par courrier électronique que vous sélectionnez leur seront alors attribués dans les paramètres d’abonnement.

Si l&#39;inscription a été activée sur un BAT, les champs ci-dessous deviennent actifs :

* **[!UICONTROL Validation d’abonné requise]** - L’abonné doit cliquer sur un lien dans un email pour accéder à un BAT\
   Cette option signifie que la personne qui s&#39;abonne n&#39;aura pas un accès immédiat au BAT, mais qu&#39;elle aura un lien vers le BAT dans un email. La validation des abonnés a pour but de s’assurer que la personne a saisi une adresse électronique correcte à laquelle elle a accès.

* **[!UICONTROL Rôle par défaut pour les nouveaux abonnés]** : il s’agit du rôle de BAT par défaut qui sera attribué à tous les réviseurs qui s’abonnent au BAT.
* **[!UICONTROL Alerte par défaut pour les nouveaux abonnés]** : il s’agit de l’alerte par défaut qui sera attribuée à tous les réviseurs qui s’abonnent au BAT.

Voir aussi [S’abonner à un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

Pour permettre à d’autres utilisateurs de s’abonner à un BAT :

1. Créez un BAT, comme décrit dans la section [Générer des BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   Ou\
   Ouvrez la page Détails du bon à tirer pour un BAT existant, comme décrit dans la section [Gérer les détails du bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Pour un nouveau BAT, sous **[!UICONTROL Paramètres du BAT]**, désélectionnez **[!UICONTROL Abonnez-vous au BAT via une URL publique ou un code incorporé]**.\
   Ou\
   Pour un BAT existant, sous **[!UICONTROL Settings]**, sélectionnez **[!UICONTROL Subscription]**.
