---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Modification en masse des autres groupes de l’utilisateur
description: Lors de la modification en masse, j’ai tenté d’ajouter un seul groupe Autres à de nombreux utilisateurs. Après l’enregistrement des modifications, tous les autres groupes existants ont été supprimés et seul le nouveau groupe Autres restait.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Modification en masse des autres groupes de l’utilisateur

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

## Problème :

Lors de la modification en masse, j’ai tenté d’ajouter un seul groupe Autres à de nombreux utilisateurs.
Après l’enregistrement des modifications, tous les autres groupes existants ont été supprimés et seul le nouveau groupe Autres restait.

## Réponse :

Le comportement qui en résulte dépend de l’appartenance actuelle au groupe des utilisateurs sélectionnés :

* Si tous les utilisateurs sélectionnés correspondent exactement aux membres Autres groupes... Après avoir sélectionné les utilisateurs, sélectionnez [!UICONTROL edit], la variable [!UICONTROL Autres groupes] affiche la liste complète de tous les groupes auxquels ces utilisateurs appartiennent.

* Si les utilisateurs sélectionnés ont des appartenances Autres groupes différentes... Après avoir sélectionné les utilisateurs, cliquez sur [!UICONTROL Modifier], la variable [!UICONTROL Autres groupes] est vide.

Lorsque vous cliquez sur **[!UICONTROL Enregistrer les modifications]**, tout ce qui apparaît dans le champ Autres groupes est enregistré.

Le contenu précédent du champ est remplacé.
