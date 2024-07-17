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
ht-degree: 20%

---

# Afficher toutes les mises à jour dans un rapport de note

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

La zone Mises à jour d’un objet affiche, par défaut, un maximum de 200 mises à jour. Pour afficher toutes les mises à jour que l’un des utilisateurs a saisies pour un objet, vous pouvez créer un rapport Remarque qui affiche toutes les mises à jour.

>[!NOTE]
>
>Vous pouvez créer un rapport pour afficher les mises à jour des objets dans l&#39;aperçu avec le rapport d&#39;entrée Journal. Pour plus d’informations, consultez [Rapport sur la zone Mises à jour](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Nouvelle : standard </p>
   <p>Actuelle : formule</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher</p> <p><b>NOTE</b></p>
   <p>Si vous ne disposez pas de l’autorisation Afficher ou supérieure pour un objet, les informations de cet objet ne s’affichent pas dans le rapport.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Création d’un rapport Note

La création d’un rapport de notes pour n’importe quel objet est identique, quel que soit l’objet .

Par exemple, pour créer un rapport Note pour toutes les notes d’un projet :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Remarque**.

1. (Facultatif) Cliquez sur **Views**, puis **Add Column** pour ajouter le **Name** du **Project** dans la vue du rapport. 

1. (Facultatif) Cliquez sur **Groupings**, puis sur **Ajouter un groupement** pour effectuer un groupement en fonction du **nom du projet**, si vous créez des rapports simultanément sur plusieurs projets.\
   Ainsi, les notes sont regroupées par projet, ce qui facilite la lecture du rapport. 

1. (Facultatif) Cliquez sur **Filtres,**, puis **Ajouter une règle de filtre**.
1. Ajoutez un filtre pour **Remarque** > **Texte de remarque** > **N’est pas vierge**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Si un champ de projet a été mis à jour mais qu’aucune note n’a été ajoutée au moment de la mise à jour, le **texte de note** de la mise à jour s’affiche comme **(Aucun texte ajouté à mettre à jour)**.


1. (Facultatif) Ajoutez un autre filtre pour **Projet** > **Nom** > **Égal à** et ajoutez un ou plusieurs noms de projet pour lesquels vous souhaitez afficher des notes.
1. Cliquez sur **Enregistrer + Fermer**.\
   Toutes les mises à jour entrées sur le projet par tous les utilisateurs autorisés à au moins Afficher le projet s’affichent dans le rapport.
