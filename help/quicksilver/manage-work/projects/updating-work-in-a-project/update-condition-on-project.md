---
product-area: projects
navigation-topic: update-work-in-a-project
title: Condition de mise à jour d’un projet
description: La condition d’un projet est un indicateur qui indique si le travail qui y est associé se déroule sans problème ou si vous avez rencontré des obstacles. Ceci est différent de l’état du projet, qui indique si vous y travaillez activement ou non.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Condition de mise à jour d’un projet

La condition d’un projet est un indicateur qui indique si le travail qui y est associé se déroule sans problème ou si vous avez rencontré des obstacles. Ceci est différent de l’état du projet, qui indique si vous y travaillez activement ou non.

Vous pouvez définir la condition d’un projet automatiquement ou manuellement. Pour modifier manuellement la condition d’un projet, vous devez être le propriétaire du projet ou disposer des droits de gestion.

L’administrateur d’Adobe Workfront peut créer des conditions personnalisées pour votre environnement, comme décrit dans la section [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>

Pour les nouvelles licences :
<p>Standard</p>

Pour les licences actuelles :
<ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Affichage ou accès supérieur aux projets</p> <p>Modifier l’accès aux tâches et aux problèmes </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures sur des tâches et des problèmes pour afficher leur condition</p>
   <p>Gérer les autorisations sur les tâches et les problèmes pour mettre à jour la condition</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Définition automatique de la condition

La définition automatique de la condition d’un projet est déterminée par le type de condition du projet. Le type de condition doit être défini sur État de progression pour que Workfront définisse automatiquement la condition du projet.

L’administrateur Workfront ou Group détermine la valeur par défaut du champ Type de condition pour les nouveaux projets de votre système lors de la définition des préférences du projet dans la zone Configuration. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Lorsque vous créez un projet, la condition du projet est automatiquement définie pour correspondre à l’état de progression du projet à ce moment-là. L’état d’avancement du projet est basé sur l’état d’avancement des tâches sur le projet.

Pour plus d’informations sur les conditions du projet et leur calcul en fonction de l’état de progression, voir [État d’avancement du projet - Aperçu](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Mettre à jour manuellement la condition d’un projet

Si vous définissez le type de condition de votre projet sur Manuel au lieu de État de progression, vous pouvez mettre à jour manuellement la condition d’un projet.

1. Accédez au projet pour lequel vous souhaitez mettre à jour la condition.
1. Cliquez sur le bouton **Détails du projet** dans le panneau de gauche.

1. Assurez-vous que la variable **Type de condition** est défini sur **Manuel**.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Dans le **Condition** , sélectionnez parmi les options suivantes celle qui correspond à votre compréhension du bon déroulement du travail ou des retards :

   * **Sur Target**
   * **À risque**
   * **En difficulté**

   Pour plus d’informations sur les conditions du projet, voir [Présentation de la condition et du type de condition du projet](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Les conditions peuvent être personnalisées pour votre environnement. Vous pouvez donc trouver plus de trois options pour Condition dans votre environnement. Les noms des Conditions peuvent être différents de ceux répertoriés ci-dessus. Pour plus d’informations sur la personnalisation des conditions dans Workfront, voir [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Cliquez sur **Enregistrer les modifications**.
