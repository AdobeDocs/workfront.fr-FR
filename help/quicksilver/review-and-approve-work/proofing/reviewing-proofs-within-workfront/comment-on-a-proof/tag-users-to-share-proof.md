---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Baliser des utilisateurs et utilisatrices pour partager une épreuve
description: Lorsque vous commentez un BAT dans la visionneuse de BAT, vous pouvez marquer d’autres utilisateurs pour attirer leur attention sur votre commentaire par e-mail et les ajouter au workflow du BAT.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 8%

---

# Baliser des utilisateurs et utilisatrices pour partager une épreuve

Lorsque vous commentez un BAT dans la visionneuse de BAT, vous pouvez marquer d’autres utilisateurs pour attirer leur attention sur votre commentaire par e-mail et les ajouter au workflow du BAT.

Lors du balisage des utilisateurs dans des commentaires sur un BAT, les utilisateurs que vous pouvez baliser peuvent varier en fonction de divers facteurs, tels que les permissions utilisateur individuelles et votre appartenance à l’organisation :

* Si vous êtes le créateur, le propriétaire ou si des autorisations spécifiques sont activées, vous pouvez baliser les utilisateurs en dehors du workflow de BAT et partager le BAT avec eux.
* Si vous avez été ajouté au BAT en tant qu’utilisateur externe et que vous êtes membre d’un autre environnement avec un compte de BAT différent, vous pouvez baliser uniquement ces utilisateurs de votre environnement d’origine. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Conditions d’accès {#access-requirements}

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Rôle de BAT</td> 
   <td>Auteur, modérateur</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Administrateur de superviseur</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

## Baliser des utilisateurs et utilisatrices pour partager une épreuve

Les utilisateurs disposant du rôle Profil d’autorisation de BAT ou Bon à tirer décrits dans la section [Exigences d’accès](#access-requirements) ci-dessus peuvent baliser les utilisateurs pour partager un BAT par défaut. Vous pouvez également baliser les utilisateurs pour partager un BAT, quel que soit le rôle Profil d’autorisation de BAT ou Bon à tirer si vous êtes le propriétaire ou le créateur du BAT. Vous pouvez permettre aux utilisateurs disposant de rôles Profil d’autorisation de BAT ou Bon à tirer (BAT) inférieurs de marquer les utilisateurs pour qu’ils partagent un BAT lors de la création d’un BAT. Pour plus d&#39;informations, consultez la section [Configurer le workflow et ajouter des réviseurs](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) de l&#39;article [Créer un BAT avancé avec un workflow de base](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) .

>[!NOTE]
>
>Vous ne pouvez baliser un collaborateur externe à l’aide de son adresse électronique que si l’une des conditions suivantes est vraie :>
>* Un utilisateur du compte Workfront de votre entreprise a précédemment ajouté l’adresse électronique du collaborateur à un BAT.
>* Le collaborateur a déjà utilisé l’adresse électronique pour s’abonner à un BAT dans le compte Workfront de votre entreprise.
>

Pour marquer quelqu&#39;un et partager un bon à tirer dans un commentaire :

1. Lorsque vous commentez un BAT, tapez un signe @ suivi du nom ou de l’adresse électronique de la personne. Lorsque vous commencez à saisir du texte, les noms disponibles apparaissent dans une liste déroulante.
1. Sélectionnez le nom de la personne qui apparaîtra dans la liste déroulante.

   >[!TIP]
   >
   >Si vous souhaitez fermer la liste déroulante sans sélectionner d’utilisateur, vous pouvez appuyer sur la touche **Echap** ou cliquer n’importe où en dehors de la liste.

1. Répétez les étapes 1 à 2 pour tous les autres utilisateurs que vous souhaitez baliser dans le commentaire.
1. Terminez le commentaire, puis cliquez sur **Post**.
1. (Conditionnel) Si vous avez balisé une personne qui n’a pas encore été ajoutée au BAT, spécifiez un paramètre **Rôle BAT** et **Alertes par e-mail** pour chaque utilisateur répertorié dans la zone qui s’affiche, puis cliquez sur **Ajouter des personnes et publier un commentaire**.

   ![](assets/add-people-to-proof-350x220.png)

   Pour plus d’informations sur les rôles de BAT, voir . Pour plus d’informations sur les alertes par courrier électronique de BAT, reportez-vous à la section de l’article [ Configuration des paramètres de notification électronique dans Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Si le BAT comporte un workflow automatisé, les utilisateurs que vous marquez sont ajoutés à l’étape dans laquelle vous vous trouvez. Pour plus d’informations, voir [Présentation du processus automatisé](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Toute personne que vous marquez reçoit un email de notification à propos de votre commentaire de BAT, quels que soient les paramètres d’alerte par email de BAT qu’elle utilise :

   * Si l’utilisateur reçoit un email de résumé quotidien ou horaire, Workfront envoie la notification séparément et inclut des informations sur votre commentaire de BAT dans l’email de résumé.
   * Si l’utilisateur reçoit des alertes pour toute l’activité ou pour les réponses à ses commentaires, la notification remplace les notifications concernant ces commentaires et réponses.

Pour plus d’informations sur d’autres façons d’ajouter des utilisateurs à un BAT, voir [Partage d’un BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
