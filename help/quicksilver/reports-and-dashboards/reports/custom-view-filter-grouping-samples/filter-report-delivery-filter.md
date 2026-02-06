---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : affichage des rapports planifiés pour la diffusion'
description: Ce filtre affiche tous les rapports planifiés pour être remis automatiquement dans Adobe Workfront. Il est préférable de l’utiliser avec la vue standard.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: be102fd5f490b12837a231774253c030973c1c4f
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 88%

---

# Filtre : afficher les rapports dont la diffusion est prévue

<!--Audited: 10/2024-->

Ce filtre affiche tous les rapports planifiés pour être remis automatiquement dans Adobe Workfront. Il est préférable de l’utiliser avec la vue standard.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtre de remise de rapport

Pour appliquer ce filtre :

1. Accédez à une liste de rapports.

1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. Cliquez sur **Basculer en mode texte**.

1. Dans la zone **Définir les règles de filtrage pour votre rapport**, copiez et collez le code suivant :

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. Cliquez sur **Enregistrer le filtre**.
