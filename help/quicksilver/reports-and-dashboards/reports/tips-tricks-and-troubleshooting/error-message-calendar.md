---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '« Message d’erreur sur le calendrier : "Ce calendrier dispose des droits d’affichage d’un profil utilisateur désactivé." »'
description: En savoir plus sur le message d’erreur « Ce calendrier dispose des droits d’affichage d’un profil utilisateur désactivé. »
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 100%

---

# Message d’erreur sur le calendrier : « Ce calendrier dispose des droits d’affichage d’un profil utilisateur désactivé. »

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan, Travail</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations à un calendrier</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Problème

Vous recevez l’erreur suivante lorsque vous accédez à un calendrier partagé avec vous :

*Ce calendrier dispose des droits d’affichage d’un profil utilisateur désactivé. Demandez à un administrateur ou une administratrice de corriger les privilèges du calendrier.*

## Cause

La personne qui a créé ce calendrier (sa personne propriétaire originale) est une personne qui a été désactivée. 

## Solution

Vous pouvez résoudre ce problème de la manière suivante :

1. Copiez le calendrier d’origine. Lorsque vous copiez un calendrier, vous en devenez propriétaire. Le calendrier copié doit contenir toutes les informations du calendrier d’origine.\
   Pour plus d’informations sur la copie d’un calendrier, voir [Copier un rapport de calendrier](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Partagez le calendrier copié avec les mêmes utilisateurs et utilisatrices que le calendrier original. Tous les utilisateurs et utilisatrices devraient voir les mêmes informations sur le nouveau calendrier.
1. (Facultatif et le cas échéant) Si vous recevez l’autorisation de gérer le calendrier d’origine, supprimez tous les autres utilisateurs et utilisatrices avec lesquels le calendrier est partagé de la zone de partage du calendrier. Cela épargne toute confusion aux utilisateurs et utilistratrices qui tentent d’afficher un calendrier erroné.
