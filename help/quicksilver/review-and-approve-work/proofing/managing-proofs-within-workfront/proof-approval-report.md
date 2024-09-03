---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Utiliser le rapport d’approbation de l’épreuve
description: Vous pouvez utiliser le rapport d’approbation des épreuves pour afficher des informations sur les épreuves dans votre environnement.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 8a388ffa2d30683c08637a4273f628c553e55fdb
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 100%

---

# Utiliser le rapport d’approbation de l’épreuve

Vous pouvez utiliser le rapport d’approbation des épreuves pour afficher des informations sur les épreuves dans votre environnement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Forfait Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Vue d’ensemble des licences Adobe Workfront*</p> </td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Niveau d’accès*</strong> </td> 
   <td> <p>Accès en modification aux éléments suivants :</p> 
    <ul> 
     <li> <p>Créer des rapports, des tableaux de bord et des calendriers</p> </li> 
     <li> <p>Créer des filtres, des vues et des regroupements</p> </li> 
    </ul> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Utiliser le rapport d’approbation de l’épreuve

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis faites défiler l’écran pour sélectionner **Approbation des épreuves**.

   ![](assets/proof-approval-report.png)

1. (Facultatif) Ajoutez des champs supplémentaires.
1. Cliquez sur **Enregistrer + Fermer**.

## Champs supplémentaires

Vous pouvez ajouter les champs suivants au rapport d’approbation des épreuves :

* **Date de décision** : affiche la date à laquelle une personne approbatrice prend une décision sur une épreuve. Vous pouvez également trouver cette date dans le Résumé d’impression de l’épreuve.
* **Étape d’approbation** : affiche les informations sur l’étape en cours.
* **Modèle de workflow** : affiche tous les modèles de workflow attachés à l’épreuve. Si aucun modèle n’est joint, la colonne est vide.
* **En attente de décision** : affiche « true » pour signaler qu’une décision n’a pas été prise sur la dernière version lorsque les conditions suivantes sont remplies :

   * L’épreuve n’a pas été archivée.
   * L’étape à laquelle se trouve la personne approbatrice est active.
   * L’épreuve est en attente d’approbation.

* **Date d’échéance pour la relecture** : affiche la date d’échéance de l’épreuve. Chaque étape doit être assortie d’une date d’échéance pour que ce champ soit renseigné. Le champ affiche la date d’échéance de la dernière étape activée.

 
