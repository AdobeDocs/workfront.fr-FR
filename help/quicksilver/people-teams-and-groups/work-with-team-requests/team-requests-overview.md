---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Présentation des requêtes d’équipe
description: Les demandes de l’équipe se trouvent dans la zone Équipes du menu principal.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Présentation des requêtes d’équipe

## Présentation des requêtes de l’équipe

Les demandes de l’équipe se trouvent dans la variable [!UICONTROL Équipes] dans la zone [!UICONTROL Menu Principal]. Cliquez sur le bouton [!UICONTROL Requêtes d’équipe] icon ![Icône Requête](assets/request-icon.png) dans le panneau de gauche pour afficher les requêtes de l’équipe.

>[!NOTE]
>
>Les équipes agiles n’ont pas de demandes d’équipe.

Le [!UICONTROL Requêtes d’équipe] affiche les requêtes en attente d’affectation pour l’équipe actuellement sélectionnée dans la liste déroulante. Le nombre entre parenthèses indique le nombre d’éléments prêts à être traités.

Une requête d’équipe représente une tâche en attente qui n’est pas affectée à un utilisateur spécifique. Au lieu de cela, elle est affectée à une équipe et tout membre de cette équipe peut se porter volontaire pour accepter la responsabilité de l’article. Si un utilisateur se porte volontaire pour travailler sur une demande d’équipe, il accepte l’affectation de travail comme étant la sienne. La tâche est assignée à chaque utilisateur en plus de l’équipe.

>[!NOTE]
>
>Une demande d’équipe ne doit pas être utilisée pour les affectations de tâches collaboratives. Si vous devez affecter plusieurs utilisateurs à une tâche, procédez comme suit : [!UICONTROL Affectations avancées] et non par le biais de demandes d’équipe. Pour plus d’informations, voir [Création d’affectations avancées](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Comprendre le [!UICONTROL Prêt à démarrer] et [!UICONTROL Tous] options

Deux options se trouvent en haut de la section Demandes d’équipe : [!UICONTROL Prêt à démarrer] et [!UICONTROL Tous].

Le [!UICONTROL Prêt à démarrer] n’affiche que les tâches et les problèmes qui répondent à tous les critères suivants :

* Tous les prédécesseurs ont rempli les conditions de leur type de dépendance prédécesseur.\
   Par exemple, si le type de relation de prédécesseur est [!UICONTROL Finish-Start] (la tâche du prédécesseur doit se terminer avant que la tâche dépendante puisse commencer), le prédécesseur doit être marqué comme [!UICONTROL Terminer]. (Pour plus d’informations sur les types de dépendance de prédécesseur, voir [Présentation des types de dépendances des tâches](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* L’utilisateur connecté est la personne affectée à ces tâches et problèmes (pour les demandes de travail), ou l’équipe sélectionnée est affectée à ces tâches et problèmes (pour les demandes d’équipe).
* Le statut du projet est défini sur [!UICONTROL Actuel].
* Le [!UICONTROL Date de début prévue] ou [!UICONTROL Date de début planifiée] est écoulé ou est prévu pour commencer dans les deux semaines à compter de la date d’aujourd’hui (ou non [!UICONTROL Date de début prévue] ou [!UICONTROL Date de début planifiée] a été défini).
* Le [!UICONTROL Date de remise] s’est déjà produit ou se produira dans les deux semaines à compter de la date actuelle.

>[!NOTE]
>
>Si la tâche répond aux trois premiers critères et dispose d’une date de passation dans les deux semaines suivant la date actuelle, la valeur [!UICONTROL Prêt à démarrer] même si les dates prévues et prévues sont supérieures à deux semaines. Si la tâche ne comporte pas de date de passation, les dates prévues/prévues doivent être dans les deux semaines suivant la date courante.

Le [!UICONTROL Tous] affiche toutes les tâches et problèmes des projets en cours affectés à l’utilisateur connecté ou toutes les tâches ou problèmes affectés à l’équipe.
