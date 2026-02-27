---
product-area: reporting
navigation-topic: report-usage
title: Utilisation de dossiers de rapports partageables
description: Utilisez des dossiers de rapports partageables pour organiser les rapports que vous créez et partager ces dossiers avec d’autres utilisateurs dans Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 65831f2e-9092-4e99-a86b-40df42c713bf
source-git-commit: 650d24c36c3ccee810b8918ccdf456f607b055e9
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 10%

---

# Utilisation de dossiers de rapports partageables

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

<!-- This article is linked in the UI -->

Vous pouvez utiliser des dossiers de rapports partageables pour organiser les rapports et partager ces dossiers avec d’autres utilisateurs. Cette fonctionnalité est conçue pour les équipes qui gèrent d’importants volumes de rapports et ont besoin d’un contrôle d’accès évolutif et cohérent.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>n’importe lequel</p> </td> 
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

## Présentation des autorisations de dossier

Les dossiers de rapports partageables utilisent deux niveaux d’autorisation :

* **Afficher** : les utilisateurs peuvent ouvrir des rapports dans le dossier, mais ils ne peuvent pas modifier les détails du dossier, ajouter ou supprimer des éléments, ni supprimer le dossier. Vous pouvez autoriser les utilisateurs disposant d’un accès en lecture seule à partager le dossier en activant le paramètre **Partager** lorsque vous accordez l’accès.
* **Gérer** : les utilisateurs peuvent modifier les détails du dossier et ajouter ou déplacer des éléments de rapport. Ils bénéficient également d’un accès de niveau Gérer aux rapports dans le dossier . Vous pouvez permettre aux utilisateurs disposant d’un accès de niveau Gérer de partager le dossier ou de supprimer des dossiers en activant les paramètres **Partager** et **Supprimer** lorsque vous accordez l’accès.

Comportement supplémentaire :

* Les administrateurs système peuvent voir tous les dossiers.
* Les autres utilisateurs voient uniquement les dossiers auxquels ils ont accès.
* Les autorisations accordées à un dossier parent s’appliquent à tous les sous-dossiers et rapports de cette arborescence de dossiers.
* Les utilisateurs ayant accès à un sous-dossier peuvent voir ses dossiers parents pour la navigation, mais pas les dossiers frères, sauf si l’accès est accordé.

## Création d’un dossier de rapports partageable

Seuls les administrateurs système peuvent créer des dossiers au niveau supérieur. Après la création d’un dossier partageable, les utilisateurs disposant d’un accès de niveau Gérer peuvent créer des sous-dossiers dans celui-ci.

{{step1-to-reports}}

1. Activez le bouton (bascule) **Dossiers de rapports partageables**.
1. Cliquez sur **Créer un dossier**.
1. Saisissez un nom pour le dossier.
1. Cliquez sur **Créer**.

![créer un dossier partageable](assets/add-sharable-folder.png)

## Créer un sous-dossier dans un dossier de rapports partageable

Vous pouvez créer jusqu’à 3 niveaux de sous-dossiers dans un dossier de rapports partageable. Les sous-dossiers héritent des autorisations du dossier parent, mais vous pouvez également définir des autorisations uniques pour chaque sous-dossier.

{{step1-to-reports}}

1. Recherchez le dossier dans lequel vous souhaitez créer un sous-dossier.
1. Cliquez sur **Plus** > **Ajouter un sous-dossier**.
1. Saisissez un nom pour le sous-dossier.
1. Cliquez sur **Créer**.

## Partager un dossier de rapports avec d’autres utilisateurs

Lorsque vous partagez un dossier avec des utilisateurs, ces derniers héritent de l’accès à tous les sous-dossiers de cette arborescence de dossiers. Les utilisateurs doivent également avoir accès à chaque rapport, soit par le biais d’autorisations de dossiers, soit par le partage direct de rapports.

{{step1-to-reports}}

1. Recherchez le dossier que vous souhaitez partager.
1. Cliquez sur **Plus** > **Partager**.
1. Ajoutez des utilisateurs, des équipes, des rôles, des groupes ou des entreprises.
1. Choisissez **Afficher** ou **Gérer** l’accès :
   * L’accès en affichage permet aux utilisateurs d’ouvrir des rapports dans le dossier . Vous pouvez également autoriser les utilisateurs disposant d’un accès en lecture seule à repartager le dossier en sélectionnant **Partager** dans les paramètres supplémentaires.
   * La gestion de l’accès permet aux utilisateurs de modifier les détails du dossier et d’ajouter ou de supprimer des éléments. Vous pouvez également permettre aux utilisateurs disposant d’un accès de niveau Gérer de supprimer des dossiers ou de partager le dossier en sélectionnant **Supprimer** et **Partager** dans les paramètres supplémentaires.
1. Cliquez sur **Enregistrer**.

   ![partager un dossier et affiner l’accès](assets/share-settings-sharable-folders.png)

## Déplacer un rapport vers un dossier partageable

Pour déplacer un rapport dans un dossier, vous devez disposer des droits **Gérer** sur le rapport et le dossier partageable.

{{step1-to-reports}}

1. Cochez la case en regard du rapport à déplacer.
1. Cliquez sur **Déplacer vers le dossier** dans la barre d’actions située en bas de l’écran.
1. Recherchez le dossier dans lequel déplacer le rapport, puis cliquez sur **Déplacer**. L’arborescence du rapport est réduite par défaut. Vous devrez peut-être donc développer les dossiers pour trouver le dossier de destination.

   ![déplacer un rapport vers un dossier partageable](assets/move-to-folder.png)

## Suppression d’un dossier de rapports partageable

Lorsque vous supprimez un dossier, tous les sous-dossiers qu’il contient sont également supprimés. Vous devez disposer d’un accès **Gérer** au dossier pour le supprimer. Les rapports du dossier ne sont pas supprimés et se trouvent toujours dans la liste de rapports principale.

Les autorisations de rapport accordées par le biais des autorisations de dossier sont supprimées lorsque le dossier est supprimé. Les autorisations de rapport accordées directement à partir du rapport ou héritées d’un tableau de bord restent en place.


{{step1-to-reports}}

1. Cliquez sur **Plus** > **Supprimer**.
1. Cliquez sur **Oui, supprimer** pour confirmer.


## Nouvelle expérience de liste pour les dossiers partageables

Lorsque vous accédez à des dossiers partageables dans la zone Rapports , une nouvelle expérience de liste s’affiche, qui vous permet d’afficher et de gérer facilement vos dossiers et rapports. Pour plus d’informations sur la nouvelle expérience de liste, voir [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).