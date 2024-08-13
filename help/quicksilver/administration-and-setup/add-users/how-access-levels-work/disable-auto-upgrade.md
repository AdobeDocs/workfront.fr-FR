---
title: Désactivation de l’option de mise à niveau automatique pour les utilisateurs non payés du nouveau plan de licence
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,standard,light,contributor
navigation-topic: access-levels
description: Chaque utilisateur doit disposer d’un niveau d’accès pour se connecter et travailler dans Workfront. Vous utilisez le niveau d’accès pour contrôler ce qu’un utilisateur peut voir et faire avec certains objets et zones Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 24%

---

# Désactiver l’option de mise à niveau automatique pour les utilisateurs et utilisatrices non payants du nouveau forfait de licence

Les décisions concernant les BAT et les documents sont limitées pour toutes les licences Workfront non payantes sur les nouveaux plans. Lorsque les utilisateurs atteignent le nombre de décisions qui leur est alloué, ils sont mis à niveau vers une licence Light par défaut.

Vous pouvez désactiver l’option de mise à niveau automatique dans la zone de configuration. Pour en savoir plus sur le fonctionnement des mises à niveau automatiques, consultez la [présentation d&#39;un document limité et d&#39;une décision de BAT pour les utilisateurs non payants](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>Une fois désactivé, tout utilisateur non payant qui passe en revue le nombre de décisions autorisé ne sera pas automatiquement mis à niveau.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Nouvelle formule : standard
   <p>ou</p>
   <p>Formule actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Désactivation des mises à niveau automatiques pour les utilisateurs non payants

{{step-1-to-setup}}

1. Développez [!UICONTROL **Système**] dans le volet de navigation de gauche, puis cliquez sur [!UICONTROL **Préférences**].
1. Dans la section [!UICONTROL **Préférences générales**] , cochez la case [!UICONTROL **Désactiver la mise à niveau automatique dans les niveaux d’accès**] .
1. Cliquer sur [!UICONTROL **Enregistrer**].
