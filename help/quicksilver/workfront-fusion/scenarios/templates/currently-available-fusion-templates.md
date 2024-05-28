---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Modèles Adobe Workfront Fusion actuellement disponibles
description: Les modèles publics suivants sont actuellement disponibles dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: e569469c2b5e0ba40569ef86043294acae7a6aa8
workflow-type: tm+mt
source-wordcount: '1186'
ht-degree: 1%

---

# Modèles Adobe Workfront Fusion actuellement disponibles

Les modèles publics suivants sont actuellement disponibles dans Adobe Workfront Fusion.

D’autres modèles créés par l’équipe ou l’entreprise peuvent être disponibles pour votre équipe.

Pour afficher les modèles disponibles, cliquez sur le bouton **Modèles** icon ![](assets/fusion-template-icon.png) dans le menu de navigation latéral de Fusion.

## Modèles Workfront

Ces modèles automatisent les processus et les workflows Workfront.

### [!BADGE Nouveau !]{type=Informative}

Ce modèle de fusion crée une liste de contrôle standard pour toutes les cartes qui entrent ponctuellement une colonne spécifique sur un panorama spécifique.

### Workfront - Création de projet à partir de CSV

Cette automatisation crée de nouveaux projets dans Workfront en fonction du nom, du Portfolio, de l’état, de la date de début planifiée et des détails du modèle que vous spécifiez dans un fichier CSV.

### Workfront - Demandes de nettoyage sans nouvelles notes au cours des 30 derniers jours

Utilisez ce modèle pour appliquer une mise à jour de note de 30 jours à vos requêtes. Les demandes qui ne sont pas mises à jour dans 30 jours voient leur état changé et fermé à 60 jours.

### Workfront : définissez l’état du projet sur Terminé à 100 %.

Cette automatisation met à jour les projets à l’état Terminé pour lequel toutes les tâches à 1 005 sont terminées. Les projets avec des problèmes en cours ou des tâches ouvertes ou des approbations de projet recevront une mise à jour. Une fois résolus, les projets passeront à l’état Terminé.

### Workfront - Avertissement et tentative de fermeture de projets obsolètes

Utilisez ce scénario pour automatiser l’avertissement et la fermeture des projets qui correspondent à la stratégie de projet obsolète de votre entreprise.

### Workfront : copiez les nouvelles notes et réponses du problème/de la demande source au projet ou à la tâche déjà converti.

Utilisez ce modèle pour copier les notes et les réponses d’un problème ou d’une requête vers un projet ou une tâche déjà converti.

### Workfront - Copier le programme Forms personnalisé et les données de champ dans les nouveaux projets associés

Cette automatisation recherche de nouveaux projets dans les programmes avec des formulaires personnalisés. Il ajoute ensuite ces formulaires et champs personnalisés de programme aux nouveaux projets.

### Workfront - Copie de Portfolios de données de champ et de Forms personnalisées dans les nouveaux projets associés

Cette automatisation recherche de nouveaux projets dans les portefeuilles avec des formulaires personnalisés. Il ajoute ensuite ces champs et formulaires personnalisés de portefeuille aux nouveaux projets.

### Workfront - Convertir le problème approuvé en projet

Ce modèle convertit les problèmes en projets. Vous pouvez la modifier pour répondre aux normes de votre entreprise.

### Workfront - Copie de documents provenant de problèmes/requêtes vers des projets ou des tâches déjà convertis

Ce scénario flexible copie des documents provenant de problèmes ou de requêtes vers des projets ou des tâches précédemment convertis.

### Notification personnalisée basée sur le changement de champ

Ce modèle crée des mises à jour personnalisées (et des notifications associées) pour les personnes travaillant sur un projet Workfront, en fonction d’un événement unique, tel qu’un changement de valeur de champ. Le scénario recherche Workfront lorsqu’un champ spécifié change dans une tâche ou un problème. Lorsqu’il est rencontré, le scénario évalue les informations du projet associé et crée une mise à jour personnalisée pour une personne affectée à un rôle spécifique dans le projet.

### Workfront : ajout groupé au nom du projet avec convention

Ce modèle de mise à jour en bloc renomme tous les projets qui répondent aux critères d’une recherche (appartenant à un portfolio) et les renomme avec un format standard.

### Workfront - Renommer les projets avec convention

Ce modèle localise tous les projets répondant aux critères d’un filtre (appartenant à un portfolio) et les renomme avec un format standard.

### Workfront - Créer une ligne de base lors de la modification de l’état

Ce modèle capture une ligne de base de projet lors de tout changement d’état de projet noté dans les modules &quot;switch&quot; et crée une mise à jour dans le flux de mise à jour pour la journalisation.

### Workfront : création de base hebdomadaire

Ce modèle capture une ligne de base de projet sur une base hebdomadaire chaque lundi à 6h00 ET sur les projets filtrés par portefeuille, et crée une mise à jour dans le flux de mise à jour pour la journalisation.

### Recherche de modèles de projet non utilisés au moment de la stratégie et notification

Une fois par mois, consultez vos modèles de projet en utilisant votre propre stratégie avec ce modèle facile à gérer qui avertit les utilisateurs appropriés des modèles en violation de votre stratégie.

## Workfront - Modèles Workfront Proof

Ces modèles automatisent les workflows qui combinent Workfront à Workfront Proof.

### Workfront Proof > Workfront - Mise à jour du projet sur la décision de BAT

Lorsqu’une décision est prise sur un BAT ajouté directement à un projet, cette automatisation rassemble des informations sur la décision du BAT, telles que les personnes qui ont pris la décision, puis reflète cette progression dans le projet Workfront correspondant sous forme de mise à jour.

### Workfront Proof > Workfront - Mise à jour et exécution de la tâche (si approuvée) sur la décision de BAT

Lorsque des BAT individuels sont liés à des tâches individuelles, ce scénario ferme la tâche associée lorsqu&#39;une décision de validation est prise sur le BAT. S’il est approuvé, il termine la tâche et met à jour le projet.

## HTTP - Modèles Workfront

Ces modèles récupèrent les informations d’un service Web et les intègrent à Workfront.

>[!NOTE]
>
> Vous devez disposer d’une licence Workfront Fusion for Work Automation and Integration pour utiliser des modèles dans cette section.

### Établissement de la connexion à l’aide de JWT (JSON Web Token)

Définition de l’autorisation JWT pour une API client.

### APILayer > Workfront - Mise à jour du taux d’Exchange quotidien (EUR)

Ce modèle crée un scénario qui automatise la mise à jour d’un taux d’exchange à un moment donné. Ce scénario extrait le taux d’euros (EUR) en dollars US (USD) d’une API APIlayers.com et le met à jour dans Workfront.

## Modèles Workfront-Marketo

Ces modèles prennent en charge l’intégration Workfront-Marketo.

>[!NOTE]
>
> Vous devez disposer d’une licence Workfront Fusion for Work Automation and Integration pour utiliser des modèles dans cette section.

### Approbation de votre brouillon de courrier électronique Marketo Engage avec les workflows d’approbation Workfront

Il fait partie de l’intégration de vérification et d’approbation entre Workfront et Marketo Engage. Ce modèle détecte si un BAT d’email dans Workfront a été approuvé, puis met à jour l’email correspondant dans Marketo Engage comme approuvé.

### Récupérer les requêtes de campagne marketing dans Workfront et automatiser la création des campagnes dans Marketo Engage

Ce scénario fournit un moyen programmatique de créer des campagnes par courrier électronique et des webinaires en Marketo Engage à partir d’une demande effectuée dans Workfront. Grâce à l’automatisation de la création, de l’organisation et de la configuration des campagnes, les équipes peuvent améliorer leur efficacité.

### Vérification d’un BAT d’email de votre brouillon de courrier électronique de Marketo Engage dans Workfront

Ce modèle détecte si une tâche Workfront a été définie sur un état prêt à être examinée, puis exporte le brouillon de l’email depuis Marketo Engage pour l’enregistrer en tant que BAT dans Workfront.

## Modèles Workfront-SharePoint

Ces modèles connectent Workfront et SharePoint.

>[!NOTE]
>
> Vous devez disposer d’une licence Workfront Fusion for Work Automation and Integration pour utiliser des modèles dans cette section.

### Surveillance des modifications du dossier SharePoint

Ce modèle vous permet de voir si un dossier SharePoint a été modifié.


## Modèles Workfront-Anaplan

Ces modèles prennent en charge l’intégration Workfront-Anaplan et nécessitent une configuration spécifique dans les deux interfaces dans Workfront. Pour plus d’informations sur ces modèles et leurs configurations requises, consultez les articles relatifs aux modèles individuels.

Pour plus d’informations sur l’intégration Workfront-Anaplan, voir [Adobe Workfront avec Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> Vous devez disposer d’une licence Workfront Fusion for Work Automation and Integration pour utiliser des modèles dans cette section.

### Workflows d&#39;optimisation des dépenses

* [Envoyer [!DNL Adobe Workfront] mises à jour de projet à une [!DNL Anaplan] élément de liste](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [Envoyer [!DNL Adobe Workfront] dépenses d’un [!DNL Anaplan] élément de liste](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [Envoyer [!DNL Adobe Workfront] mises à jour des heures réelles à une [!DNL Anaplan] élément de liste](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### Workflows pour lier les requêtes de budget

* [Créez un [!DNL Anaplan] élément de liste d’un [!DNL Adobe Workfront] requête budget](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] project](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### Workflows pour lier des requêtes de campagne

* [Créez un [!DNL Anaplan] élément de liste d’un [!DNL Adobe Workfront] requête de campagne](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] requête de campagne ou projet de campagne](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)


<!--[!BADGE New!]{type=Informative} -->