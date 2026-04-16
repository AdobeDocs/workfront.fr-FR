---
title: Joindre une carte tarifaire à un projet
description: Lorsque vous joignez une carte tarifaire à un projet, tous les rôles par emplacement et leurs taux de facturation associés sont ajoutés au projet.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 23%

---

# Joindre une carte tarifaire à un projet

Les cartes tarifaires stockent plusieurs taux de facturation par fonction, en fonction des attributs. Par exemple, vous pouvez avoir une fonction Designer basée à Paris pour l’agence A, une autre Designer basée à Paris pour l’agence B et une troisième Designer basée à New York non affectée à une agence, chacune avec des taux de facturation différents. Toutefois, les attributs ne sont pas obligatoires pour les fonctions sur une carte tarifaire. Les attributs servent d’outils pour établir des taux plus granulaires. Un taux de facturation sur une carte tarifaire peut également être valide pour une date effective, de sorte que le taux commence et se termine à des dates spécifiées.

Lorsque vous joignez une carte tarifaire à un projet, tous les rôles et leurs taux de facturation associés sont ajoutés au projet.

>[!NOTE]
>
>L’ajout d’une carte tarifaire remplace tous les taux de facturation par carte tarifaire existants pour le projet. Les remplacements de taux de facturation qui ont été ajoutés directement au projet ne sont pas supprimés.

Pour plus d’informations sur la création de cartes tarifaires, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Pour obtenir des informations générales sur le remplacement des taux de facturation des fonctions pour les projets et le calcul du revenu du projet, voir [Présentation du remplacement des taux de facturation et du calcul du revenu sur un projet](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Modifier l’accès aux projets, aux données financières et aux cartes tarifaires</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Gérez les autorisations du projet avec les autorisations de Modifier les taux de facturation</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Joindre une carte tarifaire à un projet

1. Accédez au projet.
1. Cliquez sur **Taux** dans le panneau de gauche, puis sélectionnez **Facturation**.
1. Cliquez sur **Ajouter un taux de facturation > Joindre une carte tarifaire**.

   La boîte de dialogue **Joindre une carte tarifaire** s’ouvre. Vous pouvez rechercher une carte tarifaire dans la liste.

   ![Joindre une boîte de carte tarifaire](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >Le groupe et l’entreprise figurant sur les cartes tarifaires sont utilisés comme filtres sur cette liste. Comme les projets incluent également des champs Groupe et Société, Workfront utilise ces valeurs pour limiter la liste des cartes tarifaires disponibles à celles qui correspondent au contexte du projet, et pas à toutes les cartes tarifaires du système.
   >
   >La correspondance n’a pas besoin d’être exacte. Des cartes tarifaires avec des valeurs Groupe et/ou Société vides peuvent toujours apparaître en fonction de la configuration Groupe/Société du projet. Par exemple, si un groupe est sélectionné pour un projet mais que l&#39;entreprise est vide, vous pouvez voir des cartes tarifaires associées à ce groupe même si l&#39;entreprise de la carte tarifaire est différente ou vide.

1. Sélectionnez la carte tarifaire à ajouter au projet et cliquez sur **Joindre**.

   La carte tarifaire et tous ses taux des fonctions sont ajoutés à la liste des taux de facturation.

   ![Carte tarifaire ajoutée au projet](assets/rate-card-on-project.png)

## Supprimer une carte tarifaire d’un projet

Lorsque vous supprimez une carte tarifaire d’un projet, tous ses taux de fonctions sont supprimés. Vous ne pouvez pas supprimer du projet un taux individuel provenant d’une carte tarifaire.

Les remplacements du taux de facturation pour les utilisateurs ou les fonctions qui ont été ajoutés directement au projet peuvent être supprimés sans supprimer la totalité de la carte tarifaire.

1. Accédez au projet.
1. Cliquez sur **Taux** dans le panneau de gauche, puis sélectionnez **Facturation**.
1. Cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/remove-icon.png).
1. Cliquez sur **Confirmer** dans le message de confirmation pour supprimer la carte tarifaire.

