---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurer Kanban
description: Vous pouvez configurer les options suivantes pour les équipes agiles de Kanban pendant ou après la création de l’équipe.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Configurer [!UICONTROL Kanban]

Vous pouvez configurer les options suivantes pour les équipes agiles pendant ou après la création de l’équipe. Vous créez une équipe agile (Kanban ou Scrum) dans [!DNL Adobe Workfront] comme décrit dans [Création d’une équipe agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Configurer l’estimation des articles en points ou en heures

Vous pouvez configurer les articles à estimer en points ou en heures.

Pour configurer l’estimation des articles pour votre équipe agile :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** , puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.\
   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , dans la section **[!UICONTROL Estimation des articles dans]** , choisissez si vous souhaitez utiliser des points ou des heures pour estimer la taille (charge de travail) des articles. Si vous sélectionnez Points, indiquez le nombre d’heures égal à 1 point. (La valeur par défaut est de 1 point = 8 heures.) Il s’agit du nombre d’heures planifiées ajoutées à l’article.

   **Exemple :** Si vous avez choisi d’estimer les articles en points et qu’un point équivaut à 8 heures, et qu’un article est estimé à 3 points, 24 Heures planifiées sont ajoutées à l’article.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration des colonnes d’état sur le tableau de bord agile

Vous pouvez définir les états qui existent sur le tableau de bord de l’équipe agile. Ce sont les seuls statuts qui s&#39;affichent sur le tableau.

Pour définir les états disponibles pour le panorama d’articles associé à l’équipe agile :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!UICONTROL Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , recherchez la **[!UICONTROL Story Board]** zone.

1. (Facultatif) Cliquez sur **[!UICONTROL Ajouter une colonne]** pour ajouter une colonne d’état supplémentaire au tableau de bord.
1. (Facultatif) Faites glisser une colonne d’état à l’aide de l’indicateur glisser-déposer pour réorganiser les colonnes d’état sur le tableau d’articles. La première colonne ne peut pas être déplacée et vous ne pouvez pas faire glisser une autre colonne devant la première colonne.

   ![Glisser-déposer](assets/agile-story-card-drag-and-drop.png)

1. Sélectionnez les états de la tâche.

   >[!IMPORTANT]
   >
   >Seuls les états verrouillés à l’échelle du système peuvent être sélectionnés ; vous ne pouvez pas sélectionner d’états spécifiques à un groupe. En outre, l’état de la première colonne correspond toujours à **[!UICONTROL Nouveau]**.

   Vous pouvez ajouter des états personnalisés si votre [!DNL Workfront] l’administrateur les a configurés ; les états personnalisés peuvent être configurés comme décrit dans la section [Création ou modification d’un état](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration de champs supplémentaires à afficher sur les cartes d’articles sur le tableau de bord agile

Lorsque vous ajoutez des champs aux cartes d’article, ils sont en lecture seule et s’affichent uniquement lorsque le champ est renseigné.

Par défaut, les types de données suivants s’affichent sur la fiche d’article pour les tâches et les problèmes :

* Nom de l’article avec un lien direct vers la tâche ou le problème
* Nom du projet avec un lien direct vers le projet
* Ce lien s’affiche uniquement pour les articles, et non pour les sous-tâches.
* Description de la tâche ou du problème
* Engagement actuel
* Affichez et modifiez le pourcentage terminé en ajustant le pourcentage terminé ou en ajustant le nombre de points ou d’heures terminé
* Utilisateurs affectés

Vous pouvez afficher des données supplémentaires (y compris des données personnalisées) sur les cartes d’article. Pour plusieurs raisons, vous pouvez afficher des champs supplémentaires sur les cartes d’articles. Par exemple, vous pouvez afficher l’ID de client si vous travaillez sur des articles pour plusieurs clients au cours de l’itération ou si vous souhaitez afficher la date de début du projet ou la date de fin du projet.

>[!NOTE]
>
>Si vous utilisez un champ personnalisé sur une carte d’article, il ne peut pas contenir de point/point dans le nom.

Pour configurer les fiches d’article affectées à l’équipe agile afin d’afficher des champs supplémentaires :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.\
   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , saisissez un nom de champ pour le localiser.

   ![Champs supplémentaires](assets/agile-additional-fields-kanban.png)

1. Sélectionnez le nom du champ que vous souhaitez ajouter.
1. Saisissez le **[!UICONTROL Nom d’affichage]** pour que le champ s’affiche sur l’article ou la carte de problème.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration de la limite de travail en cours (WIP)

Kanban en [!DNL Workfront] vous permet de contrôler la quantité de travail sur laquelle travaille actuellement l’équipe en limitant le nombre de tâches pouvant apparaître dans la variable [!UICONTROL En cours] sur la [!UICONTROL Kanban] panorama.

Lorsque la limite de travaux en cours est configurée, vous pouvez afficher la limite de travaux en cours ou même la mettre à jour à partir de la [!UICONTROL Kanban] tableau de bord agile, comme décrit à la section [Gérez la limite du travail en cours (WIP) sur la [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Pour limiter les travaux en cours pour votre équipe Kanban :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe Kanban que vous souhaitez gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , dans la section **[!UICONTROL Méthodologie]** Vérifiez que Kanban est sélectionné.

1. Dans le **[!UICONTROL Story Board]** , dans la section **[!UICONTROL LIMITE DE TRAVAIL]** , indiquez le nombre maximal d’éléments autorisés dans chaque colonne du [!UICONTROL Kanban] tableau de bord agile. Vous pouvez définir une limite différente pour chaque colonne. La limite maximale que vous pouvez définir pour chaque colonne est de 100.\
   Lorsqu’elle est définie, la limite de travaux en cours affiche un message d’avertissement sur la variable [!UICONTROL Kanban] tableau de bord agile chaque fois que la limite est dépassée pour n’importe quelle colonne du tableau de bord. Ce message d’avertissement s’affiche uniquement la première fois que la limite de travaux en cours est dépassée. Ce message d’avertissement ne s’affiche sur aucune colonne dont l’état est égal à [!UICONTROL Terminer].\
   La limite de travaux en cours est simplement un avertissement visuel et ne limite pas votre équipe à un nombre d’articles supérieur à la limite que vous avez définie.

   ![Limite de travail](assets/wip-limit-350x193.png)

1. Cliquez sur **Enregistrer les modifications**.

## Configurer des articles à ajouter automatiquement à partir du journal

Vous pouvez configurer les articles du journal pour qu’ils soient automatiquement ajoutés à la première colonne du [!UICONTROL Kanban] panorama immédiatement après le déplacement d’un élément de cette colonne.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe Kanban que vous souhaitez gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Sélectionner **[!UICONTROL Ajout automatique de l’article suivant depuis le journal des logs]** pour configurer les articles à ajouter automatiquement du journal en souffrance à la première colonne du [!UICONTROL Kanban] tableau de bord.

   Cela se produit chaque fois qu’un article est déplacé dans une colonne du panorama qui représente un statut Terminé (état qui correspond à Terminé). Lorsqu’il est ajouté à partir du journal, l’article ayant la priorité la plus élevée est ajouté au tableau d’articles. sélectionnez cette option pour configurer l’élément suivant du journal à ajouter automatiquement au journal. **[!UICONTROL En cours]** lorsqu’un élément est déplacé hors de la colonne **[!UICONTROL En cours]** colonne .

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configurez la durée pendant laquelle les cartes restent sur le [!UICONTROL Kanban] board

Vous pouvez choisir la durée pendant laquelle les cartes terminées restent sur la variable [!UICONTROL Kanban] panorama. Tâches qui abandonnent la fonction [!UICONTROL Kanban] le panorama est toujours accessible dans leur projet d’origine.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Kanban dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Sélectionnez l&#39;équipe Kanban.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **Edit**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Nombre de jours pendant lesquels les cartes terminées restent sur le panorama Kanban]** , sélectionnez une valeur dans le menu déroulant.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
