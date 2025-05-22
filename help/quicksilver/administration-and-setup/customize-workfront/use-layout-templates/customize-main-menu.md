---
title: Personnalisation du menu principal à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Adobe Workfront ou de groupes, vous pouvez utiliser un modèle de disposition pour configurer les options que les personnes voient lorsqu’elles ouvrent le menu principal dans Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 7640016921e421d2aec0ab1aadc0edd304125feb
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 68%

---

# Personnaliser le menu principal avec des modèles de disposition

<!--Audited: 01/2024-->

En tant qu’administrateur ou administratrice Adobe Workfront ou de groupes, vous pouvez utiliser un modèle de disposition pour configurer les options que les personnes voient lorsqu’elles ouvrent le menu principal dans Workfront.

![Options du menu principal](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>Les options du menu principal que les personnes voient dépendent de leur type de licence et des paramètres configurés à leur niveau d’accès. Certaines personnes qui utiliseront ce modèle de disposition ne verront peut-être pas toutes les options que vous choisissez ici. Pour plus d’informations, voir [Fonctionnement des niveaux d’accès et des autorisations](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) et [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Il se peut que différentes options s’affichent dans le menu principal si votre organisation a été intégrée à l’expérience unifiée Adobe Workfront. Pour plus d’informations, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Pour plus d’informations sur la création de modèles de disposition, voir [Créer et gérer des modèles de disposition](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de disposition aux utilisateurs et utilisatrices, voir [Affecter des utilisateurs et utilisatrices à un modèle de disposition](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront</strong></td> 
   <td><p>Tous</p>

<p>L’ajout d’applications personnalisées au menu principal n’est disponible que pour les organisations sous licence Adobe App Builder.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td><p>Actuel : formule</p>
   Ou
   <p>Nouveau : Standard</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.</p>
    <p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser le menu principal

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur **Définir le menu principal** dans le coin supérieur droit du modèle.

   La boîte de dialogue Menu principal s’ouvre. Vous pouvez y voir les zones qui s’affichent actuellement dans le menu principal pour le modèle, ainsi que les éléments disponibles à ajouter. Vous trouverez ci-dessous tous les éléments que vous pouvez ajouter :
   * Page d’accueil

     >[!TIP]
     >
     >Par défaut, l’icône Accueil du menu principal affiche la zone Mes mises à jour pour les utilisateurs disposant d’une licence de révision (dans le plan de licence actuel), à moins qu’ils n’aient un modèle de mise en page associé à leur profil qui inclut la zone Mes mises à jour du menu principal, en plus de la zone Accueil .

   * Portefeuilles
   * Programmes
   * Projets
   * Rapports
   * Tableaux de bord
   * Calendriers
   * Ressources
   * Scénarios

     >[!NOTE]
     >
     >Le planificateur de scénarios nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

   * Équipes
   * Utilisateurs

     >[!NOTE]
     >
     >Seuls les utilisateurs disposant d&#39;une licence de plan (dans le modèle de licence actuel) ou d&#39;une licence standard (dans le nouveau modèle de licence) peuvent voir la zone Utilisateurs ![icône Utilisateurs](assets/users-icon-in-main-menu.png) dans le menu principal.

   * Demandes
   * Feuilles de temps
   * Documents
   * Modèles
   * Analytique
   * Relecture
   * Objectifs

     >[!NOTE]
     >
     >La solutoin Objectifs nécessite une licence supplémentaire. Pour plus d’informations sur Objectifs Workfront, voir [Vue d’ensemble d’Objectifs Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Mes mises à jour
   * Panneaux
   * Plans directeurs
   * Planification

     >[!NOTE]
     >
     >Planning requiert une licence supplémentaire. Pour plus d’informations sur Workfront Planning, consultez la [Présentation d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
      * Application personnalisée

     >[!NOTE]
     >
     > Les applications personnalisées doivent être créées séparément avant d&#39;être disponibles en tant qu&#39;options du menu principal. Pour plus d’informations, voir [Création d’une application personnalisée pour Workfront avec Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).


1. Effectuez l’une des opérations suivantes :

   * Masquez ![Icône Masquer](assets/remove-icon---x-in-circle.png) **Éléments actifs** que vous ne souhaitez pas afficher
   * Afficher ![Afficher l&#39;icône](assets/add-icon-plus-in-circle.png) **Éléments disponibles** à afficher dans le menu principal.
   * Faites glisser ![Icône Faire glisser](assets/move-icon---dots.png) **Éléments actifs** pour modifier leur ordre d&#39;affichage dans le menu principal.

1. Cliquez sur **Terminé**.

   Cliquez également sur **Annuler** à tout moment si vous souhaitez ignorer vos modifications.

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur Enregistrer pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.

Pour plus d’informations sur les modèles de disposition, voir [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
