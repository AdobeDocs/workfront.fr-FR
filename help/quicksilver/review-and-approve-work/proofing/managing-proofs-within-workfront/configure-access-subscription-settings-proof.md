---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Configurer les paramètres d’accès et d’abonnement d’une épreuve
description: Vous pouvez configurer certains paramètres d’accès et d’abonnement pour des bons à tirer individuels, par exemple s’il est nécessaire d’obliger les utilisateurs à se connecter et s’il est possible d’autoriser les utilisateurs à s’abonner au BAT. Vous pouvez configurer les paramètres d’accès et d’abonnement pour un BAT pendant que vous le créez ou vous pouvez les configurer pour un BAT qui existe déjà dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 9%

---

# Configurer les paramètres d’accès et d’abonnement d’une épreuve

Vous pouvez configurer certains paramètres d’accès et d’abonnement pour des bons à tirer individuels, par exemple s’il est nécessaire d’obliger les utilisateurs à se connecter et s’il est possible d’autoriser les utilisateurs à s’abonner au BAT. Vous pouvez configurer les paramètres d’accès et d’abonnement pour un BAT pendant que vous le créez ou vous pouvez les configurer pour un BAT qui existe déjà dans Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

+++

## Configurer les paramètres d’accès et d’abonnement lors de la création d’un BAT

Pour configurer les paramètres d&#39;accès et d&#39;abonnement pour un BAT pendant sa création :

1. Accédez au projet, à la tâche ou à l’emplacement où vous souhaitez obtenir le BAT, puis cliquez sur la section **Documents** .
1. Cliquez sur **Ajouter nouveau** dans la zone supérieure droite.
1. Accédez à la section **Paramètres du bon à tirer** dans le coin inférieur droit de la page **Nouveau BAT** .

1. Configurez les paramètres suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Autoriser le partage de BAT via une URL publique ou un code incorporé </strong> </td> 
      <td>Lorsque cette option est sélectionnée, le BAT peut être partagé via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Autoriser l'abonnement au BAT via une URL publique ou un code incorporé</strong> </td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées au BAT peuvent s’abonner au BAT. La personne qui s'abonne au BAT se voit attribuer le rôle et l'email que vous définissez dans les paramètres suivants :
       <ul>
        <li><p><strong>Rôle d’abonné : </strong> rôle de BAT par défaut attribué à tous les réviseurs qui souscrivent au BAT. </p><p>Important : Si <strong>Autoriser le partage avec </strong> est défini sur autre chose que <strong>Tout le monde</strong> dans les paramètres de Workfront Proof, l’abonnement ne fonctionne que pour les personnes de l’entreprise. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuration des paramètres de BAT dans Workfront Proof</a>.</p></li>
        <li><strong>Paramètres des alertes par email pour les abonnés :</strong> L’alerte par défaut qui est attribuée à tous les réviseurs qui souscrivent au BAT.</li>
       </ul><p>
        <ul>
         <li><strong>L'accès au BAT par le biais d'un lien d'email est requis pour :</strong> Configurez si l'abonné reçoit un email avec un lien vers le BAT. Vous pouvez sélectionner <strong>Aucun email</strong> (aucun lien d'email n'est nécessaire pour accéder au BAT), <strong>Email de notification de BAT uniquement</strong> (l'abonné reçoit un lien vers le BAT par email sans vérification) ou <strong>Email de validation et de notification de BAT</strong> (l'abonné reçoit un lien vers le BAT par email et doit cliquer sur le lien pour accéder à un BAT, l'option permettant de s'assurer que la personne que l'adresse email indiquée dans un email adresse à laquelle ils ont accès).</li>
        </ul><p>Remarque :  Si le workflow automatisé est joint aux bons à tirer, tous les abonnements génèrent des emails de confirmation pour les propriétaires du BAT, afin qu’ils puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continuez à créer votre BAT.

## Configurer les paramètres d&#39;accès et d&#39;abonnement pour un BAT existant

Pour configurer les paramètres d’accès et d’abonnement pour un BAT qui existe déjà dans Workfront :

1. Dans la zone Documents, sélectionnez le document contenant le BAT pour lequel vous souhaitez configurer les paramètres, puis cliquez sur **Document Details**.
1. Dans le panneau de gauche, cliquez sur **Paramètres de la visionneuse de vérification**.
1. Configurez les paramètres suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Autoriser le partage de BAT via une URL publique ou un code incorporé</strong><strong>e</strong> </td> 
      <td>Lorsque cette option est sélectionnée, le BAT peut être partagé via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Autoriser l'abonnement au BAT via une URL publique ou un code incorporé</strong> </td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées au BAT peuvent s’abonner au BAT. La personne qui s'abonne au BAT se voit attribuer le rôle et l'email que vous définissez dans les paramètres suivants :
       <ul>
        <li><p><strong>Rôle d’abonné : </strong> rôle de BAT par défaut attribué à tous les réviseurs qui souscrivent au BAT. </p><p>Important : Si <strong>Autoriser le partage avec </strong> est défini sur autre chose que <strong>Tout le monde</strong> dans les paramètres de Workfront Proof, l’abonnement ne fonctionne que pour les personnes de l’entreprise. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuration des paramètres de BAT dans Workfront Proof</a>.</p></li>
        <li><strong>Paramètres des alertes par email pour les abonnés :</strong> L’alerte par défaut qui est attribuée à tous les réviseurs qui souscrivent au BAT.</li>
       </ul><p>
        <ul>
         <li><strong>L'accès au BAT par le biais d'un lien d'email est requis pour :</strong> Configurez si l'abonné reçoit un email avec un lien vers le BAT. Vous pouvez sélectionner <strong>Aucun email</strong> (aucun lien d'email n'est nécessaire pour accéder au BAT), <strong>Email de notification de BAT uniquement</strong> (l'abonné reçoit un lien vers le BAT par email sans vérification) ou <strong>Email de validation et de notification de BAT</strong> (l'abonné reçoit un lien vers le BAT par email et doit cliquer sur le lien pour accéder à un BAT, l'option permettant de s'assurer que la personne que l'adresse email indiquée dans un email adresse à laquelle ils ont accès).</li>
        </ul><p>Remarque :  Si le workflow automatisé est joint aux bons à tirer, tous les abonnements génèrent des emails de confirmation pour les propriétaires du BAT, afin qu’ils puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
