---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Nouvel e-mail d’épreuve
description: Rendre cet article plus efficace pour PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 1030d4110fd5dabb3b5751387585cc66968c2326
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 3%

---

# Nouvel e-mail d’épreuve

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Lorsque vous créez un BAT ou une nouvelle version d&#39;un BAT, que vous ajoutez de nouvelles personnes à un BAT ou que vous ajoutez un workflow à un BAT, vous pouvez décider si vous souhaitez envoyer un email aux validants, comme expliqué dans ces articles :

* [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

L’e-mail que vos destinataires reçoivent s’appelle l’e-mail [!UICONTROL New Proof]. Seul le créateur du BAT et les utilisateurs autorisés à ajouter des validants à un BAT peuvent contrôler cet email. Les destinataires ne peuvent pas le désactiver.

L&#39;email Nouveau BAT contient :

* Votre message personnel (si vous choisissez d’en inclure un)
* Si vous envoyez toujours le même message personnalisé à vos réviseurs, il peut être préférable de l’enregistrer dans vos [!UICONTROL Paramètres personnels] sous l’onglet [!UICONTROL  Paramètres de vérification] . Pour plus d’informations, poursuivez votre lecture.
* Lien personnel vers le BAT
* **[!UICONTROL Afficher les détails]** permettant d’accéder à l’objet [!DNL Workfront] associé (tel un projet, une tâche ou un problème)
* Miniature de l’image de BAT
* Les détails du BAT suivants :

   * Nom de l&#39;épreuve
   * Numéro de version
   * Liste des validants et leur état d&#39;avancement sur le BAT
   * Un lien pour partager le BAT avec une autre personne

     Vous pouvez ainsi partager l’URL du BAT et/ou le lien de téléchargement du fichier d’origine. Cela ne vous permet pas d&#39;ajouter explicitement des validants au BAT, vous ne partagerez que l&#39;URL publique du BAT et le destinataire recevra un accès en lecture seule au BAT.

     Pour plus d’informations, voir [Partager un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) .

     Si vous ne souhaitez pas que ce lien apparaisse dans l&#39;email de votre destinataire, vous pouvez désactiver les paramètres de [!UICONTROL Partage public] sur le BAT.

     (Téléchargez le fichier d’origine et l’URL publique). Pour plus d’informations, voir [Gérer les détails du BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) .

## Journal d’activité

L&#39;envoi d&#39;un [!UICONTROL nouvel Bon à tirer] à un réviseur est consigné dans la section [!UICONTROL Activité] de la page [!UICONTROL Détails du bon à tirer]. Pour plus d’informations, voir [Gérer[!UICONTROL  les détails du bon à tirer] dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md). Vous pouvez vérifier si l&#39;email [!UICONTROL New Proof] a été activé au moment de la création d&#39;un BAT.

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Si les emails [!UICONTROL BAT fait] du créateur ou du propriétaire du BAT sont désactivés par défaut (dans leurs paramètres personnels), il ne recevra aucun [!UICONTROL BAT fait] ou [!UICONTROL Nouveau BAT] même si la case [!UICONTROL Notifier les personnes par email] est cochée sur la page Nouveau BAT. Pour plus d’informations, poursuivez votre lecture.
>* Si les notifications par e-mail sont désactivées par défaut dans les [!UICONTROL Paramètres du compte], le créateur/propriétaire du BAT ne recevra aucun email [!UICONTROL BAT fait] ou [!UICONTROL Nouveau BAT] même si cela est activé dans leurs paramètres personnels et que la case [!UICONTROL Notifier] par e-mail est cochée sur la page Nouveau BAT. Pour plus d’informations, [l’email [!UICONTROL BAT Made]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) et reportez-vous à la section .
>



## Activez l’email [!UICONTROL New Proof] et insérez un message personnalisé.

Vous pouvez indiquer si vous souhaitez envoyer une alerte par email aux réviseurs d’un BAT lors de sa création ou lorsque vous y ajoutez une personne.

* [Lorsque vous créez un BAT](#when-you-create-a-proof)
* [Lorsque vous ajoutez un validant à un BAT](#when-you-add-a-reviewer-to-a-proof)

### Lorsque vous créez un BAT {#when-you-create-a-proof}

Lorsque vous créez un BAT sur la page [!UICONTROL New BAT] , sous la section **[!UICONTROL Partager]** , vous pouvez choisir d&#39;envoyer des alertes par courrier électronique :

* Ici, vous pouvez décider si vous souhaitez [!UICONTROL  avertir les gens par email] (1). Si vous désélectionnez cette option, aucun de vos réviseurs ne reçoit d&#39;email pour lui signaler que le BAT est prêt pour la révision.
* Vous pouvez également inclure un message personnalisé dans la notification électronique (2).
* Si vous décidez d’ajouter votre propre message personnalisé, vous pourrez insérer un objet personnalisé (3) et un message dans le corps de l’email (4).
* Pour ignorer le message personnalisé, cliquez simplement sur le lien (5).

  >[!NOTE]
  >
  >Si vous envoyez toujours le même message personnalisé aux réviseurs, il peut être préférable de l&#39;enregistrer dans vos paramètres personnels sous l&#39;onglet [!UICONTROL Valeurs par défaut de la vérification]. Pour plus d’informations, poursuivez votre lecture.

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### Lorsque vous ajoutez un validant à un BAT {#when-you-add-a-reviewer-to-a-proof}

Vous pouvez choisir si un nouveau validant ajouté à un BAT existant sera informé du BAT (comme ci-dessus).

* Pour commencer, ajoutez de nouveaux réviseurs en cliquant sur le bouton **[!UICONTROL Partager cette version]** sur la page **[!UICONTROL Détails du bon à tirer]** (1).

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* Une boîte de dialogue s’affiche, dans laquelle vous pouvez ajouter de nouveaux réviseurs. Vous pouvez ensuite décider si vous souhaitez qu’ils soient avertis par email (2) et choisir d’ajouter un message personnalisé à l’email (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Si vous choisissez d’ajouter un message personnalisé, la zone se développe et vous pourrez insérer une ligne d’objet personnalisée (4) et du texte personnalisé dans le corps de l’email (5). Vous pouvez également ignorer le message personnalisé en cliquant sur le lien (6).

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
