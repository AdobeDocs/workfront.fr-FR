---
title: Créer des briefs dans l’espace d’idéation
description: Cet article décrit comment réfléchir et élaborer des stratégies dans l'espace Idéation pour créer des briefs. Vous pouvez exporter les résumés d'idées terminés dans un fichier ou dans Workfront Planning pour créer ou mettre à jour des enregistrements.
feature: Workfront Planning
role: User, Admin
author: Alina
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: e209f8e5ada29b1c488fcfe42c13c6c9523a26bd
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 3%
---

# Créer des briefs dans l’espace Idéation

<!--add to TOC and miniTOC-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans le cadre du programme **Ideation space Beta**. </span>

<span class="preview">Pour plus d’informations, voir [Prise en main de l’espace d’idéation pour Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Grâce à l&#39;Espace d&#39;idéation, une nouvelle fonctionnalité d&#39;Adobe Workfront Planning, vous pouvez transformer des résumés en enregistrements Planning ou les enregistrer en tant que fichier externe. Les briefs exportés créent de nouveaux enregistrements ou mettent à jour des enregistrements existants.

Cet article décrit comment réfléchir et élaborer des stratégies dans l&#39;espace Idéation pour créer des briefs.

Vous pouvez effectuer les opérations suivantes :

* Pour créer ou mettre à jour des enregistrements, exportez les résumés d&#39;idéation terminés dans Workfront Planning.

* Pour utiliser les informations d&#39;un brief dans une autre application, exportez-les vers l&#39;un des types de fichiers suivants :

  * PDF
  * Mot
  * PowerPoint
  * Modèle PowerPoint

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront ou workflow avec un package Planning</p></li>
<!--
Add this at GA - not available in beta:
Or
<li><p>Any Planning package when purchased as a standalone product</p></li>
-->
</ul>
   </td> 
<!--
<tr> 
<td role="rowheader"><p>Additional products</p></td> 
<td><ul>
<li><p>Adobe GenStudio for Performance Marketing</p></li>
<li><p>Adobe Customer Journey Analytics</p></li>
</ul>
</td> 
</tr> 
-->
  <tr> 
   <td role="rowheader"><p>Licence de workflow Adobe</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr>  
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> 
   <ul>
   <li><p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   </li>
   <li><p>Le paramètre Désactiver l’espace d’idéation de votre niveau d’accès doit être désélectionné</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Autorisations de niveau Contributeur ou supérieur à l’espace de travail et au type d’enregistrement dans lesquels vous souhaitez ajouter des enregistrements </p>
      <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
      <!--
      not available right now:
      <p>View permissions to Workfront objects to add them to briefs </p>
      -->
      <p>Autorisations d’éditeur dans l’espace Idéation pour créer des résumés</p>
   </td> 
  </tr>  
    <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Créer des résumés d’espace d’idéation

Vous pouvez créer des résumés pour créer ou modifier des enregistrements Planning ou pour créer des fichiers que vous pouvez exporter vers d&#39;autres applications.

1. Connectez-vous à Workfront avec Planning dans lequel Coworker a été activé et effectuez l’une des opérations suivantes :

   * Accédez à **Menu principal** > **Espace idéation**
   * Accédez à **Menu principal** > **Planification** > cliquez sur un espace de travail > cliquez sur un type d’enregistrement > **Nouvel enregistrement** > **Espace de création d’idées**

     Pour plus d&#39;informations sur la création d&#39;enregistrements à l&#39;aide de l&#39;espace Idéation, voir [Créer des enregistrements Planning à partir de résumés d&#39;espace Idéation](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).
   * Accédez à **Menu principal** > **Planification** > cliquez sur un espace de travail > cliquez sur un type d’enregistrement > cliquez sur un enregistrement existant > **Ouvrir dans l’espace d’idéation**

   L’espace Idéation s’ouvre et une nouvelle idéation est intitulée par défaut en suivant le format suivant :

   `catalyze-canvas-< number > - Month date, year at time` <!--submitted bug to change the default name to "Untitled ideation"-->

   Si vous ouvrez une idéation à partir d&#39;un enregistrement existant, le nom de l&#39;idéation correspond au nom de l&#39;enregistrement.

1. (Recommandé) Cliquez sur le nom de l’idéation pour le modifier.

1. (Conditionnel et facultatif) Pour ouvrir un autre espace d&#39;idéation existant, cliquez sur le menu déroulant à droite du nom de l&#39;idéation, recherchez-le par nom, puis cliquez sur l&#39;idéation lorsqu&#39;elle s&#39;affiche dans la liste.

1. Lorsque l’**Espace d’idéation** s’ouvre, le CX Coworker s’ouvre à droite. Utilisez l’invite du collègue pour décrire le type de brief que vous souhaitez créer.

   Par exemple, tapez « Créer une campagne de rentrée pour les élèves de la maternelle à la 12e année pour le mois d’août, pour les parents et les enseignants aux États-Unis ».  Pour que le résumé soit aussi complet que possible, indiquez autant d’informations que vous disposez sur le type de campagne, le calendrier, les parties prenantes, les points de contrôle des approbations et d’autres détails.

1. Cliquez sur Entrée.

1. Répondez aux questions de votre collègue pour poursuivre l&#39;idéation, puis cliquez sur **Soumettre**

   Ou

   Cliquez sur **Ignorer le questionnaire** pour ignorer les questions supplémentaires.

1. (Conditionnel) Lorsque Collègue propose de créer des cartes pour l&#39;idéation, répondez **Oui**.

   Des cartes sont ajoutées à l&#39;espace d&#39;idéation et vous pouvez voir les sources de chaque carte et décider laquelle ajouter à votre brief.

1. Cliquez sur l’icône **Rechercher** ![Icône Rechercher](assets/search-icon.png) pour rechercher des éléments dans l’espace d’idéation, puis cliquez sur lorsqu’il s’affiche dans la liste pour y accéder.

1. (Facultatif) Cliquez sur **Sources** au bas de chaque carte pour comprendre d’où proviennent les informations.

   Les informations peuvent être importées depuis Workfront Planning ou le Web.

   Vous pouvez également cliquer sur l’icône **Sources** ![Icône Sources](assets/sources-icon.png) dans le coin supérieur droit de l’espace pour afficher une liste de sources pour toutes les cartes de cet espace.
1. (Facultatif) Cliquez sur **Commentaires** ![Icône Commentaire](assets/comments-icon.png) dans le coin supérieur droit de l’espace, puis sur **@** pour baliser les autres utilisateurs et lancer un brainstorming à l’intérieur de l’espace.

   Les utilisateurs recevront une notification par e-mail concernant la balise .
1. (Facultatif) Cliquez sur l’icône **Filtrer** ![](assets/filter-comments-icon.png) à l’intérieur de la carte de commentaire pour filtrer les commentaires selon les critères suivants :

   * Réviseurs
   * Heure à laquelle le commentaire a été ajouté
   * Statut (le commentaire a été résolu ou est en attente)
   * Non lu (affiche uniquement les commentaires non lus)
1. (Facultatif) Utilisez les icônes **Pouces vers le haut** ou **Pouces vers le bas** sur une carte ![Pouces vers le haut ou vers le bas](assets/thumbs-up-and-down-icons.png) pour donner votre avis sur l’exactitude des informations figurant sur la carte.
1. Cliquez sur une carte ou sur le cadre contenant toutes les cartes, puis cliquez sur **Ajouter au brief** pour ajouter leurs informations au brief.

   Workfront associe chaque information au champ qu’il trouve le plus susceptible de la stocker.

   Par exemple, les chronologies sont ajoutées aux champs de type date et les descriptions aux champs de type paragraphe.

1. (Conditionnel) Cliquez sur une carte, puis sur **Demander à l’IA de ...** pour obtenir des idées sur l’étape suivante, avant d’ajouter les informations au brief. Les réponses se situent dans le contexte des informations de chaque carte.
1. Cliquez sur l’icône **Ajouter des documents** ![Icône Ajouter des documents](assets/add-documents-in-ideation-space.png) dans le coin supérieur gauche de l’espace Idéation pour charger des documents dans l’espace. Vous pouvez ajouter de nouveaux documents ou des documents que vous avez déjà ajoutés à l&#39;espace.

   >[!TIP]
   >
   >Le paramètre Documents doit être activé pour pouvoir accéder aux documents et les charger dans l’espace.
   >Pour plus d’informations, consultez la section [Configurer l’espace d’idéation](#configure-the-ideation-space) dans cet article.
   > 
1. Cliquez sur l&#39;icône **Ajouter une carte Taxonomie WF** ![Ajouter à partir de Workfront Planning](assets/add-from-wf-planning-on-ideations-space.png) <!--asked to change this tooltip--> et sélectionnez un type d&#39;enregistrement connecté, puis un enregistrement de chaque type pour ajouter les informations de cet enregistrement au type d&#39;enregistrement que vous avez sélectionné.

   Une carte est créée pour l’enregistrement que vous avez sélectionné pour l’ajouter à l’espace. Le type d’enregistrement s’affiche dans le coin supérieur gauche de la carte de l’enregistrement.

   >[!TIP]
   >
   >L&#39;icône **Ajouter une taxonomie WF** <!--check UI name--> n&#39;est pas disponible lorsque vous accédez à l&#39;espace Idéation à partir du menu Principal et le brief n&#39;est pas connecté à un enregistrement Planning.

1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) sur la carte d’enregistrement connectée, puis cliquez sur **Afficher dans Workfront**.

   La page de détails de l’enregistrement s’ouvre dans un autre onglet du navigateur dans Workfront Planning.
1. (Facultatif) Sélectionnez le cadre d’idéation ou une carte, cliquez sur l’icône **Supprimer**, puis sur **Supprimer** pour confirmer. La carte est retirée de l’espace Idéation .

   Lorsque vous supprimez des cartes correspondant à un document stocké ou à un enregistrement, les éléments sont supprimés de l’espace Idéation , mais ils restent dans leurs applications respectives.

1. (Facultatif) Utilisez à tout moment la zone **Demandez à un collègue** dans le coin inférieur droit pour affiner votre idée.

   Par exemple, saisissez `regenerate` pour une carte spécifique afin que l’IA rétablisse cette carte à l’aide du contexte mis à jour. L&#39;espace idéation reprend ses étapes de raisonnement (recherche, synthèse, citation) et met à jour les cartes concernées.

1. (Facultatif) Cliquez sur l&#39;un des connecteurs violets de n&#39;importe quel jeu de cartes d&#39;idéation, puis cliquez sur l&#39;icône **Copier l&#39;invite complète** pour copier l&#39;invite qui a généré la carte dans le presse-papiers, puis collez-la dans la zone d&#39;invite de Coworker.

   ![Icône Copier dans la barre d’invite](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Facultatif) Cliquez sur les icônes **Annuler** ou **Rétablir** ![Annuler et rétablir](assets/undo-redo-icons.png) en haut de l’espace d’idéation pour annuler ou inverser une action.
1. Effectuez un zoom arrière pour obtenir une vue d’ensemble : l’objectif de votre campagne d’origine, toutes les cartes conceptuelles générées par l’IA avec des citations, des documents supplémentaires, les enregistrements Workfront Planning réels que vous avez extraits (produits, personnes, etc.). La carte de résumé **Brief** dans le coin inférieur gauche regroupe l’ensemble.

1. Cliquez sur l’image d’aperçu du résumé dans le coin inférieur gauche et passez en revue le résumé, puis cliquez sur l’une des options suivantes :

   * **Exporter dans un fichier**. Vous pouvez exporter le brief vers les types de fichiers suivants :

     * PDF
     * Mot
     * PowerPoint (avec ou sans modèle)
   * **Exporter vers Workfront Planning**. L&#39;exportation remplace toutes les données de champ existantes dans l&#39;enregistrement Planning correspondant à l&#39;idéation.

   >[!TIP]
   >
   >L&#39;option **Exporter vers Workfront Planning** est grisée lorsque vous accédez à l&#39;espace Idéation à partir du menu Principal et le brief n&#39;est pas associé à un enregistrement Planning.

   Cela met fin à la création de l’enregistrement ou du fichier avec les informations supplémentaires. Si vous avez démarré à partir d’un enregistrement existant, les informations du brief sont ajoutées à l’enregistrement. Si vous avez commencé avec un nouvel enregistrement, celui-ci est créé avec les informations contenues dans le mémoire.

   Pour plus d&#39;informations sur la mise à jour des enregistrements Planning à l&#39;aide de résumés, consultez la section « Considérations relatives à l&#39;utilisation de l&#39;espace Idéation pour créer des enregistrements » de l&#39;article [Créer des enregistrements Planning à partir de résumés d&#39;espace Idéation](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).


## Configuration de l’espace d’idéation

Il existe des commandes pour l’espace Idéation qui configurent ce que vous voyez à l’écran et vous aident à naviguer dans l’espace.

1. Cliquez sur l’icône **Paramètres** ![Paramètres](assets/setting-icon.png) pour contrôler où l’IA extrait les informations, puis choisissez l’un des **types de Source suivants** :

   * **Documents** — documents téléchargés dans l&#39;espace sélectionné
   * **Recherche Web** — recherche Web externe
   <!--
     **CJA** — Adobe Customer Journey Analytics
    -->
1. Cliquer sur **Enregistrer**.

1. Cliquez sur l’icône déroulante **niveau de zoom** à gauche de l’icône **Aide** ou de l’icône **Aide** ![Icône d’aide](assets/more-information-icon.png) pour sélectionner une option ou passer en revue les raccourcis clavier que vous pouvez utiliser pour naviguer dans l’espace d’idéation ou sélectionner une autre valeur de zoom.

   Effectuez un choix parmi les niveaux de zoom suivants :

   * Zoom à 100 %
   * Zoom à 200 %
   * Zoom pour ajuster

   Vous pouvez également utiliser l’un des raccourcis suivants pour naviguer sur la page :

   | Action | Raccourci |
   | --- | --- |
   | Zoom avant/arrière | Ctrl/⌘ + / − |
   | Zoom pour ajuster/ajuster la sélection | — |
   | Zoom sur le curseur | Ctrl/⌘ + défilement |
   | Panoramique de la zone de travail | Maintenir la touche Espace + glisser |
   | Afficher/masquer la grille de points | Go |



<!--

    Once opened, the Ideation space agent goes through the following steps:

    1. **Data ingestion and synthesis**:  Pulls relevant information from connected sources. For example: 
    
        * Existing record types or the existing record type that you started from. 
        * Recent documents you might have uploaded in the ideation space. 
        * Web information that matches your prompt criteria.

            >[!TIP]
            >
            >The Web search setting must be turned on for AI to be able to look for information on the web.  
            >For information, see the section [Configure the Ideation space](#configure-the-ideation-space)in this article.
            >
    1. **Audience definition**: Identifies or recommends target audience parameters based on historical patterns
    1. **Strategy framing**: Structures the strategic narrative for the campaign
    1. **Messaging and concept ideation**: Generates initial message options and creative concept directions
    1. **Brief generation and planning handoff**: Produces a structured brief that feeds back into the Workfront Planning workspace

        When the Ideation agent finishes the process of collecting all the information, the following things occur: 
    
        * Five cards are created and are organized by relevant and like-information. 

            The cards are titled using various steps in the creation of the requested record, for easy recognition. 
    
            For example, they could be named:

            * Plan
            * Timeline
            * Segments
            * Mechanics  
            * Messaging 

        The cards titles are custom to each card in the ideation. 

        * The cards are placed inside the same frame indicating this is the result of one ideation. 

        * A brief is created and displays in a preview image in the lower-left corner of the Ideation space. <!
    
        The brief contains suggested fields that the system considers pertinent to the ideas you are exploring. 
-->






