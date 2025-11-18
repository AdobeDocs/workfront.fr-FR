---
title: Personnalisation de la page d’entrée à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Workfront, vous pouvez utiliser un modèle de mise en page pour spécifier la zone que les utilisateurs et utilisatrices doivent voir chaque fois qu’ils se connectent à Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 57a1046a-434a-4453-a101-c5f0a16e079e
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 78%

---

# Personnaliser la page de destination à l’aide d’un modèle de mise en page

{{preview-fast-release-general}}

En tant qu’administrateur ou administratrice Workfront, vous pouvez utiliser un modèle de mise en page pour spécifier la zone que les utilisateurs et utilisatrices doivent voir chaque fois qu’ils se connectent à Workfront.

Les utilisateurs peuvent ouvrir l’un des fichiers suivants :

* Une zone Workfront désignée
* d’un tableau de bord personnalisé.

Pour plus d’informations sur la création de modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Créer et modifier des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de mise en page à des utilisateurs et utilisatrices, voir [Attribuer un modèle de mise en page à des utilisateurs et utilisatrices](../use-layout-templates/assign-users-to-layout-template.md).

>[!NOTE]
>
>Lorsque Requêtes est défini comme page de destination, les contributeurs et contributrices, ou demandeurs et demandeuses, affectés au modèle de mise en page voient la page d’accueil comme page de destination à la place. Il est recommandé de choisir une page de destination autre que Requêtes pour les modèles de mise en page destinés aux contributeurs et contributrices, ou demandeurs et demandeuses.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
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

## Personnaliser la page de destination

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Dans le **zone de navigation supérieure**, cliquez sur **Sélectionner une page de destination**, puis sélectionnez la zone que les utilisateurs et utilisatrices doivent voir lorsqu’ils se connectent.

   Sélectionnez l’une des zones suivantes ou ajoutez un tableau de bord personnalisé :

   * Calendriers
   * Tableaux de bord
   * Documents
   * Objectifs
   * Page d’accueil
   * Mes mises à jour
   * Portefeuilles
   * Programmes
   * Projets
   * Rapports
   * Demandes
   * Ressources
   * Scénarios
   * Équipes
   * Modèles
   * Feuilles de temps
   * Utilisateurs
   * Plans directeurs
   * Planification

   >[!IMPORTANT]
   >
   >L’affichage des zones Scénarios, Objectifs et Planification nécessite des licences supplémentaires.
   >
   >* Pour plus d’informations sur les Objectifs Workfront, voir [Vue d’ensemble des Objectifs Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).
   >
   >* Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).
   >
   >* Pour plus d’informations sur Workfront Planning, consultez [Prise en main de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

1. <span class="preview">Dans l’environnement d’aperçu : Poursuivez la personnalisation du modèle de mise en page. Vous pouvez cliquer sur **Appliquer** à tout moment pour enregistrer votre progression.</span>

   <span class="preview">Ou</span>

   <span class="preview">Si vous avez terminé la personnalisation, cliquez sur **Enregistrer et fermer**.</span>

1. Dans l’environnement de production : Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé la personnalisation, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer sur **Enregistrer** à tout moment pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
