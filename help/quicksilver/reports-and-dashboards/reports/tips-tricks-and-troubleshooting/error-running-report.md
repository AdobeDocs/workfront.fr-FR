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
ht-degree: 4%

---

# Message d’erreur lors de l’exécution d’un rapport : &quot;Vous n’êtes pas actuellement connecté.&quot;

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Planifier, travailler</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Problème

Lors de l’exécution d’un rapport ou de son affichage dans un tableau de bord, l’erreur suivante renvoie :\
*Réessayons. Vous n’êtes pas connecté actuellement.*

Aucun résultat ne s’affiche dans le rapport.

## Cause

Le rapport est actuellement défini pour s’exécuter en tant qu’utilisateur désactivé.

## Solution

Pour pouvoir modifier les paramètres du rapport, vous devez disposer des autorisations Gérer .\
Pour ajuster le rapport et afficher les résultats :

1. Accédez au rapport.
1. Cliquez sur **Actions de rapport** > **Modifier** > **Paramètres des rapports**.

1. Indiquez le nom d’un utilisateur actif dans la variable **Exécutez ce rapport avec les droits d’accès de :** champ .\
   Ou\
   Laissez le champ **Exécutez ce rapport avec les droits d’accès de :** champ vide.

1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer + Fermer**.\
   L’erreur ne doit pas réapparaître lors de l’exécution de ce rapport.
