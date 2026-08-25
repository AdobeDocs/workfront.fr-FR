---
user-type: administrator
product-area: system-administration;setup
title: Affichage et gestion de l’historique des modifications
description: L’historique des modifications vous permet d’afficher un journal des modifications apportées aux objets et champs Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1e06115eb5688271e2a6f4c8a41647eb644d8292
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 6%

---

# Affichage et gestion de l’historique des modifications

{{preview-fast-release-general}}

L’historique des modifications permet à l’administrateur système de configurer et de suivre les modifications apportées aux objets et aux champs spécifiques dans Adobe Workfront. La configuration flexible permet à l’administrateur de configurer les objets et champs qui font l’objet d’un suivi.

L’historique des modifications peut effectuer le suivi des types de données définis suivants :

* Activité dans la zone Configuration telle que la création ou la suppression d’un niveau d’accès ou d’une fonction
* Mises à jour au niveau du champ, telles que la modification d’une description de projet ou du modèle de mise en page d’un utilisateur
* Mises à jour des objets, telles que la mise à jour du statut d’un projet ou l’association d’un formulaire personnalisé à une tâche
* <span class="preview">Activité de workflow de révision et d’approbation unifiée, y compris les participants et les décisions</span>

Pour plus d&#39;informations sur la définition des objets et des champs suivis, voir [Configurer les champs à suivre dans l&#39;historique des modifications](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

Dans la liste Historique des modifications , vous pouvez afficher le journal des modifications apportées aux objets Workfront, notamment les attributs suivants :

* Nom de l&#39;objet
* Type d’objet
* Type de modification (opération)
* Date et heure de la modification
* Source de la modification, comme des utilisateurs spécifiques, des API, Workfront Fusion, des LLM d’IA ou le système Workfront

>[!NOTE]
>
>Lorsque vous accédez à l&#39;historique des modifications, vous ne verrez les modifications suivies que pour les champs que vous êtes autorisé à consulter.
>Par exemple, si les données financières sont suivies sur des projets et que vous n&#39;avez pas accès aux données financières, les champs financiers ne s&#39;afficheront pas dans la liste Historique des modifications.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td><span class="preview">Accès administratif à l'historique des modifications</span></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher la liste Historique des modifications

Vous pouvez afficher les journaux de l&#39;historique des modifications dans la zone Configuration.

La liste Historique des modifications est une liste améliorée comprenant des filtres, des colonnes, une hauteur de ligne, un sélecteur de date et une barre de recherche.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Suivi des modifications > Liste des modifications de l’historique**.

   La liste Historique des modifications s’ouvre.

1. Pour ajuster les dates pour lesquelles des modifications s’affichent, cliquez sur le sélecteur de date et sélectionnez les nouvelles dates.

   Les modifications sont disponibles pour les 90 derniers jours.

1. Pour rechercher un terme spécifique, cliquez dans la zone de recherche et saisissez le terme. Les résultats sont mis en surbrillance dans la liste au fur et à mesure que vous saisissez.
1. (Facultatif) Pour filtrer selon une colonne, consultez la section [Filtrer les éléments dans une liste améliorée](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) de l’article [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Facultatif) Pour masquer, afficher ou réorganiser des colonnes, consultez la section [Personnaliser les colonnes](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) dans l’article [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Facultatif) Pour ajouter ou supprimer des colonnes, consultez la section [Ajouter et supprimer des colonnes à l’aide du gestionnaire de colonnes](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) dans l’article [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Facultatif) Pour ajuster la hauteur de ligne, consultez la section [Modifier la hauteur de ligne dans une vue](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) dans l’article [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Exporter l&#39;historique des modifications

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Suivi des modifications > Liste des modifications de l’historique**.
1. Filtrez la liste pour afficher les éléments à exporter.
1. Cliquez sur l’icône **Exporter** ![Icône Exporter](assets/export-icon.png) et choisissez d’enregistrer au format XLSX ou CSV.

   La boîte de dialogue Enregistrer le fichier s’ouvre et vous pouvez enregistrer le fichier exporté sur votre ordinateur.
   Terminez d’enregistrer le fichier exporté. Vous pouvez maintenant le trouver sur votre ordinateur et le partager avec d&#39;autres personnes.



