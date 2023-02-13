---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Les administrateurs de groupe doivent disposer d’un accès supérieur à celui qu’ils gèrent.
description: Si un administrateur de groupe dispose d’autorisations dont le niveau d’accès est inférieur à celui qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Les administrateurs de groupe doivent disposer d’un accès supérieur à celui qu’ils gèrent.

Si un administrateur de groupe dispose d’autorisations dont le niveau d’accès est inférieur à celui qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.

## Problème

Si un administrateur de groupe se voit attribuer un niveau d’accès planificateur modifié avec les autorisations d’affichage pour les équipes, mais que certains utilisateurs se voient attribuer un niveau d’accès Worker avec les autorisations d’édition pour les équipes, l’administrateur de groupe ne pourra pas interagir avec le niveau d’accès Worker modifié.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Cette logique s’applique également au menu déroulant Régler vos paramètres . Les deux niveaux d’accès peuvent disposer de l’accès Modifier, mais les paramètres du menu déroulant Régler vos paramètres doivent être supérieurs pour l’administrateur du groupe.
> ![](assets/fine-tune-your-settings.png)

## Solution

Les administrateurs de groupe doivent disposer d’autorisations plus élevées dans toutes les zones du niveau d’accès que celles qu’ils gèrent.