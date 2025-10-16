---
product-area: reporting
navigation-topic: reporting-elements
title: Supprimer des filtres, des vues et des regroupements
description: Vous pouvez supprimer un filtre, une vue ou un regroupement des listes et des rapports si vous les avez créés ou s’ils ont été partagés avec vous. Vous ne pouvez pas supprimer les filtres, les vues ou les regroupements par défaut.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 95%

---

# Supprimer des filtres, des vues et des regroupements

<!-- Audited: 11/2024 -->

Vous pouvez supprimer un filtre, une vue ou un regroupement des listes et des rapports si vous les avez créés ou s’ils ont été partagés avec vous. Vous ne pouvez pas supprimer les filtres, les vues ou les regroupements par défaut.

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
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
    <td> <p>Autorisations en affichage avec accès au partage du filtre, de la vue ou du regroupement que vous souhaitez supprimer.</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer un filtre à l’aide du créateur standard

Vous pouvez supprimer un filtre qui a été partagé avec vous dans les listes de projets, de tâches ou de problèmes à l’aide de l’interface de création standard. L’interface de création standard n’est pas disponible pour les autres objets, ni pour les vues ou les regroupements.

Vous pouvez également supprimer les filtres que vous possédez dans les listes de projets, de tâches ou de problèmes à l’aide de l’interface de création standard.

Les filtres par défaut du système ne peuvent pas être supprimés.

### Considérations relatives à la suppression de filtres à l’aide de l’interface de création standard

Les scénarios suivants existent lorsque vous supprimez un filtre à l’aide de l’interface de création standard :

* Si le filtre a été partagé avec vous et que vous le supprimez, le filtre n’est supprimé que pour vous. La personne qui a créé le filtre et toutes les personnes avec qui il a été partagé ont toujours accès au filtre.
* Si vous êtes propriétaire du filtre et que vous le supprimez, le filtre est supprimé du système Workfront. Le filtre n’est plus disponible pour les utilisateurs et les utilisatrices avec qui vous l’aviez partagé.
* Si vous faite partie de l’équipe d’administration de Workfront, vous pouvez supprimer le filtre. Personne n’y aura plus accès, y compris la personne propriétaire.

### Supprimer un filtre à l’aide de l’interface de création standard

1. Accédez à une liste de projets, de tâches, de problèmes, de portfolios, de programmes, d’utilisateurs et d’utilisatrices, de modèles ou de groupes.
1. Cliquez sur l’icône **Filtre** ![Icône Filtre](assets/filter-nwepng.png).
1. Pointez sur un filtre sous **Partagé avec moi**, cliquez dans le menu **Plus** ![Icône Plus](assets/more-icon-spectrum.png), puis cliquez sur **Supprimer**.
1. Sélectionnez **Supprimer** dans le message de confirmation pour supprimer définitivement le filtre.

### Supprimer un filtre à l’aide de l’interface de création standard

1. Accédez à une liste de projets, de tâches, de problèmes, de portfolios, de programmes, d’utilisateurs et d’utilisatrices, de modèles ou de groupes.
1. Cliquez sur l’icône **Filtre** ![Icône Filtre](assets/filter-nwepng.png).
1. Pointez sur un filtre que vous avez le droit de supprimer, cliquez dans le menu **Plus** ![Icône Plus](assets/more-icon-spectrum.png), puis cliquez sur **Supprimer**.

   ![Supprimer le filtre](assets/new-filters-more-menu-options-with-delete.png)

1. (Facultatif) Cliquez sur **Annuler** dans le message de confirmation pour éviter la suppression et revenir à la liste des filtres.
1. Cliquez sur **Supprimer** dans le message de confirmation pour confirmer la suppression.

   Le filtre est supprimé pour vous et toutes les personnes autorisées à l’utiliser.

## Supprimer un filtre, une vue ou un regroupement à l’aide de l’interface de création héritée

Vous pouvez supprimer un filtre, une vue ou un regroupement pour toutes les listes d’objets à l’aide de l’interface du créateur hérité.

### Considérations sur la suppression des filtres, des vues et des regroupements à l’aide du créateur hérité

Pour supprimer un élément de rapport, la méthode varie selon que vous l’avez créé ou qu’il a été partagé avec vous.

Les scénarios suivants existent lorsque vous supprimez un filtre, une vue ou un regroupement :

* **Si vous avez créé l’élément et que vous le supprimez**, l’élément est supprimé du système Workfront. Il n’est plus disponible pour les utilisateurs et utilisatrices avec lesquels vous l’avez partagé.
* **Si l’élément a été partagé avec vous et que vous le supprimez**, l’élément est suppirmé uniquement pour vous. Le créateur ou la créatrice de l’élément et toutes les autres personnes avec lesquelles il a été partagé y ont toujours accès.

### Supprimer un filtre, une vue ou un regroupement à l’aide de l’interface de création héritée

1. Accédez à une liste d’objets ou à un rapport.
1. (Conditionnel) Dans une liste, cliquez sur l’icône **Filtre**, **Affichage** ou **Regroupement**, puis survolez le filtre, la vue ou le regroupement à supprimer et cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png), puis **Supprimer**. Le filtre, la vue ou le regroupement est supprimé(e).
1. (Le cas échéant) Dans un rapport, cliquez sur le menu déroulant **Regroupement**, **Filtre** ou **Vue** et sélectionnez **Supprimer le regroupement**, **Supprimer le filtre** ou **Supprimer la vue**.

   La boîte de dialogue **Mes regroupements**, **Mes filtres,** ou **Mes vues** s’affiche.

   Tous les éléments de rapport que vous avez le droit de supprimer sont disponibles pour la suppression. Les autres éléments de rapport sont grisés.

1. Cliquez sur l’icône **x** à côté de l’élément de rapport à supprimer.
1. (Le cas échéant) Cliquez sur **Oui, supprimer** si vous avez choisi de supprimer un filtre, une vue ou un regroupement que vous avez créé puis partagé avec d’autres personnes. Cette opération supprime le filtre, la vue ou le regroupement du système Workfront.

   >[!TIP]
   >
   >La suppression d’un filtre, d’une vue ou d’un regroupement que vous avez créé(e) sans le ou la partager avec d’autres personnes le ou la supprime du système sans demander de confirmation.

1. Cliquez sur **Terminé**.

