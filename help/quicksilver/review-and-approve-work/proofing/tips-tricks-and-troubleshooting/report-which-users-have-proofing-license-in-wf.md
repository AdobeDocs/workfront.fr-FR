---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Répertorier les titulaires d’une licence de relecture dans Adobe Workfront
description: Pour afficher les utilisateurs et utilisatrices d’Adobe Workfront dont l’option « L’utilisateur ou l’utilisatrice peut générer des épreuves » est activée, procédez de l’une des manières suivantes.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 100%

---

# Répertorier les titulaires d’une licence de relecture dans Adobe Workfront

Pour afficher les utilisateurs et utilisatrices d’Adobe Workfront dont l’option « L’utilisateur ou l’utilisatrice peut générer des épreuves » est activée, procédez de l’une des manières suivantes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule héritée : Select ou Premium</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en modification aux éléments suivants :</p> 
    <ul> 
     <li> <p>Créer des rapports, des tableaux de bord et des calendriers</p> </li> 
     <li> <p>Créer des filtres, des vues et des regroupements</p> </li> 
    </ul> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice Workfront ou Workfront Proof.

+++

## Créer un rapport utilisateur

Vous pouvez créer un rapport utilisateur pour consulter les utilisateurs et utilisatrices autorisés à générer des épreuves :

1. Accédez à la zone **Rapports**.
1. Cliquez sur le menu déroulant **Nouveau rapport** et sélectionnez **Rapport utilisateur**.

1. Sous l’onglet **Filtres**, cliquez sur **Ajouter une règle de filtre**.

1. Dans le champ disponible, développez **Utilisateur ou utilisatrice**, puis cliquez sur **Détient une licence d’épreuve**.

1. Sélectionnez **Égal** > **Vrai**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Cliquez sur **Enregistrer + Fermer**.

   Le rapport affiche tous les titulaires d’une licence d’épreuve dans Workfront.

## Mettre à jour la vue Personnes

Vous pouvez ajouter une nouvelle colonne dans la vue Personnes afin d’afficher les utilisateurs et utilisatrices autorisés à générer des épreuves :

1. Accédez à la zone **Personnes**.
1. Cliquez sur l’onglet **Personnes**.
1. Dans le menu déroulant **Vue**, effectuez l’une des opérations suivantes :

   * Pour ajouter ces informations à une vue existante, sélectionnez la vue à personnaliser, puis cliquez sur **Personnaliser la vue**.
   * Pour ajouter ces informations à une nouvelle vue, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Dans le champ disponible, développez **Utilisateur ou utilisatrice**, puis cliquez sur **Détient une licence d’épreuve**.

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue** ou **Enregistrer en tant que nouvelle vue**.

   La vue indique **Vrai** ou **Faux** selon que l’utilisateur ou l’utilisatrice dispose ou non d’une licence de relecture.
