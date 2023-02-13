---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Utiliser le rapport d'approbation des BAT
description: Vous pouvez utiliser le rapport d’approbation de BAT pour afficher des informations sur les bons à tirer dans votre environnement.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Utiliser le rapport d&#39;approbation des BAT

Vous pouvez utiliser le rapport d’approbation de BAT pour afficher des informations sur les bons à tirer dans votre environnement.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Formule Workfront*</p> </td> 
   <td>Tous</td> 
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
    </ul> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Utiliser le rapport d&#39;approbation des BAT

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis faites défiler l’écran pour sélectionner **Approbation du BAT**.

   ![](assets/proof-approval-report.png)

1. (Facultatif) Ajoutez des champs supplémentaires.
1. Cliquez sur **Enregistrer + Fermer**.

## Champs supplémentaires

Vous pouvez ajouter les champs suivants au rapport de validation des BAT :

* **Date de décision**: Affiche la date à laquelle un approbateur prend une décision sur un BAT. Vous pouvez également trouver cette date dans le Résumé d&#39;impression du BAT.
* **Étape d’approbateur**: Affiche les informations de l’étape actuelle.
* **Modèle de workflow**: Affiche tous les modèles de workflow associés au BAT. Si aucun modèle n’est joint, la colonne est vide.
* **En attente de décision**: Affiche true pour signaler qu’une décision n’a pas été prise sur la dernière version lorsque les conditions suivantes sont vraies :

   * Le BAT n&#39;a pas été archivé
   * L’étape sur laquelle se trouve l’approbateur est principale.
   * Le BAT est en attente d’approbation

* **Date limite de BAT**: Affiche la date limite du BAT. Pour que ce champ soit renseigné, une échéance doit être affectée à chaque étape. Le champ affiche la date limite de la dernière étape activée.

 
