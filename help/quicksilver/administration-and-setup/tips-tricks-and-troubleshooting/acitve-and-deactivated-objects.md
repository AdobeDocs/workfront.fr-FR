---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Objets actifs et désactivés
description: En tant qu'administrateur  [!DNL Adobe Workfront] , vous pouvez activer ou désactiver des objets dans le système. Nous vous recommandons de ne jamais supprimer les objets que vous pouvez désactiver. Il vous suffit de désactiver l’objet pour l’empêcher d’être utilisé ultérieurement et de le supprimer des menus déroulants d’autres objets.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a0617270-e233-4ebe-a5ee-8df7a8a85823
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 4%

---

# Objets actifs et désactivés

En tant qu&#39;administrateur [!DNL Adobe Workfront], vous pouvez activer ou désactiver des objets dans le système. Nous vous recommandons de ne jamais supprimer les objets que vous pouvez désactiver. Il vous suffit de désactiver l’objet pour l’empêcher d’être utilisé ultérieurement et de le supprimer des menus déroulants d’autres objets.

Par exemple, pour afficher un certain [!UICONTROL type d’heure], le [!UICONTROL type d’heure] doit être actif. Un [!UICONTROL Type d’heure] inactif ou désactivé n’apparaît pas dans le menu déroulant [!UICONTROL Type d’heure], mais reste dans le système pour conserver l’enregistrement historique intact de l’emplacement où ce [!UICONTROL Type d’heure] a pu être utilisé dans le passé.

Le terme &quot;actif&quot; permet d’identifier si certains objets sont activés dans le système. Dans ce contexte, &quot;Actif&quot; est utilisé pour les objets suivants :

## Notifications par e-mail

Vous pouvez activer les notifications par courrier électronique pour permettre à certaines actions de déclencher des notifications par courrier électronique pour tous les utilisateurs.

Pour plus d’informations sur l’activation ou la désactivation des notifications par e-mail, voir [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Types d&#39;heures

Vous pouvez activer les types d’heures pour les permettre à l’utilisateur de les sélectionner lors de la journalisation de l’heure.

Pour plus d’informations sur l’activation ou la désactivation des types d’heure, voir [Gestion des types d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Portefeuilles

Un portfolio doit être actif pour apparaître sur le formulaire [!UICONTROL New Project (Business Case)].

Vous pouvez activer un portfolio lors de sa modification.

Pour plus d’informations sur la modification des portefeuilles, voir [Création d’un portfolio](../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

## Programmes

Un programme doit être actif pour apparaître dans le champ [!UICONTROL Program] pour un projet.

Vous pouvez activer un programme lors de sa modification.

Pour plus d&#39;informations sur la modification des programmes, voir [Création d&#39;un programme](../../manage-work/portfolios/create-and-manage-programs/create-program.md).

## Modèles

Un modèle doit être actif pour apparaître dans le champ Modèle d’un projet.

Vous pouvez activer un modèle lors de sa modification.

Pour plus d’informations sur la modification de modèles, voir [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Processus d&#39;approbation

Un processus d’approbation doit être actif pour apparaître dans le champ [!UICONTROL Processus d’approbation] pour un projet, une tâche ou un problème.

Vous pouvez activer un processus d’approbation lors de la modification du processus d’approbation.

Pour plus d&#39;informations sur la modification des processus d&#39;approbation, voir [Création d&#39;un processus d&#39;approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Chemins Milestone

Un chemin de jalon doit être actif pour apparaître dans le champ [!UICONTROL Chemin de jalon] pour un projet.

Vous pouvez activer un chemin de jalon lors de la modification du chemin de jalon.

Pour plus d’informations sur la modification des chemins de jalon, voir [Création d’un chemin de jalon](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

## Formulaires personnalisés dans mon groupe

Un formulaire personnalisé doit être actif pour apparaître dans le champ [!UICONTROL Formulaire personnalisé] pour un autre objet.

Vous pouvez activer un formulaire personnalisé lors de sa modification.

Pour plus d’informations sur la modification de formulaires personnalisés et pour obtenir la liste des objets auxquels vous pouvez les associer, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Entreprises

Une société doit être active pour apparaître dans le champ [!UICONTROL Société] pour un projet, un utilisateur ou un modèle.

Vous pouvez rendre une entreprise active lors de la modification de la société.

Pour plus d&#39;informations, voir [Création et modification d&#39;entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Utilisateurs

Un utilisateur doit être actif pour apparaître dans n’importe quel champ de type anticipé de tous les autres objets lors d’affectations ou de partages.

Vous pouvez désactiver les utilisateurs à partir de la page utilisateur ou pendant que vous modifiez un utilisateur.

Pour plus d’informations sur la désactivation des utilisateurs, voir [Désactivation ou réactivation d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

>[!IMPORTANT]
>
>Si votre organisation a été intégrée à [!DNL Adobe Business Platform], vous devez désactiver les utilisateurs par le biais de [!UICONTROL Adobe Admin Console].
>
>Pour obtenir des instructions sur la désactivation d’un utilisateur dans [!UICONTROL Adobe Admin Console], reportez-vous à la section &quot;Suppression d’utilisateurs&quot; de l’article [Gérer les utilisateurs individuellement](https://helpx.adobe.com/fr/enterprise/using/manage-users-individually.html) ou contactez votre administrateur [!UICONTROL Adobe Admin Console].
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à [!DNL Adobe Business Platform], voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Équipes

Une équipe doit être active afin d’apparaître dans tous les champs de type anticipé de tous les autres objets lors d’affectations ou de partages.

Vous pouvez désactiver les équipes lorsque vous modifiez une équipe.

Pour plus d’informations sur la désactivation des équipes, voir [Désactivation d’une équipe](../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md).

## Fonctions

Un rôle de tâche doit être actif pour apparaître dans tous les champs de type anticipé de tous les autres objets lors d’affectations ou de partages.

Vous pouvez désactiver les rôles de tâche lorsque vous les modifiez.

Pour plus d’informations sur la désactivation des rôles de tâche, voir [Désactivation des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).
