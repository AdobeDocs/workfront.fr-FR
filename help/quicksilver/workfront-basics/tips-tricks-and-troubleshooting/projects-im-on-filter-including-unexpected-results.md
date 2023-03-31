---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtre Projets actifs incluant des résultats inattendus
description: Lisez cet article pour résoudre les problèmes liés au filtre Projets sur lesquels je suis actif, y compris les résultats inattendus.
feature: Get Started with Workfront
author: Nolan
source-git-commit: 5a4c98f9ce6bb7eb936a0b24b634d2545a0f13ee
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 1%

---

# Le filtre Projets actifs comprend des résultats inattendus

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problème

Le [!UICONTROL **Projets actifs**] filtre inclut des résultats auxquels je ne m’attendrais pas, car je ne suis pas affecté ou associé à ces projets.

## Solution

Le [!UICONTROL **Projets actifs**] filtre inclut les projets qui contiennent l’utilisateur dans l’un de ses [!UICONTROL **Détails du projet**] , y compris les champs facilement manqués ou remplis automatiquement, tels que [!UICONTROL **Entré par**] ou [!UICONTROL **Identifiant du parrain**]. Pour supprimer les résultats indésirables, deux solutions sont possibles :

1. Vérifiez les [!UICONTROL **Détails du projet**] pour chaque projet inattendu inclus par le filtre et supprimez votre nom de tous les champs.

OU

1. Essayez d’utiliser un filtre similaire, tel que [!UICONTROL **Projets que je possède**], qui inclut uniquement les projets qui vous sont spécifiquement affectés.

Pour plus d’informations sur l’utilisation des filtres dans [!DNL Workfront], voir [Présentation des filtres dans [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)