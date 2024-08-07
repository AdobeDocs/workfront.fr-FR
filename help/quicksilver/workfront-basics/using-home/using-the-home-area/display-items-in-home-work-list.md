---
product-area: projects
navigation-topic: use-the-home-area
title: Afficher les éléments dans la [!UICONTROL liste de travail] de la zone Accueil
description: La [!UICONTROL liste de travail] de la zone [!UICONTROL Accueil] affiche toutes les tâches qui vous sont affectées. Vous pouvez contrôler quels éléments s’affichent dans votre [!UICONTROL liste de travail] en utilisant des filtres et en regroupant et en triant vos éléments de travail.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1837'
ht-degree: 12%

---

# Afficher les éléments dans la [!UICONTROL liste de travail] de la zone [!UICONTROL Accueil]

<!-- Audited: 1/2024 -->


La [!UICONTROL liste de travail] de la zone [!UICONTROL Accueil] affiche toutes les tâches qui vous sont affectées. Vous pouvez contrôler quels éléments s’affichent dans votre [!UICONTROL liste de travail] en utilisant des filtres et en regroupant et en triant vos éléments de travail.

>[!NOTE]
>
>* Lors de la conversion d’un problème en une tâche ou un projet, le problème est supprimé de la zone Accueil de l’utilisateur affecté au problème.
>
>* Lors de la conversion d’une tâche en projet, la tâche est supprimée de la zone Accueil de l’utilisateur affecté à la tâche.


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
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence</strong></td> 
   <td> <p>Nouveau :</p><ul><li>[!UICONTROL Contributeur] pour les approbations uniquement</li> <li>[!UICONTROL Standard] ou version ultérieure pour tous les autres objets</li> <p>Ou</p> 
  </ul><p>Actuel :</p><ul><li>Révision [!UICONTROL] pour les approbations uniquement</li> <li>[!UICONTROL Travail] ou version ultérieure pour tous les autres objets</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>Accès à [!UICONTROL View] ou à un accès supérieur à Projects, Tasks, Issues et Documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de contribution ou niveau supérieur pour les tâches et les problèmes sur lesquels vous devez travailler</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrage de la [!UICONTROL liste de travail]

Vous pouvez filtrer les éléments dans la [!UICONTROL liste de travail] pour n’afficher que des types d’éléments spécifiques. Par exemple, vous pouvez filtrer la [!UICONTROL Liste de travail] pour n’afficher que les problèmes ou les requêtes.

>[!NOTE]
>
>Les options de filtre sont stockées dans le navigateur. Si vous utilisez systématiquement le même navigateur sur le même ordinateur (et que vous n’effacez pas les données du site), les filtres sélectionnés ne changent pas. Si vous changez de navigateur ou d’ordinateur, l’option par défaut est rétablie. Tous les filtres sont alors désélectionnés.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sélectionnez **[!UICONTROL Accueil]**.
1. Cliquez sur le menu déroulant **[!UICONTROL Filtre]** ![](assets/filter-nwepng.png) . Si des filtres sont sélectionnés, le nombre de filtres sélectionnés s’affiche à la place de l’icône.
1. Sélectionnez l’une des options de filtre suivantes pour spécifier le type d’élément à afficher :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>Affiche et sélectionne tous les éléments. Cela inclut les tâches, les problèmes, les approbations, les tâches personnelles et les tâches et problèmes terminés. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tâches : Utilisation]</strong></td> 
      <td> <p>Affiche uniquement les tâches sur lesquelles vous travaillez activement. Il s’agit des tâches qui vous ont été affectées et pour lesquelles vous avez cliqué sur le bouton [!UICONTROL Travailler dessus] .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tâches : prêtes à démarrer]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les tâches que vous êtes prêt à démarrer. Les deux instructions suivantes doivent être vraies :</p> 
        <ul> 
         <li> <p>Les tâches et leurs parents n'ont pas de prédécesseurs ou de contraintes de tâche qui les empêchent de travailler.</p> </li> 
         <li> <p>La [!UICONTROL Date de début planifiée] des tâches se situe dans le passé ou jusqu’à deux semaines à l’avenir.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tâches : non prêtes]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les tâches qui ne sont pas encore prêtes à démarrer. L’une des instructions suivantes doit être vraie :</p> 
        <ul> 
         <li> <p>Les tâches et leurs parents peuvent avoir des prédécesseurs ou des contraintes de tâche qui les empêchent de travailler.</p> </li> 
         <li> <p>Les tâches comportent une [!UICONTROL Date de début planifiée] qui se situe à plus de deux semaines à l’avenir.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues : Working On]</strong></td> 
      <td> <p>Affiche uniquement les problèmes sur lesquels vous travaillez activement. Il s’agit des problèmes qui vous ont été attribués pour lesquels vous avez cliqué sur le bouton [!UICONTROL Travailler dessus] .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problèmes : Requis]</strong></td> 
      <td>Affiche uniquement les problèmes auxquels vous êtes affecté, mais pour lesquels vous n’avez pas cliqué sur le bouton [!UICONTROL Travailler dessus].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personnel</strong></td> 
      <td>Affiche uniquement les tâches personnelles. Il s’agit des tâches que vous créez en tant que tâche [!UICONTROL À faire], comme décrit dans la section <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Créer une tâche personnelle</a> de l’article <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Créer des tâches à partir de la zone [!UICONTROL Accueil]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approbations]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les approbations qui vous ont été attribuées ou qui vous ont été déléguées, ainsi que les approbations que vous avez soumises. Les approbations comprennent les approbations sur les tâches (projets, tâches et problèmes), ainsi que les approbations pour les documents, les bons à tirer, les demandes d’accès et les feuilles de temps. Pour plus d’informations sur les approbations, consultez les articles suivants :</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref"> Afficher les approbations</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Approbations de travail</a> </p> </li> 
        </ul> 
        <p>Remarque : les approbations que vous avez envoyées et pour lesquelles vous êtes également l’un des approbateurs sont comptabilisées deux fois.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Délégué : Délégué par moi]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les tâches que vous avez déléguées à un autre utilisateur.</p> 
        <p>Pour plus d’informations sur la délégation de tâches, voir <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Délégation de tâches et de problèmes à un autre utilisateur</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Délégué : délégué à moi]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les tâches qui vous ont été temporairement déléguées par un autre utilisateur.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL terminé]</strong></td> 
      <td> <p>Affiche uniquement les tâches terminées, les problèmes et les tâches personnelles. Les tâches terminées s’affichent pendant les deux semaines précédentes et sont regroupées dans la liste des tâches en fonction de la semaine au cours de laquelle elles ont été terminées. Les validations ne sont pas incluses.</p> <p>Le travail terminé est masqué dans la [!UICONTROL Liste de travail], sauf si vous sélectionnez ce filtre.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Les options de filtre sont basées sur des objets (Tâches, Problèmes, Approbations, Tâches personnelles).
   >* Les tâches et les problèmes sont filtrés davantage par leur état en relation avec notre disposition à les traiter ([!UICONTROL Travailler sur], [!UICONTROL Prêt à démarrer], [!UICONTROL Non prêt] pour les tâches, et [!UICONTROL Travail sur] et [!UICONTROL Demandé] pour les problèmes). Vous pouvez choisir d’afficher les tâches ou les problèmes dans un état spécifique ou cliquer sur Tâches ou Problèmes pour sélectionner et afficher tous les états.
   >* Il existe un filtre distinct pour les éléments terminés et il inclut les tâches et les problèmes. Cela n’inclut pas les approbations. Le filtre [!UICONTROL Completed] comprend les tâches personnelles.
   >* Vous pouvez choisir d’afficher un seul état à la fois. Par exemple, vous pouvez afficher uniquement les tâches [!UICONTROL Working On] et uniquement les problèmes [!UICONTROL Requested]. Vous pouvez également sélectionner plusieurs états simultanément.
   >* Vous ne pouvez pas appliquer de filtres aux éléments affectés à l’une de vos équipes, et les affectations d’équipe ne sont pas incluses dans les éléments qui vous sont directement affectés.


1. (Facultatif) Organisez davantage la [!UICONTROL liste de travail], comme décrit dans la section [Groupe et triez par date, projet et priorité](#group-and-sort-by-date-project-and-priority) de cet article.

## Regroupez et triez par [!UICONTROL Date], [!UICONTROL Projet] et [!UICONTROL Priorité]

Vous pouvez regrouper et trier la [!UICONTROL liste de travail] par [!UICONTROL Date d’achèvement prévue], [!UICONTROL Date de validation], [!UICONTROL Projet] ou [!UICONTROL Ma priorité]. L’option choisie détermine le mode de regroupement des éléments dans la [!UICONTROL liste de travail].

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sélectionnez **[!UICONTROL Accueil]**.
1. Cliquez sur le menu déroulant **[!UICONTROL Group by]** ![Group by](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png) .

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td> 
      <td> <p> Les éléments s’affichent dans les regroupements suivants dans la [!UICONTROL Liste de travail], en fonction de leur [!UICONTROL Date d’achèvement prévue] (le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre de l’en-tête) :</p> 
       <ul> 
        <li> <p>[!UICONTROL en retard]</p> </li> 
        <li> <p>[!UICONTROL Aucune date d’achèvement planifiée]</p> </li> 
        <li> <p>[!UICONTROL Cette Semaine]</p> <p>Ce regroupement est développé par défaut.</p> </li> 
        <li> <p>[!UICONTROL Semaine prochaine]</p> </li> 
        <li> <p>[!UICONTROL Planifié], suivi de diverses [!UICONTROL Dates d’achèvement prévues] (plusieurs regroupements)</p> </li> 
        <li> <p>[!UICONTROL Terminé]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Démarrage planifié]</strong></td> 
      <td> <p>Les éléments s’affichent dans les regroupements suivants dans la [!UICONTROL Liste de travail], en fonction de leur [!UICONTROL Date de début planifiée] (le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre de l’en-tête) :</p> 
       <ul> 
        <li> <p>[!UICONTROL en retard]</p> </li> 
        <li> <p>[!UICONTROL Cette Semaine] </p> <p>Ce regroupement est développé par défaut.</p> </li> 
        <li> <p>[!UICONTROL Semaine prochaine]</p> </li> 
        <li> <p>[!UICONTROL Planifié], suivi de diverses [!UICONTROL Dates de début planifiées] (regroupements multiples)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Date de validation]</strong></td> 
      <td> <p>Les éléments s’affichent dans les regroupements suivants dans la [!UICONTROL Liste de travail] (le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre du titre) :</p> 
       <ul> 
        <li> <p>[!UICONTROL No Validation Date]</p> </li> 
        <li> <p>[!UICONTROL Engagé La Semaine Prochaine]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>Les éléments sont regroupés en fonction du projet et les projets apparaissent par ordre alphabétique dans la [!UICONTROL Liste de travail]. (Le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre du titre.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Ma priorité]</strong></td> 
      <td>Les éléments s’affichent dans l’ordre de votre choix. Pour plus d’informations, voir <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Définir la priorité du travail dans la zone [!UICONTROL Accueil]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>Le tri par défaut est croissant. Si vous définissez le tri sur descendant, les options de tri sélectionnées sont stockées dans le navigateur. Si vous utilisez systématiquement le même navigateur sur le même ordinateur (et que vous n’effacez pas les données du site), le tri ne change pas, mais si vous changez de navigateur ou d’ordinateur, le tri passe au tri par défaut.

## Afficher les éléments en retard

[!DNL Adobe Workfront] utilise les dates suivantes pour déterminer si les demandes de travail sont en retard :

* **Tâches** : [!UICONTROL Date d’achèvement planifiée]
* **Problèmes** : [!UICONTROL Date d’achèvement prévue]
* **Documents** : [!UICONTROL Date d’envoi]
* **** : [!UICONTROL Date d’envoi]
* **Validations** : [!UICONTROL Date d’envoi]
* **Approbation de BAT** : [!UICONTROL Date limite de BAT]

## Recherchez la [!UICONTROL liste de travail]

Lorsque vous effectuez une recherche dans la [!UICONTROL liste de travail], tous les éléments qui vous sont affectés sont renvoyés dans la recherche (même les éléments qui ne sont pas actuellement chargés à l’écran). Si l’option [!UICONTROL Afficher terminé] est sélectionnée, tous les éléments marqués comme terminé au cours des deux dernières semaines sont également renvoyés.

En outre, seuls les noms des tâches sont recherchés (les informations contenues dans l’élément de travail ne sont pas recherchées, pas plus que les noms des projets où réside l’élément de travail).

Pour rechercher la [!UICONTROL liste de travail] :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sélectionnez **[!UICONTROL Accueil]**.
1. (Facultatif) Filtrez et regroupez la [!UICONTROL liste de travail], comme décrit dans la section [Filtrez la [!UICONTROL liste de travail]](#filter-the-work-list) et [Groupez et triez par date, projet et priorité](#group-and-sort-by-date-project-and-priority).

1. (Facultatif) Si vous recherchez un élément de travail déjà terminé, vous devez configurer la [!UICONTROL liste de travail] pour afficher les éléments terminés avant de le rechercher.

1. Cliquez sur l’icône de recherche ![Rechercher](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Commencez à saisir le nom de l’élément que vous recherchez.\
   La [!UICONTROL liste de travail] est automatiquement filtrée afin d’inclure des éléments avec un nom correspondant.

## Modification de la taille de la liste de tâches

Vous pouvez modifier la taille de la [!UICONTROL liste de travail] de sorte qu’elle consomme entre environ un quart de la zone d’accueil et environ la moitié de la zone [!UICONTROL d’accueil].

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sélectionnez **[!UICONTROL Accueil]**.
1. Passez la souris sur le bord droit de la [!UICONTROL liste de travail], puis faites glisser vers la gauche ou la droite jusqu’à ce que la liste de travail ait la taille souhaitée.

## Réduire et développer des groupements

Les éléments de la [!UICONTROL liste de travail] s’affichent dans des regroupements. Vous pouvez réduire et développer des regroupements afin de contrôler le volume d’informations affichées sur la page à un moment donné.

Vous pouvez réduire et développer des groupes dans la [!UICONTROL liste de travail] pour mieux contrôler les informations visibles.\
Par défaut, le regroupement [!UICONTROL Cette semaine] est développé et tous les autres regroupements sont réduits. Toutes les modifications que vous apportez sont mémorisées la prochaine fois que vous accédez à la zone Accueil.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sélectionnez **[!UICONTROL Accueil]**.
1. Cliquez sur la flèche **[!UICONTROL Développer]** ou **[!UICONTROL Réduire]** située en regard d’un regroupement que vous souhaitez développer ou réduire.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Ou\
   Pour développer ou réduire tous les regroupements simultanément, cliquez sur la flèche **[!UICONTROL Développer]** ou **[!UICONTROL Réduire]** en regard d’un groupement tout en maintenant la touche [!UICONTROL Maj] enfoncée.
