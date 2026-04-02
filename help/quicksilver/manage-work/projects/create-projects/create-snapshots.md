---
product-area: projects
navigation-topic: create-projects
title: Création et affichage d’instantanés de projet
description: Les instantanés d’Adobe Workfront vous permettent de voir les différences entre les instantanés (pris à une date et une heure spécifiques) et les données actuelles du projet.
author: Lisa
feature: Work Management
hidefromtoc: true
hide: true
source-git-commit: 6ccb4669a973a8f855120e83de7c0d437c9495a4
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 4%

---

# Création et affichage d’instantanés de projet

{{highlighted-preview-article-level}}

Les chefs de projet ont souvent besoin de comparer les données antérieures d’un projet avec l’état actuel pour prendre des décisions éclairées et voir comment leurs projets ont changé au fil du temps.

Dans Adobe Workfront, les instantanés vous permettent de voir rapidement et précisément ces différences entre les instantanés (pris à une date et une heure spécifiques) et les données actives du projet, ce qui vous permet de gérer les projets plus efficacement et de prendre de meilleures décisions. Les comparaisons d’instantanés montrent côte à côte comment le projet a évolué.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Workflow Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
    <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configuration du niveau d’accès</td> 
   <td>Accès en modification aux projets</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Lors de l’affichage d’un instantané, vous pouvez afficher tous les champs que vous êtes autorisé à afficher sur le projet d’origine </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’un instantané

1. Accédez à un projet.
1. Dans le panneau de gauche, cliquez sur **Instantanés**.

   ![Instantanés d’un projet](assets/snapshot-list.png)

1. Cliquez sur **Nouveau snapshot**.
1. Saisissez le nom de l’instantané dans la boîte de dialogue **Nouvel instantané**, puis cliquez sur **Enregistrer**.

   Le nom de l’instantané apparaît dans la liste.

   >[!NOTE]
   >
   >Lorsque vous créez un instantané, il n’est pas disponible pour être affiché immédiatement. Selon les données s’exécutant en arrière-plan, la préparation peut prendre jusqu’à 4 heures. Le statut de création est **En attente** lorsque l’instantané n’est pas encore disponible et **Prêt** lorsque vous pouvez l’afficher.

## Affichage d’un seul instantané

1. Accédez à un projet et cliquez sur **Instantanés** dans le panneau de gauche.
1. Cliquez sur un nom d’instantané dans la liste pour l’ouvrir. Le statut doit être **Prêt** avant de pouvoir l’ouvrir.

   >[!TIP]
   >
   >Les chemins de navigation situés en haut de l’écran renvoient au projet et vous aident à identifier que vous visionnez un instantané.

   L&#39;instantané affiche les éléments suivants tels qu&#39;ils existaient au moment où l&#39;instantané a été créé :

   * La hiérarchie des tâches et sous-tâches dans le projet
   * Détails du projet et tout formulaire personnalisé joint à ces détails
   * Projets associés et leur hiérarchie
   * Problèmes
   * Taux
   * Enregistrements de facturation
   * &#x200B;<!--* Bookings (on its own line of course when they get released)--> des dépenses
   * Équipe du projet (onglet Personnes)

   Vous pouvez personnaliser n’importe quelle liste de l’instantané en filtrant, triant, ajoutant et supprimant des colonnes ou en appliquant une vue. Des indicateurs de performance clés temporels peuvent être ajoutés à la vue d’instantané. Pour plus d’informations, consultez [Personnalisation des listes d’instantanés](#customize-snapshot-lists) dans cet article.

## Comparer des instantanés

1. Accédez à un projet et cliquez sur **Instantanés** dans le panneau de gauche.
1. Sélectionnez une option pour comparer des instantanés :

   * Pour comparer plusieurs instantanés, activez les cases à cocher en regard des instantanés dans la liste, puis cliquez sur **Comparer** dans la barre d’actions située en bas de l’écran.
   * Pour comparer des instantanés au projet en cours, activez les cases à cocher en regard des instantanés dans la liste, puis cliquez sur **Comparer avec actuel** dans la barre d’actions située en bas de l’écran.

     >[!NOTE]
     >
     >Le statut de chaque instantané à comparer doit être **Prêt**.

1. Sur l’écran Comparaison , développez chaque instantané et le projet en cours pour afficher la hiérarchie sous-jacente.

   ![Écran Comparaison des instantanés](assets/snapshot-comparison.png)

1. Vous pouvez personnaliser la comparaison en triant, en ajoutant et en supprimant des colonnes ou en appliquant une vue. Pour plus d’informations, consultez [Personnalisation des listes d’instantanés](#customize-snapshot-lists) dans cet article.

## Exporter des instantanés

Vous pouvez exporter la liste de tous les instantanés ou une comparaison d’instantanés au format .xlsx ou .csv. Toutes les colonnes affichées sont incluses dans le fichier exporté.

1. Cliquez sur l’icône **Exporter** ![Icône Exporter](assets/export-icon.png) dans la liste d’instantanés ou la comparaison d’instantanés.
1. Sélectionnez le format du fichier d’exportation.

   Le fichier est enregistré sur votre ordinateur. Vous serez peut-être invité à choisir l’emplacement.

1. (Facultatif) Ouvrez la liste exportée à l’aide de l’application appropriée.

## Personnalisation des listes d’instantanés

Vous pouvez personnaliser la liste de tous les instantanés, ainsi que toutes les listes d&#39;un instantané ou d&#39;une comparaison, en filtrant, en triant, en ajoutant et en supprimant des colonnes ou en appliquant une vue.

Pour plus d’informations sur la personnalisation des listes, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Filtrer les éléments d’une liste

Les filtres vous aident à réduire la quantité d’informations que vous affichez dans la liste.

1. Cliquez sur **Filtrer** au-dessus de la liste.
1. Dans la zone Filtre, cliquez sur **Ajouter une condition**.
1. Sélectionnez un champ en fonction duquel effectuer le filtrage.
1. Sélectionnez un modificateur de filtre, tel que « A l’un des », « N’a aucun des », « Est avant » ou « Est après ». Les options des modificateurs sont différentes selon le type de champ en fonction duquel vous effectuez le filtrage.
1. Sélectionnez la ou les valeurs du champ. Selon le type de champ en fonction duquel vous effectuez le filtrage, vous pouvez être invité à sélectionner l’élément dans une liste, à le rechercher ou à utiliser un calendrier pour sélectionner une période.

   ![Filtrer la liste d’instantanés](assets/filter-snapshot-list.png)

   Le filtre est automatiquement appliqué à la liste.

1. Cliquez sur **Ajouter une condition** pour ajouter une autre condition au filtre.

   Vous pouvez joindre plusieurs filtres à l’aide d’un connecteur ET ou OU.

1. Lorsque le filtre est appliqué, vous pouvez ouvrir à nouveau les options **Filtre** pour modifier les options de filtre ou effacer tous les filtres.

   Un indicateur apparaît sur le bouton **Filtrer** lorsqu&#39;un filtre est appliqué à la liste.

   ![Indicateur de filtre appliqué](assets/glist-filter-applied-indicator.png)

### Tri dans une liste

Pour trier des colonnes individuelles :

1. Pointez sur la colonne, puis cliquez sur la flèche vers le bas et sélectionnez **Trier**.

   Une icône en regard d’un nom de colonne indique que la liste est triée en fonction des valeurs de cette colonne et du sens du tri.

   ![Trier la liste d’instantanés](assets/sort-snapshot-list.png)

### Personnaliser les colonnes d’une liste

Vous pouvez masquer, afficher et réorganiser les colonnes d’une liste.

1. Cliquez sur **Colonnes** au-dessus de la liste.

   ![Colonnes de la liste d’instantanés](assets/hide-display-columns-on-snapshot.png)

1. Utilisez les boutons pour afficher ou masquer des colonnes dans la liste.
1. Pour réorganiser les colonnes, cliquez sur l’icône **Faire glisser** ![Icône Faire glisser](assets/drag-icon.png) et déplacez une colonne vers l’emplacement souhaité. Le déplacement de colonnes modifie automatiquement la liste.

   >[!NOTE]
   >
   >Le champ principal est la première colonne de la liste. Il est fixe en première position et vous ne pouvez pas modifier sa colonne. Si le nombre de colonnes est important, le champ principal est figé à gauche et lorsque vous faites défiler l’écran horizontalement, il est toujours visible.
   >
   >L’icône en regard d’un nom de champ affiche le type de champ, tel que du texte ou un champ de date.

   Un indicateur s’affiche sur le bouton **Colonnes** lorsque des colonnes sont masquées. L’indicateur n’apparaît pas lorsque vous réorganisez les colonnes.

   ![Indicateur des colonnes masquées](assets/glist-columns-hidden-indicator.png)

### Ajouter et supprimer des colonnes à l’aide du gestionnaire de colonnes

Vous pouvez utiliser le gestionnaire de colonnes dans certaines listes améliorées pour ajouter et supprimer facilement des colonnes de la liste. Vous pouvez ajouter ou supprimer des champs système et personnalisés qui existent déjà dans Workfront sous forme de colonnes.

1. Cliquez sur l’icône **+** dans le coin supérieur droit du tableau pour ouvrir la zone **Gestionnaire de colonnes**.

   ![Gestionnaire de colonnes pour les instantanés](assets/column-manager-on-snapshot-no-kpi-tab.png)

1. Recherchez un champ d’objet existant dans la colonne **Disponible**, puis cliquez sur **+** à droite du nom du champ pour l’ajouter à la colonne **Sélectionné**.
1. Cliquez sur **-** à droite d’un champ dans la colonne **Sélectionné** pour le supprimer de la liste.
1. Cliquez sur **Enregistrer**.

   La liste met à jour les colonnes en fonction des choix que vous avez effectués.

### Application d’une vue à une liste

Pour appliquer ou créer une vue :

1. Cliquez sur le menu déroulant **Vues** et sélectionnez une vue existante pour l’appliquer à la liste

   OU

   Cliquez sur **Nouvelle vue** pour en créer une.

   ![Menu Vues d’un instantané](assets/views-on-snapshot-list.png)

1. (Conditionnel) Pour ajouter une nouvelle vue, saisissez un nom pour la vue, puis cliquez sur **Créer**.
1. (Facultatif) Masquez, affichez ou réorganisez les colonnes. Pour plus d’informations, voir [&#x200B; Personnaliser les colonnes d’une liste &#x200B;](#customize-columns-in-a-list).
1. (Facultatif) Filtrez la liste. Pour plus d’informations, voir [Filtrer les éléments dans une liste](#filter-items-in-a-list).

Les modifications apportées aux vues sont enregistrées automatiquement. La prochaine fois que vous appliquerez cette vue, les paramètres de colonne et de filtre resteront tels que vous les avez définis. Pour plus d&#39;informations sur les vues, voir [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

