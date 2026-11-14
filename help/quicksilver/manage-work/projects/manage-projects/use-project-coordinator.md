---
title: Utiliser le collaborateur du coordinateur de projet
content-type: reference
description: Découvrez comment utiliser le coordinateur de projet, un collaborateur IA prêt à l’emploi qui surveille le statut des projets et assure le suivi des tâches en retard.
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 8%

---
# Utiliser le collaborateur du coordinateur de projet

{{highlighted-preview-article-level}}

Le coordinateur de projet est un collaborateur IA prêt à l’emploi qui surveille votre projet et informe les parties prenantes des informations de statut importantes.

L’utilisation d’un coordinateur de projet ne nécessite pas la configuration d’un agent en dehors de Workfront.

Pour obtenir des instructions sur la configuration d’un coordinateur de projet, consultez [Configuration d’un coordinateur de projet](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) dans l’article Configuration des collaborateurs de l’IA.

Pour plus d’informations sur les collaborateurs AI en général, consultez [Configurer des collaborateurs AI](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

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
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Pour affecter un coordinateur de projet, vous devez disposer de l’autorisation Gestion aux projets.</td> 
  </tr>
  </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Présentation du coordinateur de projet

Le coordinateur de projet surveille votre projet et vous aide à rester sur la bonne voie. Lorsqu’il est affecté à un projet, il envoie les mises à jour du projet selon un planning configuré par votre administrateur. Les mises à jour peuvent inclure les éléments suivants :

* Résumé de la progression
* Intégrité du projet
* Tâches ou approbations en retard ou à risque
* Champs ou affectations manquants

Le coordinateur de projet peut également apporter des commentaires sur le projet et ses tâches.

Votre administrateur configure la fréquence d’envoi des mises à jour, l’heure et la personne qui les reçoit.

Vous pouvez également exécuter le coordinateur de projet à la demande en le mentionnant dans une mise à jour du projet. Le coordinateur de projet s’exécute lorsqu’il est mentionné, même s’il n’est pas planifié pour s’exécuter à ce moment-là.

>[!NOTE]
>
>Le comportement du coordinateur de projet peut changer avant la disponibilité générale.

## Ajouter le coordinateur de projet à un projet

Un administrateur doit d’abord créer le coordinateur de projet et ajouter le champ **coordinateur de projet** à l’en-tête du projet dans votre modèle de mise en page. Le champ s’affiche alors dans l’en-tête du projet.

Pour plus d’informations, voir la section [Personnaliser des en-têtes d’objet à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Pour affecter un coordinateur de projet à un projet :

1. Accédez au projet pour lequel vous souhaitez affecter un coordinateur de projet.
1. Dans l&#39;en-tête du projet, cliquez sur le champ **Coordinateur de projet**.
1. Sélectionnez le coordinateur de projet que vous souhaitez affecter.

   La fenêtre affiche une description du coordinateur de projet sélectionné, ainsi que les actions qu&#39;il effectue.
1. Cliquez sur **Appliquer**.

## Exécuter le coordinateur de projet en le mentionnant

Outre ses mises à jour planifiées, vous pouvez déclencher le coordinateur de projet à tout moment en l’@mentioning dans une mise à jour du projet. Le coordinateur de projet s’exécute dès qu’il est mentionné, même s’il n’est pas prévu qu’il s’exécute à ce moment-là.

Pour mentionner le coordinateur de projet :

1. Accédez au projet auquel le coordinateur de projet est affecté.
1. Ouvrez la zone **Mises à jour** du projet.
1. Dans le champ de mise à jour, saisissez **@** et sélectionnez le coordinateur de projet.
1. Ajoutez votre message, puis publiez la mise à jour.

   Le coordinateur du projet exécute et publie sa réponse.

>[!NOTE]
>
>Le coordinateur de projet doit être affecté au projet avant de pouvoir le déclencher avec un @mention.

## Configuration du coordinateur de projet

Pour obtenir des instructions sur la configuration du coordinateur de projet, consultez [Configuration du coordinateur de projet](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) dans l’article Configuration des collaborateurs de l’IA.
