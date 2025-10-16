---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Créer des tâches  [!DNL Adobe Workfront]  depuis  [!DNL Microsoft]  Teams
description: Si une personne responsable d’une équipe a installé et configuré  [!DNL Workfront]  pour Microsoft Teams pour votre équipe et que la connexion à Workfront se fait à partir de Microsoft Teams, vous pouvez créer des tâches personnelles dans Adobe  [!DNL Workfront]  depuis Microsoft Teams.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 4cf780aa1b1221cd6ff8e6ce58fbb7d3621f7fa9
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 76%

---

# Créer des tâches [!DNL Adobe Workfront] à partir de [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>Comme [Microsoft passe au client Nouvelles équipes](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability), le client Équipes classiques ne sera plus disponible après le 1er juillet 2025. Pour continuer à utiliser Microsoft Teams et les applications intégrées telles que Workfront, les clients doivent passer au client New Teams avant cette date.
>
>L’intégration Workfront mise à jour est désormais disponible et entièrement compatible avec la nouvelle expérience Équipes . Dans la plupart des cas, Workfront s’affiche automatiquement une fois la transition effectuée. Si ce n’est pas le cas, l’intégration peut être installée manuellement à partir de Microsoft Teams App Store. Pour installer ou vérifier l’intégration de Workfront dans le client New Teams, voir [Installer [!DNL Adobe Workfront] pour Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).



## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Travail ou supérieur</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous pouvez créer des tâches personnelles dans [!DNL Adobe Workfront] à partir de [!DNL Microsoft Teams] si les conditions suivantes sont remplies :

* Une personne propriétaire d’équipe a installé et configuré [!DNL Workfront for Microsoft Teams] pour votre équipe.
* La connexion à [!DNL Workfront] est établie à partir de [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] ne prend plus en charge [!DNL Internet Explorer]. Pour profiter de l’intégration de [!DNL Adobe Workfront for Microsoft Teams], utilisez un navigateur web autre qu’[!DNL Internet Explorer].

Pour plus d’informations sur l’installation de [!DNL Workfront for Microsoft Teams] et la connexion à [!UICONTROL Workfront] à partir de [!DNL Microsoft Teams], consultez la section [Installer  [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Créer des tâches personnelles à partir de [!DNL Microsoft Teams]

1. Connectez-vous à [!DNL Workfront] à partir de [!DNL Microsoft Teams].

   Pour plus d’informations sur la connexion à [!DNL Workfront], consultez la section [Installer  [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Pour ouvrir une carte **[!UICONTROL Nouvelle tâche]**, procédez comme suit :

   * Si vous vous trouvez dans le canal de conversation avec le robot [!DNL Workfront], saisissez **[!UICONTROL Nouvelle tâche]** dans le champ de [!UICONTROL conversation] pour créer une tâche.
   * Si vous êtes dans un canal de conversation autre que le canal de conversation avec le robot [!DNL Workfront], procédez comme suit :

      * Commencez à saisir **[!DNL @workfront]** dans le champ de [!UICONTROL conversation], puis sélectionnez le canal du robot [!DNL Workfront] que vous souhaitez.
      * Continuez la saisie de la **[!UICONTROL nouvelle tâche]** dans le champ de [!UICONTROL conversation] pour créer une tâche.

        La carte [!UICONTROL Nouvelle tâche] s’affiche dans le canal du robot [!DNL Workfront].

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. Dans le canal du robot [!UICONTROL Workfront], spécifiez les informations suivantes sur la carte [!UICONTROL Nouvelle tâche] :

   * Nom de la tâche dans le champ **[!UICONTROL Écrire le titre de la tâche]**.
   * Description de la tâche dans le champ **[!UICONTROL Écrire la description de la tâche]**.
   * Date à laquelle la tâche doit être effectuée, dans le champ **[!UICONTROL Date d’échéance]**.

1. Cliquez sur **[!UICONTROL Enregistrer].**

   La nouvelle tâche personnelle est créée dans [!DNL Workfront]. Un [!UICONTROL numéro de référence] y est affecté et est visible dans la carte de la [!UICONTROL nouvelle tâche].

   Pour plus d’informations sur les numéros de référence, consultez la section [[!UICONTROL Numéros de référence] des objets ](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) dans l’article [Comprendre les objets dans  [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facultatif) Cliquez sur **[!UICONTROL Modifier]** pour modifier les informations de la tâche.
1. (Facultatif) Cliquez sur **[!UICONTROL Afficher dans[!DNL Workfront]]** pour ouvrir la tâche dans un nouvel onglet dans [!DNL Workfront] et la modifier, la déplacer vers un projet ou l’affecter à une autre personne.
