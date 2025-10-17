---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Vue d'ensemble des demandes de l'équipe
description: Les demandes de l’équipe se trouvent dans la zone Équipes du menu principal.
author: Jenny
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 99%

---

# Vue d’ensemble des demandes de l’équipe

## Comprendre les demandes de l’équipe

Les demandes de l’équipe se trouvent dans la zone [!UICONTROL Équipes] dans le [!UICONTROL Menu principal]. Cliquez sur l’icône [!UICONTROL Demandes de l’équipe] ou sur l’![icône Demandes](assets/request-icon.png) dans le panneau de gauche pour afficher les demandes de l’équipe.

>[!NOTE]
>
>Les équipes Agile ne disposent pas de demandes de l’équipe.

L’onglet [!UICONTROL Demandes de l’équipe] affiche les demandes en attente d’affectation pour l’équipe actuellement sélectionnée dans la liste déroulante. Le nombre entre parenthèses indique le nombre d’éléments prêts à être traités.

Une demande de l’équipe représente un élément de travail en attente qui n’est pas affecté à une personne spécifique. Au lieu de cela, elle est affectée à une équipe et toute personne membre de cette équipe peut se porter volontaire pour accepter la responsabilité de l’élément. Si une personne se porte volontaire pour travailler sur une demande de l’équipe, elle accepte l’affectation du travail comme étant la sienne. La tâche est affectée à un utilisateur ou une utilisatrice en plus de l’équipe.

>[!NOTE]
>
>Une demande de l’équipe ne doit pas être utilisée pour les affectations de tâches collaboratives. Si vous devez affecter plusieurs personnes à une tâche, faites-le en créant des [!UICONTROL Affectations avancées] et non par le biais de demandes de l’équipe. Pour plus d’informations, voir [Créer des affectations avancées](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Comprendre les options [!UICONTROL Prêt à démarrer] et [!UICONTROL Tous]

Deux options se trouvent en haut de la section Demandes de l’équipe : [!UICONTROL Prêt à démarrer] et [!UICONTROL Tous].

L’option [!UICONTROL Prêt à démarrer] n’affiche que les tâches et les problèmes qui répondent à tous les critères suivants :

* Toutes les tâches antérieures ont rempli les conditions de leurs types de dépendance des tâches antérieures.\
  Par exemple, si le type de relation de la tâche antérieure est [!UICONTROL Terminer-Démarrer] (la tâche antérieure doit se terminer avant que la tâche dépendante puisse commencer), la tâche antérieure doit être marquée comme [!UICONTROL Terminée]. (Pour plus d’informations sur les types de dépendance des tâches antérieures, voir [Vue d’ensemble des types de dépendances des tâches](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* La personne connectée est la personne affectée à ces tâches et problèmes (pour les demandes de travail), ou bien l’équipe sélectionnée est affectée à ces tâches et problèmes (pour les demandes de l’équipe).
* Le statut du projet est défini sur [!UICONTROL Actuel].
* La [!UICONTROL date de début prévisionnelle] ou la [!UICONTROL date de début prévue] est passée ou planifiée pour commencer dans les deux semaines à compter de la date du jour (ou alors aucune [!UICONTROL date de début prévisionnelle] ou [!UICONTROL date de début prévue] n’a été définie).
* La [!UICONTROL date de remise] s’est déjà produite ou se produira dans les deux semaines à compter de la date actuelle.

>[!NOTE]
>
>Si la tâche répond aux trois premiers critères et dispose d’une date de remise dans les deux semaines suivant la date actuelle, la valeur [!UICONTROL Prêt à démarrer] s’affiche même si les dates prévues et prévisionnelles se situent plus de deux semaines après. Si la tâche ne dispose pas de date de remise, les dates prévues et prévisionnelles doivent se situer dans les deux semaines suivant la date actuelle.

L’option [!UICONTROL Tous] affiche toutes les tâches et tous les problèmes des projets en cours affectés à la personne connectée ou toutes les tâches ou problèmes affectés à l’équipe.
