---
product-area: reporting
navigation-topic: reporting-elements
title: Créer ou modifier des vues dans Adobe Workfront
description: Vous pouvez personnaliser le type d’informations affichées à l’écran à l’aide des vues. Vous pouvez utiliser plusieurs types de vues dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 95%

---

# Créer ou modifier des vues dans Adobe Workfront

<!-- Audited: 11/2024 -->

Vous pouvez personnaliser le type d’informations affichées à l’écran à l’aide des vues. Vous pouvez utiliser plusieurs types de vues dans Adobe Workfront.

Cet article explique comment créer et modifier des vues standard pour les listes et les rapports, et comment créer des vues Agile. Pour plus d’informations, consultez l’article [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Contributeur ou version ultérieure</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Requête ou supérieure</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux rapports, aux tableaux de bord et aux calendriers pour créer une vue dans un rapport</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet*</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour créer ou modifier une vue dans un rapport</p> <p>Gérer les autorisations d’une vue pour la modifier</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer ou personnaliser une vue

Le processus de création ou de personnalisation d’une vue diffère selon qu’il s’agit d’une vue standard ou d’une vue Agile.

* [Créer ou personnaliser une vue standard](#create-or-customize-a-standard-view)
* [Créer ou personnaliser une vue Agile](#create-or-customize-an-agile-view)

### Créer ou personnaliser une vue standard {#create-or-customize-a-standard-view}

Vous pouvez créer une nouvelle vue standard ou personnaliser une vue standard existante que vous avez créée précédemment.

1. Cliquez sur le menu déroulant **Vue** dans toute liste où vous souhaitez créer ou personnaliser une vue.

1. Cliquez sur le bouton **+ Nouvelle vue** pour créer une vue.
Ou
Cliquez sur l&#39;icône **Modifier** ![Icône Modifier](assets/edit-icon.png) qui s&#39;affiche lorsque vous pointez sur la droite d&#39;une vue existante que vous souhaitez modifier.
La boîte de dialogue **Personnaliser la vue** s’affiche.

1. Dans la section **Aperçu de la colonne**, effectuez l’une des opérations suivantes :

   * Modifiez la valeur de n’importe quelle colonne en cliquant sur le titre de la colonne et en sélectionnant un nouveau champ.
   * Ajoutez une colonne en cliquant sur **Ajouter une colonne**, commencez à saisir le nom de la colonne que vous souhaitez ajouter, puis cliquez dessus lorsqu’elle apparaît dans la liste déroulante.
   * Ajustez l’ordre d’apparition des colonnes en faisant glisser le titre de la colonne vers un nouvel emplacement.

      * (Facultatif) Dans la zone **Paramètres de colonne**, cliquez dans la liste déroulante sur **Résumer cette colonne par**, puis sélectionnez l’une des options disponibles pour résumer les informations. Lorsque vous choisissez cette option, les informations de votre colonne sont agrégées dans les regroupements du rapport.\
        Pour les champs de date, vous pouvez résumer les valeurs en utilisant les options suivantes :

         * Maximum
         * Minimum

        Pour les champs numériques et monétaires, vous pouvez résumer les valeurs en utilisant les options suivantes :

         * Nombre
         * Sum
         * Moyenne
         * Maximum
         * Minimum

        >[!NOTE]
        >
        >Les exceptions suivantes s’appliquent aux objets parent (par exemple, les tâches parent) lorsque vous agrégez des valeurs pour les champs suivants en regroupements :
        >   
        >   * Tous les champs de nombre et de devise, à l’exception des heures effectives (par exemple, le coût prévu/réel de main-d’œuvre, le coût réel/prévu des dépenses, le coût prévu/réel, le nombre d’heures prévues), n’agrègent que les valeurs des tâches enfant et des tâches autonomes. Ils n’agrègent pas les valeurs des tâches parent ou des parents des parents.
        >   * Les heures effectives agrègent les valeurs principales des tâches parent et des tâches autonomes. Elles n’agrègent pas les nombres pour les parents des tâches parent ou des tâches enfant.
        >   * Les champs de données personnalisées de valeurs numériques et de devise regroupent toutes les tâches : parents, enfants, parents de parents et tâches autonomes.
        >   
        >

        Pour plus d’informations sur l’utilisation des regroupements dans un rapport, voir l’article [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Facultatif) Cliquez sur **Options avancées** pour spécifier les informations suivantes de la colonne :

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
           <td>Sélectionnez le format dans lequel vous souhaitez que les valeurs soient affichées pour les champs de la colonne.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Afficher cette colonne lorsque le graphique est visible sur un tableau de bord.</strong></td> 
           <td><p>Sélectionnez cette option pour afficher cette colonne dans un tableau de bord, lorsque le rapport est affiché côte à côte avec un autre rapport. Lorsque cette option n’est pas sélectionnée, cette colonne n’apparaît pas lorsque le rapport est affiché sur un tableau de bord où les rapports sont affichés côte à côte.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Règles de la colonne</strong></td> 
           <td><p>Cliquez sur <strong>+ Ajouter une règle pour cette colonne </strong> pour définir une règle pour la colonne. Après avoir ajouté une règle, vous pouvez définir des styles de champ et de texte définissant le mode d’affichage des champs correspondant à cette règle. Cliquez sur <strong>Ajouter une règle</strong> lorsque vous avez terminé de définir la règle.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Pour plus d’informations sur la mise en forme conditionnelle des vues dans les rapports, voir l’article [Utiliser la mise en forme conditionnelle en mode texte](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Le cas échéant) Si vous avez cliqué sur **Options avancées**, cliquez sur **Terminé**.

1. Cliquez sur **Enregistrer la vue** pour créer une vue ou remplacer la vue actuelle par vos modifications.\
   Ou\
   Cliquez sur **Enregistrer en tant que nouvelle vue** pour enregistrer vos modifications dans une nouvelle vue.

   >[!TIP]
   >
   >L’option **Enregistrer en tant que nouvelle vue** est la seule option disponible lorsque vous personnalisez une vue Workfront intégrée.

   Votre accès détermine la manière selon laquelle la vue est enregistrée. Si vous avez créé la vue à l’origine, vous pouvez enregistrer les modifications ; sinon, vous recevez une invitation à enregistrer une version. Gardez à l’esprit que que les modifications que vous apportez à l’affichage ont un impact sur les utilisateurs et utilisatrices avec lesquels l’affichage a été partagé.

### Créer ou personnaliser une vue Agile {#create-or-customize-an-agile-view}

Vous pouvez créer une vue Agile ou personnaliser une vue Agile existante que vous avez précédemment créée.

>[!IMPORTANT]
>
>Les vues Agile ne sont disponibles que lors l’affichage d’un projet.

Pour plus d’informations sur les vues Agile, voir l’article [Gérer un projet dans la vue Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
>Cette procédure ne s’applique qu’à la vue Agile héritée, et non à la vue du tableau d’un projet.

Pour créer ou personnaliser une vue Agile :

1. Accédez à la liste des tâches d’un projet.
1. Cliquez sur l’icône **Panorama** ![ icône Panorama](assets/board-icon-for-agile-view.png), puis sur **Utiliser la méthode Agile héritée** dans la vue du tableau.

1. (Le cas échéant) Pour personnaliser une vue Agile existante :

   1. Cliquez sur le menu déroulant **Vue**, puis sélectionnez la vue Agile que vous souhaitez personnaliser.\
      Vous ne pouvez pas personnaliser la vue Agile par défaut.

   1. Cliquez à nouveau sur le menu déroulant **Vue**, puis sur **Personnaliser la vue**.\
      ![](assets/view-agile-customize.png)

1. (Le cas échéant) Pour créer une vue Agile, cliquez sur **Nouvelle vue**.\
   La boîte de dialogue **Personnaliser la vue Agile** s’affiche.

1. Dans la boîte de dialogue **Personnaliser la vue Agile**, spécifiez un nom pour la vue Agile.\
   Nous vous recommandons d’inclure le mot « Agile » dans le nom de votre vue, afin que les utilisateurs et utilisatrices sachent qu’il s’agit d’une vue Agile.\
   Ce nom est affiché dans le menu déroulant **Vue** lors de la sélection d’une vue.

1. Définissez les colonnes de statut à afficher sur le StoryBoard dans la vue Agile. Il s’agit des statuts de tâches définis par l’administrateur ou l’administratrice Workfront, comme décrit dans [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Seuls les statuts du système peuvent être utilisés dans le StoryBoard Agile. Si un statut n’est disponible que pour un groupe individuel dont vous êtes membre, le statut n’est pas disponible sur le StoryBoard Agile. En outre, les tâches dont le statut est réservé à un groupe personnalisé ne sont pas visibles lorsque le projet est affiché dans une vue Agile.

   Les utilisateurs et utilisatrices peuvent déplacer les histoires entre ces colonnes de statut sur le StoryBoard Agile.\
   Lors de la définition des colonnes de statut, vous pouvez effectuer les opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Réorganiser les colonnes de statut :</strong> </td> 
      <td> Faites glisser une colonne de statut dans l’ordre dans lequel vous souhaitez qu’elle apparaisse.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Supprimer les colonnes de statut :</strong> </td> 
      <td>Cliquez sur l’icône (x) de la colonne que vous souhaitez supprimer.<br>Vous ne pouvez pas supprimer le statut « Nouveau » à moins qu’un statut personnalisé n’ait été ajouté à la vue et que ce statut personnalisé corresponde à « Nouveau ».<br>Pour plus d’informations sur la création d’un statut personnalisé, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Créer ou modifier un statut</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ajouter des colonnes de statut :</strong> </td> 
      <td> <p>Cliquez sur l’icône <strong>Plus</strong>, puis sélectionnez le statut que vous souhaitez ajouter.<br>Tous les statuts par défaut du système sont affichés, ainsi que les statuts personnalisés qui ont été partagés avec vous.<br>Vous pouvez configurer jusqu’à 10 statuts à afficher.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. Dans la zone **Associer une couleur de carte à**, sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Histoire :</strong> </td> 
      <td>Toutes les sous-tâches correspondent à la couleur de la tâche parent, de sorte que les couleurs de toutes les histoires d’un couloir donné sont les mêmes.<br>Des couleurs sont attribuées de manière aléatoire aux tâches lors de leur création si la tâche n’a pas de sous-tâches ou de tâche parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Forme libre :</strong> </td> 
      <td> Toutes les cartes sont affichées en bleu par défaut jusqu’à ce qu’un utilisateur ou une utilisatrice change la couleur manuellement, comme décrit dans l’article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Catégoriser les histoires par couleur sur le panorama Scrum</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité :</strong> </td> 
      <td> <p> Les couleurs sont associées à la priorité de l’histoire, comme suit :</p> 
       <ul> 
        <li>Élevée = Rouge</li> 
        <li>Moyenne = Jaune</li> 
        <li>Faible = Vert<br> Si votre administrateur ou administratrice Workfront a configuré des priorités personnalisées pour votre système Workfront, la priorité la plus élevée est rouge, la moyenne est jaune et la faible est verte.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personne propriétaire de la tâche :</strong> </td> 
      <td> Toutes les histoires ayant la même personne cessionnaire principale partagent la même couleur.<br>La personne cessionnaire principale est la personne qui a été assignée la première à la tâche. </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans la zone **Champs supplémentaires**, cliquez sur **Ajouter un champ**, puis sélectionnez le champ que vous souhaitez ajouter aux cartes d’article. (Il s’agit des mêmes champs que ceux que vous pouvez ajouter lors de la personnalisation d’un affichage ou de la création de colonnes pour un rapport.)\
   Répétez ce processus pour ajouter jusqu’à trois champs supplémentaires aux cartes d’histoire.\
   Lorsque vous ajoutez des champs à des cartes d’histoire, ces champs ne s’affichent que lorsque le champ est renseigné.

   Par défaut, les types de données suivants sont affichés sur la carte d’histoire :

   * Nom de l’histoire avec un lien direct vers la tâche
   * Nom du projet avec un lien direct vers le projet\
     Ce lien n’est affiché que lors de l’utilisation de la vue Agile sur une itération ; il n’est pas affiché lors de l’utilisation de la vue Agile sur un projet.
   * Description de la tâche
   * Engagement actuel
   * Visualiser et modifier le pourcentage terminé, soit en ajustant le pourcentage terminé lui-même, soit en ajustant le nombre de points terminés ou d’heures terminées.
   * Personnes affectées

   Vous pouvez afficher des données supplémentaires (y compris des données personnalisées) sur les cartes d’histoire. Il se peut que vous vouliez afficher des champs supplémentaires sur les cartes d’histoire pour un certain nombre de raisons. Par exemple, vous pouvez afficher l’ID client si vous travaillez sur des histoires pour plusieurs clientes et clients dans le projet, ou vous pouvez afficher la date de début de la tâche.

1. Cliquer sur **Enregistrer**.\
   Votre accès détermine la manière selon laquelle la vue est enregistrée. Si vous avez créé la vue à l’origine, vous pouvez enregistrer les modifications ; sinon, vous recevez une invitation à enregistrer une version. Gardez à l’esprit que que les modifications que vous apportez à l’affichage ont un impact sur les utilisateurs et utilisatrices avec lesquels l’affichage a été partagé.

1. (Facultatif) Cliquez sur l’icône **Liste** pour revenir à la liste des tâches.
