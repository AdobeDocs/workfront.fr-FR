---
title: Créer et gérer des modèles de mise en page
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Workfront ou administrateur ou administratrice de groupes, vous pouvez créer et modifier des modèles de mise en page pour personnaliser les éléments de mise en page dans Workfront pour vos utilisateurs et utilisatrices.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 94%

---

# Créer et gérer des modèles de mise en page

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

En tant qu’administrateur ou administratrice Adobe Workfront ou administrateur ou administratrice de groupes, vous pouvez créer et modifier des modèles de mise en page pour personnaliser les éléments de disposition suivants dans Workfront pour vos utilisateurs et utilisatrices :

* Menu principal
* Panneau de navigation de gauche
* Zone d’accueil
* Panneau Résumé
* Vues, filtres et regroupements que les personnes utilisent avec les listes et les rapports.
* Terminologie à l’écran
* En-têtes pour les projets, tâches et problèmes

Après avoir créé ou modifié un modèle de mise en page, vous pouvez l’affecter à des utilisateurs et utilisatrices individuels, à des équipes, à des groupes ou à des fonctions.

La disposition par défaut de Workfront de chaque personne dépend de son niveau d’accès et de son type de licence. Par exemple, certaines personnes peuvent ne pas voir certaines zones du menu principal. Pour plus d’informations, voir [À propos de la disposition par défaut d’Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.</p>
        <p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à la création et à la gestion des modèles de mise en page

* Les utilisateurs et utilisatrices peuvent personnaliser quelques zones de leur propre disposition. Lorsque vous modifiez un modèle de mise en page, vos modifications s’intègrent à toutes les personnalisations effectuées, sans les écraser ni les réinitialiser. Il en va de même si vous attribuez un nouveau modèle de mise en page à des utilisateurs ou utilisatrices.
* Les administrateurs et administratrices de groupes et les personnes disposant d’une licence Plan qui peuvent modifier d’autres utilisateurs et utilisatrices peuvent ajouter des modèles de mise en page au niveau du système et du groupe aux personnes qu’ils peuvent gérer lorsqu’ils modifient leur profil.
* Les administrateurs et administratrices de groupes ne peuvent pas attribuer de modèles de mise en page à des fonctions ou à des équipes.

Pour plus d’informations sur les modèles de mise en page, voir [Modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Créer ou modifier un modèle de mise en page

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Interface** > **Modèles de mise en page**.

1. Cliquez sur **Nouveau modèle de mise en page**.

   Ou

   Cliquez sur le nom du modèle de mise en page que vous souhaitez modifier.

1. Si vous créez un nouveau modèle de mise en page, saisissez le **nom du modèle de mise en page** et (facultatif) sa **description**.

1. Personnalisez des zones de l’interface d’utilisation, tel que décrit dans les articles suivants :

   * [Personnaliser le menu principal à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personnaliser les pages épinglées à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personnaliser la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personnalisation du panneau Résumé à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personnaliser l’accueil à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   * [Personnaliser la page de destination à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personnaliser la terminologie de l’interface d’utilisation à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continuez à tester votre modèle de mise en page et mettez-le à la disposition des personnes, comme décrit dans les articles ci-dessous :

   * [Tester un nouveau modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Accorder un accès administratif pour un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Affecter des utilisateurs et utilisatrices à un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Vous pouvez également créer un modèle de mise en page en le copiant et en modifiant la copie. Pour plus d’informations, voir [Copier un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

