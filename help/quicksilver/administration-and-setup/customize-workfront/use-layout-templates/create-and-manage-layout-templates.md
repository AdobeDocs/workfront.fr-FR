---
title: Création et gestion des modèles de mise en page
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: En tant qu’administrateur Workfront ou administrateur de groupe, vous pouvez créer et modifier des modèles de mise en page afin de personnaliser les éléments de mise en page dans Workfront pour vos utilisateurs.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Création et gestion des modèles de mise en page

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

En tant qu’administrateur Workfront ou administrateur de groupe, vous pouvez créer et modifier des modèles de mise en page afin de personnaliser les éléments de mise en page suivants dans Workfront pour vos utilisateurs :

* Menu principal
* Panneau de navigation gauche
* Zone d’accueil
* Vues, filtres et regroupements que les utilisateurs utilisent avec des listes et des rapports.
* Terminologie à l’écran

Après avoir créé ou modifié un modèle de mise en page, vous pouvez l’affecter à des utilisateurs, équipes, groupes ou rôles de tâche individuels.

La mise en page Workfront par défaut de chaque utilisateur dépend de son niveau d’accès et de son type de licence. Par exemple, certains utilisateurs peuvent ne pas voir certaines zones dans le menu principal. Pour plus d’informations, voir [A propos de la disposition Adobe Workfront par défaut](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.
Pour les exécuter pour un groupe, vous devez être un responsable de ce groupe.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Observations relatives à la création et à la gestion des modèles de mise en page

* Les utilisateurs peuvent personnaliser quelques zones de leur propre disposition. Lorsque vous modifiez un modèle de mise en page, vos modifications fusionnent avec les personnalisations qu’elles ont effectuées, sans les remplacer ni les réinitialiser. C’est également le cas si vous affectez des utilisateurs à un nouveau modèle de mise en page.
* Les anciens modèles de mise en page créés dans Adobe Workfront Classic sont automatiquement disponibles dans votre instance de la nouvelle expérience Adobe Workfront depuis leur migration début à l’automne 2019. Les modèles de mise en page créés dans Adobe Workfront Classic après cette période ont été migrés en avril 2020. Nous vous recommandons de mettre à jour ces modèles de mise en page dans la nouvelle expérience Adobe Workfront afin de profiter des nouvelles fonctionnalités et de les rendre encore plus utiles dans cet environnement.
* Les administrateurs de groupe et les utilisateurs disposant d’une licence Plan qui peuvent modifier d’autres utilisateurs peuvent ajouter des modèles de mise en page au niveau du système et du groupe aux utilisateurs qu’ils peuvent gérer lors de la modification de leur profil.
* Les administrateurs de groupe ne peuvent pas affecter de modèles de mise en page à des rôles de tâche ou à des équipes.

Pour plus d’informations sur les modèles de mise en page, voir [Modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Création ou modification d’un modèle de mise en page

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Interface** > **Modèles de mise en page**.

1. Cliquez sur **Nouveau modèle de mise en page**.

   Ou

   Cliquez sur le nom du modèle de mise en page que vous souhaitez modifier.

1. Si vous créez un modèle de mise en page, saisissez une **Nom du modèle de mise en page** et (facultatif) a **Description** pour cela.

1. Personnalisez les zones de l’interface utilisateur, comme décrit dans les articles suivants :

   * [Personnalisation du menu principal à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personnalisation des pages épinglées à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personnaliser la landing page à l&#39;aide d&#39;un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personnalisation de la terminologie de l’interface utilisateur à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Passez à l’étape de test de votre modèle de mise en page et rendez-le disponible pour les utilisateurs, comme décrit dans les articles ci-dessous :

   * [Test d’un nouveau modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Octroi d’un accès administratif pour un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Affecter des utilisateurs à un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

Vous pouvez également créer un modèle de mise en page en le copiant et en modifiant la copie. Pour plus d’informations, voir [Copier un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
