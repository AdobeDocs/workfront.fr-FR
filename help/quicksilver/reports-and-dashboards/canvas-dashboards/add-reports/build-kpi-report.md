---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Créer un rapport sur les indicateurs de performance clés
description: Un rapport sur les indicateurs de performance clés qui affiche de manière bien visible un indicateur de performance clé agrégé unique peut être ajouté à un tableau de bord de zone de travail.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: 981d86fa7d54d9d26c0a2b6142db98d5989cbed2
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 9%

---

# Créer un rapport sur les indicateurs de performance clés

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Pour plus d’informations, voir [Informations bêta sur les tableaux de bord de la zone de travail](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Vous pouvez créer et ajouter un rapport sur les indicateurs de performance clés à un tableau de bord de la zone de travail, qui représente visuellement les données de vos indicateurs clés de performance sous la forme d’un nombre, que vous pouvez ensuite utiliser pour voir comment se portent vos projets et vos équipes.

![Exemple de rapport sur les KPI](assets/kpi-example-main.png)

+++ Développez pour afficher les exigences d’accès.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront</p></td> 
   <td> 
<p>Tous </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Actuelle : formule </p> 
<p>Nouveau : Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p>
  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Vous devez créer un tableau de bord avant de pouvoir créer un rapport sur les indicateurs de performance clés.

## Créer un rapport de KPI dans un tableau de bord de zones de travail

De nombreuses options de configuration sont disponibles pour créer un rapport sur les indicateurs de performance clés. Dans cette section, nous vous guiderons à travers le processus général de création d’un rapport.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Cliquez sur **Nouveau tableau de bord** dans le coin supérieur droit.

1. Dans la zone **Créer un tableau de bord**, saisissez les **Nom** et **Description** du tableau de bord.

1. Cliquez sur **Créer**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **KPI**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez un rapport **Nom**.
   1. Saisissez un état **Description**.

      >[!NOTE]
      >
      >La description sera utilisée comme légende sous la valeur de l’indicateur de performance clé. Si vous ne saisissez pas de description, une légende est générée pour vous en fonction de l’agrégateur et du type d’agrégation que vous sélectionnez dans les étapes suivantes.

1. Suivez les étapes ci-dessous pour configurer la section **Créer un KPI** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un indicateur de performance clé** ![Créer un indicateur de performance clé](assets/build-kpi-icon.png).

   1. Cliquez sur **Sélectionner un champ** puis spécifiez le champ que vous souhaitez ajouter au rapport.

   1. Dans le menu déroulant **Type d’agrégation**, sélectionnez la manière dont les données sont cumulées pour produire la sortie d’indicateurs de performance clés. Les options de ce champ varient en fonction du type de champ sélectionné à l’étape précédente.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre.

   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres des colonnes d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes d’analyse** ![Icône Colonnes d’analyse](assets/drilldown-column.png). Les champs de votre graphique s’affichent automatiquement sous forme de colonnes dans la section de prévisualisation à droite.

   1. (Facultatif) Pour mettre à jour l’une des configurations de colonne existantes, sélectionnez la colonne à mettre à jour dans la section **Colonnes actives** puis mettez à jour les informations souhaitées (par exemple, le libellé, le statut lié et les règles de mise en forme).

   1. Cliquez sur **Ajouter une colonne** puis sélectionnez le champ à afficher en tant que colonne dans le tableau. Répétez ce processus pour chaque colonne à ajouter.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres du groupe d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Paramètres de groupe** ![Icône de groupe d’analyse](assets/drilldown-group-icon.png).

   1. Cliquez sur le bouton **Ajouter un regroupement** puis sélectionnez le champ à créer en tant que regroupement.

1. Cliquez sur **Enregistrer** pour créer le rapport et l’ajouter au tableau de bord.


