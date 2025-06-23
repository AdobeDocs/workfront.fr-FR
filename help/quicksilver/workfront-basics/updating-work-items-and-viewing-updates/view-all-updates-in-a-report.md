---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Afficher toutes les mises à jour dans un rapport de note
description: Pour afficher toutes les mises à jour que l’un des utilisateurs ou l’une des utilisatrices a saisies pour un objet, vous pouvez créer un rapport de note qui affiche toutes les mises à jour.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 63%

---

# Afficher toutes les mises à jour dans un rapport de note

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

La zone Mises à jour d’un objet affiche, par défaut, un maximum de 200 mises à jour. Pour afficher toutes les mises à jour que l’un des utilisateurs ou l’une des utilisatrices a saisies pour un objet, vous pouvez créer un rapport de note qui affiche toutes les mises à jour.

>[!NOTE]
>
>Vous pouvez créer un rapport pour afficher les mises à jour des objets dans la prévisualisation avec le rapport d’entrée du journal. Pour plus d&#39;informations, voir [Rapport sur la zone Mises à jour avec un rapport Entrée de journal](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard </p>
   <p>Actuel : formule</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux éléments suivants :</p> 
    <ul> 
     <li> <p>Créer des rapports, des tableaux de bord et des calendriers</p> </li> 
     <li> <p>Créer des filtres, des vues et des regroupements</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher</p>
    <p>Remarque : Si vous ne disposez pas d'une autorisation d'affichage ou d'une autorisation supérieure pour un objet, les informations relatives à cet objet ne s'affichent pas dans l'état.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créer un rapport de notes

La création d’un rapport de notes est identique, quel que soit l’objet.

Par exemple, pour créer un rapport de notes pour toutes les notes d’un projet :

{{step1-to-reports}}

1. Dans le coin supérieur gauche de la page, cliquez sur **Nouveau rapport**, puis sélectionnez **Note**.

1. (Facultatif) Cliquez sur **(Colonnes) Affichage** puis sur **Ajouter une colonne** pour ajouter le **Nom** du **Projet** dans l’affichage du rapport. 

1. (Facultatif) Si vous créez des rapports sur plusieurs projets en même temps, cliquez sur **Regroupements**, puis sur **Ajouter un regroupement** pour effectuer un regroupement à l’aide du **Nom** du **Projet**. Cela permet de s’assurer que les notes sont regroupées selon leurs projets respectifs, ce qui facilite la lecture du rapport. 

1. (Facultatif) Cliquez sur **Filtres**, puis **Ajouter une règle de filtre**.
1. Ajoutez un filtre pour **Note** > **Texte de la note** > **N’est pas vide**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Si un champ de projet a été mis à jour mais qu’aucune note n’a été ajoutée au moment de la mise à jour, le **Texte de la note** de la mise à jour s’affiche sous la forme **(Aucun texte ajouté à la mise à jour)**.


1. (Facultatif) Ajoutez un autre filtre pour **Projet** > **Nom** > **Est égal à** et ajoutez un ou plusieurs noms de projets dont vous souhaitez afficher les notes.
1. Cliquez sur **Enregistrer + Fermer**. Toutes les mises à jour saisies sur le projet par tous les utilisateurs autorisés à afficher le projet s’affichent dans le rapport.
