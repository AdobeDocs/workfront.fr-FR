---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Modifier l’historique
description: L’historique des modifications vous permet d’afficher un journal des modifications apportées aux objets Workfront
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 44292bc9cf8654d1ecfb398b0f118a6c001f544f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 8%

---

# Affichage et gestion de l’historique des modifications

Vous pouvez afficher l’historique des modifications, y compris les journaux d’audit, dans la zone Suivi des modifications de la configuration.

* Les **journaux d’audit** sont des modifications déclenchées par les utilisateurs.
Pour plus d’informations sur les journaux d’audit et la zone Journaux d’audit, consultez [Présentation des journaux d’audit](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)
* **Configuration** affiche les champs qui font l’objet d’un suivi pour la liste Historique des modifications.
La configuration n’est actuellement disponible que comme information et ne peut pas être modifiée. La possibilité de modifier les champs suivis sera disponible dans un avenir proche.
* La liste Historique des modifications vous permet d’afficher un journal des modifications apportées aux objets Workfront, y compris les attributs tels que :

   * Objet
   * Type d’objet
   * Type de modification (opération)
   * Source de la modification, comme des utilisateurs spécifiques, des API, Workfront Fusion, des LLM d’IA ou le système Workfront

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur Workfront pour afficher l’historique des modifications</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Affichage et gestion des journaux d’audit

Pour afficher et gérer les journaux d’audit, voir [Afficher et exporter les journaux d’audit](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Afficher la zone Configuration pour le suivi des modifications

>[!NOTE]
>
>La configuration n’est actuellement disponible que comme information et ne peut pas être modifiée. La possibilité de modifier les champs suivis sera disponible dans un avenir proche.

Pour afficher les types de modifications qui font l’objet d’un suivi :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Suivi des modifications** ![Icône Modifier l’historique](assets/change-history-icon.png).
1. Cliquez sur **Configuration**.

   Les champs s’affichent regroupés par type d’objet.

1. Pour afficher les champs sous un objet spécifique, cliquez sur la flèche de liste déroulante en regard du type d’objet.

## Afficher la liste Historique des modifications

Les administrateurs et administratrices de Workfront peuvent afficher l’historique des modifications dans la zone Configuration .

La liste Historique des modifications est une liste améliorée comprenant des filtres, des colonnes, une hauteur de ligne, un sélecteur de date et une barre de recherche.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Suivi des modifications** ![Icône Modifier l’historique](assets/change-history-icon.png).
1. Cliquez sur **Modifier la liste d’historique**.

   La liste Historique des modifications s’ouvre.

1. Pour ajuster les dates pour lesquelles des modifications s’affichent, cliquez sur le sélecteur de date et sélectionnez les nouvelles dates.

   Les modifications sont disponibles pour les 90 derniers jours.
1. Pour rechercher un terme spécifique, cliquez sur la barre de recherche et saisissez le terme. Les résultats sont filtrés au fur et à mesure que vous tapez.
1. (Facultatif) Pour filtrer selon une colonne, reportez-vous à la section [Filtrer les éléments dans une liste améliorée](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) de l’article Utilisation de listes améliorées.
1. (Facultatif) Pour masquer, afficher ou réorganiser des colonnes, consultez la section [Personnaliser les colonnes](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) dans l’article Utilisation de listes améliorées.
1. Pour ajouter ou supprimer des colonnes, reportez-vous à la section [Ajouter et supprimer des colonnes à l’aide du gestionnaire de colonnes](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) de l’article Utilisation de listes améliorées.
1. Pour ajuster la hauteur de ligne, voir [Modifier la hauteur de ligne dans une vue](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) dans l’article Utilisation de listes améliorées.





