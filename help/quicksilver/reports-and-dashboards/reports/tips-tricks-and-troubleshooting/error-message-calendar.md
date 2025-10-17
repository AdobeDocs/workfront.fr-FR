---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Message d’erreur sur le calendrier : « Ce calendrier dispose des droits d’affichage d’un utilisateur désactivé. »'
description: En savoir plus sur le message d’erreur « Ce calendrier dispose des droits d’affichage d’un profil utilisateur désactivé. »
author: Jenny
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 93%

---

# Message d’erreur sur le calendrier : « Ce calendrier dispose des droits d’affichage d’un profil utilisateur désactivé. »

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
   <td> <p>Gérer les autorisations à un calendrier</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
