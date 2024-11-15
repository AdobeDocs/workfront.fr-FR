---
navigation-topic: use-lists
title: Modification de l’affichage d’une liste
description: Dans  [!DNL Adobe Workfront], vous pouvez personnaliser l’affichage d’une liste. Les autres personnes qui consultent la liste ne voient pas vos modifications.
feature: Get Started with Workfront
author: Nolan
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 97%

---

# Modifier l’affichage d’une liste

<!--Audited: 11/2024-->

Dans [!DNL Adobe Workfront], vous pouvez personnaliser l’affichage d’une liste. Les autres personnes qui consultent la liste ne voient pas vos modifications.

Vous pouvez effectuer les personnalisations suivantes :

* Le nombre d’éléments qui s’affichent
* Largeur ou ordre des colonnes
* Si les groupes sont développés ou réduits

>[!NOTE]
>
>Les modifications d’affichage que vous avez effectuées sont annulées lorsque vous vous déconnectez de [!DNL Workfront] ou que vous fermez votre navigateur. Ces modifications peuvent également être annulées après une période de 8 heures.

Outre les personnalisations temporaires susmentionnées, vous pouvez également définir les colonnes par lesquelles la liste est triée, ce que [!DNL Workfront] conserve même lorsque vous vous déconnectez ou que vous fermez votre navigateur. Toutefois, si quelqu’un modifie les options de tri dans la vue d’une liste, la sélection précédente n’est pas conservée.

Pour plus d’informations sur la modification des informations qui s’affichent dans votre liste, voir [Éléments de rapports : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur ou version ultérieure </p></li>
   </ul>

<p>Actuel :</p>
   <ul><li><p>Requête ou supérieure</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès [!UICONTROL View] à la zone dans laquelle se trouve la liste.</p> <p>Par exemple, pour modifier la vue d’un projet, vous devez disposer d’un accès [!UICONTROL View] aux projets.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisation [!UICONTROL View] ou autorisations plus élevées pour la vue appliquée à la liste</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier une liste

1. Accédez à la liste que vous souhaitez modifier dans [!DNL Workfront].

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (Facultatif et le cas échéant) Si les groupes de la liste sont réduits et que vous souhaitez afficher davantage d’informations, cliquez sur le groupe souhaité pour développer la liste et afficher les informations qu’elle contient.

   Ou

   Pour développer tous les groupes, cliquez sur la flèche à droite de la case à cocher dans l’en-tête de la colonne.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (Facultatif et le cas échéant) Si vous souhaitez afficher un nombre spécifique d’éléments à l’écran, cliquez sur le menu déroulant **[!UICONTROL Afficher]** dans le coin inférieur droit de l’écran, puis choisissez d’afficher **100**, **250**, **500**, **[!UICONTROL Tous]**, ou **2 000** éléments.

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >Par défaut, 2 000 éléments s’affichent pour les listes mises à jour et 100 éléments pour les listes héritées. Si la liste contient plus de 2 000 éléments, vous ne pouvez pas afficher tous les éléments sur une seule page.
   >
   >
   >Pour obtenir les meilleures performances dans les grandes listes où les objets contiennent des champs de texte formaté, nous recommandons de limiter ce nombre à 250.
   >
   >
   >Pour plus d’informations sur les deux types de listes, voir la section [Différence entre les listes mises à jour et les listes héritées](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) dans l’article [Commencer avec les listes dans  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   Les résultats de votre liste sont paginés de manière à afficher le nombre sélectionné d’éléments par page. Vous pouvez accéder aux résultats d’autres pages en cliquant sur les flèches vers l’arrière et vers l’avant ou en sélectionnant une page spécifique.

1. Pour redimensionner la largeur d’une colonne, passez la souris sur la ligne qui sépare deux colonnes, puis cliquez pour la faire glisser jusqu’à la largeur souhaitée.

   La colonne est redimensionnée jusqu’à ce que vous vidiez le cache du navigateur ou que vous la redimensionniez manuellement.

1. Pour réorganiser les colonnes d’une liste, passez la souris sur l’en-tête d’une colonne pour afficher l’outil main, puis cliquez pour faire glisser la colonne à l’endroit où vous souhaitez qu’elle s’affiche.

   La position de la colonne est sauvegardée jusqu’à ce que vous actualisiez votre page.

   Pour plus d’informations sur la personnalisation de la largeur et l’ordre des colonnes dans une liste, voir l’article [Modifier la largeur et l’ordre des colonnes](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. Pour modifier l’ordre de tri d’une liste, cliquez sur un en-tête de colonne pour le sélectionner, puis maintenez enfoncée la touche CMD (sur [!DNL Mac]) ou la touche CTRL (sur [!DNL Windows]) de votre clavier et sélectionnez jusqu’à deux en-têtes de colonne supplémentaires pour les trier.

   La liste est triée sur chacune des colonnes sélectionnées dans l’ordre de votre sélection.

   Toutes les modifications que vous apportez à la liste sont enregistrées instantanément.

   >[!NOTE]
   >
   >Si vous triez les groupes dans la zone [!UICONTROL Groups] de [!UICONTROL Configuration], la vue hiérarchique des groupes et de leurs sous-groupes n’est pas interrompue lorsque vous modifiez le mode de tri de la liste : les sous-groupes restent avec leurs groupes parent. La liste est d’abord triée par groupes de niveau supérieur. Ensuite, sous chaque groupe parent, les sous-groupes de la liste qui se trouvent au même niveau sont triés ensemble.
