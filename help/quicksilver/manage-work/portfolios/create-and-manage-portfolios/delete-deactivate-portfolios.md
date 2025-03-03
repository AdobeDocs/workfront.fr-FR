---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Supprimer et désactiver des portfolios
description: Les portfolios sont des collections de projets ou de programmes dans Adobe Workfront. Vous pouvez supprimer ou désactiver un portefeuille si vous estimez qu’il n’est pas pertinent pour votre système.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 90%

---

# Supprimer et désactiver des portfolios

<!--Audited: 2/2024-->

Les portefeuilles sont des collections de projets ou de programmes dans [!DNL Adobe Workfront]. Vous pouvez supprimer ou désactiver un portefeuille si vous estimez qu’il n’est pas pertinent pour votre système.

Plutôt que de supprimer un portfolio qui n’a plus besoin d’être associé à des projets futurs, nous recommandons de le désactiver, afin de conserver les informations historiques sur les projets qui sont actuellement associés au portfolio et à ses programmes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard] </p>
   <p>Actuelle : [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès [!UICONTROL Edit] aux projets et aux portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Manage] au portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble de la suppression et de la désactivation de portfolios

Tenez compte des éléments suivants lorsque vous décidez de supprimer ou de désactiver des portfolios :

* La suppression d’un portfolio entraîne la suppression des programmes qui lui sont associés.

  >[!IMPORTANT]
  >
  >Vous n’avez pas besoin d’avoir des autorisations sur les programmes pour pouvoir supprimer le portfolio.

* La suppression d’un portfolio ne supprime pas les projets qui lui sont associés.
* Vous ne pouvez pas récupérer les portfolios supprimés.
* La désactivation d’un portfolio garantit que son nom et ses programmes ne peuvent plus être attribués aux projets lors de la création d’un projet.

## Désactiver un portfolio

Lorsque vous désactivez un portfolio, vous pouvez toujours y accéder à partir de la zone [!UICONTROL Portfolios], mais il ne s’affiche plus dans la liste des portfolios lorsque les utilisateurs et utilisatrices tentent de l’ajouter à un projet.

>[!NOTE]
>
>Selon la manière dont votre administrateur ou administratrice de groupes [!DNL Workfront] configure votre modèle de disposition, la zone [!UICONTROL Portfolios] peut ne pas s’afficher dans le [!UICONTROL Menu principal]. Pour plus d’informations, voir [Personnaliser le menu principal à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Cliquez sur **[!UICONTROL Portfolios]**.
1. Cliquez sur le nom du portfolio.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-icon.png) à droite du nom du portfolio, puis cliquez sur **[!UICONTROL Désactiver Portfolio]**.

## Supprimer un portfolio

{{step1-click-main-menu}}

1. Cliquez sur **[!UICONTROL Portfolios]**.
1. Sélectionnez le portfolio, puis cliquez sur **[!UICONTROL Supprimer]**&#x200B; l’icône [!UICONTROL Supprimer] ![Icône Supprimer](assets/delete.png).
1. Cliquez sur **[!UICONTROL Oui, supprimer]** pour confirmer.
