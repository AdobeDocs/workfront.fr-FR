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
TQID: 'https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 58%
---
# Les administrateurs et administratrices de groupe doivent avoir un accès plus élevé que ceux qu’ils gèrent.

Si un administrateur de groupes dispose d’autorisations de niveau d’accès inférieur à celles qu’il gère, il ne pourra pas afficher, modifier ni attribuer de niveaux d’accès inférieurs.

## Problème

Si une personne chargée de l’administration de groupes se voit attribuer un niveau d’accès planificateur modifié avec les autorisations d’affichage pour les équipes, mais que certains utilisateurs et utilisatrices reçoivent un niveau d’accès travail avec les autorisations de modification pour les équipes, elle ne pourra pas interagir avec le niveau d’accès travail modifié.

![Accès modifié par l’administrateur de groupe](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Cette logique s’applique également au menu déroulant Ajuster vos paramètres. Les deux niveaux d’accès peuvent disposer de l’accès en modification, mais les paramètres du menu déroulant Ajuster vos paramètres doivent être supérieurs pour l’administrateur ou l’administratrice de groupes.
> ![Ajustez vos paramètres](assets/fine-tune-your-settings.png)

## Solution

Les administrateurs et administratrices de groupes doivent disposer d’autorisations plus élevées dans toutes les zones du niveau d’accès que celles qu’ils gèrent.
