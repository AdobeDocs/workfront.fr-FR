---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Objets principaux et désactivés
description: En tant que [!DNL Adobe Workfront] , vous pouvez activer ou désactiver des objets dans le système. Nous vous recommandons de ne jamais supprimer les objets que vous pouvez désactiver. Il vous suffit de désactiver l’objet pour l’empêcher d’être utilisé ultérieurement et de le supprimer des menus déroulants d’autres objets.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a0617270-e233-4ebe-a5ee-8df7a8a85823
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 2%

---

# Objets principaux et désactivés

En tant que [!DNL Adobe Workfront] , vous pouvez activer ou désactiver des objets dans le système. Nous vous recommandons de ne jamais supprimer les objets que vous pouvez désactiver. Il vous suffit de désactiver l’objet pour l’empêcher d’être utilisé ultérieurement et de le supprimer des menus déroulants d’autres objets.

Par exemple, pour qu’un [!UICONTROL Type d’heure], la variable [!UICONTROL Type d’heure] doit être principale. Inactif ou désactivé [!UICONTROL Type d’heure] n’apparaît pas dans la variable [!UICONTROL Type d’heure] , mais reste dans le système pour conserver l’enregistrement historique intact de l’emplacement [!UICONTROL Type d’heure] aurait pu être utilisé dans le passé.

Le terme &quot;Principal&quot; permet de déterminer si certains objets sont activés dans le système. Dans ce contexte, &quot;Principal&quot; est utilisé pour les objets suivants :

## Notifications par e-mail

Vous pouvez activer les notifications par courrier électronique pour permettre à certaines actions de déclencher des notifications par courrier électronique pour tous les utilisateurs.

Pour plus d’informations sur l’activation ou la désactivation des notifications électroniques, voir [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Types d&#39;heures

Vous pouvez activer les types d’heures pour les permettre à l’utilisateur de les sélectionner lors de la journalisation de l’heure.

Pour plus d’informations sur l’activation ou la désactivation des types d’heure, voir [Gestion des types d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Portefeuilles

Un portfolio doit être principal pour apparaître sur le [!UICONTROL Nouveau projet (analyse de cas)] formulaire.

Vous pouvez principal un portfolio lors de sa modification.

Pour plus d’informations sur la modification de portefeuilles, voir [Création d’un portfolio](../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

## Programmes

Un programme doit être principal pour apparaître sur la [!UICONTROL Programme] pour un projet.

Vous pouvez rendre un programme principal lors de la modification du programme.

Pour plus d’informations sur la modification des programmes, voir [Créer un programme](../../manage-work/portfolios/create-and-manage-programs/create-program.md).

## Modèles

Un modèle doit être principal pour apparaître dans le champ Modèle d’un projet.

Vous pouvez rendre un modèle principal lors de sa modification.

Pour plus d’informations sur la modification de modèles, voir [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Processus d&#39;approbation

Un processus de validation doit être principal pour apparaître sur le [!UICONTROL Processus d’approbation] champ d’un projet, d’une tâche ou d’un problème.

Vous pouvez rendre le processus de validation principal lors de la modification du processus de validation.

Pour plus d’informations sur la modification des processus de validation, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Chemins Milestone

Un chemin d’accès de jalon doit être principal pour apparaître sur la variable [!UICONTROL Chemin Milestone] pour un projet.

Vous pouvez principal un chemin de jalon lors de la modification du chemin de jalon.

Pour plus d’informations sur la modification des chemins de jalon, voir [Création d’un chemin de jalon](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

## Formulaires personnalisés

Un formulaire personnalisé doit être principal pour s’afficher sur le [!UICONTROL Formulaire personnalisé] pour un autre objet.

Vous pouvez rendre un formulaire personnalisé principal lors de la modification du formulaire personnalisé.

Pour plus d’informations sur la modification de formulaires personnalisés et pour obtenir la liste des objets auxquels vous pouvez les associer, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Entreprises

Une société doit être principale pour apparaître sur la variable [!UICONTROL Société] pour un projet, un utilisateur ou un modèle.

Vous pouvez rendre une société principale lors de la modification de la société.

Pour plus d’informations, voir [Création et modification d’entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Utilisateurs

Un utilisateur doit être principal afin d’apparaître dans n’importe quel champ de type anticipé de tous les autres objets lors d’affectations ou de partages.

Vous pouvez désactiver les utilisateurs à partir de la page utilisateur ou pendant que vous modifiez un utilisateur.

Pour plus d’informations sur la désactivation des utilisateurs, voir [Désactivation ou réactivation d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

>[!IMPORTANT]
>
>Si votre entreprise a été intégrée à la variable [!DNL Adobe Business Platform], vous devez désactiver les utilisateurs via le [!UICONTROL Adobe Admin Console].
>
>Pour plus d’informations sur la désactivation d’un utilisateur dans la variable [!UICONTROL Adobe Admin Console], voir la section &quot;Suppression d’utilisateurs&quot; de l’article . [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou contactez votre [!UICONTROL Adobe Admin Console] Administrateur.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à la variable [!DNL Adobe Business Platform], voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Équipes

Une équipe doit être principale afin d’apparaître dans tous les champs de type anticipé de tous les autres objets lors d’affectations ou de partages.

Vous pouvez désactiver les équipes lorsque vous modifiez une équipe.

Pour plus d’informations sur la désactivation des équipes, voir [Désactivation d’une équipe](../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md).

## Fonctions

Un rôle de tâche doit être principal afin d’apparaître dans tous les champs de type anticipé de tous les autres objets lors d’affectations ou de partages.

Vous pouvez désactiver les rôles de tâche lorsque vous les modifiez.

Pour plus d’informations sur la désactivation des rôles de tâche, voir [Désactivation des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).
