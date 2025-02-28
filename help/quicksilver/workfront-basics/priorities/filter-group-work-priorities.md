---
navigation-topic: get-started-with-workfront
title: Filtrer et regrouper votre travail avec les priorités
description: Vous pouvez utiliser des filtres pour trouver le travail que vous recherchez, puis appliquer un regroupement pour le garder organisé.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 8eb9dcaf-bba3-466d-b06d-5383991bc4ea
source-git-commit: 116b9823818ac6103641c2e6ce283dfb47282851
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 15%

---

# Filtrer et regrouper votre travail avec les priorités

Vous pouvez utiliser des filtres pour trouver le travail que vous recherchez, puis appliquer un regroupement pour le garder organisé.

Priorités affiche les éléments de travail qui vous sont affectés. Vous ne pouvez pas voir les éléments de travail affectés à votre équipe dans la liste de travail Priorités.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> 
   <p>Actuelle : demande ou niveau supérieur</p>
   <p>Nouvelle : contributeur ou supérieure</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>Accès Afficher ou Modifier à l’objet mis à jour</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Accès Afficher à l’objet</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrer votre travail à l’aide de filtres standard

Vous pouvez filtrer les tâches et les événements qui vous sont affectés.

{{step1-to-priorities}}

1. Cliquez sur **Filtres** en haut à gauche de la liste de travail.
1. cliquez sur **Filtres standard**.
1. Sélectionnez un ou plusieurs filtres pour affiner vos éléments de travail.
   ![](assets/filter-new.png)

+++Développer pour afficher des informations détaillées sur les filtres disponibles
<table>
  <tbody>
   <tr>
   <th>Filtre</th>
   <th>Description</th>
   </tr>
    <tr>
      <td>Travail en cours</td>
      <td>Affiche les éléments sur lesquels vous travaillez actuellement</td>
    </tr>
    <tr>
      <td>Démarrage possible</td>
      <td>Affiche les éléments avec 
      <ul>
      <li>Aucune contrainte de tâches ou de prédécesseurs incomplète</li>
      <p>et</p>
      <li>La date de début prévue est dans le passé ou peut être dans les deux semaines à venir</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>À préparer</td>
      <td>Affiche les éléments qui ont
       <ul>
      <li>Prédécesseurs incomplets ou contraintes de tâche empêchant le traitement de l'élément</li>
      <p>ou</p>
      <li>La date de début prévue est dans le futur depuis plus de deux semaines</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Demandé</td>
      <td>Affiche les problèmes sur lesquels vous n'avez pas encore commencé à travailler</td>
    </tr>
      <td>Terminé</td>
      <td>Affiche le travail effectué au cours des deux dernières semaines. Cette option de filtre n’inclut pas les validations.</td>
    </tr>
    <tr>
    <td>Projet</td>
    <td>Affiche les projets contenant des tâches ou des événements qui vous ont été affectés</td>
    </tr>
    <tr>
    <td>Date d’échéance</td>
    <td>Affiche le travail par date d'achèvement prévue</td>
    </tr>
    <tr>
    <td>Statut</td>
    <td>Affiche les tâches ou les événements dont le statut est nouveau, en cours ou terminé</td>
    </tr>
    <tr>
    <td>Mon focus</td>
    <td>Affiche les tâches ou les événements dans auxquels des niveaux de focus ont été affectés. Les niveaux de focus sont attribués et gérés par l’utilisateur individuel.</td>
    </tr>
  </tbody>
</table>

+++

1. (Facultatif) Cliquez sur **Retour aux valeurs par défaut** pour réinitialiser votre sélection.

## Filtrer votre travail à l’aide de filtres dynamiques

Utilisez le langage naturel pour filtrer rapidement le travail.

>[!NOTE]
>
>Cette fonctionnalité est uniquement disponible pour les clients disposant d’une expérience Adobe unifiée à l’aide de l’assistant AI. Pour plus d’informations sur l’assistant AI, voir [Présentation de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

{{step1-to-priorities}}

1. Cliquez sur **Filtres** en haut à gauche de la liste de travail.
1. Cliquez sur **Filtres intelligents**.
1. Saisissez la manière dont vous souhaitez filtrer votre travail.

   Vous pouvez saisir des éléments tels que :

   * Afficher les tâches en retard
   * Afficher mes principales priorités
   * Afficher le travail dû aujourd&#39;hui

</div>

## Regrouper votre travail

{{step1-to-priorities}}

1. Cliquez sur **Groupes** en haut à gauche de la liste de travail.
1. Sélectionner un groupe pour organiser votre liste de travail
   ![](assets/groups-new.png)

+++Développer pour afficher des informations détaillées sur les groupes disponibles

| Groupe | Description |
|-----------|-------------|
| Projet | Cette option regroupe les éléments par projet. |
| Mon focus | Cette option regroupe les éléments en fonction du niveau de focus que vous affectez. |
| Semaine d’échéance | Cette option regroupe les éléments en fonction de la semaine à laquelle ils sont dus. Les dates d&#39;échéance sont déterminées par la date d&#39;achèvement prévue. |
| Statut | Cette opération regroupe les éléments selon les statuts suivants : Nouveau, En cours, Terminé. <br>Remarque : pour le moment, vous ne pouvez pas utiliser de statuts personnalisés dans Priorités. |

+++

### Glisser-déposer des éléments de travail lors du regroupement par Ma priorité ou Statut

Vous pouvez faire glisser et déposer des éléments de travail individuels entre les catégories lors du regroupement par Ma priorité ou Statut.

1. Regroupez vos travaux par **Statut** ou **Ma priorité**.
2. Pointez sur l’élément de travail pour trouver l’icône Déplacer et faites-la glisser vers la catégorie souhaitée.
   ![icône glisser](assets/drag-and-drop.png)

## Trier votre travail

### Tri par groupes

Pour trier votre travail au sein d’un groupe, ouvrez **Groupe** et cliquez sur **Tri croissant** ou **Tri décroissant**.

![](assets/sort-in-groups.png)

### Colonnes de tri

Pour trier des colonnes individuelles, accédez à la colonne et cliquez sur la flèche vers le bas.

![flèche vers le bas dans la colonne](assets/sort-columns.png)

### Développer ou réduire toutes les sections de groupe

Pour développer ou réduire toutes les sections de groupe, ouvrez **Groupe** et cliquez sur **Développer tout** ou **Tout réduire**.

![](assets/expand-collapse-groups.png)