---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Configurer les emplacements
description: Vous pouvez configurer les emplacements par défaut disponibles pour les affecter en tant qu’attributs aux fonctions dans des cartes tarifaires.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
source-git-commit: d0464b7f055b9351ba5c3353c7e806c51008e30b
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 26%

---

# Configurer les emplacements

{{preview-fast-release-general}}

Vous pouvez configurer les emplacements par défaut disponibles pour les affecter en tant qu’attributs aux fonctions dans des cartes tarifaires. Cela vous permet de vous assurer que les cartes tarifaires reflètent fidèlement les tarifs du marché dans chaque emplacement.

Les cartes tarifaires permettent à votre organisation de gérer facilement les taux de facturation pour les projets. Pour plus d’informations, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md) et [Définir des attributs de taux](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

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
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un emplacement

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Emplacements**].
1. Dans l’environnement de production, cliquez sur [!UICONTROL **Ajouter d’autres emplacements**] au bas de la liste.
   <span class="preview">Dans l’environnement Aperçu, cliquez sur [!UICONTROL **Nouvelle ligne**] au bas de la liste.</span>

1. Saisissez le nom et la description de l’emplacement.
1. Cliquez en dehors de la ligne pour enregistrer l’emplacement.
1. Pour supprimer un emplacement dans l’environnement de production, sélectionnez-le dans la liste et cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete.png).
   <span class="preview">Pour supprimer un emplacement dans l&#39;environnement Aperçu, sélectionnez-le dans la liste et cliquez sur [!UICONTROL **Supprimer**] dans la barre d&#39;actions située en bas de l&#39;écran.</span>

>[!NOTE]
>
>Les emplacements associés à des fonctions affectées sur une carte tarifaire ne peuvent pas être supprimés.

## Ajouter un sous-emplacement

Vous pouvez ajouter un sous-emplacement à un emplacement existant. Par exemple, si vous avez déjà un emplacement au Royaume-Uni, Londres peut être un sous-emplacement.

Trois niveaux de sous-emplacements sont autorisés. Le pays, l’État ou la province et la ville sont des utilisations courantes des sous-emplacements.

Chaque sous-emplacement peut être ajouté en tant qu’attribut sur une carte tarifaire de la même manière qu’un emplacement de niveau supérieur, afin de définir le taux pour une fonction spécifique à cet emplacement.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Emplacements**].
1. Dans l’environnement de production , sélectionnez un emplacement existant dans la liste, puis cliquez sur [!UICONTROL **Ajouter un sous-emplacement**].
   <span class="preview">Dans l’environnement Aperçu , sélectionnez un emplacement existant dans la liste, puis cliquez sur [!UICONTROL **Ajouter un sous-emplacement**] dans la barre d’actions située en bas de l’écran.</span>

1. Saisissez le nom et la description de l’emplacement.
1. Cliquez en dehors de la zone de saisie pour enregistrer l’emplacement.

   Le sous-emplacement est mis en retrait sous l’emplacement de niveau supérieur.

   Exemple d’image dans l’environnement de production :
   ![&#x200B; Emplacements et sous-emplacements &#x200B;](assets/locations-sublocations.png)

   <span class="preview">Exemple d’image dans l’environnement de prévisualisation :</span>
   ![&#x200B; Emplacements et sous-emplacements &#x200B;](assets/locations-sublocations-082526.png)


