---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Répertorier les titulaires d’une licence de relecture dans Adobe Workfront
description: Pour afficher les utilisateurs et utilisatrices d’Adobe Workfront dont l’option « L’utilisateur ou l’utilisatrice peut générer des épreuves » est activée, procédez de l’une des manières suivantes.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 385f4a6663cacfdcf519bf5699fc1840c2cb2adc
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 99%

---

# Répertorier les titulaires d’une licence de relecture dans Adobe Workfront

Pour afficher les utilisateurs et utilisatrices d’Adobe Workfront dont l’option « L’utilisateur ou l’utilisatrice peut générer des épreuves » est activée, procédez de l’une des manières suivantes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
   <p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en modification aux éléments suivants :</p> 
    <ul> 
     <li> <p>Créer des rapports, des tableaux de bord et des calendriers</p> </li> 
     <li> <p>Créer des filtres, des vues et des regroupements</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
