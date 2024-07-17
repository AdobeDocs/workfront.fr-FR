---
navigation-topic: use-lists
title: Appliquer le filtre rapide à une liste
description: Vous pouvez utiliser le filtre rapide dans une liste d’objets pour vous aider à localiser uniquement les éléments qui vous intéressent, afin de pouvoir rapidement les vérifier, les mettre à jour ou les partager avec d’autres personnes.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 7%

---

# Appliquer le filtre rapide à une liste

<!--
{{highlighted-preview}}
-->

Vous pouvez utiliser le filtre rapide dans une liste d’objets pour vous aider à localiser uniquement les éléments qui vous intéressent, afin de pouvoir rapidement les vérifier, les mettre à jour ou les partager avec d’autres personnes.

>[!IMPORTANT]
>
>Vous pouvez trouver les éléments qui contiennent un mot de recherche à l’aide de filtres rapides, que l’élément ait été affiché physiquement à l’écran ou qu’il s’affiche une fois que vous avez fait défiler la page vers le bas. Lorsque vous utilisez les fonctionnalités de recherche de votre navigateur, vous ne pouvez trouver que les éléments physiquement affichés à l’écran. Si votre liste comporte plusieurs pages, les filtres rapides ne trouvent pas les éléments qui se trouvent sur les pages qui ne s’affichent pas.

Si vous souhaitez enregistrer un filtre rapide, nous vous recommandons plutôt de créer un filtre permanent pour votre liste.\
Pour plus d’informations sur la création de filtres dans [!DNL Adobe Workfront], consultez l’article [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Le filtre rapide est actuellement disponible dans les zones suivantes :


Vous pouvez utiliser des filtres rapides temporaires dans toutes les listes, sauf dans les cas suivants :

* Zone [!UICONTROL Reports]
* Listes et rapports de document
* Plusieurs zones [!UICONTROL Setup]
  >[!NOTE]
  >
  >Les filtres rapides sont disponibles dans les zones de configuration suivantes : [!UICONTROL Groupes], [!UICONTROL Équipes], [!UICONTROL Entreprises], [!UICONTROL Planifications], [!UICONTROL Modèles de mise en page] et [!UICONTROL Forms personnalisé].


Tenez compte des points suivants lorsque vous appliquez des filtres rapides à une liste :

* Vous pouvez utiliser des mots-clés pour filtrer n’importe quel champ qui s’affiche dans l’affichage de la liste. Cela inclut les champs personnalisés ou les champs complexes tels que [!UICONTROL Predecessors], [!UICONTROL Assignments], [!UICONTROL Assignment] et [!UICONTROL Status], [!UICONTROL Approver] et [!UICONTROL Status], etc.
* Si votre liste contient des groupements réduits, ils sont automatiquement développés lorsque vous utilisez des filtres rapides. Lorsque vous supprimez le filtre rapide, les regroupements sont réduits à nouveau.
* Les groupes conservent les informations agrégées de la liste d’origine, quels que soient les filtres rapides appliqués ou les modifications apportées aux objets de la liste.
* Les filtres rapides sont temporaires. La modification du groupement, de l&#39;affichage, du filtrage ou du tri de la liste supprime les critères de filtrage rapide.
* Vous ne pouvez pas enregistrer un filtre rapide. Si vous souhaitez enregistrer un filtre pour l’utiliser à nouveau, envisagez de créer un filtre permanent pour la liste.
* Si la liste contient plusieurs regroupements et que le filtre rapide trouve les éléments dans un seul groupe, seul ce regroupement s’affiche avec les éléments trouvés. Tous les autres regroupements sont masqués.
* Dans une liste de tâches ou de sous-tâches, la hiérarchie de tâches est supprimée lorsque les résultats du filtre rapide s’affichent.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] forfait*</b></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] licence*</b></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Configurations des niveau d’accès*</b></td> 
   <td> <p>Afficher l’accès à la zone dans laquelle se trouve la liste</p> <p>Par exemple, pour appliquer un filtre rapide à un projet, vous avez besoin de l’accès [!UICONTROL Affichage] aux projets.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès.<br>Pour plus d'informations sur la façon dont un administrateur [!DNL Workfront] peut modifier votre niveau d'accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d'accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Autorisations d’objet</b></td> 
   <td> <p>[!UICONTROL View]</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Appliquer un filtre rapide à une liste

1. Accédez à une liste ou un rapport qui prend en charge les filtres rapides, puis cliquez sur l’icône **[!UICONTROL Filtre rapide]** ![](assets/qs-quick-filter-icon.png) de la barre d’outils.

   Ou

   Selon votre système d’exploitation ou navigateur et lors de l’utilisation d’un clavier QWERTY standard, appuyez sur l’ensemble de commandes suivant pour lancer le filtre rapide :

   * ALT+F pour [!DNL Windows] ordinateurs
   * ALT/ Option+F pour [!DNL Mac] ordinateurs

     >[!TIP]
     >
     >Si vous appuyez sur CTRL+F ou CMD+F, une info-bulle s’affiche en regard du filtre rapide pour vous rappeler ces commandes. Les commandes s’affichent également dans la zone de recherche de filtre rapide.

1. Dans la zone **[!UICONTROL Filtrer la page]**, saisissez le mot-clé par lequel vous souhaitez filtrer.

   Vous pouvez utiliser n’importe quel mot qui s’affiche actuellement dans l’affichage de la liste.

   >[!NOTE]
   >
   >Si vous utilisez un mot pouvant s’afficher sur une autre page de la liste, le filtre rapide ne trouve aucun résultat.

   Une liste des éléments correspondant aux critères de recherche s’affiche dynamiquement dans la liste lorsque vous tapez et que tous les autres éléments sont masqués. Le mot-clé utilisé dans votre recherche est surligné en jaune dans tous les champs autonomes et complexes. Des exemples de champs complexes sont des colonnes partagées ou l’une des colonnes suivantes : [!UICONTROL Affectations], [!UICONTROL Affectations] et [!UICONTROL État], [!UICONTROL Pourcentage terminé], [!UICONTROL Prédécesseurs], [!UICONTROL Approbateurs et état], [!UICONTROL Chargés de ressources], [!UICONTROL Catégories 5}, [!UICONTROL Condition], [!UICONTROL Mise à jour de condition], etc.]

1. (Facultatif) Pour modifier en masse les éléments trouvés par le filtre rapide :

   1. Sélectionnez tous les éléments de la liste ou plusieurs d’entre eux, puis cliquez sur **[!UICONTROL Modifier]** pour les modifier en masse.
   1. Une fois les modifications effectuées, cliquez sur **[!UICONTROL Enregistrer les modifications]**.

1. (Facultatif) Pour exporter les éléments trouvés par le filtre rapide, sélectionnez l’ensemble ou plusieurs des éléments de la liste, puis cliquez sur **[!UICONTROL Exporter]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Seuls les éléments trouvés dans la recherche de filtre rapide sont exportés vers le fichier que vous avez sélectionné. Si vous ne sélectionnez aucun élément avant d’exporter la liste, la liste complète non filtrée est exportée.\
   >Pour plus d’informations, voir [Export d’une liste](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Facultatif) Pour effacer les résultats filtrés, cliquez sur l’icône **[!UICONTROL Filtre rapide]** dans le coin supérieur droit de la fenêtre.\
   Ou\
   Actualisez la page.
