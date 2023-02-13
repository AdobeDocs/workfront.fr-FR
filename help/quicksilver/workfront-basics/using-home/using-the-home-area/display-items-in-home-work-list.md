---
product-area: projects
navigation-topic: use-the-home-area
title: Afficher les éléments dans le [!UICONTROL Liste de tâches] dans la zone Accueil
description: Le [!UICONTROL Liste de tâches] dans le [!UICONTROL Accueil] affiche toutes les tâches qui vous sont affectées. Vous pouvez contrôler les éléments qui s’affichent dans la variable [!UICONTROL Travail] Liste comme décrit ci-dessous.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# Afficher les éléments dans le [!UICONTROL Liste de tâches] dans la zone Accueil

Le [!UICONTROL Liste de tâches] dans le [!UICONTROL Accueil] affiche toutes les tâches qui vous sont affectées. Vous pouvez contrôler les éléments qui s’affichent dans la variable [!UICONTROL Travail] Liste comme décrit ci-dessous.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Révision [!UICONTROL] pour les approbations uniquement</p> <p>[!UICONTROL Travail] ou version ultérieure pour tous les autres objets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Accès à [!UICONTROL View] ou à un accès supérieur à Projects, Tasks, Issues et Documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Attribuez des autorisations ou des autorisations supérieures aux tâches et problèmes sur lesquels vous devez travailler.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Filtrez les [!UICONTROL Liste de tâches]

Vous pouvez filtrer les éléments de la variable [!UICONTROL Liste de tâches] pour afficher uniquement des types d’éléments spécifiques. Par exemple, vous pouvez filtrer la variable [!UICONTROL Liste de tâches] pour afficher uniquement les problèmes ou les requêtes.

>[!NOTE]
>
>Les options de filtre sont stockées dans le navigateur. Si vous utilisez systématiquement le même navigateur sur le même ordinateur (et que vous n’effacez pas les données du site), les filtres sélectionnés ne changent pas. Si vous changez de navigateur ou d’ordinateur, les filtres reviennent à l’option par défaut, qui est de ne pas sélectionner tous les filtres.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur le bouton **[!UICONTROL Filtrer]** ![](assets/filter-nwepng.png) menu déroulant.
1. Sélectionnez l’une des options de filtre suivantes pour spécifier le type d’élément à afficher :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Toutes]</strong></td> 
      <td>Affiche et sélectionne tous les éléments. Cela inclut les tâches, les problèmes, les approbations, les tâches personnelles et les tâches et problèmes terminés. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tâches En Cours D’Utilisation]</strong></td> 
      <td> <p>Affiche uniquement les tâches sur lesquelles vous travaillez activement. Il s’agit des tâches qui vous ont été affectées et pour lesquelles vous avez cliqué sur le bouton [!UICONTROL Travailler dessus] .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tâches prêtes à démarrer]</strong></td> 
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
      <td role="rowheader"><strong>[!UICONTROL Tâches non prêtes]</strong></td> 
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
      <td role="rowheader"><strong>[!UICONTROL Problèmes En Cours D’Utilisation]</strong></td> 
      <td> <p>Affiche uniquement les problèmes sur lesquels vous travaillez activement. Il s’agit des problèmes qui vous ont été attribués pour lesquels vous avez cliqué sur le bouton [!UICONTROL Travailler dessus] .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problèmes demandés]</strong></td> 
      <td>Affiche uniquement les problèmes auxquels vous êtes affecté mais pour lesquels vous n’avez pas cliqué sur le bouton [!UICONTROL Travailler dessus].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personnel</strong></td> 
      <td>Affiche uniquement les tâches personnelles. Il s’agit des tâches que vous créez en tant que tâche [!UICONTROL À faire], comme décrit dans la section . <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Créer une tâche personnelle</a> dans l’article <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Création d’éléments de travail à partir de la zone [!UICONTROL Accueil]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approbations]</strong></td> 
      <td> 
       <div> 
        <p>Affiche uniquement les approbations qui vous ont été attribuées ou qui vous ont été déléguées, ainsi que les approbations que vous avez soumises. Les approbations comprennent les approbations sur les tâches (projets, tâches et problèmes), ainsi que les approbations pour les documents, les bons à tirer, les demandes d’accès et les feuilles de temps. Pour plus d’informations sur les approbations, consultez les articles suivants :</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Afficher les approbations</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Approbations de travail</a> </p> </li> 
        </ul> 
        <p>Remarque : Les approbations que vous avez envoyées et pour lesquelles vous êtes également l’un des approbateurs sont comptabilisées deux fois.</p> 
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
   >* Les tâches et les problèmes sont filtrés davantage par leur état, en fonction de notre volonté de travailler dessus ([!UICONTROL Utilisation de], [!UICONTROL Prêt à démarrer], [!UICONTROL Pas prêt] pour les tâches, et [!UICONTROL Utilisation de] et [!UICONTROL Demandé] pour les problèmes). Vous pouvez choisir d’afficher les tâches ou les problèmes dans un état spécifique ou cliquer sur Tâches ou Problèmes pour sélectionner et afficher tous les états.
   >* Il existe un filtre distinct pour les éléments terminés et il inclut les tâches et les problèmes. Cela ne comprend pas les approbations. Le [!UICONTROL Terminé] filtre inclut les tâches personnelles.
   >* Vous ne pouvez sélectionner qu’un seul état à la fois. Par exemple, vous pouvez afficher uniquement [!UICONTROL Utilisation de] tâches et uniquement [!UICONTROL Demandé] problèmes.
   >* Vous ne pouvez pas appliquer de filtres aux éléments affectés à l’une de vos équipes et ils ne sont pas inclus dans les éléments qui vous sont directement affectés.



1. (Facultatif) Organisez davantage la variable [!UICONTROL Liste de tâches], comme décrit dans la section [Grouper et trier par date, projet et priorité](#group-and-sort-by-date-project-and-priority) dans cet article.

## Regrouper et trier par [!UICONTROL Date], [!UICONTROL Projet], et [!UICONTROL Priorité]

Vous pouvez regrouper et trier les [!UICONTROL Liste de tâches] par [!UICONTROL Date d’achèvement prévue], [!UICONTROL Date de validation], [!UICONTROL Projet]ou [!UICONTROL Ma priorité]. L’option choisie détermine le mode de regroupement des éléments dans la variable [!UICONTROL Liste de tâches].

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur le bouton **[!UICONTROL Group by]** menu déroulant.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Fin planifiée]</strong></td> 
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
>Le tri par défaut est croissant. Si vous définissez le tri sur descendant , les options de tri sélectionnées sont stockées dans le navigateur. Si vous utilisez systématiquement le même navigateur sur le même ordinateur (et que vous n’effacez pas les données du site), le tri ne change pas, mais si vous changez de navigateur ou d’ordinateur, le tri passe au tri par défaut.

## Afficher les éléments en retard

[!DNL Adobe Workfront] utilise les dates suivantes pour déterminer si les demandes de travail sont en retard :

* **Tâches**: [!UICONTROL Date d’achèvement prévue]
* **Problèmes**: [!UICONTROL Date d’achèvement prévue]
* **Documents**: [!UICONTROL Date d’envoi]
* **Feuilles de temps**: [!UICONTROL Date d’envoi]
* **Approbations**: [!UICONTROL Date d’envoi]
* **Validation des BAT**: [!UICONTROL Date limite de BAT]

## Recherchez le [!UICONTROL Liste de tâches]

Lorsque vous effectuez une recherche dans la variable [!UICONTROL Liste de tâches], tous les éléments qui vous sont affectés sont renvoyés dans la recherche (y compris les éléments qui ne sont pas actuellement chargés à l’écran). Si la variable [!UICONTROL Afficher terminé] est sélectionnée, tous les éléments que vous avez marqués comme étant terminés au cours des deux dernières semaines sont également renvoyés.

En outre, seuls les noms des tâches sont recherchés (les informations contenues dans l’élément de travail ne sont pas recherchées, de même que les noms des projets où réside l’élément de travail).

Pour rechercher la variable [!UICONTROL Liste de tâches]:

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Facultatif) Filtrez la variable [!UICONTROL Liste de tâches], comme décrit dans [Filtrez les [!UICONTROL Liste de tâches]](#filter-the-work-list) et [Grouper et trier par date, projet et priorité](#group-and-sort-by-date-project-and-priority).

1. (Facultatif) Si vous recherchez un élément de travail déjà terminé, vous devez configurer la variable [!UICONTROL Liste de tâches] pour afficher les éléments terminés avant la recherche.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Commencez à saisir le nom de l’élément que vous recherchez.\
   Le [!UICONTROL Liste de tâches] est automatiquement filtré afin d’inclure les éléments dont le nom correspond.

## Modification de la taille de la liste de tâches

Vous pouvez modifier la taille de la variable [!UICONTROL Liste de tâches] de sorte qu’elle consomme entre environ un quart de la zone d’accueil et environ la moitié de la [!UICONTROL Accueil] zone.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Passez la souris sur le bord droit de la [!UICONTROL Liste de tâches], puis faites glisser vers la gauche ou vers la droite jusqu’à ce que la liste de tâches corresponde à la taille souhaitée.

## Réduire et développer des groupements

Éléments dans la variable [!UICONTROL Liste de tâches] s’affichent dans des regroupements. Vous pouvez réduire et développer des regroupements afin de contrôler le volume d’informations affichées sur la page à un moment donné.

Vous pouvez réduire et développer des groupes au sein de la [!UICONTROL Liste de tâches] pour mieux contrôler quelles informations sont visibles.\
Par défaut, la variable [!UICONTROL Cette semaine] Le regroupement est développé et tous les autres regroupements sont réduits. Toutes les modifications que vous apportez sont mémorisées la prochaine fois que vous accédez à la zone Accueil.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur le bouton **[!UICONTROL Développer]** ou **[!UICONTROL Réduire]** flèche en regard de tout regroupement que vous souhaitez développer ou réduire.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Ou\
   Pour développer ou réduire tous les regroupements simultanément, cliquez sur le bouton **[!UICONTROL Développer]** ou **[!UICONTROL Réduire]** flèche en regard d’un groupement tout en maintenant la touche [!UICONTROL Maj] clé.
