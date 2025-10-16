---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Message d’erreur affiché lors de l’exécution d’un rapport : « Vous n’êtes pas actuellement connecté. »'
description: Découvrez le message d’erreur « Votre connexion n’est pas effective. »
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 93%

---

# Message d’erreur lors de l’exécution d’un rapport : « Votre connexion n’est pas effective ».

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
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
