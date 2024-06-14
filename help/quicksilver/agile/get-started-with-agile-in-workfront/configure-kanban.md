---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurer Kanban
description: Vous créez une équipe agile Kanban ou Scrum dans [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 2%

---

# Configurer [!UICONTROL Kanban]

<!--Audited: 12/2023-->

Vous pouvez créer une équipe agile dans [!DNL Adobe Workfront] comme décrit dans [Créer une équipe agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Lors de la création d’une équipe agile, vous pouvez choisir la méthodologie que l’équipe utilise pour terminer son travail. Vous pouvez choisir parmi les options suivantes :

* Scrum
* Kanban

Cet article décrit comment configurer les paramètres d’une équipe Kanban. Après avoir créé une équipe agile et choisi la méthodologie Kanban, vous pouvez consulter cet article pour mettre à jour les paramètres suivants :

* Si les articles sont estimés en points ou en heures
* Colonnes d’état sur le tableau de bord agile
* Champs supplémentaires à afficher sur les cartes d’article sur le tableau de bord agile
* Limite de travail en cours (WIP)
* Comment ajouter automatiquement des articles du journal
* Combien de temps les cartes restent sur le panorama Kanban ?

Pour plus d’informations sur la configuration d’une équipe Scrum, voir [Configuration de Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>Nouveau : [!UICONTROL Standard]</p> 
   ou
   <p>Actuel : [!UICONTROL Travail] ou version ultérieure</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Modifier l’accès aux équipes</p>  </td> 
  </tr>

</tbody> 
</table>

*Pour savoir quel plan ou type de licence vous disposez, contactez votre [!DNL Workfront] administrateur.

+++

## Configurer l’estimation des articles en points ou en heures

Vous pouvez configurer les articles à estimer en points ou en heures.

Pour configurer l’estimation des articles pour votre équipe agile :

{{step1-to-team}}

1. Cliquez sur le bouton **[!UICONTROL Changer d’équipe]** icon ![](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la zone de recherche.
1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![](assets/more-menu.png) , puis sélectionnez **[!UICONTROL Modifier]**.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , dans la section **[!UICONTROL Estimation des articles dans]** , choisissez si vous souhaitez utiliser des points ou des heures pour estimer la taille (charge de travail) des articles. Si vous sélectionnez Points, indiquez le nombre d’heures égal à 1 point. (La valeur par défaut est de 1 point = 8 heures.) Il s’agit du nombre d’heures planifiées ajoutées à l’article.

   **Exemple :** Si vous avez choisi d’estimer les articles en points et qu’un point équivaut à 8 heures, et qu’un article est estimé à 3 points, 24 Heures planifiées sont ajoutées à l’article.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration des colonnes d’état sur le tableau de bord agile

Vous pouvez définir les états qui existent sur le tableau de bord de l’équipe agile. Ce sont les seuls statuts qui s&#39;affichent sur le tableau.

Pour définir les états disponibles pour le panorama d’articles associé à l’équipe agile :

{{step1-to-team}}

1. Cliquez sur le bouton **[!UICONTROL Changer d’équipe]** icon ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , recherchez la **[!UICONTROL Story Board]** zone.

1. (Facultatif) Cliquez sur **[!UICONTROL Ajouter une colonne]** pour ajouter une colonne d’état supplémentaire au tableau de bord.
1. (Facultatif) Faites glisser une colonne d’état à l’aide de l’indicateur glisser-déposer pour réorganiser les colonnes d’état sur le tableau d’articles. La première colonne ne peut pas être déplacée et vous ne pouvez pas faire glisser une autre colonne devant la première colonne.

   ![Glisser-déposer](assets/agile-story-card-drag-and-drop.png)

1. Sélectionnez les états de la tâche.

   >[!IMPORTANT]
   >
   >Seuls les états verrouillés à l’échelle du système peuvent être sélectionnés. Vous ne pouvez pas sélectionner d’états spécifiques à un groupe. Le statut de la première colonne correspond toujours à **[!UICONTROL Nouveau]**.

   Vous pouvez ajouter des états personnalisés si votre [!DNL Workfront] l’administrateur les a configurés. Pour plus d’informations, voir [Création ou modification d’un état](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration de champs supplémentaires à afficher sur les cartes d’articles sur le tableau de bord agile

Lorsque vous ajoutez des champs aux cartes d’articles, ils sont en lecture seule et s’affichent uniquement lorsque le champ est renseigné.

Par défaut, les types de données suivants s’affichent sur la fiche d’article pour les tâches et les problèmes :

* Nom de l’article avec un lien direct vers la tâche ou le problème
* Nom du projet avec un lien direct vers le projet
* Ce lien s’affiche uniquement pour les articles, et non pour les sous-tâches
* Description de la tâche ou du problème
* Engagement actuel
* Affichez et modifiez le pourcentage terminé soit en ajustant le pourcentage terminé soit en ajustant le nombre de points ou d’heures terminé
* Utilisateurs affectés

Vous pouvez afficher des données supplémentaires (y compris des données personnalisées) sur les cartes d’article. Pour plusieurs raisons, vous pouvez afficher des champs supplémentaires sur les cartes d’articles. Par exemple, vous pouvez afficher l’ID de client si vous travaillez sur des articles pour plusieurs clients au cours de l’itération ou si vous souhaitez afficher la date de début du projet ou la date de fin du projet.

>[!NOTE]
>
>Si vous utilisez un champ personnalisé sur une carte d’article, il ne peut pas contenir de point (ou point) dans le nom.

Pour configurer les fiches d’article affectées à l’équipe agile afin d’afficher des champs supplémentaires :

{{step1-to-team}}

1. Cliquez sur le bouton **[!UICONTROL Changer d’équipe]** icon ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.\

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , saisissez un nom de champ pour le localiser.

   ![Champs supplémentaires](assets/agile-additional-fields-kanban.png)

1. Sélectionnez le nom du champ que vous souhaitez ajouter.
1. Saisissez le **[!UICONTROL Nom d’affichage]** pour que le champ s’affiche sur l’article ou la carte de problème.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration de la limite de travail en cours (WIP)

Lorsque vous définissez la limite de travail en cours d’une équipe Kanban, vous pouvez contrôler le nombre d’éléments sur lesquels l’équipe travaille actuellement en limitant le nombre de tâches pouvant apparaître dans la variable [!UICONTROL Nouveau] ou le [!UICONTROL En cours] sur la [!UICONTROL Kanban] panorama.

Après avoir configuré la limite de travail en cours pour une équipe Kanban, vous pouvez afficher la limite de travail en cours et la mettre à jour à partir de la [!UICONTROL Kanban] tableau de bord agile, comme décrit à la section [Gérez la limite du travail en cours (WIP) sur la [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Pour limiter les travaux en cours pour votre équipe Kanban :

{{step1-to-team}}

1. Cliquez sur le bouton **[!UICONTROL Changer d’équipe]** icon ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe Kanban que vous souhaitez gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![](assets/more-menu.png), puis sélectionnez **[!UICONTROL Modifier]**.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , dans la section **[!UICONTROL Méthodologie]** Vérifiez que Kanban est sélectionné.

1. Dans le **[!UICONTROL Story Board]** , dans la section **[!UICONTROL Limite de travaux en cours]** , indiquez le nombre maximal d’éléments autorisés dans chaque colonne du [!UICONTROL Kanban] tableau de bord agile. Vous pouvez définir une limite différente pour chaque colonne. La limite maximale que vous pouvez définir pour chaque colonne est de 100.\
   Lorsqu’elle est définie, la limite de travaux en cours affiche un message d’avertissement sur la variable [!UICONTROL Kanban] agile story board chaque fois que la limite est dépassée pour n’importe quelle colonne du forum. Ce message d’avertissement s’affiche uniquement la première fois que la limite de travaux en cours est dépassée. Ce message d’avertissement ne s’affiche sur aucune colonne dont l’état est égal à [!UICONTROL Terminer].\
   La limite de travaux en cours est simplement un avertissement visuel et ne limite pas votre équipe à un nombre d’articles supérieur à la limite que vous avez définie.

   ![Limite de travail](assets/wip-limit-350x193.png)

1. Cliquez sur **Enregistrer les modifications**.

## Configuration de l’ajout automatique d’articles dans le journal

<!-- this functionality needs to be verified-->

Vous pouvez configurer les articles du journal pour qu’ils soient automatiquement ajoutés à la première colonne du [!UICONTROL Kanban] panorama immédiatement après le déplacement d’un élément de cette colonne.

{{step1-to-team}}

1. Cliquez sur le bouton **[!UICONTROL Changer d’équipe]** icon ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe Kanban que vous souhaitez gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![](assets/more-menu.png), puis sélectionnez **[!UICONTROL Modifier]**.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Sélectionner **[!UICONTROL Ajout automatique de l’article suivant depuis le journal des logs]** pour configurer que l’élément suivant du journal en souffrance soit automatiquement ajouté au **[!UICONTROL Nouveau]** lorsqu’un élément est déplacé hors de la colonne **[!UICONTROL En cours]** colonne .

   Les utilisateurs doivent activer la variable **Afficher le journal** sur le [!UICONTROL Kanban] panorama pour que cette fonctionnalité soit prise en compte. Lorsque les utilisateurs activent la variable [!UICONTROL Afficher le journal] sur le [!UICONTROL Kanban Board], les fonctionnalités suivantes ont lieu :

   Chaque fois qu’une histoire est déplacée du [!UICONTROL En cours] dans une colonne du tableau de bord qui représente une [!UICONTROL Terminer] (ou un état qui correspond à [!UICONTROL Terminer]), un article de la colonne des logs de diffusion passe automatiquement à la [!UICONTROL Nouveau] de la colonne [!UICONTROL Kanban Board].
Une fois ajouté à partir du journal en souffrance, l’article ayant la priorité la plus élevée est ajouté au tableau de bord.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configurez la durée pendant laquelle les cartes restent sur le [!UICONTROL Kanban] board

Vous pouvez choisir la durée pendant laquelle les cartes terminées restent sur la variable [!UICONTROL Kanban] panorama. Tâches qui abandonnent la fonction [!UICONTROL Kanban] le panorama est toujours accessible dans leur projet d’origine.

{{step1-to-team}}

1. (Facultatif) Cliquez sur le **[!UICONTROL Changer d’équipe]** icon ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Kanban dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Sélectionnez l&#39;équipe Kanban.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![](assets/more-menu.png) , puis sélectionnez **[!UICONTROL Modifier]**.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Nombre de jours pendant lesquels les cartes terminées restent sur le panorama Kanban]** , sélectionnez une valeur dans le menu déroulant.

   Vous pouvez choisir un nombre compris entre 1 et 30 jours.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
