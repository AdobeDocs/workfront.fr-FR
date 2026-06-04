---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Les Administrateurs De Groupe Doivent Disposer D’Un Accès Supérieur À Celui Qu’Ils Gèrent
description: Si un administrateur de groupes dispose d’autorisations de niveau d’accès inférieur à celles qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 157
ht-degree: 47%

---

# Les administrateurs et administratrices de groupe doivent avoir un accès plus élevé que ceux qu’ils gèrent.

Si un administrateur de groupes dispose d’autorisations de niveau d’accès inférieur à celles qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.

## Problème

Si une personne chargée de l’administration de groupes se voit attribuer un niveau d’accès planificateur modifié avec les autorisations d’affichage pour les équipes, mais que certains utilisateurs et utilisatrices reçoivent un niveau d’accès travail avec les autorisations de modification pour les équipes, elle ne pourra pas interagir avec le niveau d’accès travail modifié.

![Accès modifié par l’administrateur de groupe](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Cette logique s’applique également au menu déroulant Ajuster vos paramètres . Les deux niveaux d’accès peuvent avoir un accès en modification, mais les paramètres du menu déroulant Affiner vos paramètres doivent être plus élevés pour l’administrateur de groupe.
> ![Ajuster vos paramètres](assets/fine-tune-your-settings.png)

## Solution

Les administrateurs et administratrices de groupes doivent disposer d’autorisations plus élevées dans toutes les zones du niveau d’accès que celles qu’ils gèrent.
