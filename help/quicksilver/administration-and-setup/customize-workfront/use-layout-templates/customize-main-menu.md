---
title: Personnalisation du menu principal à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Adobe Workfront ou de groupes, vous pouvez utiliser un modèle de mise en page pour configurer les options que les personnes voient lorsqu’elles ouvrent le menu principal dans Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 4fdfa1107034a48e149a5414475fbc0d7ce97564
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 62%

---

# Personnaliser le menu principal à l’aide d’un modèle de mise en page

{{preview-fast-release-general}}

<!--Audited: 01/2024-->

En tant qu’administrateur ou administratrice Adobe Workfront ou de groupes, vous pouvez utiliser un modèle de mise en page pour configurer les options que les personnes voient lorsqu’elles ouvrent le menu principal dans Workfront.

>[!NOTE]
>
>Les options du menu principal que les personnes voient dépendent de leur type de licence et des paramètres configurés à leur niveau d’accès. Certaines personnes qui utiliseront ce modèle de mise en page ne verront peut-être pas toutes les options que vous choisissez ici. Pour plus d’informations, voir [Fonctionnement des niveaux d’accès et des autorisations](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) et [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Il se peut que différentes options s’affichent dans le menu principal si votre organisation a été intégrée à l’expérience unifiée Adobe Workfront. Pour plus d’informations, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Pour plus d’informations sur la création de modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Créer et modifier des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de mise en page à des utilisateurs et utilisatrices, voir [Attribuer un modèle de mise en page à des utilisateurs et utilisatrices](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p>
       <p>L’ajout d’applications personnalisées au menu principal n’est disponible que pour les organisations sous licence Adobe App Builder.</p></td> 
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

## Personnaliser le menu principal

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur **Définir le menu principal** dans le coin supérieur droit du modèle.

   La boîte de dialogue Menu principal s’ouvre. Vous pouvez y voir les zones qui s’affichent actuellement dans le menu principal pour le modèle, ainsi que les éléments disponibles à ajouter. Vous trouverez ci-dessous tous les éléments que vous pouvez ajouter :
   * Page d’accueil

     >[!TIP]
     >
     >Par défaut, l’icône Accueil du menu principal affiche la zone Mes mises à jour pour les utilisateurs disposant d’une licence de révision (dans le plan de licence actuel), à moins qu’ils n’aient un modèle de mise en page associé à leur profil qui inclut la zone Mes mises à jour du menu principal, en plus de la zone Accueil .


   * <span class="preview"> Priorités </span>
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
     >Planning requiert une licence supplémentaire. Pour plus d’informations sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

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

1. <span class="preview">Dans l’environnement Aperçu : continuez à personnaliser le modèle de mise en page. Vous pouvez cliquer sur **Appliquer** à tout moment pour enregistrer votre progression.</span>

   <span class="preview">Ou</span>

   <span class="preview">Si vous avez terminé la personnalisation, cliquez sur **Enregistrer et fermer**.</span>

1. Dans l’environnement de production : continuez à personnaliser le modèle de disposition.

   Ou

   Si vous avez terminé la personnalisation, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer sur **Enregistrer** à tout moment pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.

Pour plus d’informations sur les modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
