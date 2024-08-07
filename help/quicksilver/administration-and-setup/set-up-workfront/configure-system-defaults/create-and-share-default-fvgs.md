---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Créer, modifier et partager des filtres, vues et groupes par défaut
description: Vous pouvez créer des filtres, des vues et des regroupements par défaut, puis les rendre disponibles pour les utilisateurs de votre entreprise.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 8%

---

# Créer, modifier et partager des filtres, vues et groupes par défaut

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Vous pouvez créer des filtres, des vues et des regroupements par défaut, puis les rendre disponibles pour les utilisateurs de votre entreprise.

Lorsque vous créez des filtres, des vues et des regroupements par défaut comme décrit dans cet article, les utilisateurs avec qui vous les partagez peuvent les exploiter lors de l’affichage de leurs listes. Les utilisateurs peuvent créer leurs propres filtres, vues et regroupements en fonction de ceux que vous créez, mais ils ne peuvent pas modifier directement ceux que vous créez.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Créer des filtres, des vues ou des regroupements par défaut

{{step-1-to-setup}}

1. Effectuez l’une des opérations suivantes, selon que vous créez ou modifiez un filtre, une vue ou un regroupement :

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Filtres]**.

   * Cliquez sur **[!UICONTROL Interface] >** **[!UICONTROL Vues]**.

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**.

1. Si vous créez un filtre, une vue ou un groupement, cliquez sur **[!UICONTROL Ajouter un filtre]**, **[!UICONTROL Ajouter une vue]** ou **[!UICONTROL Ajouter un groupement]**, puis sélectionnez le type d&#39;objet auquel vous souhaitez associer le nouveau filtre, la nouvelle vue ou le nouveau regroupement.

   Ou

   Si vous modifiez un filtre, une vue ou un groupement existant, sélectionnez-le, puis cliquez sur l’icône **[!UICONTROL Modifier]** ![Icône Modifier](assets/edit-icon.png).

1. Configurez le filtre, l’affichage ou le regroupement.

   Pour plus d’informations sur les options disponibles, voir l’un des articles suivants :

   * [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Présentation des vues dans [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Présentation des regroupements dans [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche.

Vous pouvez rendre le filtre, l’affichage ou le regroupement disponibles pour les utilisateurs de votre système. Pour plus d’informations sur le partage de filtres, vues ou regroupements avec d’autres utilisateurs, consultez la section [ Mise à disposition de filtres, vues ou regroupements pour les utilisateurs](#make-filters-views-or-groupings-available-to-users) de cet article.


## Afficher ou masquer les filtres, les vues ou les regroupements disponibles à partir du modèle de mise en page

Vous pouvez choisir d’afficher ou de masquer des filtres, des vues ou des groupements à partir du modèle de mise en page. Les filtres visibles sont disponibles pour tous les utilisateurs à l’échelle du système. Vous pouvez utiliser un modèle de mise en page pour masquer les filtres visibles pour des utilisateurs ou des groupes spécifiques.

>[!NOTE]
>
>Si un utilisateur utilise activement un filtre, une vue ou un groupement, puis qu’un administrateur le désactive, il a toujours accès jusqu’à ce qu’il choisisse un nouveau filtre, une nouvelle vue ou un nouveau regroupement. Après avoir choisi un nouveau filtre, une nouvelle vue ou un nouveau regroupement, ils ne pourront plus revenir au filtre masqué, à la vue ou au regroupement.

Pour afficher ou masquer les filtres, les vues ou les regroupements disponibles à partir du modèle de mise en page :

1. Cliquez sur **[!UICONTROL Interface]**, puis sur l’une des options suivantes : **[!UICONTROL Filtres]**, **[!UICONTROL Vues]** ou **[!UICONTROL Groupes]**.

1. (Conditionnel) Sélectionnez le filtre, l’affichage ou le regroupement que vous souhaitez rendre disponible pour les utilisateurs, puis cliquez sur **[!UICONTROL Activer à l’échelle du système]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Si vous souhaitez que le filtre, l’affichage ou le regroupement reste disponible pour la plupart des utilisateurs, mais que vous le masquez pour d’autres utilisateurs, vous pouvez utiliser le modèle de mise en page. Pour plus d’informations, voir [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Conditionnel) Sélectionnez le filtre, l’affichage ou le regroupement à masquer aux utilisateurs, puis cliquez sur **[!UICONTROL Désactiver à l’échelle du système]**. Une fois désactivé, le filtre, la vue ou le regroupement sont masqués dans le modèle de mise en page ainsi que dans les utilisateurs du système.


## Mettre les filtres, vues ou groupes à la disposition de tous les utilisateurs {#make-filters-views-or-groupings-available-to-users}

Ces étapes expliquent comment rendre des filtres, des vues et des regroupements disponibles à partir de la boîte de dialogue [!UICONTROL Partager] dans la zone [!UICONTROL Interface] de [!UICONTROL Configuration]. Ce paramètre fonctionne comme un commutateur activé/désactivé pour l’ensemble du système, y compris le modèle de mise en page.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Interface]**, puis sur l’une des options suivantes : **[!UICONTROL Filtres]**, **[!UICONTROL Vues]** ou **[!UICONTROL Groupes]**.

1. Sélectionnez le filtre, l’affichage ou le regroupement que vous souhaitez mettre à la disposition des utilisateurs, puis cliquez sur l’icône **[!UICONTROL Partager]** ![Icône Partager](assets/share-icon.png) pour ouvrir le formulaire [!UICONTROL Accès aux filtres], [!UICONTROL Accès aux vues] ou [!UICONTROL Accès aux groupes].
1. (Conditionnel) Pour rendre le filtre, l’affichage ou le regroupement disponible pour tous les utilisateurs du système, cliquez sur le menu déroulant **[!UICONTROL Gear]** ![](assets/gear-menu-for-sharing-items.png), puis cliquez sur **[!UICONTROL Rendre ce filtre visible à l’échelle du système]**. Tous les utilisateurs du système peuvent désormais afficher le filtre, l’affichage ou le regroupement.

   Ou

   Commencez à saisir le nom d’utilisateurs, d’équipes, de rôles, de groupes ou d’entreprises spécifiques avec lesquels partager le filtre, l’affichage ou le regroupement, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   Pour plus d’informations sur le partage, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Les utilisateurs que vous avez spécifiés peuvent désormais afficher le filtre, l’affichage ou le regroupement par défaut lors de l’affichage du type d’objet auquel vous l’avez associé.

## Supprimer des filtres, des vues et des regroupements

{{step-1-to-setup}}

1. Effectuez l’une des opérations suivantes, selon que vous supprimez un filtre, une vue ou un regroupement :

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Filtres]**

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Vues]**

   * Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**

1. Sélectionnez un ou plusieurs éléments dans la liste, puis cliquez sur l’icône **[!UICONTROL Supprimer]** ![Icône Supprimer](assets/delete.png).
1. Consultez l’un des articles suivants pour plus d’informations sur la configuration d’un filtre, d’une vue ou d’un regroupement.

   * [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Présentation des vues dans [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Présentation des regroupements dans [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
