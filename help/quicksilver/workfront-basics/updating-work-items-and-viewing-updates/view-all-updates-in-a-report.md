---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Afficher toutes les mises à jour dans un rapport de note
description: Afficher toutes les mises à jour dans un rapport de note
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 100%

---

# Afficher toutes les mises à jour dans un rapport de note

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

La zone Mises à jour d’un objet affiche, par défaut, un maximum de 200 mises à jour. Pour afficher toutes les mises à jour que l’un des utilisateurs ou l’une des utilisatrices a saisies pour un objet, vous pouvez créer un rapport de note qui affiche toutes les mises à jour.

>[!NOTE]
>
>Vous pouvez créer un rapport pour afficher les mises à jour des objets dans la prévisualisation avec le rapport d’entrée du journal. Pour plus d’informations, voir [Rapport sur la zone Mises à jour](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Nouveau : Standard </p>
   <p>Actuel : formule</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>Accès en modification aux éléments suivants :</p> 
    <ul> 
     <li> <p>Créer des rapports, des tableaux de bord et des calendriers</p> </li> 
     <li> <p>Créer des filtres, des vues et des regroupements</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher</p> <p><b>NOTE</b></p>
   <p>Si vous ne disposez pas de l’autorisation Afficher ou supérieure sur un objet, les informations de cet objet ne s’affichent pas dans le rapport.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créer un rapport de note

La création d’un rapport de notes est identique, quel que soit l’objet.

Par exemple, pour créer un rapport de notes pour toutes les notes d’un projet :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis choisissez **Note**.

1. (Facultatif) Cliquez sur **Vues**, puis sur **Ajouter une colonne** pour ajouter le **nom** du **projet** dans la vue du rapport.

1. (Facultatif) Cliquez sur **Regroupements**, puis sur **Ajouter un regroupement** pour les regrouper par **Nom du projet**, si vous créez des rapports sur plusieurs projets en même temps.\
   Ainsi, les notes sont regroupées par projet, ce qui facilite la lecture du rapport. 

1. (Facultatif) Cliquez sur **Filtres**, puis sur **Ajouter une règle de filtre**.
1. Ajoutez un filtre pour **Note** > **Texte de la note** > **N’est pas vide**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Si un champ de projet a été mis à jour mais qu’aucune note n’a été ajoutée au moment de la mise à jour, le **Texte de la note** de la mise à jour s’affiche sous la forme **(Aucun texte ajouté à la mise à jour)**.


1. (Facultatif) Ajoutez un autre filtre pour **Projet** > **Nom** > **Est égal à** et ajoutez un ou plusieurs noms de projets dont vous souhaitez afficher les notes.
1. Cliquez sur **Enregistrer + Fermer**.\
   Toutes les mises à jour saisies pour le projet par les utilisateurs et utilisatrices ayant au moins l’autorisation Afficher le projet s’affichent dans le rapport.
