---
title: Joindre une carte tarifaire à un projet
description: Lorsque vous joignez une carte de taux à un projet, tous les rôles par emplacement et les taux de facturation associés sont ajoutés au projet.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 37%

---

# Joindre une carte tarifaire à un projet

{{highlighted-preview-article-level}}

Les cartes de taux stockent plusieurs taux de facturation par rôle de tâche, en fonction de l’emplacement. Vous pourriez avoir un concepteur basé à Paris et un second basé à New York, chacun ayant des des taux de facturation différents. L’emplacement n’est toutefois pas requis pour les fonctions sur une carte tarifaire. Un taux de facturation pour une fonction (et éventuellement un emplacement) sur une carte tarifaire peut également inclure des dates d’entrée en vigueur.

Lorsque vous joignez une carte de taux à un projet, tous les rôles par emplacement et les taux de facturation associés sont ajoutés au projet.

>[!NOTE]
>
>Le fait de joindre une carte de taux remplace les taux de facturation existants sur le projet.

Vous pouvez modifier les taux de facturation depuis la carte de taux directement dans le projet. Cela n’a aucune incidence sur les taux stockés sur la carte de taux par défaut.

Pour plus d’informations sur la création de cartes de taux, voir [Gestion des cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Pour obtenir des informations générales sur le remplacement des taux de facturation des rôles de tâche pour les projets et le calcul des recettes du projet, voir [Présentation du remplacement des taux de facturation des rôles de tâche et le calcul des recettes sur un projet](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Standard</p><p>Ou</p><p>Formule héritée : Planifier </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets et aux données financières</p> <p>Accès administratif pour les rôles de tâche</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations du projet avec les autorisations de gestion financière</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Joindre une carte tarifaire à un projet

1. Accédez au projet.
1. Cliquez sur **Taux de facturation** dans le panneau de gauche. Vous devrez peut-être d’abord cliquer sur **Afficher plus**.
1. Cliquez sur **Ajouter un taux de facturation > Joindre une carte de taux**.

   La page Joindre une carte de taux s’affiche. Pour plus d’informations, voir [Gestion des cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Sélectionnez la carte de taux à ajouter au projet, puis cliquez sur **Joindre**.

   La carte de taux et tous ses taux de rôle de tâche sont ajoutés à la liste des taux de facturation.

   ![Carte de taux ajoutée au projet](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Dans la liste des taux de facturation, vous pouvez supprimer un ou plusieurs rôles de tâche provenant d’une carte de taux. La suppression d’un taux de facturation de rôle de tâche du projet ne le supprime pas de la carte de taux par défaut.
