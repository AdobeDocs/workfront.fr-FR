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
ht-degree: 62%

---

# Les administrateurs et administratrices de groupe doivent avoir un accès plus élevé que ceux qu’ils gèrent.

Si le niveau d’accès d’un administrateur de groupe est inférieur à celui qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.

## Problème

Si une personne chargée de l’administration de groupes se voit attribuer un niveau d’accès planificateur modifié avec les autorisations d’affichage pour les équipes, mais que certains utilisateurs et utilisatrices reçoivent un niveau d’accès travail avec les autorisations de modification pour les équipes, elle ne pourra pas interagir avec le niveau d’accès travail modifié.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Cette logique s’applique également au menu déroulant Ajuster vos paramètres. Les deux niveaux d’accès peuvent disposer de l’accès en modification, mais les paramètres du menu déroulant Ajuster vos paramètres doivent être supérieurs pour l’administrateur ou l’administratrice de groupes.
> ![](assets/fine-tune-your-settings.png)

## Solution

Les administrateurs et administratrices de groupes doivent disposer d’autorisations plus élevées dans toutes les zones du niveau d’accès que celles qu’ils gèrent.
