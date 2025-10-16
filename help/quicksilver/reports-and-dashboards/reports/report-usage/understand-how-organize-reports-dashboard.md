---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Comprendre l’organisation des rapports sur un tableau de bord
description: Vous pouvez voir si un rapport est ajouté à un tableau de bord dans Adobe Workfront. Cela peut s’avérer utile lorsque vous décidez quels rapports vous pouvez conserver et lesquels peuvent être supprimés du système. Si les rapports se trouvent sur des tableaux de bord, il se peut que les personnes continuent de s’y fier. Il est recommandé de ne pas supprimer les rapports répertoriés dans les tableaux de bord que les personnes utilisent. Pour plus d’informations sur l’ajout de rapports aux tableaux de bord, voir l’article Ajouter un rapport à un tableau de bord.
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 92%

---

# Comprendre l’organisation des rapports sur un tableau de bord

## Accéder aux informations d’un tableau de bord dans une liste de rapports

Vous pouvez voir si un rapport est ajouté à un tableau de bord dans Adobe Workfront. Cela peut s’avérer utile lorsque vous décidez quels rapports vous pouvez conserver et lesquels peuvent être supprimés du système. Si les rapports se trouvent sur des tableaux de bord, il se peut que les personnes continuent de s’y fier. Il est recommandé de ne pas supprimer les rapports répertoriés dans les tableaux de bord que les personnes utilisent.\
Pour plus d’informations sur l’ajout de rapports aux tableaux de bord, voir l’article [Ajouter un rapport à un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Pour voir si un rapport est ajouté à un tableau de bord, effectuez l’une des opérations suivantes :

* Créez une vue pour une liste de rapports et incluez les informations sur les tableaux de bord dans les colonnes.
* Filtrez une liste de rapports selon un ou plusieurs tableaux de bord spécifiques dont vous savez qu’ils sont activement utilisés.
* Créez un rapport pour l’objet de rapport et utilisez une vue ou un filtre incluant des informations sur les tableaux de bord.

N’importe qui peut créer une vue ou un filtre, mais vous devez disposer de l’accès Modifier aux rapports dans votre niveau d’accès pour créer un rapport.\
Pour plus d’informations sur l’accès aux rapports, voir l’article [Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Pour plus d’informations sur la création d’un rapport, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Standard</p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher les informations sur les tableaux de bord dans la vue d’une liste de rapports

>[!WARNING]
>
>L’inclusion de la colonne Tableaux de bord dans une liste de rapports peut augmenter considérablement les temps de chargement, en particulier pour les longues listes de rapports.

Pour créer une vue contenant les informations sur les tableaux de bord pour une liste de rapports :

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Rapports**.
1. Dans la liste des rapports, cliquez sur le menu déroulant **Affichage**.
1. Cliquez sur **Nouvelle vue**.
1. Cliquez sur **Ajouter une colonne**.
1. Commencez à saisir « Tableaux de bord » dans le champ **Commencer à saisir le nom du champ**.
1. Sous l’objet **Rapport**, sélectionnez **Tableaux de bord**.

1. Cliquez sur **Enregistrer la vue**.\
   Les tableaux de bord sur lesquels apparaît un rapport s’affichent dans la colonne Tableaux de bord de la liste des rapports.\
   ![Tableaux de bord dans le rapport](assets/qs-dashboards-in-report-view.png)

## Filtrer une liste de rapports par informations sur les tableaux de bord

Pour filtrer une liste de rapports par informations sur les tableaux de bord :

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Rapports**.

1. Dans la liste des rapports, cliquez sur le menu déroulant **Filtrer**.
1. Cliquez sur **Nouveau filtre**, puis sur **Ajouter une règle de filtre**.

1. Commencez à saisir « Tableaux de bord » dans le champ **Commencer à saisir le nom du champ**.

1. Sous l’objet **Tableaux de bord**, sélectionnez **Nom**.

1. Sélectionnez **Égal à** dans le menu déroulant des modificateurs, puis commencez à saisir le nom du tableau de bord que vous souhaitez filtrer. Vous pouvez sélectionner plusieurs tableaux de bord pour votre filtre.\
   ![Tableaux de bord dans les filtres de rapport](assets/qs-dashboards-in-report-filters-350x143.png)

1. Cliquez sur **Enregistrer + Fermer**.\
   Cette option affiche la liste des rapports répertoriés uniquement sur les tableaux de bord spécifiés.\
   Vous pouvez également créer un rapport pour l’objet du rapport et utiliser ce filtre dans le rapport.
