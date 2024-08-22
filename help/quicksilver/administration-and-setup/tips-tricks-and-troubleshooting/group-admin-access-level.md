---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Les Administrateurs De Groupe Doivent Avoir Un Accès Plus Élevé Que Ceux Qu’Ils Gèrent
description: Si le niveau d’accès d’un administrateur de groupe est inférieur à celui qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 6%

---

# Les administrateurs et administratrices de groupes doivent avoir un accès plus élevé que les personnes sous leur responsabilité.

Si le niveau d’accès d’un administrateur de groupe est inférieur à celui qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.

## Problème

Si un administrateur de groupe se voit attribuer un niveau d’accès planificateur modifié avec les autorisations d’affichage pour les équipes, mais que certains utilisateurs se voient attribuer un niveau d’accès Worker avec les autorisations d’édition pour les équipes, l’administrateur de groupe ne pourra pas interagir avec le niveau d’accès Worker modifié.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Cette logique s’applique également au menu déroulant Régler vos paramètres . Les deux niveaux d’accès peuvent disposer de l’accès Modifier, mais les paramètres du menu déroulant Régler vos paramètres doivent être supérieurs pour l’administrateur du groupe.
> ![](assets/fine-tune-your-settings.png)

## Solution

Les administrateurs de groupe doivent disposer d’autorisations plus élevées dans toutes les zones du niveau d’accès que celles qu’ils gèrent.
