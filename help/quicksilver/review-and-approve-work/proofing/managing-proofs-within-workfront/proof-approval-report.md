---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Utiliser le rapport d’approbation de l’épreuve
description: Vous pouvez utiliser le rapport d’approbation de BAT pour afficher des informations sur les bons à tirer dans votre environnement.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 8a388ffa2d30683c08637a4273f628c553e55fdb
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 28%

---

# Utiliser le rapport d’approbation de l’épreuve

Vous pouvez utiliser le rapport d’approbation de BAT pour afficher des informations sur les bons à tirer dans votre environnement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Plan Workfront*</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Présentation des licences Adobe Workfront*</p> </td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Niveau d’accès*</strong> </td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Utiliser le rapport d’approbation de l’épreuve

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis faites défiler l’écran pour sélectionner **Approbation de BAT**.

   ![](assets/proof-approval-report.png)

1. (Facultatif) Ajoutez d’autres champs.
1. Cliquez sur **Enregistrer + Fermer**.

## Champs supplémentaires

Vous pouvez ajouter les champs suivants au rapport de validation des BAT :

* **Date de décision** : affiche la date à laquelle un approbateur prend une décision sur un BAT. Vous pouvez également trouver cette date dans le Résumé d&#39;impression du BAT.
* **Étape approbateur** : affiche les informations de l’étape actuelle.
* **Modèle de workflow** : affiche tous les modèles de workflow associés au BAT. Si aucun modèle n’est joint, la colonne est vide.
* **En attente de décision** : s’affiche sur true pour signaler qu’une décision n’a pas été prise sur la dernière version lorsque les conditions suivantes sont vraies :

   * Le BAT n&#39;a pas été archivé
   * L’étape sur laquelle se trouve l’approbateur est active.
   * Le BAT est en attente d’approbation

* **Expiration du bon à tirer** : affiche la date limite du bon à tirer. Pour que ce champ soit renseigné, une échéance doit être affectée à chaque étape. Le champ affiche la date limite de la dernière étape activée.

 
