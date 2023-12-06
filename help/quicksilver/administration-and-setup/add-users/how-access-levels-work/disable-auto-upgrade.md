---
title: Désactivez l’option de mise à niveau automatique pour les utilisateurs non payants du nouveau plan de licence.
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,standard,light,contributor
navigation-topic: access-levels
description: Chaque utilisateur doit disposer d’un niveau d’accès pour se connecter et travailler dans Workfront. Vous utilisez le niveau d’accès pour contrôler ce qu’un utilisateur peut voir et faire avec certains objets et zones Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 1%

---

# Désactivez l’option de mise à niveau automatique pour les utilisateurs non payants du nouveau plan de licence.

Les décisions concernant les BAT et les documents sont limitées pour toutes les licences Workfront non payantes sur les nouveaux plans. Lorsque les utilisateurs atteignent le nombre de décisions qui leur est alloué, ils sont mis à niveau vers une licence Light par défaut.

Vous pouvez désactiver l’option de mise à niveau automatique dans la zone de configuration. Pour en savoir plus sur le fonctionnement des mises à niveau automatiques, voir [Présentation des documents et des BAT limités pour les utilisateurs non payants](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>Une fois désactivé, tout utilisateur non payant qui passe en revue le nombre de décisions autorisé ne sera pas automatiquement mis à niveau.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Nouveau plan : Standard
   <p>ou</p>
   <p>Formule actuelle : Formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Désactivation des mises à niveau automatiques pour les utilisateurs non payants

{{step-1-to-setup}}

1. Développer [!UICONTROL **Système**] dans la navigation de gauche, puis cliquez sur [!UICONTROL **Préférences**].
1. Dans le [!UICONTROL **Préférences générales**] , vérifiez les [!UICONTROL **Désactivation de la mise à niveau automatique dans les niveaux d’accès**] de la boîte.
1. Cliquer sur [!UICONTROL **Enregistrer**].
