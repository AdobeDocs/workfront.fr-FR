---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Création, modification et partage des filtres, vues et groupes par défaut
description: Vous pouvez créer des filtres, des vues et des regroupements par défaut, puis les mettre à la disposition des personnes de votre organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 98%

---

# Créer, modifier et partager des filtres, des vues et des regroupements par défaut

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Vous pouvez créer des filtres, des vues et des regroupements par défaut, puis les mettre à la disposition des personnes de votre organisation.

Lorsque vous créez des filtres, des vues et des regroupements par défaut comme décrit dans cet article, les personnes avec lesquelles vous les partagez peuvent les utiliser lorsqu’elles consultent leurs listes. Les personnes peuvent créer leurs propres filtres, vues et regroupements sur la base de ceux que vous créez, mais elles ne peuvent pas modifier directement ceux que vous créez.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être administrateur ou administratrice de [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice de [!DNL Workfront] s’il ou elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Créer des filtres, des vues ou des regroupements par défaut

{{step-1-to-setup}}

1. Effectuez l’une des opérations suivantes, selon que vous créez ou modifiez un filtre, une vue ou un regroupement :

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Filtres]**.

   * Cliquez sur **[!UICONTROL Interface] >** **[!UICONTROL Vues]**.

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Regroupements]**.

1. Si vous créez un filtre, une vue ou un regroupement, cliquez sur **[!UICONTROL Ajouter un filtre]**, **[!UICONTROL Ajouter une vue]** ou **[!UICONTROL Ajouter un regroupement]**, puis sélectionnez le type d’objet auquel vous souhaitez associer le nouveau filtre, la nouvelle vue ou le nouveau regroupement.

   Ou

   Si vous modifiez un filtre, une vue ou un regroupement existant(e), sélectionnez l’élément puis cliquez sur l’icône **[!UICONTROL Modifier]** ![Icône Modifier](assets/edit-icon.png).

1. Configurez le filtre, la vue ou le regroupement.

   Pour plus d’informations sur les options disponibles, consultez l’un des articles suivants :

   * [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Vue d’ensemble des vues dans [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Vue d’ensemble des regroupements dans [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Cliquez sur **[!UICONTROL Enregistrer]** dans le coin inférieur gauche.

Vous pouvez mettre le filtre, la vue ou le regroupement à la disposition des personnes de votre système. Pour plus d’informations sur le partage de filtres, de vues ou de regroupements avec d’autres personnes, voir la section [Mettre des filtres, des vues ou des regroupements à la disposition des personnes](#make-filters-views-or-groupings-available-to-users) dans cet article.


## Afficher ou masquer les filtres, les vues ou les regroupements disponibles dans le modèle de disposition

Vous pouvez choisir d’afficher ou de masquer les filtres, les vues ou les regroupements du modèle de disposition. Les filtres visibles sont disponibles pour toutes les personnnes du système. Vous pouvez utiliser un modèle de disposition pour masquer les filtres visibles pour des personnes ou des groupes spécifiques.

>[!NOTE]
>
>Si une personne utilise activement un filtre, une vue ou un regroupement et qu’un administrateur ou une administratrice désactive l’élément, la personne conserve l’accès jusqu’à ce qu’elle choisisse un nouveau filtre, une nouvelle vue ou un nouveau regroupement. Après avoir choisi un nouveau filtre, une nouvelle vue ou un nouveau regroupement, elle ne pourra plus revenir au filtre, à la vue ou au regroupement masqué(e).

Pour afficher ou masquer les filtres, les vues ou les regroupements disponibles dans le modèle de disposition :

1. Cliquez sur **[!UICONTROL Interface]**, puis sur l’un des éléments suivants : **[!UICONTROL Filtres]**, **[!UICONTROL Vues]** ou **[!UICONTROL Regroupements]**.

1. (Le cas échéant) Sélectionnez le filtre, la vue ou le regroupement que vous souhaitez mettre à la disposition des personnes, puis cliquez sur **[!UICONTROL Activer à l’échelle du système]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Si vous souhaitez que le filtre, la vue ou le regroupement reste disponible pour la plupart des personnes, mais que l’élément soit masqué pour les autres, vous pouvez utiliser le modèle de disposition. Pour plus d’informations, voir [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Le cas échéant) Sélectionnez le filtre, la vue ou le regroupement que vous souhaitez masquer aux personnes, puis cliquez sur **[!UICONTROL Désactiver à l’échelle du système]**. Une fois la désactivation effectuée pour le filtre, la vue ou le regroupement, l’élément sera masqué dans le modèle de disposition ainsi que pour les personnes du système.


## Mettre les filtres, les vues ou les regroupements à la disposition de toutes les personnes {#make-filters-views-or-groupings-available-to-users}

Ces étapes expliquent comment mettre les filtres, les vues et les regroupements à disposition à partir de la boîte de dialogue [!UICONTROL Partager] dans la zone [!UICONTROL Interface] de [!UICONTROL Configuration]. Ce paramètre agit comme un interrupteur marche/arrêt pour l’ensemble du système, y compris le modèle de disposition.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Interface]**, puis sur l’un des éléments suivants : **[!UICONTROL Filtres]**, **[!UICONTROL Vues]** ou **[!UICONTROL Regroupements]**.

1. Sélectionnez le filtre, la vue ou le regroupement que vous souhaitez mettre à la disposition des personnes, puis cliquez sur l’icône **[!UICONTROL Partager]** ![Icône Partager](assets/share-icon.png) pour ouvrir le formulaire [!UICONTROL Accès aux filtres], [!UICONTROL Accès aux vues] ou [!UICONTROL Accès aux regroupements].
1. (Le cas échéant) Pour rendre le filtre, la vue ou le regroupement accessible à toutes les personnes du système, cliquez sur le menu déroulant en forme d’**[!UICONTROL engrenage]** ![](assets/gear-menu-for-sharing-items.png), puis cliquez sur **[!UICONTROL Rendre cet élément visible à l’échelle du système]**. Toutes les personnes du système peuvent maintenant voir le filtre, la vue ou le regroupement.

   Ou

   Commencez à taper le nom des personnes, des équipes, des rôles, des groupes ou des entreprises avec lesquels vous souhaitez partager le filtre, la vue ou le regroupement, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   Pour plus d’informations sur le partage, voir [Vue d’ensemble du partage des autorisations sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Les personnes que vous avez spécifiées peuvent désormais voir le filtre, la vue ou le regroupement par défaut lorsqu’elles consultent le type d’objet auquel vous avez associé l’élément.

## Supprimer des filtres, des vues et des regroupements

{{step-1-to-setup}}

1. Effectuez l’une des opérations suivantes, selon que vous supprimez un filtre, une vue ou un regroupement :

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Filtres]**.

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Vues]**.

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Regroupements]**.

1. Sélectionnez un ou plusieurs éléments dans la liste, puis cliquez sur l’icône **[!UICONTROL Supprimer]** ![Icône Supprimer](assets/delete.png).
1. Consultez l’un des articles suivants pour obtenir des informations détaillées sur la configuration d’un filtre, d’une vue ou d’un regroupement.

   * [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Vue d’ensemble des vues dans  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Vue d’ensemble des regroupements dans  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
