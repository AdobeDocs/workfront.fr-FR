---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Envoyer des e-mails aux réviseurs et réviseuses d’une épreuve
description: Pendant le processus de révision et d'approbation, vous pouvez envoyer un message à l'un ou tous les réviseurs sur un BAT. Les messages sont un moyen facile de rappeler aux opérateurs validants de terminer la vérification d'un BAT ou de fournir d'autres informations relatives au BAT.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 20%

---

# Envoyer des e-mails aux réviseurs et réviseuses d’une épreuve

Pendant le processus de révision et d&#39;approbation, vous pouvez envoyer un message à l&#39;un ou tous les réviseurs sur un BAT. Les messages sont un moyen facile de rappeler aux opérateurs validants de terminer la vérification d&#39;un BAT ou de fournir d&#39;autres informations relatives au BAT.

Vous pouvez choisir d’envoyer un email de rappel générique ou d’envoyer un message personnalisé à l’un des utilisateurs ou à tous les utilisateurs associés à une étape donnée.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : sélectionnez ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
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
   <td role="rowheader">Rôle de BAT</td> 
   <td>Auteur ou modérateur</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

## Envoyer des emails aux utilisateurs sur un BAT

1. Recherchez le document correspondant au BAT qui contient les utilisateurs que vous souhaitez envoyer par message.
1. Passez la souris sur le document, puis cliquez sur **Processus de vérification**.

   ![](assets/proof-workflow-doc-list-350x92.png)

1. Pour envoyer un message à tous les utilisateurs sur la scène, cliquez sur le menu **Plus** sur la scène et choisissez **Message All**.

   ![](assets/message-stage-350x122.png)

1. Pour envoyer un message à un utilisateur individuel, cliquez sur le menu **Plus** en regard de l’utilisateur et sélectionnez **Message**.

   ![](assets/message-user-350x121.png)

1. Dans la section **Détails du message** , spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Notifier les personnes par e-mail</td> 
      <td>Cette option ne peut pas être désélectionnée. Tous les utilisateurs reçoivent le message par email.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ignorer le message personnalisé</td> 
      <td> <p>Cliquez sur <strong>Ignorer le message personnalisé</strong> si vous souhaitez inclure uniquement le contenu d’email par défaut.</p> <p>L’email de rappel par défaut contient les informations suivantes :</p> 
       <ul> 
        <li>Lien personnel vers la vignette du BAT<br>Miniature de l'image du BAT<br></li> 
        <li>Les détails du BAT suivants : le nom du BAT, le numéro de version, le nom du dossier (le cas échéant), ainsi qu'une liste des validants et leur état d'avancement sur le BAT.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Objet</td> 
      <td>Saisissez l’objet du message.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Message</td> 
      <td>Saisissez le contenu de votre message.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Envoyer.**
