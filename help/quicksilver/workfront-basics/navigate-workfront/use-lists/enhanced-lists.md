---
navigation-topic: get-started-with-workfront
title: Utiliser des listes améliorées
description: Les listes améliorées utilisent un format de tableau pour afficher les éléments de liste et leur aspect est différent de celui des listes standard
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
source-git-commit: ee5bb3cbf6a69b85c3d6b87500164f85a1ba114a
workflow-type: tm+mt
source-wordcount: '1617'
ht-degree: 5%

---

# Utiliser des listes améliorées

Des listes améliorées sont disponibles dans certaines parties d’Adobe Workfront. Ces listes utilisent un format de tableau pour afficher les éléments de liste et leur aspect est différent de celui des listes standard. La gestion des vues est également améliorée, notamment le filtrage, le regroupement, la gestion des colonnes et la recherche.

Pour plus d’informations sur les listes standard, voir [Prise en main des listes dans Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

>[!NOTE]
>
>Chaque liste améliorée peut être configurée différemment pour vous aider à afficher les données dont vous avez besoin. Chaque liste n’utilise pas toutes les fonctionnalités décrites dans cet article. En outre, certaines listes peuvent comporter des fonctionnalités spécifiques qui s’appliquent uniquement à cette liste.

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
   <td>
   <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p></td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objets utilisant des listes améliorées

Vous trouverez ci-dessous certains types de listes d’objets Workfront qui utilisent le format de liste amélioré et certaines des zones où elles s’affichent par défaut lorsque vous disposez des droits pour afficher l’objet.

>[!NOTE]
>
>Cette liste n’est pas exhaustive. Chacune de ces listes d’objets peut également apparaître dans un rapport ou un tableau de bord. Par exemple, un rapport de requête ou un tableau de bord contenant un rapport de requête affiche également une liste de requêtes.

| Liste Workfront | Emplacement de la liste d’objets |
|--- |--- |
| Priorités | <ul><li>Accueil > sélectionnez l’icône Priorités dans le menu de gauche</li><li>Menu principal > Priorités</li></ul> |
| Liste des requêtes | <ul><li>Demandes (nouvelle expérience uniquement)</li><li>Widget Mes demandes sur l’Accueil</li></ul> |
| Listes de statuts, priorités, gravités et taux de change dans la configuration | <ul><li>Configuration > Préférences du projet > Statuts</li><li>Configuration > Préférences du projet > Priorités</li><li>Configuration > Préférences du projet > Gravités</li><li>Configuration > Préférences du projet > Taux de change</li></ul> |

## Ajouter des éléments à une liste améliorée

Selon la liste améliorée que vous consultez, effectuez l’une des opérations suivantes :

1. Cliquez sur le bouton bleu en haut à droite de la liste. Cette option ouvre une boîte de dialogue dans laquelle vous pouvez saisir des informations. Les données sont enregistrées en tant que nouvelle ligne dans le tableau.

   OU

1. Cliquez sur **Nouvelle ligne** au bas de la liste. Cette option ajoute une nouvelle ligne au tableau. Double-cliquez dans une cellule pour y saisir des informations. Chaque cellule représente un champ pour l’élément de liste. Les champs doivent exister avant de les voir dans la liste.

   Les listes améliorées prennent en charge les types de champs suivants :

   * Texte
   * Nombre
   * Devise
   * Date
   * Date et heure
   * Listes déroulantes à sélection unique/multiple
   * Frappe continue
   * Paragraphe
   * Personne désignée (une ou plusieurs)
   * Sélecteur de couleurs

   >[!NOTE]
   >
   >Chaque type de champ possède ses propres options de modification. Certains champs peuvent être en lecture seule.

![ Exemple de liste améliorée ](assets/glist-exchange-rates.png)

## Modifier les éléments à l’aide de la barre d’actions

Vous pouvez utiliser la barre d’actions d’une liste améliorée pour modifier des éléments de la liste. Toutes les barres d’actions n’incluent pas les mêmes options. En outre, certaines listes peuvent ne pas vous permettre de sélectionner des éléments et la barre d’actions n’est pas disponible.

1. Cochez la case en regard d’un élément d’une liste améliorée.

   La barre d’actions s’affiche en bas de l’écran.

   >[!NOTE]
   >
   >Selon la liste que vous modifiez, vous pouvez sélectionner un ou plusieurs éléments pour utiliser la barre d’actions.

1. Cliquez sur une action de la barre pour modifier des éléments. Voici quelques exemples d’actions :

   * Afficher
   * Modifier
   * Supprimer

   Si aucune action n’est disponible pour l’élément sélectionné, la barre d’actions indique « Aucune action disponible ».

   ![ Exemple de barre d’actions ](assets/glist-action-bar-statuses.png)

1. Pointez sur le champ principal d’un élément de liste, puis cliquez sur le menu **Plus** ![icône de menu Plus](assets/more-icon.png) pour afficher des actions supplémentaires. Certaines actions peuvent être spécifiques à cette liste.

   >[!TIP]
   >
   >Le champ principal s’affiche dans la première colonne de la liste.

   ![Exemple de menu Plus](assets/glist-more-menu-priorities.png)

## Personnaliser les colonnes

Selon les objets que vous consultez dans une liste améliorée, vous pouvez masquer, afficher ou réorganiser les colonnes de la liste.

1. Cliquez sur **Colonnes** au-dessus de la liste.

   ![Exemple d’affichage des colonnes](assets/glist-display-move-columns.png)

1. Utilisez les boutons pour afficher ou masquer des colonnes dans la liste.
1. Pour réorganiser les colonnes, cliquez sur l’icône **Faire glisser** ![Icône Faire glisser](assets/drag-icon.png) et déplacez une colonne vers l’emplacement souhaité. Le déplacement de colonnes modifie automatiquement la liste.

   >[!NOTE]
   >
   >Le champ principal est la première colonne de la liste. Il est fixe en première position et vous ne pouvez pas modifier sa colonne. Si le nombre de colonnes est important, le champ principal est figé à gauche et lorsque vous faites défiler l’écran horizontalement, il est toujours visible.
   >
   >L’icône en regard d’un nom de champ affiche le type de champ, tel que du texte ou un champ de date.

   Un indicateur s’affiche sur le bouton **Colonnes** lorsque des colonnes sont masquées. L’indicateur n’apparaît pas lorsque vous réorganisez les colonnes.

   ![Indicateur des colonnes masquées](assets/glist-columns-hidden-indicator.png)

## Ajouter et supprimer des colonnes à l’aide du gestionnaire de colonnes

Vous pouvez utiliser le **Gestionnaire de colonnes** dans certaines listes améliorées pour ajouter et supprimer facilement des colonnes de la liste. Vous pouvez ajouter ou supprimer des champs système et personnalisés qui existent déjà dans Workfront sous forme de colonnes à une liste améliorée.

Pour ajouter et supprimer des colonnes :

1. Cliquez sur l’icône + dans le coin supérieur droit du tableau pour ouvrir la zone **Gestionnaire de colonnes**.
1. Recherchez un champ d’objet existant dans la colonne **Disponible**, puis cliquez sur + à droite du nom du champ pour l’ajouter à la colonne **Sélectionné**.
1. Cliquez sur - à droite d’un champ de la colonne **Sélectionné** pour le supprimer de la liste.

   >[!NOTE]
   >
   >Certains champs peuvent être corrigés et ne peuvent pas être supprimés.

   <!-- Add info about Properties and KPIs when something gets released with those options -->

1. Cliquer sur **Enregistrer**.

   ![Gestionnaire de colonnes](assets/glist-column-manager.png)

   La liste met à jour les colonnes en fonction des choix que vous avez effectués.

## Affichage des données avec des vues dans une liste améliorée

Une vue est un ensemble personnalisé de dispositions de colonnes et de filtres que vous pouvez appliquer à une liste. Vous pouvez créer des vues et modifier des vues existantes.

### Application et création de vues

Pour appliquer une vue, cliquez sur la liste déroulante **Vues** et sélectionnez la vue à appliquer à la liste.

Pour créer une vue :

1. Cliquez sur la liste déroulante **Vues** et sélectionnez **Nouvelle vue**.
1. Attribuez un nom à la vue, puis cliquez sur **Créer**.
1. (Facultatif) Masquez, affichez ou réorganisez les colonnes. Pour plus d’informations, voir [ Personnaliser les colonnes d’une liste améliorée ](#customize-columns-in-an-enhanced-list).
1. (Facultatif) Filtrez et regroupez les éléments de liste. Pour plus d’informations, voir [Filtrer et regrouper des éléments dans une liste améliorée](#filter-and-group-items-in-an-enhanced-list).

   Les modifications apportées aux vues sont enregistrées automatiquement et sont visibles par toute personne utilisant la vue.

   La prochaine fois que vous appliquerez cette vue, les paramètres de colonne et de filtre resteront tels que vous les avez définis.

### Partager une vue

Dans la liste déroulante **Vues**, vous pouvez voir trois catégories de vues :

* **Vues système** : vues que l&#39;administrateur système vous a affectées.
* **Vues partagées** : vues qui ont été partagées avec vous par d&#39;autres utilisateurs.
* **Mes vues** : vues que vous avez créées et que vous pouvez partager avec d’autres utilisateurs. Vous pouvez partager des vues avec d’autres utilisateurs, équipes ou groupes.

Pour partager une vue :

1. Dans la liste déroulante **Vues**, passez la souris sur la vue de **Mes vues** que vous souhaitez partager, puis cliquez sur le menu à trois points lorsqu’il s’affiche.
1. Sélectionnez **Partager**.
1. Dans la boîte de dialogue Partager, saisissez les noms des utilisateurs, des équipes ou des groupes avec lesquels vous souhaitez partager la vue, puis sélectionnez-les dans la liste lorsqu’ils apparaissent.

   Vous pouvez accorder les autorisations suivantes aux destinataires :

   * **Affichage** : les utilisateurs et utilisatrices peuvent appliquer l’affichage à la liste, mais pas le partager.
   * **Gérer** : les utilisateurs et utilisatrices peuvent renommer la vue, la partager avec d’autres personnes et la supprimer.

1. Cliquer sur **Enregistrer**.

## Filtrer et regrouper des éléments

Les filtres vous aident à réduire la quantité d’informations que vous affichez dans la liste. Les regroupements permettent de séparer les objets de la liste dans des zones selon des critères spécifiques.

### Utiliser des filtres

1. Cliquez sur **Filtrer** au-dessus de la liste.
1. Dans la zone Filtre, cliquez sur **Ajouter une condition**.
1. Sélectionnez un champ en fonction duquel effectuer le filtrage.
1. Sélectionnez un modificateur de filtre, tel que « A l’un des », « N’a aucun des », « Est avant » ou « Est après ». Les options des modificateurs sont différentes selon le type de champ en fonction duquel vous effectuez le filtrage.
1. Sélectionnez la ou les valeurs du champ. Selon le type de champ en fonction duquel vous effectuez le filtrage, vous pouvez être invité à sélectionner l’élément dans une liste, à le rechercher ou à utiliser un calendrier pour sélectionner une période.

   ![Filtrer dans des listes améliorées](assets/glist-filter-with-options.png)

   Le filtre est automatiquement appliqué à la liste.

   >[!TIP]
   >
   >Pour appliquer un caractère générique à l’utilisateur actuel, sélectionnez **Moi (utilisateur connecté)** comme valeur du champ. Le filtre s’applique alors à l’utilisateur ou l’utilisatrice qui consulte la liste. Ce caractère générique est disponible dans les champs où la valeur est un utilisateur.

1. Cliquez sur **Ajouter une condition** pour ajouter une autre condition au filtre sous la forme d’une instruction OR.
1. Lorsque le filtre est appliqué, vous pouvez ouvrir à nouveau les options **Filtre** pour modifier les options de filtre ou effacer tous les filtres.

   Un indicateur apparaît sur le bouton **Filtrer** lorsqu&#39;un filtre est appliqué à la liste.

   ![Indicateur de filtre appliqué](assets/glist-filter-applied-indicator.png)

### Utiliser les regroupements

1. Cliquez sur **Grouper** au-dessus de la liste.
1. Sélectionnez un regroupement pour organiser votre liste.

   ![Sélectionner un regroupement](assets/glist-grouping-choose-a-group-by.png)

1. Lorsque le regroupement est appliqué, vous pouvez ouvrir à nouveau les options Regrouper pour réduire ou développer tous les regroupements à la fois, modifier le regroupement pour les regrouper selon un autre champ ou effacer tous les regroupements.

   ![Regroupement dans des listes améliorées](assets/glist-group-by-due-date-priorities.png)

   Un indicateur apparaît sur le bouton **Regrouper** lorsqu&#39;un regroupement est appliqué à la liste.

   ![Indicateur de groupement appliqué](assets/glist-grouping-applied-indicator.png)

## Tri et recherche dans une liste améliorée

Pour trier des colonnes individuelles :

1. Accédez à la colonne et cliquez sur la flèche vers le bas.

   Une icône en regard d’un nom de colonne indique que la liste est triée en fonction des valeurs de cette colonne et du sens du tri.

   >[!NOTE]
   >
   >Selon la liste, certaines colonnes peuvent ne pas être triables.

   ![Trier par colonne](assets/glist-sort-by-column.png)

Pour trier votre travail dans un regroupement :

1. Cliquez sur **Grouper** et choisissez si vous souhaitez effectuer un tri par ordre croissant ou décroissant.

   ![Trier dans un regroupement](assets/sort-in-groups.png)

Pour effectuer une recherche :

1. Saisissez le terme à rechercher dans le champ de recherche situé au-dessus de la liste. Les résultats sont mis en surbrillance dans la liste au fur et à mesure que vous saisissez.

   ![Terme de recherche mis en surbrillance](assets/glist-search-highlighted.png)
