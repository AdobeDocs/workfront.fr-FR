---
title: Utiliser des agents de travail
content-type: reference
description: Découvrez comment utiliser des agents de travail, des collaborateurs de l’IA qui peuvent être affectés à des tâches Workfront.
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 3%
---
# Utiliser des agents de travail

Les agents de travail sont des collaborateurs de l’IA qui peuvent être affectés directement à des tâches Workfront, en plus du réviseur de l’IA utilisé pour les révisions de documents et de ressources. Comme les autres collaborateurs de l’IA, les agents de travail sont configurés dans la zone Configuration et affectés aux tâches comme un utilisateur.

Les agents de travail se connectent aux agents que vous avez configurés dans Copilot Studio, Claude ou Writer.

Pour plus d’informations et d’instructions sur la création d’un agent de travail dans Workfront, consultez [Configurer un agent de travail](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) dans l’article Configuration des collaborateurs de l’IA.

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

* Vous devez configurer un agent dans Copilot, Claude ou Writer.ai avant de pouvoir l&#39;utiliser comme agent de travail.

## Présentation de l’agent de travail

Les agents de travail permettent d’affecter des agents MCP à des tâches spécifiques dans Workfront. Vous configurez l’agent dans une application telle que Copilot Studio, Claude ou Writer.ai, puis vous connectez cet agent à Workfront en tant qu’agent de travail. Vous pouvez ensuite l’affecter à des tâches comme vous le feriez pour un utilisateur.

Voici quelques exemples de workflows :

* Détecter les images chargées dans une tâche, générer les variations en fonction des critères donnés à l’agent et charger les nouvelles images dans la tâche.
* Générer une copie à partir d’une description de tâche, vérifier la copie par rapport aux directives configurées dans l’agent et publier la copie dans le flux de mise à jour.
* Lecture des détails d’un événement, identification des détails manquants et publication de questions sur les détails manquants dans le flux de mise à jour.

>[!NOTE]
>
>* Les détails spécifiques relatifs aux responsabilités et capacités d’un agent sont configurés dans l’application dans laquelle l’agent est créé, et non dans Workfront.
>* Il n’est pas nécessaire d’ajouter le serveur Workfront MCP à l’agent utilisé comme agent de travail et il n’est pas nécessaire de le connecter pour que cet agent fonctionne.
>* Les agents de travail prennent actuellement en charge les agents créés dans Copilot Studio, Claude et Writer.ai.
>* Lors de la configuration d&#39;un agent dans Copilot Studio, vous devez définir la sécurité sur **Aucune authentification**.
>* Pour plus d’informations et d’instructions sur la création d’un agent de travail dans Workfront, consultez [Configurer un agent de travail](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) dans l’article Configuration des collaborateurs de l’IA.

## Informations lues par un agent de travail

Lorsqu’un agent de travail commence à travailler sur une tâche, il lit automatiquement les informations de tâche suivantes en tant que contexte :

* Titre de la tâche
* Description de la tâche
* Commentaires dans le flux de mise à jour de la tâche
* Informations dans tout formulaire personnalisé joint à la tâche

Ces informations sont toujours lues et ne peuvent pas être configurées en tant que paramètre Workfront.

>[!TIP]
>
>Pour de meilleurs résultats, nous vous recommandons :
>
>* Incluez toutes les informations d’arrière-plan que l’agent doit utiliser directement dans la description de la tâche ou dans un champ de formulaire personnalisé approprié.
>* Assurez-vous que la tâche correspond à ce que votre agent a reçu pour instruction de faire. Par exemple, si votre agent a pour instruction de traduire du texte de l’anglais vers le français, incluez le texte que vous souhaitez traduire dans la description de la tâche.

## Déclencheurs de démarrage de l’agent de travail

Lorsqu’un agent de travail est affecté à une tâche, il commence à travailler lorsque l’une des situations suivantes est remplie :

* L&#39;agent de travail est affecté à une tâche prête à démarrer. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci sont terminés.)
* L’agent de travail et un utilisateur sont affectés à une tâche, et l’agent de travail est affecté en premier.
* Une tâche à laquelle un agent de travail est déjà affecté devient prête à démarrer et l&#39;agent de travail est la seule personne désignée ou la personne désignée principale. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci sont terminés.)
* Une tâche à laquelle un agent de travail et un utilisateur sont déjà affectés devient prête à démarrer et l’agent de travail a été affecté en premier ou est le cessionnaire principal. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci sont terminés.)
* Un utilisateur et un agent de travail sont affectés à une tâche et l&#39;utilisateur est supprimé.
* Un utilisateur et un agent de travail sont affectés à une tâche, et l’agent de travail est défini comme cessionnaire par Principal pour la tâche.

Les situations suivantes ne provoquent pas le début du travail de l’agent de travail sur la tâche :

* Un agent de travail est affecté à une tâche à laquelle un utilisateur est déjà affecté.
* Un agent de travail @mentioned une tâche.
* Un agent de travail est affecté à une tâche à laquelle un agent de travail est déjà affecté. Dans ce cas, le premier agent de travail affecté aura déjà commencé le travail, et le second agent de travail ne fera rien.
* Un agent de travail est affecté à une tâche qui n&#39;est pas prête à démarrer. (Par exemple, si la tâche comporte des prédécesseurs, ceux-ci ne sont pas encore terminés.)

## Affecter un agent de travail à une tâche

Les agents de travail sont affectés aux tâches de la même manière que les utilisateurs.

Lorsque vous recherchez un agent de travail dans la liste des cessionnaires disponibles, le nom de l&#39;agent de travail est un prénom uniquement.

Pour obtenir des instructions, voir [Affecter des tâches](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

>[!NOTE]
>
>Les agents de travail ne peuvent pas être affectés à la révision ou à l&#39;approbation d&#39;un document.

## Dépannage des agents de travail

Si votre agent de travail ne renvoie pas de réponse ou de sortie, vérifiez les points suivants :

* Assurez-vous que votre agent est publié du côté du fournisseur de la plateforme d’IA.
* Assurez-vous de disposer de crédits d’IA suffisants avec la plateforme de votre agent.
* Assurez-vous que l’action effectuée sur la tâche ne nécessite pas un niveau d’accès spécifique.
* Si vous utilisez Copilot comme fournisseur d’agent, assurez-vous d’utiliser le paramètre « aucune authentification ».
* Si vous utilisez Copilot, assurez-vous que votre agent est configuré dans un environnement global. La fonctionnalité de Work Agent ne prend actuellement pas en charge les versions régionales de Copilot Studio.
* Assurez-vous que le collaborateur est la personne principale désignée pour la tâche.
* Assurez-vous que la tâche à laquelle l&#39;agent de travail est affecté peut démarrer. Par exemple, vérifiez que toutes les tâches antérieures à cette tâche sont terminées.

>[!TIP]
>
>Vous pouvez également accéder à la plateforme du fournisseur d’agents et demander à l’agent d’effectuer la tâche dans la plateforme. Si l’agent ne peut pas effectuer la tâche dans la plateforme, l’agent de travail rencontrera également des problèmes dans Workfront.
