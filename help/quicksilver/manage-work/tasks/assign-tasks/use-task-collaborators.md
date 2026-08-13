---
title: Utiliser les collaborateurs de la tâche
content-type: reference
description: Découvrez comment utiliser les collaborateurs de tâches, des collaborateurs d’IA qui peuvent être affectés à des tâches Workfront.
author: Becky
feature: Work Management, Tasks
source-git-commit: 1894bbb5ec7f44f93468c202fb9c07fa656a83cf
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 3%

---

# Utiliser les collaborateurs de la tâche

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

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

## Déclencheurs de démarrage de Task Collaborator

Lorsqu&#39;un collaborateur de tâches est affecté à une tâche, il commence à travailler lorsque l&#39;une des situations suivantes est remplie :

* Le collaborateur de tâches est affecté à une tâche prête à démarrer. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci sont terminés.)
* Le collaborateur de tâches et un utilisateur sont affectés à une tâche, et le collaborateur de tâches est affecté en premier.
* Une tâche à laquelle un collaborateur de tâches est déjà affecté devient prête à démarrer et le collaborateur de tâches est le seul ou le principal cessionnaire. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci sont terminés.)
* Une tâche à laquelle un collaborateur de tâches et un utilisateur sont déjà affectés est prête à démarrer et le collaborateur de tâches a été affecté en premier ou est le cessionnaire principal. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci sont terminés.)
* Un utilisateur et un collaborateur de tâches sont affectés à une tâche et l&#39;utilisateur est supprimé.
* Un utilisateur et un collaborateur de tâches sont affectés à une tâche, et le collaborateur de tâches est défini comme cessionnaire Principal pour la tâche.

Les situations suivantes n&#39;entraînent pas le début du travail sur la tâche par le collaborateur de tâches :

* Un collaborateur de tâches est affecté à une tâche à laquelle un utilisateur est déjà affecté.
* Un collaborateur de tâches est @mentioned dans une tâche.
* Un collaborateur de tâches est affecté à une tâche à laquelle un collaborateur de tâches est déjà affecté. Dans ce cas, le premier collaborateur de tâche affecté aura déjà commencé le travail, et le second collaborateur de tâche ne fera rien.
* Un collaborateur de tâches est affecté à une tâche qui n&#39;est pas prête à démarrer. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci ne sont pas encore terminés.)

## Affecter un collaborateur de tâches à une tâche

Les collaborateurs de tâches sont affectés à des tâches de la même manière que les utilisateurs.

Lorsque vous recherchez un collaborateur de tâches dans la liste des cessionnaires disponibles, le nom du collaborateur de tâches n&#39;est qu&#39;un prénom.

Pour obtenir des instructions, voir [Affecter des tâches](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

>[!NOTE]
>
>Les collaborateurs de tâche ne peuvent pas être affectés à la révision ou à l&#39;approbation d&#39;un document.

## Résolution des problèmes des collaborateurs de tâches

Si votre collaborateur de tâches ne renvoie pas de réponse ou de sortie, vérifiez les points suivants :

* Assurez-vous que votre agent est publié du côté du fournisseur de la plateforme d’IA.
* Assurez-vous de disposer de crédits d’IA suffisants avec la plateforme de votre agent.
* Assurez-vous que l’action effectuée sur la tâche ne nécessite pas un niveau d’accès spécifique.
* Si vous utilisez Copilot comme fournisseur d’agent, assurez-vous d’utiliser le paramètre « aucune authentification ».
* Si vous utilisez Copilot, assurez-vous que votre agent est configuré dans un environnement global. La fonctionnalité Task Collaborator ne prend actuellement pas en charge les versions régionales de Copilot Studio.
* Assurez-vous que le collaborateur est la personne principale désignée pour la tâche.
* Assurez-vous que la tâche à laquelle le collaborateur de tâches est affecté peut démarrer. Par exemple, vérifiez que toutes les tâches antérieures à cette tâche sont terminées.

>[!TIP]
>
>Vous pouvez également accéder à la plateforme du fournisseur d’agents et demander à l’agent d’effectuer la tâche dans la plateforme. Si l’agent ne peut pas effectuer la tâche dans la plateforme, Task Collaborator rencontrera également des problèmes dans Workfront.
