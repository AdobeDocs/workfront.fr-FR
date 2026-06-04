---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtre Projets auxquels je participe incluant des résultats inattendus
description: Lisez cet article pour résoudre les problèmes liés au filtre Projets auxquels je participe incluant des résultats inattendus.
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 100%

---

# Le filtre Projets auxquels je participe inclut des résultats inattendus.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
   <td>Tous</td>
  </tr>
  <tr>
   <td>Licences Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problème

Le filtre [!UICONTROL **Projets auxquels je participe**] inclut des résultats inattendus, car il n’existe aucune affectation ni association pour moi avec ces projets.

## Solution

Le filtre [!UICONTROL **Projets auxquels je participe**] inclut des projets qui contiennent l’utilisateur ou l’utilisatrice dans l’un de ses champs [!UICONTROL **Détails du projet**], y compris les champs facilement manqués ou remplis automatiquement, tels que [!UICONTROL **Saisi par**] ou [!UICONTROL **ID de sponsor**]. Pour supprimer les résultats indésirables, deux solutions sont possibles :

1. Vérifiez les [!UICONTROL **Détails du projet**] pour chaque projet inattendu inclus par le filtre et supprimez votre nom de tous les champs.

   OU

1. Essayez d’utiliser un filtre similaire, tel que [!UICONTROL **Projets dont je suis propriétaire**], qui inclut uniquement les projets qui vous sont spécifiquement affectés.

Pour plus d’informations sur l’utilisation des filtres dans [!DNL Workfront], voir [Vue d’ensemble des filtres](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
