---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtre Projets actifs incluant des résultats inattendus
description: Lisez cet article pour résoudre les problèmes liés au filtre Projets sur lesquels je suis actif, y compris les résultats inattendus.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 18%

---

# Résultats inattendus du filtre « Projets auxquels je participe »

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe de la licence [!DNL Workfront]</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problème

Le filtre [!UICONTROL **Projets sur lesquels je suis sur**] comprend des résultats auxquels je ne m’attendrais pas, car je ne suis pas affecté ni associé à ces projets.

## Solution

Le filtre [!UICONTROL **Projets sur lesquels je suis activé**] comprend des projets qui contiennent l’utilisateur dans l’un de ses champs [!UICONTROL **Détails du projet**], y compris des champs facilement ignorés ou automatiquement remplis tels que [!UICONTROL **Entré par**] ou [!UICONTROL **ID de parrain**]. Pour supprimer les résultats indésirables, deux solutions sont possibles :

1. Vérifiez les [!UICONTROL **détails du projet**] pour chaque projet inattendu inclus par le filtre et supprimez votre nom de tous les champs.

   OU

1. Essayez d’utiliser un filtre similaire, tel que [!UICONTROL **Projets que je possède**], qui inclut uniquement les projets qui vous sont spécifiquement affectés.

Pour plus d’informations sur l’utilisation des filtres dans [!DNL Workfront], voir [Présentation des filtres](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
