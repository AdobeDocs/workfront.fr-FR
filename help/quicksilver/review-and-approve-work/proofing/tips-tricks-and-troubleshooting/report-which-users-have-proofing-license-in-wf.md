---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Répertorier les titulaires d’une licence de relecture dans Adobe Workfront
description: Pour afficher les utilisateurs et utilisatrices d’Adobe Workfront dont l’option « L’utilisateur ou l’utilisatrice peut générer des épreuves » est activée, procédez de l’une des manières suivantes.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
TQID: https://experienceleague.adobe.com/9P5Bp9TrJ1ECSwpK7C4AW4rQlTQOBH4U7-CPYl92RKU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 312
ht-degree: 100%

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
   <td role="rowheader">Package Adobe Workfront</td> 
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

   Le rapport affiche tous les titulaires d’une licence de relecture dans Workfront.

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
