---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: FAQ - Créer et partager des bons à tirer et des fichiers
description: Un BAT est un fichier statique, audio ou vidéo qui peut être consulté dans la visionneuse de vérification. Les validants ajoutés à un BAT disposent d'un ensemble d'outils leur permettant de faire des commentaires et des décisions sur le BAT.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: d5ffd576fcedf9b10dce5e5d5bd9245dd7f67ef8
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# FAQ - Créer et partager des bons à tirer et des fichiers

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

## Qu&#39;est-ce qu&#39;une preuve ?

### Réponse

Un BAT est un fichier statique, audio ou vidéo qui peut être consulté dans la visionneuse de vérification. Les validants ajoutés à un BAT disposent d&#39;un ensemble d&#39;outils leur permettant de faire des commentaires et des décisions sur le BAT.

## Quels types de fichiers sont pris en charge ?

### Réponse

Les bons à tirer peuvent être créés à partir de fichiers statiques, audio et vidéo. Vous ne pouvez pas charger de fichiers d’une taille supérieure à 4 Go. [!DNL Workfront] prend en charge plus de 150 types de fichiers (voir [Types et limites de taille de fichier de vérification pris en charge - Aperçu](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) pour obtenir une liste complète).

## Quelle est la différence entre un bon à tirer et un fichier ?

### Réponse

Lorsque vous transférez un fichier vers [!DNL Workfront Proof], le système stocke le fichier dans votre [!DNL Workfront Proof] compte . Lorsque vous le partagez, [!DNL Workfront Proof] Envoie à vos destinataires un lien sur lequel ils peuvent cliquer pour télécharger le fichier. Vous pouvez partager n’importe quel type de fichier.

Lorsque vous créez un BAT à partir d’un fichier dans lequel vous avez transféré [!DNL Workfront Proof], vous pouvez rendre le fichier disponible pour révision dans la visionneuse de vérification. Les validants reçoivent un email avec un lien vers le BAT. Lorsqu&#39;ils ouvrent le BAT, ils voient l&#39;image du BAT et peuvent y ajouter des commentaires et prendre des décisions. Vous pouvez créer des BAT à l’aide de fichiers de la liste des types de fichiers pris en charge. Vous pouvez également créer des BAT à l’aide d’URL pour les sites web et d’autres contenus web.

Pour obtenir la liste complète des types de fichiers pris en charge, voir [Types et limites de taille de fichier de vérification pris en charge - Aperçu](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## Comment créer un BAT ?

### Réponse

Vous pouvez créer des bons à tirer à partir de fichiers statiques, de fichiers audio, de fichiers vidéo et d’URL (voir ).

Pour créer un BAT dans le compte, vous devez être un utilisateur disposant du profil d’autorisation approprié (voir [[!UICONTROL Profils d’autorisations de BAT] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Si vous transférez plusieurs fichiers simultanément, vous créez plusieurs BAT que vous pouvez envoyer au même groupe de réviseurs à l’aide d’un seul email. Si votre organisation dispose d’un [!UICONTROL Entreprise] ou [!UICONTROL Illimitées] compte, vous pouvez combiner des fichiers en un seul BAT (voir [Création d’un BAT multi-page](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)).

## Que sont les rôles de BAT et les alertes par email ?

### Réponse

Les rôles de BAT définissent les actions qu’un réviseur doit effectuer sur un BAT. Il existe différentes options de rôle que vous pouvez utiliser pour les réviseurs lorsque vous créez un BAT, selon que vous souhaitez qu’ils puissent faire des commentaires, prendre des décisions, etc. Pour plus d’informations, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

Les alertes par email mettent à jour les validants sur l&#39;état d&#39;avancement d&#39;un BAT (elles sont différentes des nouvelles notifications de BAT et de BAT tardif). Vous pouvez sélectionner différentes options pour différents opérateurs validants, en fonction du rôle de chaque opérateur validant dans le BAT. Pour plus d’informations, voir [Créez un BAT avancé avec un [!UICONTROL Processus automatisé]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Puis-je créer un BAT à partir de plusieurs fichiers ?

### Réponse

La combinaison de plusieurs fichiers en un seul BAT est une fonctionnalité disponible sur [!UICONTROL Entreprise] et [!UICONTROL Illimitées] plans d’édition. Cette option est possible uniquement pour les fichiers statiques, et non pour les fichiers vidéo. Pour plus d’informations, voir  [Création d’un BAT multi-page](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Puis-je créer des bons à tirer à partir d’URL ?

### Réponse

Oui, vous pouvez créer des BAT à partir de sites web et d’autres contenus web. Lorsque vous ajoutez une URL pour créer un BAT, vous pouvez indiquer si vous souhaitez un BAT statique ou interactif :

* Dans un BAT interactif, les réviseurs peuvent naviguer et interagir comme ils le feraient habituellement avec le site web ou tout autre contenu web, comme les publicités avec diffusion vidéo ou audio en continu, [!DNL Flash] éléments dans une publicité, des animations de HTML et des bannières interactives. Pour plus d’informations, voir [Création d’un BAT pour le contenu interactif dans un fichier ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).
* Pour un BAT statique, [!DNL Workfront] prend une série de captures d’écran des pages et des sous-pages que vous spécifiez. Les liens hypertexte sont en direct dans le BAT, de sorte que vous pouvez tester s’ils mènent ou non à la destination correcte. Pour plus d’informations, voir [Créer un BAT statique pour un site web ou tout autre contenu web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

Vous pouvez ajouter plusieurs URL à la fois si vous les séparez par un espace. Notez que la combinaison n’est disponible que sur [!UICONTROL Entreprise] et [!UICONTROL Illimitées] plans d’édition.

## Les personnes qui n’ont pas de connexion peuvent-elles créer des bons à tirer dans mon compte ?

### Réponse

Vous avez besoin des informations de connexion pour créer des BAT directement dans un [!DNL Workfront Proof] compte .

## Que signifie partager une preuve ?

### Réponse

Le partage d&#39;un BAT permet aux opérateurs validants d&#39;y accéder afin de leur permettre d&#39;ajouter des commentaires et des annotations et de prendre des décisions sur le BAT. Les réviseurs invités accèdent aux BAT à partir de la notification électronique qu’ils reçoivent. Les réviseurs avec leurs propres [!DNL Workfront Proof] Le compte peut accéder aux bons à tirer sur le [!UICONTROL Tableau de bord].

## Comment partager une preuve ?

### Réponse

Lorsque vous créez un BAT, vous pouvez ajouter des réviseurs dans le [!UICONTROL Workflow] de la section [!UICONTROL Nouvelle preuve] page. Lorsque le BAT est prêt, [!DNL Workfront Proof] envoie un email aux opérateurs validants contenant un lien vers le BAT.

Si vous disposez de droits suffisants sur un BAT, vous pouvez utiliser la visionneuse de vérification, votre [!UICONTROL Tableau de bord], ou l’un des affichages de liste pour ajouter des réviseurs à un BAT existant (voir [Partage d’un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] Page dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

L’ajout de réviseurs est le moyen le plus courant de partager des bons à tirer. Si vous souhaitez explorer d’autres options disponibles, voir :

* [Partage de liens de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [Partage de l’URL publique dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [Abonnement à un BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Créer un BAT mini dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## Devez-vous être un utilisateur pour examiner un BAT ?

### Réponse

Non. Réviseurs invités (personnes sans [!DNL Workfront Proof] informations de connexion) peut accéder à un BAT à partir de la notification électronique du BAT qu’il reçoit. Vous pouvez partager une preuve avec autant d&#39;invités que vous voulez.

Il est possible de restreindre le partage des bons à tirer avec les personnes avec [!DNL Workfront Proof] informations de connexion. Cela ajoute une autre couche de sécurité à vos bons à tirer. Pour une sécurité renforcée, les administrateurs système des organisations avec [!UICONTROL Entreprise] et [!UICONTROL Illimitées] les plans peuvent configurer cette exigence pour tous les bons à tirer créés dans l’organisation.

Pour plus d’informations sur l’exigence d’une connexion, voir [Sécurité du BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Si votre entreprise requiert des réviseurs qu’ils signent des bons à tirer par voie électronique, ce qui nécessite la connexion à [!DNL Workfront Proof], les utilisateurs peuvent partager des bons à tirer uniquement avec les utilisateurs enregistrés. Cette option est disponible sur [!UICONTROL Entreprise] et [!UICONTROL Illimitées] plans d’édition. Pour plus d’informations, voir [Présentation des signatures électroniques dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## Puis-je définir un délai pour les opérateurs validants ?

### Réponse

Vous pouvez définir une date limite pour un nouveau BAT ou une nouvelle version du BAT lors de la création du BAT. Vous procédez comme suit dans la variable [!UICONTROL Workflow] de la section [!UICONTROL Nouvelle preuve] page. Si vous utilisez [!UICONTROL Processus automatisé], vous pouvez définir une date limite différente pour chaque étape de votre révision.

Vous pouvez également définir ou mettre à jour une date limite pour un BAT existant à l’aide de la fonction [!UICONTROL Détails du BAT] page. Pour plus d’informations, voir [Gérer les détails du BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Comment créer une nouvelle version de mon BAT ?

### Réponse

Les réviseurs demandent souvent des modifications dans leurs commentaires sur un BAT et souhaitent voir une nouvelle version du BAT. Vous pouvez créer de nouvelles versions d’un BAT. [!DNL Workfront Proof] mémorise les paramètres du BAT de la version précédente. Vous pouvez toujours modifier ces paramètres si vous devez effectuer une opération comme ajouter ou supprimer des réviseurs pour le BAT.

Vous devez partager chaque version avec les réviseurs spécifiques qui doivent la visualiser. Par exemple, si vous partagez uniquement la version 3 avec un réviseur, cette personne ne peut pas voir les versions 1 et 2. Les superviseurs et administrateurs de votre compte supervisent tous les projets du compte, afin qu’ils puissent visualiser et modifier toutes les versions du BAT.

Pour plus d’informations, voir .

## Puis-je partager des fichiers à l’aide de [!DNL Workfront Proof]?

### Réponse

Oui. Si vous souhaitez partager quelque chose avec d’autres personnes, mais que vous n’avez pas besoin d’eux pour le voir comme un bon à tirer (ou s’il s’agit d’un type de fichier non pris en charge par [!DNL Workfront Proof]), vous pouvez le charger en tant que fichier dans votre [!DNL Workfront Proof] compte . Comme pour les bons à tirer, vous pouvez organiser vos fichiers en dossiers, baliser les fichiers et ajouter un message personnalisé à l’e-mail de notification lorsque vous partagez le fichier. Pour plus d’informations, voir [Transfert de fichiers et de contenu web vers [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

Lorsque vos destinataires reçoivent la notification par e-mail d’un fichier que vous partagez, ils peuvent télécharger le fichier en cliquant sur le lien contenu dans la notification.

[!DNL Workfront Proof] les utilisateurs peuvent convertir des fichiers en BAT après les avoir enregistrés dans leur compte.

<!--Is there a limit-->
