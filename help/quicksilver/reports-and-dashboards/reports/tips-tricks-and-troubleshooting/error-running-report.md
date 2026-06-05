---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Message d’erreur affiché lors de l’exécution d’un rapport : « Vous n’êtes pas actuellement connecté. »'
description: Découvrez le message d’erreur « Votre connexion n’est pas effective. »
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Vg-z-oXY25if70i5l2GBZad4iBj6hNRhu9LHE-6kCU8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 94%

---

# Message d’erreur lors de l’exécution d’un rapport : « Votre connexion n’est pas effective ».

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
     <p>Standard</p>
     <p>Travail ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problème

Lors de l’exécution d’un rapport ou de son affichage dans un tableau de bord, l’erreur suivante renvoie :\
*Réessayons. Votre connexion n’est pas effective dans*.

Aucun résultat ne s’affiche dans le rapport.

## Cause

Le rapport est actuellement défini pour s’exécuter en tant que personne désactivée.

## Solution

Pour pouvoir modifier les paramètres du rapport, vous devez disposer des autorisations Gérer.\
Pour ajuster le rapport et afficher les résultats, procédez comme suit :

1. Accédez au rapport.
1. Cliquez sur **Actions de rapport** > **Modifier** > **Paramètres des rapports**.

1. Indiquez le nom d’une personne active dans le champ **Exécuter ce rapport avec les droits d’accès suivants :**.\
   Ou\
   Laissez le champ **Exécuter ce rapport avec les droits d’accès suivants :** vide.

1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer + Fermer**.\
   L’erreur ne devrait pas réapparaître lors de l’exécution de ce rapport.
