---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configuration de Scrum
description: Vous pouvez configurer les options suivantes pour les équipes agiles Scrum pendant ou après la création de l’équipe.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# Configurer [!UICONTROL Scrum]

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

>[!NOTE]
>
>Ce paramètre ne peut pas être modifié si l’équipe possède des itérations actuellement en cours.

Vous pouvez configurer les articles à estimer en points ou en heures.

Pour configurer l’estimation des articles pour votre équipe agile :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!UICONTROL Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** , puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.\
   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , dans la section **[!UICONTROL Estimation des articles dans]** , choisissez si vous souhaitez utiliser des points ou des heures pour estimer la taille (charge de travail) des articles. Si vous sélectionnez Points, indiquez le nombre d’heures égal à 1 point. (La valeur par défaut est de 1 point = 8 heures.) Il s’agit du nombre d’heures planifiées ajoutées à l’article.

   **Exemple :** Si vous avez choisi d’estimer les articles en points et qu’un point équivaut à 8 heures, et qu’un article est estimé à 3 points, 24 Heures planifiées sont ajoutées à l’article.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration des colonnes d’état sur le tableau de bord agile

Vous pouvez configurer les colonnes qui s’affichent sur le tableau de bord agile pour toutes les itérations affectées à votre équipe ou pour un projet donné.

* [Configuration des colonnes d’état pour les itérations](#configure-status-columns-for-iterations)
* [Configuration des colonnes d’état pour les projets](#configure-status-columns-for-projects)

### Configuration des colonnes d’état pour les itérations {#configure-status-columns-for-iterations}

Vous pouvez définir les états qui existent sur le tableau de bord de l’équipe agile. Ce sont les seuls statuts qui s&#39;affichent sur le tableau.

Pour définir les états disponibles pour le panorama d’articles associé à l’équipe agile :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , recherchez la **[!UICONTROL Story Board]** zone.

1. (Facultatif) Cliquez sur **[!UICONTROL Ajouter une colonne]** pour ajouter une colonne d’état supplémentaire au tableau de bord.
1. (Facultatif) Faites glisser une colonne d’état à l’aide de l’indicateur glisser-déposer pour réorganiser les colonnes d’état sur le tableau d’articles. La première colonne ne peut pas être déplacée et vous ne pouvez pas faire glisser une autre colonne devant la première colonne.

   ![Glisser-déposer](assets/agile-story-card-drag-and-drop.png)

1. Sélectionnez les statuts des tâches et des problèmes. Les statuts des tâches sont affichés sous forme de titre de colonne pour chaque colonne du panorama. Les états du problème que vous sélectionnez correspondent aux états de la tâche. Cela signifie que lorsque vous déplacez un problème vers une autre colonne du panorama des articles, l’état du problème est modifié dans les états du problème affichés ici, et non dans le nom de la colonne du panorama des articles (qui reflète l’état de la tâche).

   >[!IMPORTANT]
   >
   >Seuls les états verrouillés à l’échelle du système peuvent être sélectionnés ; vous ne pouvez pas sélectionner d’états spécifiques à un groupe. En outre, l’état de la première colonne correspond toujours à **[!UICONTROL Nouveau]**.

   Vous pouvez ajouter des états personnalisés si votre [!DNL Workfront] l’administrateur les a configurés ; les états personnalisés peuvent être configurés comme décrit dans la section [Création ou modification d’un état](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Lors de la sélection des états d’un problème, la troisième colonne est toujours définie par défaut sur [!UICONTROL Fermé]. Si vous disposez de plus de trois colonnes, veillez à les mettre à jour manuellement pour qu’elles reflètent les états appropriés.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

### Configuration des colonnes d’état pour les projets {#configure-status-columns-for-projects}

Pour plus d’informations sur la configuration des colonnes d’état pour un projet, voir la section [Créez ou personnalisez une [!UICONTROL Agile] view](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) dans l’article [Créer ou modifier des vues dans [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

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

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!UICONTROL Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.\
   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le **[!UICONTROL Agile]** , saisissez un nom de champ pour le localiser.

   ![Champs supplémentaires](assets/agile-additional-fields-scrum.png)

1. Sélectionnez le nom du champ que vous souhaitez ajouter.
1. Saisissez le **[!UICONTROL Nom d’affichage]** pour que le champ s’affiche sur l’article ou la carte de problème.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configuration de l’utilisation des indicateurs de couleur pour les articles sur le tableau de bord agile

Par défaut, les mosaïques de panorama dans une itération agile sont codées par couleur en fonction du projet auquel l’article est associé. Chaque projet se voit attribuer arbitrairement une couleur sur le tableau de bord. Vous pouvez modifier ce comportement par défaut pour chaque équipe agile. Les couleurs des articles agiles peuvent être liées à la priorité des articles, à leur propriétaire, etc.

Pour modifier le comportement de l’affectation des couleurs aux articles pour une équipe agile :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.

   ![Éditer l’équipe](assets/edit-team-settings-350x205.png)

1. Dans le [!UICONTROL Agile] , dans la section [!UICONTROL Associer la couleur de la carte à] , sélectionnez l’une des options suivantes :

   * **[!UICONTROL Projet]**: Les couleurs sont associées au projet auquel l’histoire est liée. (Lorsqu’un article est créé, il doit être associé à un projet, comme décrit à la section [Création d’un article agile](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Toutes les tâches d’un même projet s’affichent avec la même couleur.
   * **[!UICONTROL Libre de forme]**: Toutes les cartes sont affichées en bleu par défaut jusqu’à ce qu’un utilisateur modifie manuellement la couleur, comme décrit dans la section [[!UICONTROL Catégorisation des articles par couleur] sur le panneau Scrum](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Priorité]**: Les couleurs sont associées à la priorité de l’article, comme suit :

      * Élevé = Rouge
      * Moyen = Jaune
      * Faible = Vert\

         Si votre administrateur système a configuré des priorités personnalisées pour votre [!DNL Workfront] système, la priorité la plus élevée est le rouge, la seconde le jaune et la troisième le vert.
   * **[!UICONTROL Propriétaire de la tâche]**: Toutes les histoires avec la même personne désignée Principale sont de la même couleur. La personne désignée Principale est l’utilisateur qui a été affecté la première fois à la tâche.


1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Configurer l’application des dates lors de l’ajout d’éléments de travail à une itération

Par défaut, lorsque vous ajoutez un élément de travail à une itération par flux, la Date de début planifiée et la Date de fin planifiée de l’élément de travail sont modifiées pour correspondre aux dates de début et de fin de l’itération. Vous pouvez choisir de conserver les dates d’origine sur toutes les tâches de l’équipe.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Équipes]**.
1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.\
   Uniquement les membres de l’équipe qui disposent d’une [!UICONTROL Plan] ou [!UICONTROL Travail] voir cette option.
1. Dans le [!UICONTROL Agile] , dans la section [!UICONTROL Lorsqu’un élément de travail est ajouté à une itération] , sélectionnez l’une des options suivantes :

   * **[!UICONTROL Modifier la date de début planifiée et la date de fin planifiée pour qu’elles correspondent aux dates de début et de fin de l’itération]**: Lorsque des éléments de travail sont ajoutés à une itération, les dates de l’élément de travail sont remplacées par les dates d’itération.\

      Pour plus d’informations sur la façon dont les dates sont modifiées, voir la section [Comprendre comment l’ajout d’articles affecte les dates des tâches](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) dans l’article [Ajouter des articles à une itération existante](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Ne modifiez pas la date de début planifiée et la date de fin planifiée pour qu’elles correspondent aux dates de début et de fin de l’itération.]**: Lorsque des éléments de travail sont ajoutés à une itération, ils conservent leurs dates d’origine.

   Si vous modifiez l’option de date, les dates des tâches déjà en itération ne sont pas ajustées.

   Ces options peuvent affecter les dates lorsque les équipes assignent des tâches aux itérations les unes des autres. Par exemple, l’équipe A modifie les dates des tâches en fonction des dates d’itération et l’équipe B ne modifie pas les dates des tâches. Si l’équipe B affecte un élément de travail à l’itération de l’équipe A, les dates de l’élément de travail seront modifiées. Cependant, si l’équipe A affecte un élément de travail à l’itération de l’équipe B, les dates ne changent pas.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
