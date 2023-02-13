---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Conversion d’un workflow de base en workflow automatisé sur un BAT
description: Si vous êtes le propriétaire du BAT, vous pouvez convertir le workflow de base d’un BAT existant en workflow automatisé.
author: Courtney
feature: Digital Content and Documents
exl-id: c676c696-ab7d-415b-bf5e-5d0335a3920f
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 4%

---

# Conversion d’un workflow de base en workflow automatisé sur un BAT

Si vous êtes le propriétaire du BAT, vous pouvez convertir le workflow de base d’un BAT existant en workflow automatisé.

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
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Conversion d’un workflow de base en workflow automatisé

1. Dans la liste des documents, passez la souris sur le document, puis cliquez sur **Workflow de vérification** lorsqu’elle s’affiche.
1. Dans le coin supérieur droit d’Adobe Workfront, cliquez sur **Convertir en processus automatisé**.
1. Cliquez sur **Nouvelle étape** dans le coin supérieur droit de l’écran.
1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nom</strong> </td> 
      <td>Ajoutez un nom pour votre scène.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Échéance</strong> </td> 
      <td>Choisissez une date d'échéance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p><strong>Activer l’étape</strong> </p> </td> 
      <td>Choisissez quand l’étape doit s’activer.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Options de date d'échéance</strong> </td> 
      <td>Sélectionnez le mode de déclenchement de l’échéance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Verrouiller l’étape</strong> </td> 
      <td>Choisissez si la scène doit être verrouillée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Décisionnaire principal</strong> </td> 
      <td>Indiquez le Principal décideur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Décision</strong> </td> 
      <td>Choisissez si une seule décision est requise. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Confidentialité</strong> </td> 
      <td>Choisissez si la scène est privée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ajouter des utilisateurs</strong> </td> 
      <td>Saisissez un nom de contact ou une adresse email, choisissez le rôle du BAT, puis configurez les alertes par email.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Ajout d’une étape**.
1. (Facultatif) Répétez les étapes 3 et 4 jusqu’à ce que vous soyez satisfait de votre workflow.
