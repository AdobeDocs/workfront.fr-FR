---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Liste des objets avec un processus d’approbation en attente utilisant un certain état
description: Si vous essayez de supprimer un état, un message d’erreur peut vous indiquer qu’il ne peut pas être supprimé car il est utilisé dans les processus d’approbation en attente sur les objets de votre système. Si vous souhaitez rechercher et consulter ces objets afin de décider ce que vous devez faire, vous pouvez exécuter un rapport qui les répertorie.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Liste des objets dont le processus de validation est en attente avec un certain état

Si vous essayez de supprimer un état, un message d’erreur peut vous indiquer qu’il ne peut pas être supprimé, car il se trouve dans au moins un processus d’approbation en attente de votre système. Vous pouvez exécuter un rapport pour répertorier les objets dans un processus d’approbation en attente, puis décider de ce que vous devez faire pour chacun d’eux.

## En mode standard

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Rapport de projet**, **Rapport de tâche** ou **Rapport de problème**.
1. Ouvrez l’onglet **Filtres** .
1. Cliquez sur **Ajouter une règle de filtre**, puis procédez comme suit pour configurer la règle :
   1. Commencez à taper `status`, puis sélectionnez **Status** lors de son affichage.
   1. Laissez **Equal** dans le deuxième champ.
   1. Sélectionnez le nom du statut dans le troisième champ.
1. Cliquez de nouveau sur **Ajouter une règle de filtre**, puis procédez comme suit pour configurer la règle
   1. Commencez à saisir `pending status`, puis sélectionnez cet élément lorsqu’il s’affiche sous le type d’objet sur lequel vous recherchez (**Projet**, **Tâche** ou **Problème**).
   1. Laissez **Equal** dans le deuxième champ.
   1. Saisissez `in` dans le troisième champ.
1. Cliquez de nouveau sur **Ajouter une règle de filtre**, puis procédez comme suit pour configurer la règle
   1. Commencez à saisir le processus d’approbation, puis sélectionnez **ID de groupe** lorsqu’il s’affiche sous **Processus d’approbation**.
   1. Sélectionnez **Est vierge** dans le deuxième champ.
1. Cliquez sur **Enregistrer + Fermer** pour exécuter le rapport et répertorier tous les objets du type que vous avez spécifié avec les processus d’approbation à l’état en attente en fonction de l’état que vous avez spécifié (**Projet**, **Tâche** ou **Problème**).
1. Répétez ces étapes pour trouver les mêmes informations pour les deux autres types d’objets.


## En mode Texte

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Rapport de projet**, **Rapport de tâche** ou **Rapport de problème**.
1. Ouvrez l’onglet **Filtres** .
1. Sélectionnez **Passer en mode Texte**.
1. Copiez et collez les éléments suivants dans la fenêtre d’édition, en remplaçant XXX par la clé à 3 lettres pour l’état :

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Vous pouvez afficher la clé dans la liste des états, comme illustré dans ces articles :
   * [Accéder à la liste des états des projets système](project-statuses.md)
   * [Accéder à la liste des états des tâches système](task-statuses.md)
   * [Accéder à la liste des statuts des problèmes système](issue-statuses.md)

1. Cliquez sur **Enregistrer + Fermer** pour exécuter le rapport et répertorier tous les objets du type que vous avez spécifié avec les processus d’approbation à l’état en attente en fonction de l’état que vous avez spécifié (**Projet**, **Tâche** ou **Problème**).
1. Répétez ces étapes pour trouver les mêmes informations pour les deux autres types d’objets.
