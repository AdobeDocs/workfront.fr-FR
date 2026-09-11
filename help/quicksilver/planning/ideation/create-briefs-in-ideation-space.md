---
title: Créer des briefs dans l’espace d’idéation
description: Cet article décrit comment réfléchir et élaborer des stratégies dans l'espace Idéation pour créer des briefs. Vous pouvez exporter les résumés d'idées terminés dans un fichier ou dans Workfront Planning pour créer ou mettre à jour des enregistrements.
feature: Workfront Planning
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 4%

---


# Créer des briefs dans l’espace Idéation

<!-- add to TOC and miniTOC-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans le cadre du programme **Ideation space Beta**. </span>

<span class="preview">Pour plus d’informations, voir [Prise en main de l’espace d’idéation pour Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Grâce à l&#39;Espace d&#39;idéation, une nouvelle fonctionnalité d&#39;Adobe Workfront Planning, vous pouvez transformer des résumés en enregistrements Planning. Les briefs exportés créent de nouveaux enregistrements ou mettent à jour des enregistrements existants.

Cet article décrit comment réfléchir et élaborer des stratégies dans l&#39;espace Idéation pour créer des briefs. Pour créer ou mettre à jour des enregistrements, exportez les résumés d&#39;idéation terminés dans un fichier ou dans Workfront Planning.

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
Ou
<li><p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Produits supplémentaires</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
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
      <p>Afficher les autorisations d’accès aux objets Workfront pour les ajouter aux résumés <!--not sure if this is available--></p>
      <p>Autorisations d’éditeur dans l’espace Idéation pour créer des résumés</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Rôles utilisateur Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Tout rôle d’utilisateur GenStudio pour accéder aux campagnes, aux produits et aux rôles</li>
   <li>GenStudio System Manager pour accéder aux activations <!--and Events--></li></ul>
   Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> Rôles utilisateur et autorisations </a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Créer des résumés d’espace d’idéation

1. Commencez dans Workfront Planning et créez ou modifiez un enregistrement à l’aide de l’espace Idéation .

   Pour plus d&#39;informations, voir [Créer des enregistrements Planning à partir de résumés d&#39;espace d&#39;idéation](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).
1. Lorsque l’**Espace d’idéation** s’ouvre, utilisez l’invite fournie pour décrire le type de brief que vous souhaitez créer.

   Par exemple, tapez « Créer une campagne de rentrée pour les élèves de la maternelle à la 12e année pour le mois d’août, pour les parents et les enseignants aux États-Unis ».  Pour rendre le mémoire aussi complet que possible, indiquez autant d’informations que vous disposez pour le type de campagne, le calendrier, les parties prenantes et d’autres détails.

1. Cliquez sur **Commencer à idéaliser**.

   Une fois ouvert, l’agent d’espace d’idéation passe par les étapes suivantes :

   1. **Ingestion et synthèse des données** : extrait les informations pertinentes de sources connectées. Par exemple :

      * Types d’enregistrement existants ou type d’enregistrement existant à partir duquel vous avez démarré.
      * Documents récents que vous avez peut-être chargés dans l&#39;espace d&#39;idéation.
      * Informations web correspondant à vos critères d’invite.

        >[!TIP]
        >
        >Le paramètre de recherche web doit être activé pour que l’IA puisse rechercher des informations sur le web.\
        >Pour plus d’informations, consultez la section [Configurer l’espace d’idéation](#configure-the-ideation-space) dans cet article.
        >
   1. **Définition de l’audience** : identifie ou recommande les paramètres de l’audience cible en fonction de modèles historiques
   1. **Définition de la stratégie** : structure le récit stratégique de la campagne.
   1. **Messagerie et idéation de concept** : génère les options de message initial et les directions de concept créatives
   1. **Génération de résumés et transfert de la planification** : produit un résumé structuré qui alimente l’espace de travail de planification de Workfront.

      Lorsque l’agent d’idéation termine le processus de collecte de toutes les informations, voici ce qui se passe :

      * Cinq cartes sont créées et organisées par informations pertinentes et similaires.

        Le titre des cartes est attribué à l’aide de différentes étapes lors de la création de l’enregistrement demandé, pour une reconnaissance facile.

        Par exemple, ils peuvent être nommés :

        * Plan
        * Journal
        * Segments
        * Mécanique
        * Message

      Les titres des cartes sont personnalisés pour chaque carte de l’idéation.

      * Les cartes sont placées à l&#39;intérieur du même cadre indiquant que c&#39;est le résultat d&#39;une idéation.

      * Un brief est créé et s’affiche dans une image d’aperçu dans le coin inférieur gauche de l’espace Idéation . <!--add screen shot??-->

      Le mémoire contient des suggestions de champs que le système considère pertinents aux idées que vous explorez.

1. (Facultatif) Cliquez sur l’icône **Aide** ![](assets/more-information-icon.png) dans le coin supérieur droit pour obtenir une liste de raccourcis clavier qui vous aideront à naviguer dans l’espace Idéation.

1. (Facultatif) Cliquez sur **Sources** au bas de chaque carte pour comprendre d’où proviennent les informations.

   Les informations peuvent être importées depuis Workfront Planning ou le Web.
1. (Facultatif) Utilisez les icônes pouces vers le haut ou pouces vers le bas sur une carte pour donner votre avis.<!--is this still available??-->
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
   1. Cliquez sur l&#39;icône **Ajouter une carte Taxonomie WF** ![Ajouter à partir de Workfront Planning](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised--> et sélectionnez un type d&#39;enregistrement connecté, puis un enregistrement de chaque type pour ajouter les informations de cet enregistrement au type d&#39;enregistrement que vous avez sélectionné.

      Une carte est créée pour l’enregistrement que vous avez sélectionné pour l’ajouter à l’espace. Le type d’enregistrement s’affiche dans le coin supérieur gauche de la carte de l’enregistrement.
   1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Afficher dans Workfront**.

      La page de détails de l’enregistrement s’ouvre dans un autre onglet du navigateur dans Workfront Planning.
   1. (Facultatif) Sélectionnez le cadre d’idéation ou une carte, cliquez sur l’icône Supprimer , puis sur Supprimer pour confirmer. La carte est retirée de l’espace Idéation .

      Lorsque vous supprimez des cartes correspondant à un document stocké ou à un enregistrement, les éléments sont supprimés de l’espace Idéation , mais ils restent dans leurs applications respectives.

1. (Facultatif) Utilisez à tout moment la zone **Demander n’importe quoi** dans le coin inférieur droit pour affiner votre idée.

   Par exemple, saisissez `regenerate` pour une carte spécifique afin que l’IA rétablisse cette carte à l’aide du contexte mis à jour. L&#39;espace idéation reprend ses étapes de raisonnement (recherche, synthèse, citation) et met à jour les cartes concernées.

1. (Facultatif) Dans la zone **Poser une question**, posez une nouvelle question pour commencer une nouvelle idéation.

   Un nouveau jeu de cartes est généré, après que l&#39;espace ait réexécuté ses étapes de raisonnement.

1. (Facultatif) Cliquez sur l’un des connecteurs violets de n’importe quel jeu de cartes d’idéation, puis cliquez sur l’icône **Copier dans la barre d’invite** pour réexécuter le raisonnement de l’idéation.

   ![Icône Copier dans la barre d’invite](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Facultatif) Cliquez sur les icônes **Annuler** ou **Rétablir** ![Annuler et rétablir](assets/undo-redo-icons.png) en haut de la page pour annuler ou inverser une action.
1. Effectuez un zoom arrière pour obtenir une vue d’ensemble : l’objectif de votre campagne d’origine, toutes les cartes conceptuelles générées par l’IA avec des citations, des documents supplémentaires, les enregistrements Workfront Planning réels que vous avez extraits (produits, personnes, etc.). La carte de résumé **Brief** dans le coin inférieur gauche regroupe l’ensemble.

1. Cliquez sur l’image d’aperçu du résumé dans le coin inférieur gauche et passez en revue le résumé, puis cliquez sur l’une des options suivantes :

   * **Exporter dans un fichier**. Vous pouvez exporter le brief vers les types de fichiers suivants :

     * PDF
     * Mot
     * PowerPoint (avec ou sans modèle)
   * **Exporter vers Workfront Planning**. L’exportation remplace toutes les données de champ existantes dans l’enregistrement dans Workfront Planning.

   Cela termine la création de l’enregistrement avec les informations supplémentaires et l’ajoute au type d’enregistrement que vous avez sélectionné à l’origine.

   Pour plus d&#39;informations sur la mise à jour des enregistrements Planning à l&#39;aide de résumés, consultez la section « Considérations relatives à l&#39;utilisation de l&#39;espace Idéation pour créer des enregistrements » de l&#39;article [Créer des enregistrements Planning à partir de résumés d&#39;espace Idéation](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).


## Configuration de l’espace d’idéation

Il existe des commandes pour l’espace Idéation qui configurent ce que vous voyez à l’écran et vous aident à naviguer dans l’espace.

1. Cliquez sur l’icône **Paramètres** ![Paramètres](assets/setting-icon.png) pour contrôler où l’IA extrait les informations, puis choisissez l’un des **types de Source suivants** :

   * **Documents** — documents téléchargés dans l&#39;espace sélectionné
   * **Recherche Web** — recherche Web externe
   * **** — Adobe Customer Journey Analytics

1. Cliquer sur **Enregistrer**.

1. Cliquez sur l’icône **Aide** ![Icône Aide](assets/more-information-icon.png) pour consulter les raccourcis clavier que vous pouvez utiliser pour naviguer dans l’espace d’idéation ou sélectionner une autre valeur de zoom.

   Effectuez un choix parmi les niveaux de zoom suivants :

   * Zoom à 100 %
   * Zoom à 200 %
   * Zoom pour ajuster

   Vous pouvez également utiliser l’un des raccourcis suivants pour naviguer sur la page :

   | Action | Raccourci |
   |---|---|
   | Zoom avant/arrière | Ctrl/⌘ + / − |
   | Zoom pour ajuster/ajuster la sélection | — |
   | Zoom sur le curseur | Ctrl/⌘ + défilement |
   | Panoramique de la zone de travail | Maintenir la touche Espace + glisser |
   | Afficher/masquer la grille de points | G |

1. Cliquez sur l’icône Rechercher pour rechercher des éléments dans l’espace d’idéation, puis cliquez sur lorsqu’il s’affiche dans la liste pour y accéder.








