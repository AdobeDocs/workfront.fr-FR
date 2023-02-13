---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Modification des paramètres du BAT
description: Vous pouvez modifier les paramètres du BAT à tout moment après avoir créé un BAT.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 7%

---

# Modification des paramètres du BAT

Vous pouvez modifier les paramètres du BAT à tout moment après avoir créé un BAT.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou version ultérieure</p> <p>ou</p> <p>Plan hérité : Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Travail ou plan</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
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
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Modification des paramètres du BAT

Certains paramètres peuvent être verrouillés si votre administrateur Workfront les a désactivés au niveau du compte.

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez obtenir le BAT, puis cliquez sur le bouton **Documents** .
1. Placez le pointeur de la souris sur le BAT, puis cliquez sur **Détails du document**.
1. Dans le panneau de gauche, cliquez sur **Vérification des paramètres de la visionneuse**.
1. Ajustez les paramètres suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Authentification requise. Impossible de partager cette épreuve avec des utilisateurs invités</td> 
      <td> <p>Si vous avez besoin de niveaux de sécurité supérieurs pour votre processus de révision et d’approbation, vous pouvez utiliser l’option de connexion requise au BAT. Cela signifie que seuls les utilisateurs de Workfront peuvent être ajoutés au BAT. Il doit saisir son email et son mot de passe avant d'y accéder.</p> <p>Remarque : <em style="font-style: normal;">Si l’option Connexion requise est activée, les abonnements ne peuvent pas être activés.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td> <p>Vous pouvez exiger la signature électronique de tout réviseur qui prend une décision sur le BAT. Lorsqu’un réviseur prend une décision, une invite s’affiche, lui demandant de saisir son email et son mot de passe et de confirmer sa décision. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller le BAT lorsque toutes les décisions requises sont prises</td> 
      <td> <p>Vous pouvez définir un état de BAT à verrouiller lorsque l’approbateur final prend sa décision. Cela s’avère utile si vous souhaitez vous assurer que vos réviseurs ne pourront pas revenir au BAT et ajouter des commentaires supplémentaires ou modifier leurs décisions.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le téléchargement du fichier original</td> 
      <td> <p>Vous pouvez permettre aux réviseurs sur un BAT de télécharger le fichier d'origine à partir duquel un BAT a été créé. Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">autoriser le partage de l'épreuve via une URL publique ou un code intégré</td> 
      <td>Vous pouvez permettre aux utilisateurs de partager le BAT avec une URL publique ou un code intégré. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser l'abonnement à l'épreuve via une URL publique ou un code intégré</td> 
      <td> <p>L'inscription au BAT permet aux personnes qui n'ont pas été explicitement ajoutées au BAT de s'inscrire au BAT (c'est-à-dire de s'ajouter au BAT). Le rôle et l’alerte par email que vous sélectionnez leur seront alors attribués dans les paramètres d’abonnement.</p> <p>Si l'inscription a été activée sur un BAT, les champs ci-dessous deviennent principaux :</p> 
       <ul> 
        <li><strong>Validation des abonnés requise</strong> - L'abonné doit cliquer sur un lien dans un email pour accéder à un BAT<br>Cette option signifie que la personne qui s'abonne n'aura pas un accès immédiat au BAT, mais qu'elle aura un lien vers le BAT dans un email. La validation des abonnés a pour but de s’assurer que la personne a saisi une adresse électronique correcte à laquelle elle a accès.</li> 
        <li><strong>Rôle par défaut pour les nouveaux abonnés -</strong> Il s’agit du rôle de BAT par défaut qui sera attribué à tous les réviseurs qui s’abonnent au BAT.</li> 
        <li><strong>Alertes par défaut pour les nouveaux abonnés</strong> - Il s’agit de l’alerte par défaut qui sera affectée à tous les réviseurs qui s’abonnent au BAT.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

 
