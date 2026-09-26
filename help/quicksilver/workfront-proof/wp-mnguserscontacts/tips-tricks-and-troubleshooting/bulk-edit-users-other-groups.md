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
TQID: 'https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 67%
---
# Modifier en masse les autres groupes de l’utilisateur ou de l’utilisatrice

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture à l’intérieur d’[!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

## Problème :

Lors de la modification en masse, j’ai tenté d’ajouter un seul Autre groupe à plusieurs personnes.
Après l’enregistrement des modifications, tous les Autres groupes existants ont été supprimés et seul le nouveau groupe Autre Groupe est resté.

## Réponse :

Le comportement qui en résulte dépend de l’appartenance actuelle à un groupe des personnes sélectionnées :

* Si tous les utilisateurs sélectionnés et les appartenances aux autres groupes correspondent exactement...
Après avoir sélectionné les utilisateurs et cliqué sur [!UICONTROL modifier], le champ [!UICONTROL Autres groupes] affiche la liste complète
de tous les groupes auxquels ces utilisateurs appartiennent.

* Si les utilisateurs sélectionnés ont des appartenances à d&#39;autres groupes différentes...
Une fois que vous avez sélectionné les utilisateurs et cliqué sur [!UICONTROL Modifier], le champ [!UICONTROL Autres groupes] est vide.

Lorsque vous cliquez sur **[!UICONTROL Enregistrer les modifications]**, tout ce qui apparaît dans le champ Autres groupes est enregistré.

Le contenu précédent du champ est remplacé.
