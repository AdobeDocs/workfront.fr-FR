---
product-area: projects
navigation-topic: use-the-home-area
title: Afficher les éléments dans la [!UICONTROL Liste de travail] dans la zone Accueil
description: La [!UICONTROL Liste de travail] de la zone [!UICONTROL Accueil] affiche tous les éléments de travail qui vous sont affectés. Vous pouvez contrôler les éléments affichés dans votre [!UICONTROL Liste de travail] en utilisant des filtres et en regroupant et en triant vos éléments de travail.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1840'
ht-degree: 99%

---

# Afficher les éléments dans la [!UICONTROL Liste de travail] dans la zone [!UICONTROL Accueil]

<!-- Audited: 1/2024 -->


La [!UICONTROL Liste de travail] de la zone [!UICONTROL Accueil] affiche tous les éléments de travail qui vous sont affectés. Vous pouvez contrôler les éléments affichés dans votre [!UICONTROL Liste de travail] en utilisant des filtres et en regroupant et en triant vos éléments de travail.

>[!NOTE]
>
>* Lors de la conversion d’un problème en une tâche ou un projet, le problème est supprimé de la zone Accueil de l’utilisateur ou de l’utilisatrice à qui le problème est affecté.
>
>* Lors de la conversion d’une tâche en projet, la tâche est supprimée de la zone Accueil de l’utilisateur ou de l’utilisatrice à qui la tâche est affectée.


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
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence</strong></td> 
   <td> <p>Nouveau :</p><ul><li>[!UICONTROL Contributor] pour les approbations uniquement</li> <li>[!UICONTROL Standard] ou de niveau supérieur pour tous les autres objets</li> <p>Ou</p> 
  </ul><p>Actuel :</p><ul><li>[!UICONTROL Review] pour les approbations uniquement</li> <li>[!UICONTROL Work] ou de niveau supérieur pour tous les autres objets</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>Accès en [!UICONTROL View] ou de niveau supérieur aux projets, tâches, problèmes et documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de contribution ou niveau supérieur pour les tâches et les problèmes sur lesquels vous devez travailler</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrer la [!UICONTROL Liste de travail]

Vous pouvez filtrer les éléments de la [!UICONTROL Liste de travail] pour afficher uniquement des types d’éléments spécifiques. Par exemple, vous pouvez filtrer la [!UICONTROL Liste de travail] pour afficher uniquement les problèmes ou les demandes.

>[!NOTE]
>
>Les options de filtre sont stockées dans le navigateur. Si vous utilisez systématiquement le même navigateur sur le même ordinateur (et que vous n’effacez pas les données du site), les filtres sélectionnés ne changent pas. Si vous changez de navigateur ou d’ordinateur, l’option par défaut est rétablie et tous les filtres sont désélectionnés.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant) cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sur **[!UICONTROL Accueil]**.
1. Cliquez sur le menu déroulant **[!UICONTROL Filtrer]** ![](assets/filter-nwepng.png). Si des filtres sont sélectionnés, le nombre de filtres sélectionnés s’affiche à la place de l’icône.
1. Sélectionnez l’une des options de filtre suivantes pour spécifier le type d’élément à afficher :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>Affiche et sélectionne tous les éléments. Cela inclut les tâches, les problèmes, les approbations, les tâches personnelles et les tâches et problèmes terminés. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Working On]</strong></td> 
      <td> <p>Affiche uniquement les tâches sur lesquelles vous travaillez activement. Il s’agit des tâches qui vous ont été affectées et pour lesquelles vous avez cliqué sur le bouton [!UICONTROL Work On It].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Ready to Start]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les tâches qui sont prêtes à être démarrées. Les deux affirmations suivantes doivent être vraies :</p> 
        <ul> 
         <li> <p>Les tâches et leurs parents n’ont pas de tâches/parents antérieurs ou de contraintes de tâches qui les empêchent d’être traités.</p> </li> 
         <li> <p>Toutes les tâches du prédécesseur ont été terminées.</p> </li> 
         <li> <p>La [!UICONTROL Planned Start Date] des tâches se situe dans le passé ou jusqu’à deux semaines dans le futur.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Not Ready]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les tâches qui ne sont pas encore prêtes à démarrer. L’une ou l’autre des affirmations suivantes doit être vraie :</p> 
        <ul> 
         <li> <p>Les tâches et leurs parents peuvent avoir des tâches/parents antérieurs ou des contraintes de tâches qui les empêchent d’être traités.</p> </li> 
         <li> <p>Les tâches comportent une [!UICONTROL Planned Start Date] qui se situe plus de deux semaines dans le futur.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues: Working On]</strong></td> 
      <td> <p>Affiche uniquement les problèmes sur lesquels vous travaillez activement. Il s’agit des problèmes qui vous ont été affectés et pour lesquels vous avez cliqué sur le bouton [!UICONTROL Work On It].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues: Requested]</strong></td> 
      <td>Affiche uniquement les problèmes pour lesquels vous disposez d’une affectation, mais pour lesquels vous n’avez pas cliqué sur le bouton [!UICONTROL Work On It].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personnel</strong></td> 
      <td>Affiche uniquement les tâches personnelles. Il s’agit des tâches que vous créez en tant que tâche [!UICONTROL To Do], comme décrit dans la section <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Créer une tâche personnelle</a> dans l’article <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Créer des éléments de travail à partir de la zone [!UICONTROL Home]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les approbations qui vous ont été affectées ou déléguées, ainsi que les approbations que vous avez envoyées. Les approbations comprennent les approbations de tâches (projets, tâches et problèmes), ainsi que les approbations de documents, d’épreuves, de demandes d’accès et de feuilles de temps. Pour plus d’informations sur les approbations, consultez les articles suivants :</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Afficher les approbations</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Approbations de travail</a> </p> </li> 
        </ul> 
        <p>Note : les approbations que vous avez envoyées et pour lesquelles vous gérer également l’approbation sont comptabilisées deux fois.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated: Delegated by me]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les éléments de travail que vous avez délégués à un autre utilisateur ou une autre utilisatrice.</p> 
        <p>Pour plus d’informations sur la délégation de tâches, voir <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Délégation de tâches et de problèmes</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated: Delegated to me]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les éléments de travail qui vous ont été temporairement délégués par un autre utilisateur ou une autre utilisatrice.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completed]</strong></td> 
      <td> <p>Affiche uniquement les tâches, problèmes et tâches personnelles terminés. Le travail terminé s’affiche pour les deux semaines précédentes et est regroupé dans la liste des tâches en fonction de la semaine au cours de laquelle il a été terminé. Les approbations ne sont pas incluses.</p> <p>Le travail terminé est masqué dans la [!UICONTROL Work List], sauf si vous sélectionnez ce filtre.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Les options de filtre sont basées sur des objets (Tâches, Problèmes, Approbations, Tâches personnelles).
   >* Les tâches et les problèmes sont filtrés davantage par leur état, en fonction de notre volonté de travailler dessus ([!UICONTROL Travaille sur], [!UICONTROL Prêt à démarrer], [!UICONTROL Pas prêt] pour les tâches, et [!UICONTROL Travaille sur] et [!UICONTROL Demandé] pour les problèmes). Vous pouvez choisir d’afficher les tâches ou les problèmes dans un état spécifique ou cliquer sur Tâches ou Problèmes pour sélectionner et afficher tous les états.
   >* Il existe un filtre distinct pour les éléments terminés et il inclut les tâches et les problèmes. Cela n’inclut pas les approbations. Le filtre [!UICONTROL Terminé] inclut les tâches personnelles.
   >* Vous pouvez choisir d’afficher un seul état à la fois. Par exemple, vous pouvez afficher uniquement les tâches [!UICONTROL Travaille sur] et uniquement les problèmes avec le statut [!UICONTROL Demandé]. Vous pouvez également sélectionner plusieurs états simultanément.
   >* Vous ne pouvez pas appliquer de filtres aux éléments affectés à l’une de vos équipes. Les affectations d’équipe ne sont pas incluses dans les éléments qui vous sont directement affectés.


1. (Facultatif) Organisez davantage la [!UICONTROL Liste de travail], comme décrit dans la section [Grouper et trier par date, projet et priorité](#group-and-sort-by-date-project-and-priority) dans cet article.

## Regrouper et trier par [!UICONTROL Date], [!UICONTROL Projet], et [!UICONTROL Priorité]

Vous pouvez regrouper et trier la [!UICONTROL Liste de travail] par [!UICONTROL Date d’achèvement prévue], [!UICONTROL Date d’engagement], [!UICONTROL Projet], ou [!UICONTROL Ma priorité]. L’option choisie détermine le mode de regroupement des éléments dans la [!UICONTROL Liste de travail].

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, ou (le cas échéant) cliquez sur l’icône **[!UICONTROL Menu Principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) en haut à gauche, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur le menu déroulant **[!UICONTROL Grouper par]** ![Grouper par](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png).

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
      <td> <p> Les éléments s’affichent dans les regroupements suivants dans la [!UICONTROL Work List], en fonction de leur [!UICONTROL Planned Completion Date] (le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre de l’en-tête) :</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL No Planned Completion Date]</p> </li> 
        <li> <p>[!UICONTROL This Week]</p> <p>Ce regroupement est développé par défaut.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], suivi de diverses [!UICONTROL Planned Completion Dates] (plusieurs regroupements)</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Start]</strong></td> 
      <td> <p>Les éléments s’affichent dans les regroupements suivants dans la [!UICONTROL Work List], en fonction de leur [!UICONTROL Planned Start Date] (le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre de l’en-tête) :</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL This Week] </p> <p>Ce regroupement est développé par défaut.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], suivi de diverses [!UICONTROL Planned Start Dates] (regroupements multiples)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td> 
      <td> <p>Les éléments s’affichent dans les regroupements suivants dans la [!UICONTROL Work List] (le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre de l’en-tête) :</p> 
       <ul> 
        <li> <p>[!UICONTROL No Commit Date]</p> </li> 
        <li> <p>[!UICONTROL Committed Next Week]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>Les éléments sont regroupés en fonction du projet et les projets apparaissent par ordre alphabétique dans la [!UICONTROL Work List].(Le nombre d’éléments contenus dans chaque regroupement s’affiche entre parenthèses en regard du titre de l’en-tête.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>Les éléments s’affichent dans l’ordre de votre choix. Pour plus d’informations, voir la section <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Définir la priorité du travail dans la zone [!UICONTROL Home]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>Le tri par défaut est croissant. Si vous définissez le tri sur décroissant, les options de tri sélectionnées sont stockées dans le navigateur. Si vous utilisez systématiquement le même navigateur sur le même ordinateur (et que vous n’effacez pas les données du site), le tri ne change pas. En revanche, si vous changez de navigateur ou d’ordinateur, le tri prend les paramètres par défaut.

## Afficher les éléments en retard

[!DNL Adobe Workfront] utilise les dates suivantes pour déterminer si les demandes de travail sont en retard :

* **Tâches** : [!UICONTROL date d’achèvement prévue]
* **Problèmes** : [!UICONTROL date d’achèvement prévue]
* **Documents** : [!UICONTROL date d’envoi]
* **Feuilles de temps** : [!UICONTROL date d’envoi]
* **Approbations** : [!UICONTROL date d’envoi]
* **Approbations des épreuves** : [!UICONTROL date d’échéance pour la relecture]

## Rechercher dans la [!UICONTROL liste de travail]

Lorsque vous effectuez une recherche dans la [!UICONTROL liste de travail], tous les éléments qui vous sont affectés sont renvoyés dans la recherche (y compris les éléments qui ne sont pas actuellement chargés à l’écran). Si l’option [!UICONTROL Afficher les éléments terminés] est sélectionnée, tous les éléments que vous avez marqués comme terminés au cours des deux dernières semaines sont également renvoyés.

En outre, seuls les noms des éléments de travail sont recherchés (les informations contenues dans l’élément de travail ne font pas l’objet d’une recherche, pas plus que les noms des projets où réside l’élément de travail).

Pour effectuer une recherche dans la [!UICONTROL liste de travail], procédez comme suit :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, ou (le cas échéant) cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) en haut à gauche, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Facultatif) Filtrez et groupez les [!UICONTROL listes d’éléments de travail], comme décrit dans [Filtrer la [!UICONTROL liste de travail]](#filter-the-work-list) et [Grouper et trier par date, projet et priorité](#group-and-sort-by-date-project-and-priority).

1. (Facultatif) Si vous recherchez un élément de travail déjà terminé, vous devez configurer la [!UICONTROL liste de travail] pour qu’elle affiche les éléments terminés avant la recherche.

1. Cliquez sur l’icône Rechercher ![Rechercher](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Commencez à saisir le nom de l’élément que vous recherchez.\
   La [!UICONTROL liste de travail] est automatiquement filtrée afin d’inclure les éléments dont le nom correspond.

## Modifier la taille de la liste de travail

Vous pouvez modifier la taille de la [!UICONTROL liste de travail] de sorte qu’elle consomme entre environ un quart de la zone d’accueil et environ la moitié de la zone [!UICONTROL d’accueil].

1. Cliquez sur l’icône du **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, ou (le cas échéant) cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) en haut à gauche, puis cliquez sur **[!UICONTROL Accueil]**.
1. Passez la souris sur le bord droit de la [!UICONTROL liste de travail], puis faites-la glisser vers la gauche ou vers la droite jusqu’à ce qu’elle ait la taille souhaitée.

## Réduire et développer des regroupements

Les éléments dans la [!UICONTROL liste de travail] s’affichent dans des regroupements. Vous pouvez réduire et développer des regroupements afin de contrôler le volume d’informations affichées sur la page à un moment donné.

Vous pouvez réduire et développer des regroupements au sein de la [!UICONTROL liste de travail] pour mieux contrôler les informations qui sont visibles.\
Par défaut, le regroupement [!UICONTROL Cette semaine] est développé et tous les autres regroupements sont réduits. Toutes les modifications que vous apportez seront mémorisées la prochaine fois que vous accéderez à la zone Accueil.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, ou (le cas échéant) cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) en haut à gauche, puis sur **[!UICONTROL Accueil]**.
1. Cliquez sur la flèche **[!UICONTROL Développer]** ou **[!UICONTROL Réduire]** en regard de tout regroupement que vous souhaitez développer ou réduire.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Ou\
   Pour développer ou réduire tous les regroupements simultanément, cliquez sur la flèche **[!UICONTROL Développer]** ou **[!UICONTROL Réduire]** en regard d’un regroupement, tout en maintenant la touche [!UICONTROL Maj] enfoncée.
