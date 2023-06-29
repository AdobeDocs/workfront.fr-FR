---
title: Joindre une carte de taux à un projet
description: Lorsque vous joignez une carte de taux à un projet, tous les rôles par emplacement et les taux de facturation associés sont ajoutés au projet.
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Joindre une carte de taux à un projet

{{highlighted-preview-article-level}}

Les cartes de taux stockent plusieurs taux de facturation par rôle de tâche, en fonction de l’emplacement. Vous pourriez avoir un rôle professionnel de Designer basé à Paris et un second basé à New York, chacun avec des taux de facturation différents. Cependant, un emplacement n’est pas requis pour les rôles de tâche sur une carte de taux. Un taux de facturation pour un rôle de tâche (et éventuellement un emplacement) sur une carte de taux peut également inclure des dates d’entrée en vigueur.

Lorsque vous joignez une carte de taux à un projet, tous les rôles par emplacement et les taux de facturation associés sont ajoutés au projet.

>[!NOTE]
>
>Le fait de joindre une carte de taux remplace les taux de facturation existants sur le projet.

Vous pouvez modifier les taux de facturation depuis la carte de taux directement dans le projet. Cela n’a aucune incidence sur les taux stockés sur la carte de taux par défaut.

Pour plus d’informations sur la création de cartes de taux, voir [Gestion des cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Pour obtenir des informations générales sur le remplacement des taux de facturation des rôles de tâche pour les projets et le calcul des recettes d’un projet, voir [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Standard</p><p>Ou</p><p>Plan hérité : Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets et aux données financières</p> <p>Accès administratif pour les rôles de tâche</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations du projet avec les autorisations de gestion financière</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Joindre une carte de taux à un projet

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

