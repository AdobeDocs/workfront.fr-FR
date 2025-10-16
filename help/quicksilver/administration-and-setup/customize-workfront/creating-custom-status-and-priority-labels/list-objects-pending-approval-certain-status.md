---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Répertorier les objets avec un processus d'approbation en attente utilisant un certain statut
description: Si vous essayez de supprimer un statut, un message d’erreur peut vous indiquer qu’il ne peut pas être supprimé, car il est utilisé dans les processus d’approbation en attente sur les objets de votre système.Si vous souhaitez rechercher et consulter ces objets afin de décider des actions appropriées, vous pouvez exécuter un rapport qui les répertorie.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 89%

---

# Répertorier les objets avec un processus d&#39;approbation en attente utilisant un certain statut

Si vous essayez de supprimer un statut, un message d’erreur peut vous informer qu’il ne peut pas être supprimé, car il se trouve dans au moins un processus d’approbation en attente dans votre système.Vous pouvez exécuter un rapport pour répertorier les objets dans un processus d’approbation en attente, puis décider de ce que vous devez faire pour chacun d’eux.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
     <p>Standard</p>
     <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td><p>Accès en modification aux rapports, tableaux de bord et calendriers</p><p>Modifier l’accès aux filtres, vues et groupes</p></td>
  </tr>
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Vous obtenez des autorisations de gestion pour les rapports que vous créez.</td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## En mode standard

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Rapport de projet**, **Rapport de tâche** ou **Rapport de problème**.
1. Ouvrez l’onglet **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**, puis procédez comme suit pour configurer la règle :
   1. Commencez à saisir `status`, puis sélectionnez **Statut** lorsqu’il s’affiche.
   1. Laissez **Égal** dans le deuxième champ.
   1. Sélectionnez le nom du statut dans le troisième champ.
1. Cliquez à nouveau sur **Ajouter une règle de filtre**, et procédez comme suit pour configurer la règle.
   1. Commencez à saisir `pending status`, puis sélectionnez cet élément lorsqu’il s’affiche sous le type d’objet que vous recherchez (**Projet**, **Tâche** ou **Problème**).
   1. Laissez **Égal** dans le deuxième champ.
   1. Saisissez `in` dans le troisième champ.
1. Cliquez à nouveau sur **Ajouter une règle de filtre**, et procédez comme suit pour configurer la règle.
   1. Commencez à saisir le processus d’approbation, puis sélectionnez **ID de groupe** lorsqu’il s’affiche sous **Processus d’approbation**.
   1. Sélectionnez **Est vide** dans le deuxième champ.
1. Cliquez sur **Enregistrer et fermer** pour exécuter le rapport et répertorier tous les objets du type que vous avez spécifié avec les processus d’approbation avec le statut en attente en fonction du statut que vous avez spécifié (**Projet**, **Tâche** ou **Problème**).
1. Répétez ces étapes pour trouver les mêmes informations pour les deux autres types d’objets.


## En mode texte

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Rapport de projet**, **Rapport de tâche** ou **Rapport de problème**.
1. Ouvrez l’onglet **Filtres**.
1. Sélectionnez **Basculer en mode texte**.
1. Copiez et collez les éléments suivants dans la fenêtre de modification, en remplaçant XXX par la clé à 3 lettres pour le statut :

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Vous pouvez afficher la clé dans la liste des statuts, comme illustré dans ces articles :
   * [Accéder à la liste des statuts des projets du système](project-statuses.md)
   * [Accéder à la liste des statuts des tâches du système](task-statuses.md)
   * [Accéder à la liste des statuts des problèmes du système](issue-statuses.md)

1. Cliquez sur **Enregistrer et fermer** pour exécuter le rapport et répertorier tous les objets du type que vous avez spécifié avec les processus d’approbation avec le statut en attente en fonction du statut que vous avez spécifié (**Projet**, **Tâche** ou **Problème**).
1. Répétez ces étapes pour trouver les mêmes informations pour les deux autres types d’objets.
