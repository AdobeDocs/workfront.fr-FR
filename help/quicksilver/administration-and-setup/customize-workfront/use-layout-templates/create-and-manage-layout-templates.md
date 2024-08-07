---
title: Créer et gérer des modèles de disposition
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: En tant qu’administrateur Workfront ou administrateur de groupe, vous pouvez créer et modifier des modèles de mise en page afin de personnaliser les éléments de mise en page dans Workfront pour vos utilisateurs.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 24%

---

# Créer et gérer des modèles de disposition

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

En tant qu’administrateur Adobe Workfront ou administrateur de groupe, vous pouvez créer et modifier des modèles de mise en page afin de personnaliser les éléments de mise en page suivants dans Workfront pour vos utilisateurs :

* Menu principal
* Panneau de navigation gauche
* Zone d’accueil
* Vues, filtres et regroupements que les utilisateurs utilisent avec des listes et des rapports.
* Terminologie à l’écran
* En-têtes de projet, de tâche et de problème

Après avoir créé ou modifié un modèle de mise en page, vous pouvez l’affecter à des utilisateurs, équipes, groupes ou rôles de tâche individuels.

La mise en page Workfront par défaut de chaque utilisateur dépend de son niveau d’accès et de son type de licence. Par exemple, certains utilisateurs peuvent ne pas voir certaines zones dans le menu principal. Pour plus d’informations, voir [À propos de la disposition Adobe Workfront par défaut](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouvelle : standard</p>
   Ou
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.</p>
<p>Pour les exécuter pour un groupe, vous devez être responsable de ce groupe.</p> <p><b>NOTE</b> :</p> <p>Si vous n’y avez pas accès, demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès.

Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

+++

## Observations relatives à la création et à la gestion des modèles de mise en page

* Les utilisateurs peuvent personnaliser quelques zones de leur propre disposition. Lorsque vous modifiez un modèle de mise en page, vos modifications fusionnent avec les personnalisations qu’elles ont effectuées, sans les remplacer ni les réinitialiser. C’est également le cas si vous affectez des utilisateurs à un nouveau modèle de mise en page.
* Les administrateurs de groupe et les utilisateurs disposant d’une licence Plan qui peuvent modifier d’autres utilisateurs peuvent ajouter des modèles de mise en page au niveau du système et du groupe aux utilisateurs qu’ils peuvent gérer lors de la modification de leur profil.
* Les administrateurs de groupe ne peuvent pas affecter de modèles de mise en page à des rôles de tâche ou à des équipes.

Pour plus d’informations sur les modèles de mise en page, voir [Modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Création ou modification d’un modèle de mise en page

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Interface** > **Modèles de mise en page**.

1. Cliquez sur **Nouveau modèle de mise en page**.

   Ou

   Cliquez sur le nom du modèle de mise en page que vous souhaitez modifier.

1. Si vous créez un modèle de mise en page, saisissez un **nom de modèle de mise en page** et (facultatif) une **description** correspondant.

1. Personnalisez des zones de l’interface utilisateur, comme décrit dans les articles suivants :

   * [Personnaliser le menu principal à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personnaliser le panneau de gauche à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personnaliser les pages épinglées à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personnaliser la vue Détails à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personnaliser l’accueil et le résumé à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personnaliser la page de destination à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personnalisation de la terminologie de l’interface utilisateur à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continuez à tester votre modèle de mise en page et rendez-le disponible pour les utilisateurs, comme décrit dans les articles ci-dessous :

   * [Tester un nouveau modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Octroyer un accès d’administration à un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Affecter des utilisateurs à un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Vous pouvez également créer un modèle de mise en page en le copiant et en modifiant la copie. Pour plus d’informations, voir [Copier un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

