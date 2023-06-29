---
product-area: reporting
navigation-topic: reporting-elements
title: Création ou modification de vues dans Adobe Workfront
description: Vous pouvez personnaliser le type d’informations que vous affichez à l’écran à l’aide de vues. Vous pouvez utiliser plusieurs types de vues dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 11e239bd47a007adbec1770dafc7f7a5d97eb57e
workflow-type: tm+mt
source-wordcount: '1787'
ht-degree: 1%

---

# Création ou modification de vues dans Adobe Workfront

{{highlighted-preview}}

Vous pouvez personnaliser le type d’informations que vous affichez à l’écran à l’aide de vues. Vous pouvez utiliser plusieurs types de vues dans Adobe Workfront.

Cet article décrit comment créer et modifier des vues standard pour les listes et les rapports, ainsi que comment créer des vues agiles. Pour plus d’informations, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux Rapports, tableaux de bord et calendriers pour créer une vue dans un rapport</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour créer ou modifier une vue dans un rapport</p> <p>Gérer les autorisations pour une vue afin de la modifier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création ou personnalisation d’une vue

Le processus de création ou de personnalisation d’une vue varie selon que vous créez ou personnalisez une vue standard ou une vue agile.

* [Création ou personnalisation d’une vue standard](#create-or-customize-a-standard-view)
* [Création ou personnalisation d’une vue agile](#create-or-customize-an-agile-view)

### Création ou personnalisation d’une vue standard {#create-or-customize-a-standard-view}

Vous pouvez créer une vue standard ou personnaliser une vue standard existante que vous avez créée précédemment.

1. Cliquez sur le bouton **Affichage** menu déroulant sur toute liste dans laquelle vous souhaitez créer ou personnaliser une vue.
1. (Facultatif) Pour personnaliser une vue existante, sélectionnez la vue standard que vous souhaitez personnaliser.\
   Les vues standard sont disponibles sur tout type de liste dans Workfront, tel qu’un rapport, une liste de projets ou une liste de tâches.
1. Cliquez sur le bouton **Affichage** menu déroulant, puis cliquez sur **Vue Personnaliser** ou **Nouvelle vue**.\
   Le **Vue Personnaliser** s’affiche.

1. Dans le **Aperçu des colonnes** , effectuez l’une des opérations suivantes :

   * Modifiez la valeur d’une colonne en cliquant sur le titre de la colonne, puis en sélectionnant un nouveau champ.
   * Ajoutez une colonne en cliquant **Ajouter une colonne**, commencez à saisir le nom de la colonne à ajouter, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.
   * Ajustez l’ordre d’affichage des colonnes en faisant glisser le titre de la colonne vers un nouvel emplacement.

      * (Facultatif) Dans le **Paramètres des colonnes** , cliquez sur la zone **Résumer cette colonne par** , puis sélectionnez l’une des options disponibles pour résumer les informations. Lorsque vous sélectionnez cette option, les informations contenues dans votre colonne sont agrégées dans les regroupements du rapport.\
        Pour les champs de date, vous pouvez résumer les valeurs par les options suivantes :

         * Maximum
         * Minimum

        Pour les champs Nombre et Devise, vous pouvez résumer les valeurs par les options suivantes :

         * Nombre
         * Sum
         * Moyenne
         * Maximum
         * Minimum

        >[!NOTE]
        >
        >Les exceptions suivantes s’appliquent aux objets parents (par exemple, les tâches parents) lorsque vous agrègez des valeurs pour les champs suivants en regroupements :
        >   
        >   * Tous les champs de nombre et de devise, à l’exception des heures réelles (par exemple, le coût du travail planifié/réel, le coût des dépenses planifiées/réelles, le coût planifié/réel, les heures planifiées), ne regroupent que les valeurs des tâches enfants et des tâches autonomes. Ils n’agrégent pas les valeurs des tâches parents ou des parents des parents.
        >   * Les heures réelles combinent les valeurs du parent principal et des tâches autonomes ; ils n’agrégent pas les chiffres des parents des tâches parents ou des tâches enfants.
        >   * Les champs de données personnalisés pour les valeurs numériques et monétaires regroupent toutes les tâches : parents, enfants, parents et tâches autonomes.
        >   
        >

        Pour plus d’informations sur l’utilisation de regroupements dans un rapport, reportez-vous à l’article [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Facultatif) Cliquez sur **Options avancées** pour spécifier les informations suivantes pour la colonne :

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Personnaliser le libellé de colonne</strong></td> 
           <td><p>Spécifiez un libellé personnalisé pour la colonne. Ce libellé remplace le libellé par défaut.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Format du champ</strong></td> 
           <td>Sélectionnez le format d'affichage des valeurs des champs de la colonne.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Afficher cette colonne lorsque le graphique est visible sur un tableau de bord.</strong></td> 
           <td><p>Sélectionnez cette option pour afficher cette colonne sur un tableau de bord, lorsque le rapport est affiché côte à côte avec un autre rapport. Lorsque cette option n'est pas sélectionnée, cette colonne ne s'affiche pas lors de l'affichage du rapport dans un tableau de bord où les rapports sont affichés côte à côte.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Règles de la colonne</strong></td> 
           <td><p>Cliquez sur <strong>Ajouter une règle pour cette colonne</strong> pour définir une règle pour la colonne. Après avoir ajouté une règle, vous pouvez définir des styles de champ et de texte pour l’affichage des champs correspondant à cette règle. Cliquez sur <strong>Ajouter une règle</strong> après avoir défini la règle.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Pour plus d’informations sur le formatage conditionnel des vues dans les rapports, reportez-vous à l’article [Utilisation de la mise en forme conditionnelle en mode Texte](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Conditionnel) Si vous avez cliqué sur **Options avancées**, cliquez sur **Terminé**.

1. Cliquez sur **Enregistrer la vue** pour créer une vue ou remplacer la vue actuelle par vos modifications.\
   Ou\
   Cliquez sur **Enregistrer comme nouvelle vue** pour enregistrer vos modifications en tant que nouvelle vue.

   >[!TIP]
   >
   >Le **Enregistrer comme nouvelle vue** est la seule option disponible lorsque vous personnalisez une vue Workfront intégrée.

   Votre accès détermine le mode d’enregistrement de la vue. Si vous avez créé la vue d’origine, vous pouvez enregistrer les modifications ; dans le cas contraire, vous êtes invité à enregistrer une version. Gardez à l’esprit que les modifications que vous apportez à la vue affectent les utilisateurs avec lesquels la vue a été partagée.

### Création ou personnalisation d’une vue agile {#create-or-customize-an-agile-view}

Vous pouvez créer une vue Agile ou personnaliser une vue Agile existante que vous avez créée précédemment.

>[!IMPORTANT]
>
>Les vues agiles sont disponibles uniquement lors de l’affichage d’un projet.

Pour plus d’informations sur les vues Agile, voir l’article [Gestion d’un projet en mode Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
><span class="preview">Cette procédure s’applique uniquement à la vue Agile héritée, et non à la vue Panorama d’un projet.</span>

Pour créer ou personnaliser une vue Agile :

1. Accédez à la liste des tâches d’un projet.
1. Cliquez sur le bouton **Agile Storboard** icon ![Icône Agile Storyboard](assets/agile-storyboard-nwe.png).

   <span class="preview">Ou</span>

   <span class="preview">Cliquez sur le bouton **Panorama** icon ![Icône Panorama](assets/board-icon-for-agile-view.png), puis cliquez sur **Utiliser la version agile héritée** sur le panorama.</span>

1. (Conditionnel) Pour personnaliser une vue Agile existante :

   1. Cliquez sur le bouton **Affichage** , puis sélectionnez la vue agile à personnaliser.\
      Vous ne pouvez pas personnaliser la vue Agile par défaut.

   1. Cliquez sur le bouton **Affichage** menu déroulant, puis cliquez de nouveau sur **Vue Personnaliser**.\
      ![](assets/view-agile-customize.png)

1. (Conditionnel) Pour créer une vue agile, cliquez sur **Nouvelle vue**.\
   Le **Personnalisation de l’affichage agile** s’affiche.

1. Dans le **Personnalisation de l’affichage agile** , indiquez un nom pour la vue agile.\
   Nous vous recommandons d’inclure le mot &quot;Agile&quot; dans le nom de votre vue afin que les utilisateurs sachent qu’il s’agit d’une vue agile.\
   Ce nom s’affiche dans la variable **Affichage** lors de la sélection d’une vue.

1. Définissez les colonnes d’état à afficher sur le panorama des articles dans la vue agile. Il s’agit des états des tâches définis par l’administrateur de Workfront, comme décrit dans la section [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Seuls les états système peuvent être utilisés sur la carte Agile. Si un état est disponible uniquement pour un groupe individuel dont vous êtes membre, il n’est pas disponible sur le tableau de bord agile. En outre, les tâches dont l’état est disponible uniquement pour un groupe personnalisé ne sont pas visibles lors de l’affichage du projet dans une vue Agile.

   Les utilisateurs peuvent déplacer des articles parmi ces colonnes d’état sur le tableau Agile.\
   Lors de la définition des colonnes d’état, vous pouvez effectuer les opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Réorganiser les colonnes d’état :</strong> </td> 
      <td> Faites glisser une colonne d’état dans l’ordre dans lequel elle doit apparaître.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Supprimer les colonnes d’état :</strong> </td> 
      <td>Cliquez sur l’icône (x) dans la colonne à supprimer.<br>Vous ne pouvez pas supprimer l’état "Nouveau", à moins qu’un état personnalisé n’ait été ajouté à la vue et que l’état personnalisé corresponde à "Nouveau".<br>Pour plus d’informations sur la création d’un état personnalisé, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Création ou modification d’un état</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ajouter des colonnes d’état :</strong> </td> 
      <td> <p>Cliquez sur le bouton <strong>Plus</strong> puis sélectionnez l’état que vous souhaitez ajouter.<br>Tous les statuts système par défaut s’affichent, ainsi que tous les statuts personnalisés qui ont été partagés avec vous.<br>Vous pouvez configurer jusqu’à 10 états à afficher.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. Dans le **Associer la couleur de la carte à** , sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Histoire:</strong> </td> 
      <td>Toutes les sous-tâches correspondent à la couleur de la tâche parent, de sorte que les couleurs de tous les articles d’un couloir donné soient les mêmes.<br>Les couleurs sont attribuées de manière aléatoire aux tâches lorsqu’elles sont créées si la tâche ne comporte aucune sous-tâche ou n’a pas de tâche parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formulaire libre:</strong> </td> 
      <td> Toutes les cartes sont affichées en bleu par défaut jusqu’à ce qu’un utilisateur modifie manuellement la couleur, comme décrit dans l’article. <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Catégorisation des articles par couleur sur le panneau de défilement</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité:</strong> </td> 
      <td> <p> Les couleurs sont associées à la priorité de l’article, comme suit :</p> 
       <ul> 
        <li>Élevé = Rouge</li> 
        <li>Moyen = Jaune</li> 
        <li>Faible = Vert<br>Si votre administrateur Workfront a configuré des priorités personnalisées pour votre système Workfront, la priorité la plus élevée est le rouge, la seconde la jaune et les autres le vert.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Propriétaire de la tâche:</strong> </td> 
      <td> Toutes les histoires avec la même personne désignée Principale sont de la même couleur.<br>La personne désignée Principale est l’utilisateur qui a été affecté la première fois à la tâche. </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans le **Agile** , dans la section **Champs supplémentaires** zone, cliquez sur **Ajouter un champ**, puis sélectionnez le champ à ajouter aux cartes d’articles. (Il s’agit des mêmes champs que ceux que vous pouvez ajouter lors de la création d’une vue ou de la création de colonnes pour un rapport.)\
   Répétez cette procédure pour ajouter jusqu’à trois champs supplémentaires aux fiches d’article.\
   Lorsque vous ajoutez des champs aux cartes d’articles, ils sont en lecture seule et s’affichent uniquement lorsque le champ est renseigné.

   Par défaut, les types de données suivants s’affichent sur la carte d’article :

   * Nom de l’article avec un lien direct vers la tâche
   * Nom du projet avec un lien direct vers le projet\
     Ce lien s&#39;affiche uniquement lors de l&#39;utilisation de la vue agile sur une itération. il n’est pas affiché lors de l’utilisation d’une vue agile sur un projet.
   * Description de la tâche
   * Engagement actuel
   * Affichez et modifiez le pourcentage terminé en ajustant le pourcentage terminé ou en ajustant le nombre de points ou d’heures terminé
   * Utilisateurs affectés

   Vous pouvez afficher des données supplémentaires (y compris des données personnalisées) sur les cartes d’article. Pour plusieurs raisons, vous pouvez afficher des champs supplémentaires sur les cartes d’articles. Par exemple, vous pouvez afficher l’ID de client si vous travaillez sur des articles pour plusieurs clients dans le projet ou si vous souhaitez afficher la date de début de la tâche.

1. Cliquer sur **Enregistrer**.\
   Votre accès détermine le mode d’enregistrement de la vue. Si vous avez créé la vue d’origine, vous pouvez enregistrer les modifications ; dans le cas contraire, vous êtes invité à enregistrer une version. Gardez à l’esprit que les modifications que vous apportez à la vue affectent les utilisateurs avec lesquels la vue a été partagée.

1. (Facultatif) Cliquez sur le **Mode Liste** icon ![](assets/list-view-in-agile-view-for-tasks.png) pour revenir à la liste des tâches.
