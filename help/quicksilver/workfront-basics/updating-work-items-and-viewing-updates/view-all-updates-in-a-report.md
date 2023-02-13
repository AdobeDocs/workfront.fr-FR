---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Afficher toutes les mises à jour d’un rapport Remarque
description: Afficher toutes les mises à jour d’un rapport Remarque
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Afficher toutes les mises à jour d’un rapport Remarque

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

La zone Mises à jour d’un objet affiche, par défaut, un maximum de 200 mises à jour. Pour afficher toutes les mises à jour que l’un des utilisateurs a saisies pour un objet, vous pouvez créer un rapport Remarque qui affiche toutes les mises à jour.

>[!NOTE]
>
>Vous pouvez créer un rapport pour afficher les mises à jour des objets dans l&#39;aperçu avec le rapport d&#39;entrée Journal. Pour plus d’informations, voir [Rapport sur la zone Mises à jour](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès.<br>Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher</p> <p>Remarque : Si vous ne disposez pas de l’autorisation Afficher ou supérieure pour un objet, les informations de cet objet ne s’affichent pas dans le rapport.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’un rapport Note

La création d’un rapport de notes pour n’importe quel objet est identique, quel que soit l’objet .

Par exemple, pour créer un rapport Note pour toutes les notes d’un projet :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis choisissez **Remarque**.

1. (Facultatif) Cliquez sur **Vues**, puis **Ajouter une colonne** pour ajouter la variable **Nom** de **Projet** dans la vue du rapport. 

1. (Facultatif) Cliquez sur **Groupements**, puis **Ajouter un groupement** pour les regrouper par **Nom du projet**, si vous créez des rapports sur plusieurs projets en même temps.\
   Ainsi, les notes sont regroupées par projet, ce qui facilite la lecture du rapport. 

1. (Facultatif) Cliquez sur **Filtres,** then **Ajouter une règle de filtre** pour filtrer un seul projet ou des projets spécifiques.

1. (Conditionnel et facultatif) Définissez la variable **Nom du projet** as **Égal** au nom du projet pour lequel vous souhaitez afficher les mises à jour.  

1. Cliquez sur **Enregistrer + Fermer**.\
   Toutes les mises à jour entrées sur le projet par tous les utilisateurs autorisés à au moins Afficher le projet s’affichent dans le rapport.
