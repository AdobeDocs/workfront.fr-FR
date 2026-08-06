---
title: Utiliser les collaborateurs de la tâche
content-type: reference
description: Découvrez comment utiliser les collaborateurs de tâches, des collaborateurs d’IA qui peuvent être affectés à des tâches Workfront.
author: Becky
feature: Work Management, Tasks
source-git-commit: 2070a27e18d768dd14ce4f5c681ab08669c81766
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 8%

---

# Utiliser les collaborateurs de la tâche

{{highlighted-preview-article-level}}

Les collaborateurs de tâches sont des collaborateurs de l’IA qui peuvent être affectés directement à des tâches Workfront, en plus du collaborateur de l’IA de type réviseur existant utilisé pour les révisions de documents et de ressources. Comme les autres collaborateurs de l’IA, les collaborateurs de tâches sont configurés dans la zone Configuration et affectés à des tâches comme un utilisateur.

Les collaborateurs de tâches se connectent aux agents que vous avez configurés, à l’instar d’un serveur MCP.

Pour plus d’informations et d’instructions sur la création d’un espace de collaboration dans Workfront, consultez [Configurer un espace de collaboration de tâche](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) dans l’article Configurer des espaces de collaboration IA.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Select, Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

* Vous devez configurer un agent dans Copilote, Claude ou Writer.ai avant de pouvoir l&#39;utiliser comme collaborateur de tâches.

## Vue d&#39;ensemble de Task Collaborator

Les collaborateurs de tâches permettent d’affecter des agents MCP à des tâches spécifiques dans Workfront. Vous configurez l’agent dans une application telle que Copilot Studio, Claude ou Writer.ai, puis vous connectez cet agent à Workfront en tant que collaborateur de la tâche. Vous pouvez ensuite l’affecter à des tâches comme vous le feriez pour un utilisateur.

Voici quelques exemples de workflows :

* Détecter les images chargées dans une tâche, générer les variations en fonction des critères donnés à l’agent et charger les nouvelles images dans la tâche.
* Générer une copie à partir d’une description de tâche, vérifier la copie par rapport aux directives configurées dans l’agent et publier la copie dans le flux de mise à jour.
* Lecture des détails d’un événement, identification des détails manquants et publication de questions sur les détails manquants dans le flux de mise à jour.

>[!NOTE]
>
>* Les détails spécifiques relatifs aux responsabilités et capacités d’un agent sont configurés dans l’application dans laquelle l’agent est créé, et non dans Workfront.
>* Les collaborateurs de tâches prennent actuellement en charge les agents créés dans Copilot Studio, Claude et Writer.ai.
>* Lors de la configuration d&#39;un agent dans Copilot Studio, vous devez définir la sécurité sur **Aucune authentification**.
>* Pour plus d’informations et d’instructions sur la création d’un espace de collaboration dans Workfront, consultez [Configurer un espace de collaboration de tâche](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) dans l’article Configurer des espaces de collaboration IA.

## Affecter un collaborateur de tâches à une tâche

Les collaborateurs de tâches sont affectés à des tâches de la même manière que les utilisateurs.

Pour obtenir des instructions, voir [Affecter des tâches](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).
