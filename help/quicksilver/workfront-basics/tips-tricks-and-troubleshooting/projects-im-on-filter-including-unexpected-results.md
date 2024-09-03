---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtre Projets auxquels je participe incluant des résultats inattendus
description: Lisez cet article pour résoudre les problèmes liés au filtre Projets auxquels je participe incluant des résultats inattendus.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 100%

---

# Le filtre Projets auxquels je participe inclut des résultats inattendus.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe [!DNL Workfront]</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problème

Le filtre [!UICONTROL **Projets auxquels je participe**] inclut des résultats inattendus, car il n’existe aucune affectation ni association pour moi avec ces projets.

## Solution

Le filtre [!UICONTROL **Projets auxquels je participe**] inclut des projets qui contiennent l’utilisateur ou l’utilisatrice dans l’un de ses champs [!UICONTROL **Détails du projet**], y compris les champs facilement manqués ou remplis automatiquement, tels que [!UICONTROL **Saisi par**] ou [!UICONTROL **ID de sponsor**]. Pour supprimer les résultats indésirables, deux solutions sont possibles :

1. Vérifiez les [!UICONTROL **Détails du projet**] pour chaque projet inattendu inclus par le filtre et supprimez votre nom de tous les champs.

   OU

1. Essayez d’utiliser un filtre similaire, tel que [!UICONTROL **Projets dont je suis propriétaire**], qui inclut uniquement les projets qui vous sont spécifiquement affectés.

Pour plus d’informations sur l’utilisation des filtres dans [!DNL Workfront], voir [Vue d’ensemble des filtres](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
