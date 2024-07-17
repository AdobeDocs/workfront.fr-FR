---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Réviser une épreuve dans Basecamp Classic
description: Basecamp est un outil de gestion de projet en ligne développé par 37signals. Si vous utilisez Basecamp pour la gestion de projet, vous pouvez offrir à votre équipe de projet des outils de révision et d’approbation plus riches en utilisant [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b14f33dc-e059-4ee2-a429-9f1852a2b9bb
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# Vérification d’un bon à tirer dans [!DNL Basecamp] Classic

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Basecamp] est un outil de gestion de projet en ligne développé par [!DNL 37signals]. Si vous utilisez [!DNL Basecamp] pour la gestion de projet, vous pouvez offrir à votre équipe de projet des outils de révision et d&#39;approbation plus riches en utilisant [!DNL Workfront Proof].

## Présentation des révisions des bons à tirer dans [!DNL Basecamp Classic]

Lorsqu&#39;il est intégré à [!DNL Workfront Proof], [!DNL Basecamp] permet aux utilisateurs d&#39;effectuer les opérations suivantes avec des bons à tirer :

* Les utilisateurs peuvent consulter et approuver les bons à tirer dans [!DNL Basecamp Classic].
* Les utilisateurs disposent d’outils de révision facilement disponibles.
* Les équipes d’examen de projet reçoivent un message dans [!DNL Basecamp] avec un mini BAT pour révision et approbation.
* Les utilisateurs peuvent passer à un BAT de page entière pour révision et approbation.
* Les utilisateurs peuvent ajouter des commentaires et des annotations aux mini-bons à tirer et aux bons à tirer.
* Une fois qu’un commentaire a reçu une réponse, il ne peut pas être modifié/supprimé. Pour plus d’informations sur les commentaires, voir [Commentaire sur un BAT](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md).
* Les réviseurs peuvent répondre aux balises et effectuées par d’autres réviseurs. Pour plus d’informations sur les commentaires, voir [Commentaire sur un BAT](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md).
* Les utilisateurs sont avertis lorsqu’une nouvelle version du BAT est disponible.
* Les utilisateurs qui ne sont pas [!DNL Workfront Proof] peuvent travailler sur un BAT dans [!DNL Basecamp].

## Affichage d’un BAT via l’e-mail de notification

Si vous liez un BAT à [!DNL Basecamp], [!DNL Workfront Proof] envoie un email de notification de BAT (1) à tous les réviseurs, contenant les informations suivantes :

* **Détails du bon à tirer** (2) : affiche des informations sur le bon à tirer. Les informations affichées dépendent de la manière dont votre administrateur Workfront a configuré Basecamp.
* **[!UICONTROL Atteindre le BAT] lien** (3) : ouvre le BAT dans Workfront.
* **[!DNL Basecamp]URL** (4) : ouvre le BAT dans Basecamp. Si des réviseurs non basés sur un tampon sont ajoutés au BAT, leur notification électronique n’inclut pas le lien Basecamp .
* **[!UICONTROL Proof progress]** (5) : répertorie les étapes de validation et affiche les indicateurs de progression du BAT.
* **[!UICONTROL Stage]** (6) : répertorie les réviseurs et leur progression individuelle.

![ Basecamp_ProofHQ_email_notification1__1_.png{1](assets/basecamp-proofhq-email-notification1--1--350x202.png)

Pour ouvrir le BAT à partir de la notification électronique :

1. Pour ouvrir le BAT dans [!DNL Workfront Proof], cliquez sur **[!UICONTROL Atteindre le BAT]**.\
   Ou\
   Pour ouvrir le BAT dans [!DNL Basecamp], cliquez sur l’URL répertoriée dans le champ **[!UICONTROL [!DNL Basecamp]URL]** .\
   Pour plus d’informations sur la révision d’un BAT dans [!DNL Basecamp Classic], reportez-vous à la section [Vérification d’un BAT dans [!DNL Basecamp]](#reviewing-a-proof-in-basecamp) de cet article.

## Affichage du BAT via le message [!DNL Basecamp Classic]

Vous pouvez accéder à un BAT à partir d’un message [!DNL Basecamp Classic].

1. Dans [!DNL Basecamp], accédez à la page de votre projet (1).\
   ![ Basecamp_Classic_messages_1.png](assets/basecamp-classic-messages-1-350x120.png)

1. Cliquez sur le message correspondant au BAT que vous souhaitez ouvrir. (2)\
   Le message pour le BAT s&#39;ouvre, affichant un mini BAT. Le nom du BAT s&#39;affiche en haut de la fenêtre du message (3).\
   Vous pouvez afficher le BAT de miniature dans [!DNL Basecamp Classic] ou dans [!DNL Workfront Proof].\
   ![ Basecamp_Classic_messages_2.png](assets/basecamp-classic-messages-2-350x501.png)

1. Pour afficher le BAT en mode plein écran dans [!DNL Workfront proof], cliquez sur l’URL indiquée au-dessus du BAT (4).
1. (Conditionnel) Si vous n’êtes pas connecté à votre compte [!DNL Workfront Proof] dans l’une de vos fenêtres de navigateur, connectez-vous pour consulter le BAT :

   1. Cliquez sur **[!UICONTROL Se connecter]** (5) au-dessus du BAT.
   1. Saisissez votre adresse électronique (6).\

      Vous devez utiliser la même adresse électronique que celle utilisée lors de l’ajout du BAT.
   1. Cliquez sur **[!UICONTROL Suivant]**.
   1. Saisissez votre mot de passe [!DNL Workfront Proof] (7).\

      Ou\
      Si vous ne disposez pas d’un compte [!DNL Workfront Proof], saisissez un nom public à afficher.\
      Vous pouvez sélectionner &quot;[!UICONTROL Mémoriser]&quot; afin de n’avoir à saisir vos détails qu’une seule fois.

1. Pour passer en revue le BAT, passez à la section [Vérification d’un BAT dans [!DNL Basecamp]](#reviewing-a-proof-in-basecamp).

>[!NOTE]
>
> La zone de commentaire affichée sous le mini BAT sur la page du message s&#39;applique uniquement au message lui-même. Pour envoyer des commentaires de révision, vous devez utiliser le bouton de l’icône de commentaires en haut du mini-BAT ou le bouton [!UICONTROL Commentaires] plus grand en haut du BAT en page entière. Pour plus d’informations, voir [Vérification d’un bon à tirer dans [!DNL Basecamp]](#reviewing-a-proof-in-basecamp).

## Vérification d’un bon à tirer dans [!DNL Basecamp]

Le mini BAT de [!DNL Basecamp] vous fournit les outils que vous devez ajouter et pour [ prendre une décision sur un BAT dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) sur le BAT. Tous les utilisateurs affectés au projet voient vos balises et commentaires et peuvent répondre avec leurs propres commentaires en temps réel.

Lorsque vous ouvrez le BAT, le BAT s’affiche dans la fenêtre [!UICONTROL proofing] (1) et le nom du BAT et du numéro de version s’affiche dans le coin supérieur gauche (2).

![Basecamp_Classic_miniproof.png](assets/basecamp-classic-miniproof-350x350.png)

Pour vérifier le BAT :

1. Pour ajouter un commentaire, cliquez sur [!UICONTROL Commentaire] (3) en haut du BAT, puis saisissez votre commentaire.\
   Il n’est pas nécessaire d’envoyer une réponse au message [!DNL Basecamp], car les commentaires et [ prennent une décision sur un BAT enregistré dans la visionneuse de vérification](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) du BAT (similaire à la révision d’un BAT dans [!DNL Workfront Proof]).

1. Pour ajouter une décision, cliquez sur Décision (3) en haut du BAT, puis sélectionnez votre décision d’approbation.\
   Pour plus d’informations sur la prise de décisions sur un BAT, voir [Prendre une décision sur un BAT dans la visionneuse de vérification de performance](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

D’autres fonctionnalités de la fenêtre du BAT sont les suivantes :

* **[!UICONTROL Menus d’action]** (4) : permet de sélectionner les paramètres du BAT.
* **[!UICONTROL Bouton Plein écran]** (5) : permet de basculer entre le mode Plein écran et le mode BAT.
* **[!UICONTROL Barre latérale]** (6) : vous permet de développer ou de réduire l’affichage du BAT.
* **[!UICONTROL Nom d’utilisateur]** (7) : affiche votre nom d’utilisateur si vous êtes connecté à Workfront.
* **[!UICONTROL Outils de zoom]** (8) : permet d’agrandir une zone du BAT.
* **[!UICONTROL Outils de navigation sur les pages]** (9) : permet de faire défiler les pages vers d’autres pages du BAT.

<!--For more information on reviewing proofs, see [Legacy proofing viewer Overview](../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/legacy-proofing-viewer.md).-->
