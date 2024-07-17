---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Message d’erreur lors de l’exécution d’un rapport : "Vous n’êtes pas actuellement connecté.""'
description: Découvrez le message d’erreur "Vous n’êtes pas actuellement connecté".
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 45%

---

# Message d’erreur lors de l’exécution d’un rapport : « Votre connexion n’est pas effective ».

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Planifier, travailler</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Problème

Lors de l’exécution d’un rapport ou de son affichage dans un tableau de bord, l’erreur suivante renvoie :\
*Réessayons. Vous n&#39;êtes pas actuellement connecté.*

Aucun résultat ne s’affiche dans le rapport.

## Cause

Le rapport est actuellement défini pour s’exécuter en tant qu’utilisateur désactivé.

## Solution

Pour pouvoir modifier les paramètres du rapport, vous devez disposer des autorisations Gérer .\
Pour ajuster le rapport et afficher les résultats :

1. Accédez au rapport.
1. Cliquez sur **Actions de rapport** > **Modifier** > **Paramètres de rapport**.

1. Indiquez le nom d&#39;un utilisateur actif dans le champ **Exécuter ce rapport avec les droits d&#39;accès de :** .\
   Ou\
   Laissez vide le champ **Exécuter ce rapport avec les droits d’accès de :** .

1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer + Fermer**.\
   L’erreur ne doit pas réapparaître lors de l’exécution de ce rapport.
