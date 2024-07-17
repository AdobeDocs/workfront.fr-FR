---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Configurer les valeurs par défaut personnelles de relecture
description: Vous pouvez définir des paramètres par défaut de BAT personnels qui s’appliquent aux BAT que vous créez. Ces valeurs par défaut sont appliquées chaque fois que vous générez un nouveau BAT ou téléchargez une nouvelle version de BAT dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 6%

---

# Configurer les valeurs par défaut personnelles de relecture

Vous pouvez définir des paramètres par défaut de BAT personnels qui s’appliquent aux BAT que vous créez. Ces valeurs par défaut sont appliquées chaque fois que vous générez un nouveau BAT ou téléchargez une nouvelle version de BAT dans Workfront.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : sélection ou supérieure</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

## Configurer les valeurs par défaut personnelles de relecture

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Vérification**.

1. Dans le coin supérieur droit, cliquez sur votre avatar, puis sélectionnez **Paramètres personnels**.
1. Sélectionnez l&#39;onglet **Valeurs par défaut de la vérification** , puis spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong> Paramètres de notification par défaut</strong> </td> 
     </tr> 
     <tr> 
      <td>Alerte par défaut</td> 
      <td>Sélectionnez la fréquence à laquelle l’utilisateur reçoit les mises à jour par courrier électronique. Sélectionnez Toutes les activités, Réponses à mes commentaires, Décisions, Décision finale, Résumé horaire, Résumé quotidien ou Désactivé.</td> 
     </tr> 
     <tr> 
      <td>Alertes par défaut pour les nouveaux réviseurs invités</td> 
      <td>Sélectionnez la fréquence à laquelle les réviseurs invités reçoivent les mises à jour des emails. Les options sont identiques à celles de l’alerte par défaut.</td> 
     </tr> 
     <tr> 
      <td>Notification de nouveau BAT</td> 
      <td>Choisissez de recevoir une notification lorsque vous êtes ajouté à un BAT.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Paramètres du message</strong> </td> 
     </tr> 
     <tr> 
      <td>Modèle d’objet de BAT</td> 
      <td>Saisissez ce que vous souhaitez que les utilisateurs voient dans l’objet d’un email lorsque vous partagez un BAT avec eux.</td> 
     </tr> 
     <tr> 
      <td>Modèle de message de BAT</td> 
      <td>Saisissez ce que vous souhaitez que les utilisateurs voient dans le corps d’un email lorsque vous partagez un BAT avec eux.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Paramètres par défaut du BAT</strong> </td> 
     </tr> 
     <tr> 
      <td>Verrouiller le BAT lorsque toutes les décisions sont prises</td> 
      <td>Choisissez de verrouiller automatiquement le BAT contre d’autres modifications une fois toutes les décisions prises.</td> 
     </tr> 
     <tr> 
      <td>Seule une décision doit être prise</td> 
      <td>Choisissez de n'exiger qu'une seule décision sur un BAT.</td> 
     </tr> 
     <tr> 
      <td>Connexion requise</td> 
      <td> <p>Choisissez de rendre le BAT disponible uniquement pour les utilisateurs disposant des informations de connexion Workfront Proof.</p> <p>Remarque : Les informations d’identification Workfront Proof peuvent être différentes de celles de Workfront, sauf si l’utilisateur de votre société se connecte au service d’authentification unique. Nous vous recommandons d’utiliser cette fonctionnalité uniquement si l’authentification unique de votre entreprise est utilisée.</p> </td> 
     </tr> 
     <tr> 
      <td>Abonnement activé</td> 
      <td>Autoriser les réviseurs externes à l’organisation à s’inscrire au BAT via l’URL publique ou le code intégré. Lorsque cette option est sélectionnée, l'abonné doit cliquer sur un lien dans un email pour accéder à un BAT. Sélectionnez cette option pour obliger le validant externe à cliquer sur un lien dans l'email pour accéder au BAT. Cette option est activée par défaut si l'option Partage public est sélectionnée et appliquée à tous les BAT créés par cet utilisateur. </td> 
     </tr> 
     <tr> 
      <td>Rôle par défaut pour les nouveaux réviseurs invités</td> 
      <td>Sélectionnez un rôle de BAT par défaut pour les réviseurs invités. Les options sont identiques à celles du rôle BAT par défaut.</td> 
     </tr> 
     <tr> 
      <td>Téléchargement par bloc du fichier d’origine</td> 
      <td>Choisissez d’empêcher les utilisateurs de télécharger le fichier original. </td> 
     </tr> 
     <tr> 
      <td>Mon rôle de BAT par défaut</td> 
      <td>Choisissez votre rôle de BAT par défaut. </td> 
     </tr> 
     <tr> 
      <td>Ma couleur de balisage par défaut</td> 
      <td>Sélectionnez la couleur de balisage par défaut. </td> 
     </tr> 
    </tbody> 
   </table>
