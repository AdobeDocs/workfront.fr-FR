---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Liste des objets dont le traitement de validation est en attente avec un certain état
description: Si vous essayez de supprimer un état, un message d’erreur peut vous indiquer qu’il ne peut pas être supprimé car il est utilisé dans les processus d’approbation en attente sur les objets de votre système. Si vous souhaitez rechercher et consulter ces objets afin de décider ce que vous devez faire, vous pouvez exécuter un rapport qui les répertorie.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Liste des objets dont le traitement de validation est en attente avec un certain état

Si vous essayez de supprimer un état, un message d’erreur peut vous indiquer qu’il ne peut pas être supprimé, car il se trouve dans au moins un processus d’approbation en attente de votre système. Vous pouvez exécuter un rapport pour répertorier les objets dans un processus d’approbation en attente, puis décider de ce que vous devez faire pour chacun d’eux.

## En mode standard

1. Accédez au **Reporting** dans la barre de navigation globale, puis sélectionnez l’option **Rapports** .
1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Rapport de projet**, **Rapport de tâches** ou **Rapport de problème**.
1. Ouvrez le **Filtres** .
1. Cliquez sur **Ajouter une règle de filtre**, puis procédez comme suit pour configurer la règle :
   1. Commencez à taper `status`, puis sélectionnez **État** lorsqu’elle s’affiche.
   1. Laissez tomber **Égal** dans le deuxième champ.
   1. Sélectionnez le nom du statut dans le troisième champ.
1. Cliquez sur **Ajouter une règle de filtre** à nouveau, procédez comme suit pour configurer la règle
   1. Commencez à taper `pending status`, puis sélectionnez cet élément lorsqu’il s’affiche sous le type d’objet sur lequel vous regardez (**Projet**, **Tâche** ou **Problème**).
   1. Laissez tomber **Égal** dans le deuxième champ.
   1. Type `in` dans le troisième champ.
1. Cliquez sur **Ajouter une règle de filtre** à nouveau, procédez comme suit pour configurer la règle
   1. Commencez le processus d’approbation de la saisie, puis sélectionnez **ID de groupe** s’affiche sous **Processus d’approbation**.
   1. Sélectionner **Est vierge** dans le deuxième champ.
1. Cliquez sur **Enregistrer + Fermer** pour exécuter le rapport et répertorier tous les objets du type que vous avez spécifié avec les processus de validation dans l’état en attente en fonction de l’état que vous avez spécifié (**Projet**, **Tâche** ou **Problème**).
1. Répétez ces étapes pour trouver les mêmes informations pour les deux autres types d’objets.


## En mode Texte

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Rapport de projet**, **Rapport de tâches** ou **Rapport de problème**.
1. Ouvrez le **Filtres** .
1. Sélectionner **Passer en mode Texte**.
1. Copiez et collez les éléments suivants dans la fenêtre d’édition, en remplaçant XXX par la clé à 3 lettres pour l’état :

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Vous pouvez afficher la clé dans la liste des états, comme illustré dans ces articles :
   * [Accéder à la liste des états du projet système](project-statuses.md)
   * [Accéder à la liste des états des tâches système](task-statuses.md)
   * [Accéder à la liste des statuts des problèmes système](issue-statuses.md)

1. Cliquez sur **Enregistrer + Fermer** pour exécuter le rapport et répertorier tous les objets du type que vous avez spécifié avec les processus de validation dans l’état en attente en fonction de l’état que vous avez spécifié (**Projet**, **Tâche** ou **Problème**).
1. Répétez ces étapes pour trouver les mêmes informations pour les deux autres types d’objets.
