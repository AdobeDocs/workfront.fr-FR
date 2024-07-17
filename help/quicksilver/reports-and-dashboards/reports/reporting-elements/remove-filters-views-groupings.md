---
product-area: reporting
navigation-topic: reporting-elements
title: Supprimer des filtres, des vues et des regroupements
description: Vous pouvez supprimer un filtre, une vue ou un regroupement des listes et des rapports si vous les avez créés ou s’ils ont été partagés avec vous. Vous ne pouvez pas supprimer les filtres, les vues ou les regroupements par défaut.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 11%

---

# Supprimer des filtres, des vues et des regroupements

Vous pouvez supprimer un filtre, une vue ou un regroupement des listes et des rapports si vous les avez créés ou s’ils ont été partagés avec vous. Vous ne pouvez pas supprimer les filtres, les vues ou les regroupements par défaut.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront*</strong></td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Affichage ou accès supérieur à Filtres, Vues, Regroupements</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher les autorisations ayant accès au partage sur le filtre, l’affichage ou le regroupement que vous souhaitez supprimer</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Suppression d’un filtre à l’aide du créateur standard

Vous pouvez supprimer un filtre qui a été partagé avec vous à partir des listes de projets, de tâches ou de problèmes à l’aide de l’interface du créateur standard. L’interface du créateur standard n’est disponible pour aucun autre objet, ni pour les vues ou les regroupements.

Vous pouvez également supprimer des filtres que vous détenez dans les listes de projets, de tâches ou de problèmes à l’aide de l’interface du créateur standard.

Les filtres par défaut du système ne peuvent être ni supprimés, ni supprimés.

### Points à prendre en compte concernant la suppression ou la suppression de filtres à l’aide du créateur standard

Les scénarios suivants existent lorsque vous supprimez ou supprimez un filtre à l’aide du créateur standard :

* Si le filtre a été partagé avec vous et que vous le supprimez, il est supprimé uniquement pour vous. L’utilisateur qui l’a créée à l’origine et tous les autres utilisateurs avec lesquels elle a été partagée ont toujours accès au filtre.
* Si vous possédez le filtre et que vous le supprimez, celui-ci est supprimé du système Workfront. Le filtre n’est plus disponible pour les utilisateurs avec lesquels vous l’avez partagé.
* Si vous êtes administrateur de Workfront, vous pouvez supprimer le filtre, qui est définitivement supprimé pour tous les utilisateurs, y compris le propriétaire.

### Suppression d’un filtre à l’aide du créateur standard

1. Accédez à une liste de projets, de tâches, de problèmes, de portfolios, de programmes, d’utilisateurs, de modèles ou de groupes.
1. Cliquez sur l&#39;icône **Filtrer** ![Icône Filtrer](assets/filter-nwepng.png).
1. Passez la souris sur un filtre sous **Partagé avec moi**, cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon-spectrum.png), puis cliquez sur **Supprimer**.

   ![Supprimer le filtre](assets/new-filters-more-menu-remove-filter.png)

1. Sélectionnez **Supprimer** sur le message de confirmation pour supprimer définitivement le filtre.

### Suppression d’un filtre à l’aide du créateur standard

1. Accédez à une liste de projets, de tâches, de problèmes, de portfolios, de programmes, d’utilisateurs, de modèles ou de groupes.
1. Cliquez sur l&#39;icône **Filtrer** ![Icône Filtrer](assets/filter-nwepng.png).
1. Passez la souris sur un filtre que vous pouvez supprimer, cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon-spectrum.png), puis sur **Supprimer**.

   ![Supprimer le filtre](assets/new-filters-more-menu-options-with-delete.png)

1. (Facultatif) Cliquez sur **Annuler** dans le message de confirmation pour éviter la suppression et revenir à la liste des filtres.
1. Cliquez sur **Supprimer** dans le message de confirmation pour confirmer la suppression.

   Le filtre est supprimé pour vous et tous les utilisateurs qui y avaient des autorisations.

## Suppression d’un filtre, d’une vue ou d’un regroupement à l’aide du créateur hérité

Vous pouvez supprimer un filtre, une vue ou un regroupement pour toutes les listes d’objets à l’aide de l’interface du créateur hérité.

### Points à prendre en compte concernant la suppression des filtres, des vues et des groupes à l’aide du créateur hérité

La manière dont vous supprimez un élément de rapport varie selon que vous l’avez initialement créé ou qu’il a été partagé avec vous.

Les scénarios suivants se présentent lorsque vous supprimez un filtre, une vue ou un regroupement :

* **Si vous avez créé l’élément et que vous le supprimez**, l’élément est supprimé du système Workfront. Il n’est plus disponible pour les utilisateurs avec qui vous l’avez partagé précédemment.
* **Si l’élément a été partagé avec vous et que vous le supprimez**, l’élément est supprimé uniquement pour vous. L’utilisateur qui l’a créée à l’origine et tous les autres utilisateurs avec lesquels elle a été partagée y ont toujours accès.

### Suppression d’un filtre, d’une vue ou d’un regroupement à l’aide du créateur hérité

1. Accédez à une liste d’objets ou à un rapport.
1. (Conditionnel) Dans une liste, cliquez sur l’icône **Filtre**, **Vue** ou **Groupement**, puis survolez le filtre, la vue ou le groupe que vous souhaitez supprimer, cliquez sur l’icône **Plus** ![](assets/more-icon.png), puis **Supprimer**. Le filtre, l’affichage ou le regroupement est supprimé.
1. (Conditionnel) Dans un rapport, cliquez sur le menu déroulant **Groupement**, **Filtre** ou **Affichage** et sélectionnez **Supprimer le groupement**, **Supprimer le filtre** ou **Supprimer la vue**.

   La boîte de dialogue **Mes groupes**, **Mes filtres,** ou **Mes vues** s’affiche.

   Tous les éléments de rapports que vous pouvez supprimer peuvent être supprimés. Les autres éléments de rapport s’affichent en grisé.

1. Cliquez sur l’icône **x** en regard de tout élément de rapport à supprimer.
1. (Conditionnel) Cliquez sur **Oui, supprimez-le** si vous avez choisi de supprimer un filtre, une vue ou un regroupement que vous avez créé et que vous avez partagé ultérieurement avec d’autres utilisateurs. Cela supprime le filtre, la vue ou le regroupement du système Workfront.

   >[!TIP]
   >
   >La suppression d’un filtre, d’une vue ou d’un regroupement que vous avez créé sans le partager avec d’autres le supprime du système sans demander de confirmation.

1. Cliquez sur **Terminé**.

