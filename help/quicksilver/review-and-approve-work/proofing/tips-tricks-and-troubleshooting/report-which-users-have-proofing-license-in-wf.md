---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Liste des utilisateurs et utilisatrices disposant d’une licence de relecture dans Adobe Workfront
description: Vous pouvez voir quels utilisateurs d’Adobe Workfront disposent actuellement de l’option "L’utilisateur peut générer des bons à tirer" activée de l’une des manières suivantes.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 22%

---

# Liste des utilisateurs et utilisatrices disposant d’une licence de relecture dans Adobe Workfront

Vous pouvez voir quels utilisateurs d’Adobe Workfront disposent actuellement de l’option &quot;L’utilisateur peut générer des bons à tirer&quot; activée de l’une des manières suivantes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule héritée : sélectionnez ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

## Création d’un rapport utilisateur

Vous pouvez créer un rapport utilisateur pour savoir quels utilisateurs peuvent générer des bons à tirer :

1. Accédez à la zone **Reporting**.
1. Cliquez sur le menu déroulant **Nouveau rapport** , puis sur **Rapport utilisateur**.

1. Sur l’onglet **Filtres**, cliquez sur **Ajouter une règle de filtre**.

1. Dans le champ disponible, développez **User**, puis cliquez sur **Has Proof License**.

1. Sélectionnez **Equal** > **True**.

   ![report_profile.png](assets/report-prooflicenses-350x135.png)

1. Cliquez sur **Enregistrer+Fermer**.

   Le rapport affiche tous les utilisateurs de Workfront auxquels une licence de vérification est affectée.

## Mettre à jour la vue Personnes

Vous pouvez ajouter une nouvelle colonne dans la vue Personnes afin d&#39;afficher les utilisateurs qui peuvent générer des BAT :

1. Accédez à la zone **People** .
1. Cliquez sur l’onglet **Personnes** .
1. Dans le menu déroulant **Affichage** , effectuez l’une des opérations suivantes :

   * Pour ajouter ces informations à une vue existante, sélectionnez la vue que vous souhaitez personnaliser, puis cliquez sur **Personnaliser la vue**.
   * Pour ajouter ces informations à une nouvelle vue, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Dans le champ disponible, développez **User**, puis cliquez sur **Has Proof License**.

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue** ou **Enregistrer comme nouvelle vue**.

   La vue affiche **True** ou **False** selon que l’utilisateur est associé à une licence de vérification.
