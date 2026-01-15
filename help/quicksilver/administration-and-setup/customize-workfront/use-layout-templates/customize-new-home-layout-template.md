---
title: Personnalisation de l’accueil à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Vous pouvez utiliser un modèle de mise en page pour configurer ce que les utilisateurs voient lorsqu’ils ouvrent l’Accueil dans Adobe Workfront.
author: Lisa and Courtney
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 35%

---

# Personnaliser l’accueil à l’aide d’un modèle de disposition

Vous pouvez utiliser un modèle de mise en page pour configurer ce que les utilisateurs voient lorsqu’ils ouvrent la page d’accueil pour la première fois.

Vous pouvez configurer les éléments suivants :

* Les widgets qui s’affichent par défaut dans l’espace de travail
* L’arrière-plan sélectionné.
* Les paramètres de widget spécifiques, notamment les filtres et les groupes disponibles pour les widgets Mes projets, Mes tâches et Mes problèmes, ainsi que leurs paramètres par défaut.

>[!IMPORTANT]
>
>Les utilisateurs finaux peuvent modifier leur arrière-plan et réorganiser les widgets sur la page une fois le modèle de mise en page appliqué. Ils ne peuvent pas supprimer les widgets inclus par un administrateur Workfront.
> 
>Les administrateurs ont la possibilité d’ajouter de nouveaux widgets pour les utilisateurs. Cependant, si un utilisateur final a déjà personnalisé son ordre de widget ou sa sélection d’arrière-plan, ces personnalisations spécifiques ne sont pas modifiées.

Pour plus d’informations sur l’Accueil, voir [Prise en main de l’Accueil](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

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

## Personnaliser l’accueil à l’aide d’un modèle de disposition

Pour personnaliser l’Accueil à l’aide d’un modèle de mise en page :

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Cliquez sur la flèche vers le bas ![Flèche vers le bas](assets/dropdown-arrow.png) sous **Personnaliser ce que voient les utilisateurs**, puis cliquez sur **Workspace d’accueil**.

1. Dans les onglets de droite, cliquez sur l’un des éléments suivants :

   * **Conception et disposition** : sélectionnez cette option pour choisir et organiser les widgets et l’arrière-plan
   * **Paramètres de widget** : sélectionnez cette option pour gérer les paramètres des widgets individuels, tels que les filtres et les groupes disponibles.

   Le tableau suivant contient des détails sur chaque onglet :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Conception et disposition</td> 
      <td>
      <p>Sélectionnez les widgets qui s’afficheront dans les espaces de travail des utilisateurs, leur position et choisissez un arrière-plan.</p> 
      <p>Notez que bien que les utilisateurs ne puissent pas supprimer les widgets sélectionnés, ils peuvent les déplacer et les redimensionner librement. Ils peuvent également ajouter d’autres widgets.</p>
      <p>Cet onglet fonctionne essentiellement comme un aperçu de l’espace de travail réel de l’accueil que les utilisateurs et utilisatrices disposant de ce modèle de mise en page rencontreront.</p> 
      <p> Effectuez l’une des opérations suivantes : </p>
      <ul><li>Personnalisez cet onglet en fonction des étapes décrites dans <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Ajouter, modifier ou supprimer des widgets dans l’Accueil</a>. </li>
      <li>Sélectionnez des widgets et organisez l’espace de travail comme vous le souhaitez pour les utilisateurs et utilisatrices.</li>
      <li>Pour modifier l’arrière-plan, suivez les étapes décrites sous <b>Personnalisation de l’arrière-plan</b> dans <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Prise en main de l’Accueil</a>.</li></p>
      <p>

   >[!NOTE]
   >
   >Seul le déplacement ou le redimensionnement de widgets dans le modèle de mise en page ne déclenche pas la mise à jour de la disposition des pages d’accueil des utilisateurs. Cependant, l’ajout ou la suppression d’un widget déclenche une mise à jour des pages des utilisateurs et utilisatrices.

   </p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Paramètres du widget</td> 
      <td>
      <p>Modifier les paramètres de widgets individuels</p> 
      <p>

   >[!NOTE]
   >
   >Ces options ne s’étendent pas au panneau Résumé . Vous devez configurer cette zone dans l’onglet Résumé du modèle de mise en page.

   </p>
      <p> Sélectionnez l’un des widgets suivants dans la liste à gauche :</p>
      <ul>
        <li>Mes projets</li>
        <li>Mes tâches</li>
        <li>Mes problèmes</li>
      </ul>
      <p>Après avoir sélectionné le widget que vous souhaitez modifier, sélectionnez les <b>Filtres</b>, <b>Colonnes</b> et <b>Groupes</b> que vous souhaitez rendre disponibles pour l’Accueil sur la droite.</p>
      <p> Vous pouvez :</p>
      <ul>
      <li><p>Sélectionnez et classez les filtres, colonnes ou groupes disponibles pour les utilisateurs en cochant la case en regard des options de la liste. Les options non cochées ne s’affichent pas pour les utilisateurs et utilisatrices.</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* Les options Filtre, Colonnes et Groupe sont liées aux options de personnalisation de la liste dans le modèle de mise en page. Les modifications apportées ici s’appliqueront également à ces paramètres.
   >* Les utilisateurs doivent au moins disposer d’un accès de type Créer aux vues pour que la configuration des colonnes de l’administrateur s’applique correctement à leurs pages d’accueil.
   ></p>
   >   <li><p>Définissez un filtre ou un groupe par défaut pour le widget, en pointant sur une option et en cliquant sur <b>Définir comme valeur par défaut</b>. La valeur par défaut actuelle affiche un badge bleu <b>Default</b> à sa droite.</p></li>
   >   <li><p>Ajoutez un filtre, une colonne ou un groupe existant à la liste des options disponibles en cliquant sur le bouton représentant un signe plus au bas de chaque liste pour ajouter une option à cette liste. Notez que seuls les filtres, champs (pour les colonnes) ou groupes existants peuvent être ajoutés de cette manière.</p></li>
   >   </ul>
   >   <p>

   >[!NOTE]
   >
   >Si vous définissez un filtre ou un regroupement par défaut pour un widget spécifique à l’aide d’un modèle de mise en page, il se peut qu’il ne prenne pas effet immédiatement en raison des préférences existantes de la personne. Pour appliquer immédiatement le nouveau filtre ou regroupement, vous ou la personne concernée devrez peut-être réinitialiser ses préférences en ajoutant « /resetUser » à la fin de l’URL.

   </p>
      </td> 
      </tr>
      </tbody> 
      </table>

1. Continuez à personnaliser le modèle de mise en page. Vous pouvez cliquer sur **Appliquer** à tout moment pour enregistrer votre progression.

   Ou

   Si vous avez terminé la personnalisation, cliquez sur **Enregistrer et fermer**.

   >[!IMPORTANT]
   >
   >Les utilisateurs doivent actualiser leur page d’accueil pour afficher les personnalisations à partir du modèle de mise en page.
