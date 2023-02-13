---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Répertorier les utilisateurs disposant d’une licence de vérification dans Adobe Workfront
description: Vous pouvez voir quels utilisateurs d’Adobe Workfront disposent actuellement de l’option "L’utilisateur peut générer des bons à tirer" activée de l’une des manières suivantes.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Répertorier les utilisateurs disposant d’une licence de vérification dans Adobe Workfront

Vous pouvez voir quels utilisateurs d’Adobe Workfront disposent actuellement de l’option &quot;L’utilisateur peut générer des bons à tirer&quot; activée de l’une des manières suivantes.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan hérité : Sélectionner ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Création d’un rapport utilisateur

Vous pouvez créer un rapport utilisateur pour savoir quels utilisateurs peuvent générer des bons à tirer :

1. Accédez à **Reporting** zone.
1. Cliquez sur le bouton **Nouveau rapport** menu déroulant, puis cliquez sur **Rapport utilisateur**.

1. Sur le **Filtres** , cliquez sur **Ajouter une règle de filtre**.

1. Dans le champ disponible, développez **Utilisateur**, puis cliquez sur **Dispose d’une licence de preuve**.

1. Sélectionner **Égal** > **True**.

   ![report_profile.png](assets/report-prooflicenses-350x135.png)

1. Cliquez sur **Enregistrer + Fermer**.

   Le rapport affiche tous les utilisateurs de Workfront auxquels une licence de vérification est affectée.

## Mettre à jour la vue Personnes

Vous pouvez ajouter une nouvelle colonne dans la vue Personnes afin d&#39;afficher les utilisateurs qui peuvent générer des BAT :

1. Accédez au **Personnes** zone.
1. Cliquez sur le bouton **Personnes** .
1. Dans le **Affichage** dans le menu déroulant, effectuez l’une des opérations suivantes :

   * Pour ajouter ces informations à une vue existante, sélectionnez la vue à personnaliser, puis cliquez sur **Vue Personnaliser**.
   * Pour ajouter ces informations à une nouvelle vue, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Dans le champ disponible, développez **Utilisateur**, puis cliquez sur **Dispose d’une licence de preuve**.

1. Cliquez sur **Terminé**, puis cliquez sur **Enregistrer la vue** ou **Enregistrer comme nouvelle vue**.

   La vue s’affiche. **True** ou **False** selon que l’utilisateur dispose ou non d’une licence de vérification.
