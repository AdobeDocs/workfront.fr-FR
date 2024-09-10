---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gestion des cartes de taux
description: Les cartes tarifaires vous permettent de définir plusieurs taux de facturation par rôle, en fonction de l’emplacement.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 99%

---

# Gérer les cartes tarifaires

{{highlighted-preview-article-level}}

Les cartes tarifaires vous permettent de définir plusieurs taux de facturation par rôle, en fonction de l’emplacement. Vous pourriez par exemple avoir une fonction de concepteur ou conceptrice basé à Paris et une seconde fonction de concepteur ou conceptrice basé à New York, avec des taux de facturation différents chacun. Toutefois, il n’est pas nécessaire d’indiquer un emplacement pour les fonctions figurant sur une carte tarifaire. Un taux de facturation pour une fonction (et éventuellement un emplacement) sur une carte tarifaire peut également inclure des dates d’entrée en vigueur.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Modifier l’accès aux [!UICONTROL Financial Data]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Pour modifier une carte tarifaires partagée avec vous, vous devez disposer des autorisations Gérer sur la carte tarifaire.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter une carte tarifaire

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Cartes tarifaires**].
1. Cliquez sur [!UICONTROL **Nouvelle carte tarifaire**], puis saisissez le nom de la carte tarifaire dans la zone [!UICONTROL Nouvelle carte tarifaire] pour remplacer « Carte tarifaire sans titre ».
1. (Facultatif) Sur l’écran Détails de la carte tarifaire, ajoutez une [!UICONTROL **Description**].
1. (Facultatif) Pour joindre un formulaire personnalisé à la carte tarifaire, cliquez sur le champ [!UICONTROL **Ajouter un formulaire personnalisé**] dans le coin supérieur droit et sélectionnez un formulaire personnalisé dans la liste qui s’affiche.

   Pour plus d’informations sur l’ajout d’un formulaire personnalisé, voir [Ajouter un formulaire personnalisé à un objet](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Cliquez sur [!UICONTROL **Rôles et tarifs du poste**] dans le panneau de navigation de gauche.
1. Sur l’écran Rôles et tarifs du poste de carte tarifaire, cliquez sur [!UICONTROL **Ajouter une fonction**].
1. Dans la boîte de dialogue, sélectionnez une [!UICONTROL **Fonction**] pour laquelle définir des taux de facturation.

   Le taux de facturation par défaut affiche le taux au niveau du système pour cette fonction, le cas échéant.

   ![Boîte de dialogue du nouveau taux de facturation](assets/location-rate-for-rate-card.png)

1. Sélectionnez une [!UICONTROL **Devise**] pour la fonction.
1. (Facultatif) Sélectionnez un [!UICONTROL **Emplacement**] pour la fonction.
1. Dans le champ [!UICONTROL **Taux de facturation 1**], saisissez le taux de facturation pour l’emplacement. Cliquez ensuite sur [!UICONTROL **Enregistrer**] pour remplacer une fois le taux de facturation.

   Ou

   Cliquez sur [!UICONTROL **Ajouter un taux**] pour ajouter d’autres taux de facturation spécifique à l’emplacement avec des dates de validité.

1. (Le cas échéant) Si vous ajoutez plusieurs taux de facturation pour cet emplacement, saisissez les informations suivantes :

   * **[!UICONTROL Taux de facturation 1], 2, etc.** : valeur du taux de facturation pour la période.
   * **[!UICONTROL Date de début] :** date à laquelle le remplacement de taux commence.
   * **[!UICONTROL Date de fin] :** date à laquelle le remplacement de taux se termine.

     Le taux de facturation 1 ne comporte pas de date de début de validité et le dernier taux de facturation n’a pas de date de fin de validité. Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin de validité et que vous ajoutez le taux de facturation 2 avec une date de début de validité le 1er mai 2023, une date de fin de validité au 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait pas d’écart.

1. Cliquer sur [!UICONTROL **Enregistrer**].
1. (Facultatif) Pour ajouter un autre taux de facturation, soit pour la même fonction à un autre emplacement, soit pour une fonction distincte, cliquez sur [!UICONTROL **Ajouter fonction**].
1. (Facultatif) Pour modifier une carte tarifaire, cliquez sur le nom de la carte tarifaire dans la liste Cartes tarifaires, dans Configuration. Pour modifier un taux de facturation, cliquez sur [!UICONTROL **Rôles et tarifs du poste**] dans le panneau de navigation de gauche de la carte tarifaire. Sélectionnez ensuite le taux et cliquez sur l’icône **Modifier** ![Icône Modifier](assets/edit-icon.png).

## Copier une carte tarifaire

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte tarifaire**].
1. Cochez la case en regard de la carte tarifaire dans la liste et cliquez sur l’icône **Copier** ![Icône Copier](assets/copy-icon.png).
1. Saisissez le nom de la carte tarifaire dans la zone [!UICONTROL Copier la carte tarifaire] pour remplacer « Untitled Rate Card ». Cliquez ensuite **Enregistrer**.

   La nouvelle carte tarifaire est enregistrée. Modifiez les détails de la carte tarifaire, les fonctions et les taux selon les besoins.

## Supprimer une carte tarifaire entière

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte tarifaire**].
1. Cochez la case en regard de la carte tarifaire dans la liste, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete.png).

   >[!NOTE]
   >
   >Une carte tarifaire associée à un projet sera supprimée du projet.
