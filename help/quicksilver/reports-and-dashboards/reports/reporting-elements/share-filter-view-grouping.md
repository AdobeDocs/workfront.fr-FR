---
product-area: reporting
navigation-topic: reporting-elements
title: Partager un filtre, une vue ou un regroupement
description: Vous pouvez partager des filtres, des vues et des regroupements auxquels vous avez accès avec d’autres utilisateurs et utilisatrices.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 99%

---

# Partager un filtre, une vue ou un regroupement

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

Votre personne chargée de l’administration d’Adobe Workfront permet aux utilisateurs et utilisatrices d’afficher ou de modifier des objets lorsqu’elle attribue des niveaux d’accès. Pour plus d’informations sur l’octroi d’accès aux objets, voir [Créer ou modifier les niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Outre le niveau d’accès accordé aux utilisateurs et utilisatrices, vous pouvez leur accorder des autorisations pour afficher ou modifier des objets spécifiques que vous avez créés ou dont vous avez l’accès en partage. Pour plus d’informations sur les niveaux d’accès et les autorisations, voir [Comment les niveaux d’accès et les autorisations fonctionnent ensemble](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Vous pouvez partager des filtres, des vues et des regroupements auxquels vous avez accès avec d’autres utilisateurs et utilisatrices.

Lorsqu’un objet (filtre, vue ou regroupement) est partagé avec vous, vous pouvez appliquer ce filtre, cette vue ou ce regroupement à vos listes. Selon l’accès qui vous est accordé, vous pouvez le modifier et le partager avec d’autres utilisateurs et utilisatrices.

Pour plus d’informations sur la création d’un filtre, d’une vue ou d’un regroupement, consultez les articles suivants :

* [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</strong></td> 
   <td> 
    <p>Contributeur ou version ultérieure</p>
    <p>Requête ou supérieure</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou accès supérieur aux filtres, aux vues et aux regroupements</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
    <td> <p>Autorisations en affichage ou supérieures pour partager une vue, un filtre ou un regroupement</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Partager un filtre, une vue ou un regroupement

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

Le partage de filtres dans des listes sélectionnées est différent selon l’interface utilisée pour partager le filtre : standard ou héritée. Pour plus d’informations sur les types d’interfaces de création de filtres, consultez [Créer ou modifier des filtres dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Vous pouvez partager des vues et des regroupements uniquement dans l’interface héritée.

### Partager des filtres à l’aide de l’interface du créateur standard

Vous pouvez partager un filtre dans l’interface standard à partir de listes de projets, de tâches, de problèmes, de portfolios, de programmes, d’utilisateurs, d’utilisatrices, de modèles ou de groupes. L’interface du créateur standard pour les filtres n’est disponible pour aucun autre objet, ni pour les vues ou les regroupements.

Partagez un filtre à l’aide de l’interface du créateur standard :

1. Accédez à une liste de projets, de tâches ou de problèmes.
1. Cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-nwepng.png).

   ![Créateur de filtres standard](assets/new-filters-all-filter-types.png)

1. Consultez les listes de filtres suivantes :

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Favori</strong></td>
   <td>Filtres marqués comme favoris. Lorsque vous mettez un filtre en favori, son emplacement d’origine est indiqué sous son nom et il est masqué de la liste d’origine, sauf si vous le supprimez de vos favoris.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Enregistré</strong></td>
   <td>Filtres que vous avez personnellement créés et enregistrés. Par défaut, cette liste affiche les filtres enregistrés dans l’ordre du dernier enregistrement, mais vous pouvez réorganiser manuellement la liste en faisant glisser les noms des filtres.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Paramètres par défaut du système</strong></td>
   <td>Filtres par défaut du système Workfront, ainsi que les filtres que l’administrateur ou l’administratrice Workfront a ajoutés à votre liste de filtres, au niveau du système ou dans votre modèle de mise en page.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Partagé avec moi</strong></td>
   <td>Filtres que d’autres personnes ont créés et partagés avec vous ou qui sont partagés à l’échelle du système.</td>
   </tr>
   </tbody>
   </table>

1. Pointez sur un filtre auquel vous avez accès pour au moins afficher et partager, puis cliquez sur le menu **Plus** ![Menu Plus](assets/more-icon-spectrum.png), puis cliquez sur **Partager**.

   ![Options du menu Plus](assets/new-filters-more-menu-options-with-delete.png)

   La boîte de dialogue Partage des filtres s’affiche.

1. Commencez à saisir les noms des personnes, des équipes, des rôles, des groupes ou des entreprises avec lesquels vous souhaitez partager le contenu dans le champ **Accorder l’accès à**.

   ![Zone de partage de filtre](assets/new-filters-share-filter.png)

1. (Facultatif) Cliquez sur la flèche pointant vers la droite située en regard du nom d’une entité pour modifier ses autorisations sur le filtre, puis activez l’option **Afficher** ou **Gérer**. **Afficher** est la valeur par défaut.

   ![Autorisations de partage](assets/new-filters-sharing-permissions.png)

1. (Facultatif) Activez ou désactivez les autorisations supplémentaires pour une entité en effectuant l’une des opérations suivantes :

   1. Cliquez sur **Afficher** et désactivez l’option **Partager**. Elle est activée par défaut.
   1. Cliquez sur **Gérer** et désactivez l’option **Partager** ou **Supprimer**. Ils sont activés par défaut.

      >[!NOTE]
      >
      >Si vous activez l’accès Gérer avec l’option Supprimer, ces personnes pourront supprimer le filtre de toutes les personnes, même si elles ne sont pas propriétaires du filtre.

   >[!TIP]
   >
   >Les utilisateurs et utilisatrices ne peuvent pas recevoir d’autorisation supérieure à leur niveau d’accès. Si leur niveau d’accès n’offre pas l’accès à la section Modifier les filtres, ils ne peuvent pas recevoir d’autorisations pour gérer un filtre. Workfront désactive l’option Gérer pour ces utilisateurs et utilisatrices et l’option est grisée.

1. Cliquez sur **Partager**. Le filtre est partagé avec les entités que vous avez spécifiées.

   >[!TIP]
   >
   >Le partage avec les groupes donne des autorisations sur le filtre aux personnes membres du groupe et de tous les sous-groupes.

   Les filtres que vous avez partagés s’affichent dans la section **Partagé avec moi** du panneau de filtrage pour ces entités.

   ![Filtres partagés avec moi](assets/new-filters-shared-with-me.png)

### Partager des filtres, des vues et des regroupements à l’aide de l’interface héritée

Le partage de filtres, de vues et de regroupements dans l’interface héritée est identique.

1. Accédez à une liste d’objets ou à un rapport.
1. (Le cas échéant) Dans une liste, cliquez sur l’icône **Filtre**, **Vue**, ou **Regroupement**, puis pointez sur le filtre, la vue ou le regroupement que vous souhaitez partager et cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png), puis sur **Partager**.

   Dans un rapport, cliquez sur le menu déroulant **Filtre**, **Vue**, ou **Regroupement**, puis sélectionnez le filtre, la vue ou le regroupement à partager.

1. (Le cas échéant) Si vous partagez à partir d’un rapport, cliquez à nouveau sur le menu déroulant **Filtre**, **Vue** ou **Regroupement**, puis cliquez sur **Partager le filtre**, **Partager la vue** ou **Partager le regroupement**.\
   La boîte de dialogue **Accès aux filtres**, **Accès aux vues**, ou **Accès aux regroupements** s’affiche.

   ![Partage d’un filtre](assets/share-filter-people-box-nwe-350x458.png)

1. Procédez de l’une des manières suivantes, selon avec qui vous souhaitez partager :

   **Pour partager avec des personnes, des équipes, des rôles, des groupes ou des entreprises individuels :** dans le champ fourni, commencez à saisir le nom de la personne, de l’équipe, du rôle, du groupe ou de l’entreprise avec lequel vous souhaitez partager le contenu, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.\
   Répétez ce processus pour partager l’accès avec plusieurs personnes, équipes, rôles, groupes ou entreprises.

   >[!TIP]
   >
   >Le partage avec les groupes donne des autorisations sur les filtres, vues ou regroupements aux personnes membres du groupe et de tous les sous-groupes.

   **Pour partager avec toutes les personnes du système :** cliquez sur l’icône **Paramètres** puis cliquez sur **Rendre ceci visible sur tout le système**.\
   Pour que cette option soit disponible, votre administrateur ou administratrice doit sélectionner l’option Partager sur le système. Pour plus d’informations, voir les articles [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) et [Partager des rapports, des tableaux de bord et des calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Le cas échéant) Si vous partagez avec des personnes, équipes, rôles, groupes ou entreprises individuels, cliquez sur le menu déroulant pour définir le niveau d’accès que vous souhaitez accorder.

   Vous pouvez sélectionner l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>L'afficher</strong></td> 
      <td> <p>Sélectionnez cette option pour autoriser les personnes destinataires du partage à utiliser uniquement l’objet (filtre, vue ou regroupement) partagé. Lorsque cette option est sélectionnée, les personnes destinataires ne peuvent pas apporter de modifications à l’élément partagé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Le gérer</strong></td> 
      <td> <p>Sélectionnez cette option pour permettre aux destinataires du partage d’utiliser et de modifier le filtre, la vue ou le regroupement partagé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Partager</strong></td> 
      <td> <p>Cliquez sur <strong>Paramètres avancés</strong>, puis sélectionnez ou désélectionnez l’option <strong>Partager</strong> selon que vous souhaitez que les destinataires puissent partager avec d’autres personnes ou non.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Les personnes avec lesquelles vous avez partagé le filtre, la vue ou le regroupement peuvent y accéder en cliquant sur le menu déroulant ou l’icône **Filtre**, **Vue**, ou **Regroupement**, puis en faisant défiler l’écran jusqu’à la section **Partagé avec moi**.


