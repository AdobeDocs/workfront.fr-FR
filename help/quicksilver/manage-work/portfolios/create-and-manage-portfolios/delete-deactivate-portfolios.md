---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Supprimer et désactiver les portefeuilles
description: Les portfolios sont des collections de projets ou de programmes dans Adobe Workfront. Vous pouvez supprimer ou désactiver un portefeuille si vous estimez qu’il n’est pas pertinent pour votre système.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 66%

---

# Supprimer et désactiver des portfolios

<!--Audited: 08/2025-->

Les portefeuilles sont des collections de projets ou de programmes dans [!DNL Adobe Workfront]. Vous pouvez supprimer ou désactiver un portefeuille si vous estimez qu’il n’est pas pertinent pour votre système.

Plutôt que de supprimer un portfolio qui n’a plus besoin d’être associé à des projets futurs, nous recommandons de le désactiver, afin de conserver les informations historiques sur les projets qui sont actuellement associés au portfolio et à ses programmes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès. Développez pour afficher les exigences d’accès pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
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

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions on the portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

## Vue d’ensemble de la suppression et de la désactivation de portfolios

Tenez compte des éléments suivants lorsque vous décidez de supprimer ou de désactiver des portfolios :

* La suppression d’un portfolio entraîne la suppression des programmes qui lui sont associés.

  >[!IMPORTANT]
  >
  >Vous n’avez pas besoin d’avoir des autorisations sur les programmes pour pouvoir supprimer le portfolio.

* La suppression d’un portfolio ne supprime pas les projets qui lui sont associés.
* Vous ne pouvez pas récupérer les portfolios supprimés.
* La désactivation d’un portfolio garantit que son nom et ses programmes ne peuvent plus être attribués aux projets lors de la création d’un projet.
* La désactivation d’un portfolio déjà associé à un projet ne le supprime pas du projet. Si vous supprimez un portfolio désactivé d’un projet, vous devez le réactiver avant de pouvoir le joindre à nouveau au projet.

## Supprimer un portfolio

{{step1-to-portfolios}}

1. Utilisez l’une des méthodes suivantes :

   * Sélectionnez le portfolio dans la liste, puis cliquez sur l&#39;icône **[!UICONTROL Supprimer]** ![Icône Supprimer](assets/delete.png).
   * Cliquez sur le portfolio pour l’ouvrir, puis sur le menu **Plus** ![Plus](assets/more-icon.png) à droite du nom du portfolio, puis sur **Supprimer Portfolio**.
1. Cliquez sur **[!UICONTROL Oui, supprimer]** pour confirmer.

   Le portefeuille est supprimé et ne peut pas être récupéré.

## Désactiver un portfolio

Lorsque vous désactivez un portfolio, vous pouvez toujours y accéder à partir de la zone [!UICONTROL Portfolios], mais il ne s’affiche plus dans la liste des portfolios lorsque les utilisateurs et utilisatrices tentent de l’ajouter à un projet.

>[!NOTE]
>
>Selon la manière dont votre administrateur ou administratrice de groupes ou [!DNL Workfront] configure votre modèle de mise en page, la zone [!UICONTROL Portfolios] peut ne pas s’afficher dans le [!UICONTROL Menu principal]. Pour plus d’informations, voir [Personnaliser le menu principal à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Cliquez sur **[!UICONTROL Portfolios]**.
1. Cliquez sur le nom du portfolio.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-icon.png) à droite du nom du portfolio, puis cliquez sur **[!UICONTROL Désactiver Portfolio]**.
Le portfolio est immédiatement désactivé.
1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-icon.png) à droite du nom du portfolio, puis cliquez sur **[!UICONTROL Activer Portfolio]** pour le réactiver.


