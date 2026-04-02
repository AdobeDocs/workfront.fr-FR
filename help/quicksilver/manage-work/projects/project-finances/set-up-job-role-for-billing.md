---
content-type: overview
product-area: projects
navigation-topic: financials
title: Configurer une fonction pour la facturation
description: Workfront vous permet de facturer un utilisateur sous une fonction différente de sa fonction principale. Cela s’avère utile lorsqu’une personne effectue temporairement un travail qui doit être facturé à un taux différent.
author: Lisa
feature: Work Management
source-git-commit: d92908d358ca53ae9d443fd76556e3e8b273e3cb
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 6%

---

# Configurer une fonction pour la facturation

{{highlighted-preview-article-level}}

Workfront vous permet de facturer un utilisateur sous une fonction différente de sa fonction principale. Cela s’avère utile lorsqu’une personne effectue temporairement un travail qui doit être facturé à un taux différent.

Vous pouvez affecter une fonction à la facturation de deux manières :

* Au niveau du projet : utilisez cette option lorsque la personne doit être facturée pour la même fonction pour l’ensemble du projet.
* Au niveau de l’affectation : utilisez cette option lorsque vous souhaitez facturer différemment des tâches spécifiques.

>[!NOTE]
>
>* Une fonction pour la facturation s’applique uniquement aux personnes (utilisateurs). Elle ne s’applique pas aux fonctions génériques ni aux espaces réservés.
>* L’ajout d’une fonction pour la facturation affecte uniquement le taux de facturation, et non le coût.
>* La facturation au niveau de l’affectation a toujours la priorité sur la facturation au niveau du projet.

Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) et [Créer des affectations avancées](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

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
   <td> Modifier l’accès aux cartes tarifaires</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Autorisations de gestion pour le projet </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Affecter une fonction pour la facturation au niveau du projet

Lorsque vous créez une fonction pour la facturation d’un projet :

* Le rôle de facturation s’applique à toutes les tâches et affectations au sein du projet pour cet utilisateur.
* La facturation utilise le taux de facturation de la fonction sélectionnée, mais le coût suit toujours le rôle principal de l’utilisateur.

Pour affecter une fonction à la facturation au niveau du projet :

1. Ouvrez un projet.
1. Cliquez sur **Ressource pour la facturation** dans le panneau de gauche.
1. Sélectionnez l’onglet **Fonction pour la facturation** s’il n’est pas déjà affiché.
1. Cliquez sur **Ajouter > Ajouter une fonction pour la facturation**.
1. Dans la zone **Ajouter une fonction pour la facturation**, sélectionnez l’**Utilisateur**.
1. Sélectionnez la **Fonction** à utiliser comme fonction pour la facturation de cet utilisateur pour ce projet.
1. (Facultatif) Cliquez sur **Ajouter une fonction** pour définir les dates d’entrée en vigueur de la fonction pour la facturation. Saisissez les dates **Début** et **Fin** pour la fonction.

[Ajouter une fonction pour la facturation au niveau du projet](assets/jrfb-project-level.png)

1. Cliquez de nouveau sur **Ajouter une fonction** pour spécifier des rôles de facturation supplémentaires pour différentes périodes.
1. Cliquez sur **Enregistrer**.

### Exemple au niveau du projet

>[!BEGINSHADEBOX]

La fonction principale de John est Designer 1. Le projet nécessite un Senior Designer, et John est en train de le remplacer.

Définissez la fonction pour la facturation sur **Senior Designer** au niveau du projet.

Résultat :

* Le chiffre d’affaires de facturation est le taux de Senior Designer
* Le coût correspond au taux de coût de Designer 1 (taux de coût réel de John).

>[!ENDSHADEBOX]

## Affecter une fonction pour la facturation au niveau de l&#39;affectation

Lorsque vous ajoutez une fonction pour la facturation d’une affectation, le paramètre remplace un rôle de facturation au niveau du projet pour cette affectation spécifique uniquement.

Pour affecter une fonction pour la facturation au niveau affectation :

1. Ouvrez un projet et localisez la tâche.
1. Accédez au **Affectations avancées** de la tâche.

   Pour plus d&#39;informations, voir [Créer des affectations avancées](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Dans la grille d’affectation de tâche, recherchez la colonne **Fonction pour la facturation**.
1. Sélectionnez une fonction pour chaque affectation pour laquelle vous souhaitez une facturation différente.

   >[!NOTE]
   >
   >Si une fonction pour la facturation a été affectée au niveau du projet, elle apparaît sur l’affectation. Vous pouvez cliquer dans le champ **Fonction pour la facturation** et sélectionner une autre fonction à utiliser pour l’affectation.
   >L’icône d’information vous indique si une fonction pour la facturation a été définie au niveau du projet ou de l’affectation.

   ![Fonction de facturation pour une affectation](assets/jrfb-assignment-level.png)

### Exemple au niveau de l&#39;affectation

>[!BEGINSHADEBOX]

La fonction principale de John est Designer 1. Il est facturé en tant que Senior Designer au niveau du projet, mais il existe une tâche spéciale nécessitant un taux de facturation de Principal Designer.

Définissez la fonction pour la facturation au Designer principal sur cette affectation uniquement.

Résultat :

* Toutes les autres tâches de John sont facturées comme Senior Designer
* Cette tâche unique est facturée comme Designer principale
* Le coût reste Designer 1

>[!ENDSHADEBOX]
