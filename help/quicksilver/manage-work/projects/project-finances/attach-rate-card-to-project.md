---
title: Joindre une carte tarifaire à un projet
description: Lorsque vous joignez une carte tarifaire à un projet, tous les rôles par emplacement et leurs taux de facturation associés sont ajoutés au projet.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 100%

---

# Joindre une carte tarifaire à un projet

{{highlighted-preview-article-level}}

Les cartes tarifaires stockent plusieurs taux de facturation par fonction, selon l’emplacement. Vous pourriez par exemple avoir une fonction de concepteur ou conceptrice basé à Paris et une seconde fonction de concepteur ou conceptrice basé à New York, avec des taux de facturation différents chacun. Toutefois, il n’est pas nécessaire d’indiquer un emplacement pour les fonctions figurant sur une carte tarifaire. Un taux de facturation pour une fonction (et éventuellement un emplacement) sur une carte tarifaire peut également inclure des dates d’entrée en vigueur.

Lorsque vous joignez une carte tarifaire à un projet, tous les rôles par emplacement et leurs taux de facturation associés sont ajoutés au projet.

>[!NOTE]
>
>Le fait de joindre une carte tarifaire remplace les taux de facturation existants sur le projet.

Vous pouvez modifier les taux de facturation à partir de la carte tarifaire directement dans le projet. Cela n’affecte pas les taux enregistrés sur la carte tarifaire par défaut.

Pour plus d’informations sur la création de cartes tarifaires, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Pour des informations générales sur la modification des taux de facturation des fonctions pour les projets et le calcul des revenus d’un projet, voir [Vue d’ensemble de la modification des taux de facturation des fonctions et du calcul des revenus d’un projet](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Standard</p><p>Ou</p><p>Formule héritée : Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux projets et aux données financières</p> <p>Accès administratif pour les fonctions</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour le projet avec les autorisations de gestion financière</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Joindre une carte tarifaire à un projet

1. Accédez au projet.
1. Cliquez sur **Taux de facturation** dans le panneau de gauche. Vous devrez peut-être d’abord cliquer sur **Afficher plus**.
1. Cliquez sur **Ajouter un taux de facturation > Joindre une carte tarifaire**.

   La page Joindre une carte tarifaire s’ouvre. Pour plus d’informations, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Sélectionnez la carte tarifaire à ajouter au projet et cliquez sur **Joindre**.

   La carte tarifaire et tous ses taux des fonctions sont ajoutés à la liste des taux de facturation.

   ![Carte tarifaire ajoutée au projet](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Dans la liste des taux de facturation, vous pouvez supprimer une ou plusieurs fonctions provenant d’une carte tarifaire. La suppression d’un taux de facturation d’une fonction dans le projet ne le supprime pas de la carte tarifaire par défaut.
