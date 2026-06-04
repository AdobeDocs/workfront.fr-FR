---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Modifier en masse les autres groupes de l’utilisateur ou de l’utilisatrice
description: Lors de la modification en masse, j’ai tenté d’ajouter un seul Autre groupe à plusieurs personnes. Après l’enregistrement des modifications, tous les Autres groupes existants ont été supprimés et seul le nouveau groupe Autre Groupe est resté.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
TQID: https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 170
ht-degree: 55%

---

# Modifier en masse les autres groupes de l’utilisateur ou de l’utilisatrice

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture à l’intérieur d’[!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

## Problème :

Lors de la modification en masse, j’ai tenté d’ajouter un seul autre groupe à de nombreux utilisateurs.
Après avoir enregistré les modifications, tous les autres groupes existants ont été supprimés et seul le nouveau groupe Autre est resté.

## Réponse :

Le comportement qui en résulte dépend de l’appartenance actuelle à un groupe des personnes sélectionnées :

* Si tous les utilisateurs sélectionnés et les appartenances aux autres groupes correspondent exactement...
Après avoir sélectionné les utilisateurs et cliqué sur [!UICONTROL modifier], le champ [!UICONTROL Autres groupes] affiche la liste complète
de tous les groupes auxquels ces utilisateurs appartiennent.

* Si les utilisateurs sélectionnés ont des appartenances à d&#39;autres groupes différentes...
Une fois que vous avez sélectionné les utilisateurs et cliqué sur [!UICONTROL Modifier], le champ [!UICONTROL Autres groupes] est vide.

Lorsque vous cliquez sur **[!UICONTROL Enregistrer les modifications]**, tout ce qui apparaît dans le champ Autres groupes est enregistré.

Le contenu précédent du champ est remplacé.
