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
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 47%

---

# Configurer les emplacements

Vous pouvez configurer les emplacements par défaut disponibles pour les affecter en tant qu’attributs aux fonctions dans des cartes tarifaires. Cela vous permet de vous assurer que les cartes tarifaires reflètent fidèlement les tarifs du marché dans chaque emplacement.

Les cartes tarifaires permettent à votre organisation de gérer facilement les taux de facturation pour les projets. Pour plus d’informations, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

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
1. Cliquez sur [!UICONTROL **Ajouter d’autres emplacements**] au bas de la liste.
1. Saisissez le nom et la description de l’emplacement.
1. Cliquez en dehors de la zone de saisie pour enregistrer l’emplacement.
1. Pour supprimer un emplacement, sélectionnez-le dans la liste et cliquez sur l’icône **Supprimer** ![icône Supprimer](assets/delete.png).

>[!NOTE]
>
>Les emplacements associés à des fonctions affectées sur une carte tarifaire ne peuvent pas être supprimés.

## Ajouter un sous-emplacement

Vous pouvez ajouter un sous-emplacement à un emplacement existant. Par exemple, si vous avez déjà un emplacement au Royaume-Uni, Londres peut être un sous-emplacement.

Trois niveaux de sous-emplacements sont autorisés. Le pays, l’État ou la province et la ville sont des utilisations courantes des sous-emplacements.

Chaque sous-emplacement peut être ajouté en tant qu’attribut sur une carte tarifaire de la même manière qu’un emplacement de niveau supérieur, afin de définir le taux pour une fonction spécifique à cet emplacement.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Emplacements**].
1. Sélectionnez un emplacement existant dans la liste et cliquez sur **Ajouter un sous-emplacement**.
1. Saisissez le nom et la description de l’emplacement.
1. Cliquez en dehors de la zone de saisie pour enregistrer l’emplacement.

   Le sous-emplacement est mis en retrait sous l’emplacement de niveau supérieur.

   ![&#x200B; Emplacements et sous-emplacements &#x200B;](assets/locations-sublocations.png)


